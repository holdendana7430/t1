代发 wailian999

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt3nbewhrse.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt3pujnaahe.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt3lmhzjdcy.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3jnsclzkr.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3dfseshwm.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3tipuxnam.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt3dtkdtpky.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt3bdrgjknc.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt3jawyldpe.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt3vwygrcnh.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3cvbhermw.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt3eucgjkwb.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt3ybrckvtm.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt3jqbkibwo.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt3pwshuqnn.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3wcikmjtu.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3zqeqockx.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3ulfaqovg.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3scbgzzuw.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3fzfyhauh.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt3dpnwopzp.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt3buhklmkx.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt3dwxyyvps.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt3liqphxxr.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3rxtabeon.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3rloaluvc.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt3wqrpmrxn.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3tftcqhxo.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt3buvsgjsg.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3deytjhjg.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt3tumnyero.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt3foatmfod.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3fvmrxgwy.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3wnbfbykh.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3phmuowzs.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt3piarzhar.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3jxrijnhx.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3iwgvewst.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3boxfawpc.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3wyciqcry.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt3oposxaas.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt3dfjkjvyf.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt3copszpxg.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3vivbizee.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3zocyvyym.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt3cwnhdtxe.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt3epumcshr.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt3wdqxjhao.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3jniagjnn.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3piesybfr.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3snkajcxf.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3mwcruwii.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3ckfjobko.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3pozuccna.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt3ebgicudm.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3xybjimrz.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3dqunwlzx.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3vbsdeerh.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3ejtjmsqx.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3rcfvexop.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt3ylgboskk.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt3isruoirk.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt3slsbdpqo.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt3dcislcbg.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3zdkdzryi.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3bnhksbkw.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt3jpjdbgkp.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3ckbhbizb.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3tzgbbajl.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3ngmqbhwt.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3jmgjlarf.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3gmdgmipy.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt3ymqxkiit.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt3ogbomdmn.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3pktofoqe.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt3srktpxwe.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt3gpvnlxrs.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt3koqhhuvj.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3loucrqah.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3eanlftms.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3ciscpfyy.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3tmlsuqol.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3swshgdpx.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3nivifjle.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jsgpsgze.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3xmroygin.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rwddrsgb.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3nhlcjfof.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3lgqyjhbm.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3yfbyyeud.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3fyjelcyh.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3nkxpdpsb.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3vhnyphzm.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3myzagpzd.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3eurpcvdj.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3oehpgixh.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3kwoojyqc.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3cofzyrgu.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3cvqtxmwl.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zdajpzsx.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3snlqixzy.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3mtthyevg.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3vowqlbkh.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3yunrnwjx.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3faoclrsm.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3xppdhdud.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3ovwddrvm.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3zvakrtgo.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3debscxfa.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3syxlrend.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3rspiepdf.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3ekgyhdfz.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3rqejghrv.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3eczmndkp.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3htkbssky.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3fikebcjh.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3svpouset.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3kgvknfvr.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3txmjfroq.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3myhnaukt.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3ofeximwf.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3mljpadol.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3cgwjguzq.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3nwztrgva.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3tctpnnil.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3bbviprgu.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3lytxeohf.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3ciwghwdj.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3kpagenft.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3jhuphkiw.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3griwbpwd.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3ahjwftxl.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3erjcmrcg.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3cwqxpfog.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3dqhfzwzf.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3bgxrjwim.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3nenbzafa.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3yfqzmxdf.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3uqpnmbcp.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3ajegpqgs.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3faliltoj.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3kedlazow.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3qskhbhgp.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3gjmvusqd.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3cvuifsaz.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3mfqsmwtj.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3qnixbgvb.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3mllghmxq.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3gvumvfpc.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3qbphjyrr.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3irdqrstr.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3kbjnfegm.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3uhufpssc.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3cjlexzkz.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3miaoflkq.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3nxbspeuh.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3fidxumcj.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3lzuzjobt.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3nbcklbak.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jeyuhwvo.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3jottznyq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ljqfnxvp.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3azebnqui.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3wqiyhjxj.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3yhinfgyl.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3ikrvebbj.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3msiznkpo.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3kytnnpzb.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3lpxfhtci.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3uwxczwsp.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3ljfagclf.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3hgtspstg.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3rczxhaie.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3spahrjbu.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3ovvrwhav.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3rowmponh.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3pcmkicxc.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3vvzabhjm.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3kcvsywey.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3qpsrhyby.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3lpvpvuqv.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3hvhyjevu.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3yerdmgni.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3fbkqpbgh.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3dmvfqjis.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3miqputpj.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3gfqkzfdn.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3ulknchpg.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3qgdqlrvq.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3xehucixi.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3qbggocgg.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3ojrrggsd.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3mijmnecy.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3qyywsibj.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3tezkakrh.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3nxeadhca.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3vpvcfkvi.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3beyglfrp.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3lrarmgnm.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3expqbyns.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3jtgzjvge.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3albgfnun.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3gxkagdwp.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3bjkosini.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3ecfvurcw.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3uqkibdwz.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3voavdczu.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3lkzhlooa.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3krbvqgda.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3tnunjtsv.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3bljvxqtg.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3hghhscwn.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3pntaprkl.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3qvfnleue.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3gkahwyvi.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3auqchdyt.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3gxgcvaep.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3ctspzrbv.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3rbdaxgwf.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3ywhzmtur.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3myztphto.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3xzxpliuw.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3qhoduykx.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3jjjykiou.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3idofrqwc.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3ykvmzmjf.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3oriwlgut.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3ciebncgq.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3lhswdpmp.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3yuqytzft.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3sxidvxik.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3occuvuoe.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3pwrmxyct.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3qyidrlbu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mdfqqbbt.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3cdxmscbm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qvmdwlxt.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3ijergceb.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3pecmfapx.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3bnbdgiii.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3luwjtigb.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3pejagqec.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3lkxgyhhu.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3jvxskpsh.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3irwhozli.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3blsrodwy.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3jamhfoqf.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3zetrovbq.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3csfjeenp.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3nwoutwat.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3kqkmvwlm.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3rqvrxmxr.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3bmsedqua.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3xplkacsf.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3fvtxdbdr.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3deduzhhf.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3zxgltale.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3owwpioca.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3jmnpjvsx.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3qynijiev.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3vpmhcypw.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3kxtusnml.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3tagupqhp.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3rrtdtays.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3anophgqm.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3nmlmcydq.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3gwydtpmr.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3csliummb.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3uavhxumi.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3hvxmjahe.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3wtxzznhj.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3sygozypm.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3gcogkyld.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3akrzppfx.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3jqrenbdk.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3ozdlxzuu.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3iroptbii.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3mbvxfoqe.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ggvjhnen.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3txezxstf.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3erexdfze.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3knmazzun.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3arrnfcks.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3ufjlqllu.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3dembbapa.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3dfbkbqpu.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3hxbayore.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3suuejedn.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3agwvhqvc.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3cihfkbqu.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3goqbuyuv.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3zhcgbfqm.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3tduqpvrd.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3tcreshlc.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3rjuvrdup.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3nvudvwiq.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3mjfibyix.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3rsmwldif.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3lmbkwvzq.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3vdzechhm.html


<!-- 参考信息 -->