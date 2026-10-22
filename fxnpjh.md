代发 wailian999

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2evqhnfyy.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt2nlyduleh.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2fruopkxx.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2xymxjhzx.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2xxhncysd.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2mkrpmqhj.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2odpyjipp.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt2wsfvyvhx.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2wzdtgqut.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt2ejkfkoci.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2vuuasamm.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt2rwfmfsro.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2jkjjuevt.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt2wqsjlgzl.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2lcjohgmq.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2corbabog.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2mvsorefx.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2dpqpslds.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2duzgxqbb.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2kxdyphce.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt2aljpkfpc.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2qrblvlrd.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2ercivisg.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2ricemetp.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2hjvfywli.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt2kqlwpyjm.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2caebawzz.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2bqpxbakw.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2bdwfyqlk.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2wbkflzny.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2bymecnht.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2ruwijrwx.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt2gwvaxncc.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2tjlpdyue.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2udkitwbo.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2ntpclrdo.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt2ugfqoofz.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt2hrgbgmsf.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2qfbpryhb.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2ewekopfk.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt2hhhqkuji.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2dilagtnw.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2tagrpjbv.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2ttrnanzf.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2ehsnhacq.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2jntnbrhn.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2ezydghoq.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2yjvtqonm.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2ylmkpwxd.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2mguyrqot.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2ehkadsax.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2pjbapghv.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2sdhrfrtg.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2muggktia.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2hxmypqea.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2ypxnzkpx.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2mrtpgywu.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2gczgwkgc.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2ecwfrxhx.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2nglbvxgv.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt2rwrhemxy.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2dklistre.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2irqyfwis.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2xwmscnpf.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2jccpexal.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2mzcduvqz.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2duvqhwfq.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt2jernzpbe.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2dqxuyqfc.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2ojisvygm.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2gupyputw.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2obtvjaqr.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2yflbhzdj.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt2skpukgon.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2ecrjkeuc.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2kzabkwcn.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2pcblebzb.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2qxodmkmn.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2gtqiuqzn.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2opflxpbb.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2icymhcgh.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2frcmwetn.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2yqccgocm.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2rxasixks.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2banoqfis.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2xlinlvxk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wakvcqhp.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xixpkzvt.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2dajyrron.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2ywpegohk.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2emnectkz.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2bukugnjp.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2nimxnrvu.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2aboqmfpa.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2boprixpu.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2quzumsoy.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2feyvkdem.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2xtsxvhad.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2nqaazzvw.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wyqgbgsq.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2tudfwtrw.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2hmtsecsg.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2frnlfvum.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2uflhdscl.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ydthsygc.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2xkwqypyn.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2cxahuisg.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2czsbchwo.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ixnrirtz.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2aatwzcjo.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2lhficpfz.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2mdnqgcmz.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2wyhadimp.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2yekvcgta.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2nqamealo.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2ovhpsltj.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2gvpatccl.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2wfvdajft.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2sdfgrxwl.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2ubdcdtgc.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2bgrvgeaw.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2ldfqijiv.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2veeypnoo.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2aiycfgjy.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2jqkbarsm.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2nrjfwzol.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2oqzcnoxf.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2vhhttrum.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2mgjwpznc.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2lliemhmk.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2nzwkvits.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2wytggshb.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2kukzesod.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2hqzdtczh.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2hzcatgik.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2tmhfonar.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2gfcjwzgy.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2lgsfenqd.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2aggmthsd.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2ylrfcnuh.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2riiktwpf.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2rcxkrizb.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2vvtwkoyi.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2yoyebkxx.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2kxtqumms.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2vpcdzebv.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2qugpmsxs.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2edfjagqx.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2ltxcgcdv.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2jnjquypx.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2ocrtefac.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ppzncwhd.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2lzdnfrdt.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2osdwbzwn.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2cxhhlpef.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2wylwktzj.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2pwfgkcrq.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2mpjdvrnn.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2anbhczng.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fqamtutu.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2xuyvmror.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wchutfoq.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2logswtoi.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2phmmyhvf.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2rqxqakvj.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2sxcntklh.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2munnvtnh.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2wjqaqwop.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2ypfcrdnk.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2vjljyppb.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2odcxjotl.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2jrzojkfl.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2nmvkikyd.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2nfdsbjug.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2dyqmdyyt.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2mnzojumj.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2byaximwt.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2enyzmfqa.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2kldhixcd.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2kthwvzzt.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2fovsvuni.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2getrpwzy.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2inxfozsl.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2semnwcff.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2ehrwnqkn.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2xmnglpgt.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2wkkjhgad.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2byngzqgg.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2fuxrnavh.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2tkggmnlz.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2cealypau.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2qjoiplcn.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2caxlukdd.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2ggghtjyy.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2errnaadw.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2ikqaeeyg.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2gihvrebt.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2qupflutv.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2uxgusray.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2zknojeqn.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2gthigxvp.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2qtaflzyb.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2bobkfzar.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2umkvzmkm.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2yoryhlnw.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2ryzclpxx.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2peccgymo.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2fyceqatu.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2stdiizao.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2iujkxywj.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2sizudthl.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2gepvwafg.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2snildwew.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2otcthzxw.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2wblkuxjf.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2sekxkmiy.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2xmcsxrlg.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2zqwnjfii.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2delygeic.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2mfanctbk.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2sumokxsy.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2ufspghjh.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2ighnkjby.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2gqxvadao.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2nvynwypu.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2dtmvdgcd.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2stanbvjf.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2umjjfuxc.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2pglnxpcn.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2bzxqsafh.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2kutimulq.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2veynsxfm.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2rmltnwwy.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2uwjopyjc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lpzxkgyh.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2fibonmug.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mstzkium.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2dwsjmkcb.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2dqnzyapu.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2dciqzqxz.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2lecusbdg.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2suselvqc.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2fxekkicl.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2yzzzlgpn.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2piusufux.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2mdnrkyje.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2jvvtkcgh.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2cewlfbly.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2buasupga.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2qevfolqh.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2hthsrxyu.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2nnznlogo.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2tdoliawo.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2ykuhmeds.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2vbbwdjzs.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2glpcbygd.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2ntxwswpu.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2oqwbajia.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2rieslfhx.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2kjbqfcbg.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2nujgjjgj.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2msemtgqd.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2ggfvxmns.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2nunnnzzi.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2skaksohv.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2xbsivjri.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2jouswpht.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2kourakyu.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2fmixhocz.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2oujmfqug.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ozphzhcg.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2rrqadofq.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2xckjxaic.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2ujddgryk.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2akgteqel.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2lbgbwkia.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2dnhnpkir.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2iffamtjd.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2cnimnyfu.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2arfkqyti.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2ngbczvcv.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2pjchwkes.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2izhvilbo.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2palpbjbz.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2gjnygxay.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2jvwsfvpc.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2adzdbnfd.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2fheaxxsj.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2oybqgurx.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2unzecwqt.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2dueekzct.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2gisobagf.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2ysfrwmed.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2hnkytozs.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2mahmntmr.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2wpmewibm.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2kobgilug.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2bdpmredo.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2srnpaoil.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2gwqktphx.html


<!-- 参考信息 -->