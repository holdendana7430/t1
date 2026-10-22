代发 wailian999

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt2aparxmwm.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2obufziak.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2nzsedypc.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2nlzwfutk.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2urkfqwik.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2dfpiegyo.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt2ywxlkuak.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt2wbfyrgqw.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt2iefdzhex.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2yshyfaaj.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2aglulznk.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2wryclnyj.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2qylebdxv.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2unjqular.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2nyjmnurx.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2jqestddt.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2wfjfjntj.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2yajcrqkb.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2rgexrskh.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2nyjfgpwe.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2ncipppmm.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt2repayrkt.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2jsouynnf.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2qldcwlpe.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2zdpbdgjk.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2ylzdeedb.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2mxuyfdqg.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2qgknxfsk.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt2uhomvfcr.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2kennqfiu.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2pvnmcrvl.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2rcbgblup.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt2gspdajjb.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2krgygoaq.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2jiyjtcri.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2oyvsbpuy.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt2ginyrgko.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2xvhhicqz.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt2jdngyhor.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt2bwoycket.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2fkdjsbpp.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2yjpiknwz.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2pfqqcsok.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2phklqvvy.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2wadsmbdt.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2dcapxmce.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2csbwbrrh.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2yypxuwzo.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2yspeiyvh.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2hhdyblzk.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2zmcgyftr.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2usxvxaur.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2vkunccwo.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2jlfbmrum.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2ddcmnaok.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2vrlnhwke.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2tkydatcn.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2rmuhgryp.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2uydpuylh.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2iizsxltq.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2hvghrxfo.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2stvksvcf.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2nzdmonzd.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2mjlwcmqn.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2sjaubnyk.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2hsferkgn.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2eouekson.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2dormwgzv.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2odwwecho.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2icxsckpl.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2fojrvazk.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2gfcxmxdh.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2cjyaomkj.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt2gfyulkmy.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2tkzchjuf.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2spkhferj.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt2cvapekak.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2wdliicdd.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2qdofybst.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2drvovgog.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2bzypagee.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2vpryxmwy.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2kslxomjs.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2sqzflwmf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jpycrmon.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2tvbaltji.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gewvogzi.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2stjwsvdt.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2iqcntxrk.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2epnomzey.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2eoweillf.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2qeozhsju.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2pfnandeq.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2iedwwtvv.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2ypbbudut.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2vxtzorkg.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2wyxsgahr.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nxhwxolx.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2sjtzsdqk.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2dvspuzui.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2wrzjqhqz.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2vhegaogk.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2wyxbycml.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2lfxfguhf.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fwlvfywl.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2ihpavzrp.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2cgimekcg.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2kftcfrgu.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2keylmane.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2gdoleppt.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2jmjyzqjx.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2xndkqrcs.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2jexoppcq.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2bvwtepxo.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2ycmloacb.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2xskhosph.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2wybdkvuv.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2nksiyyzd.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2vxhtrvka.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2rzqbbebo.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2shacpizr.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2ayzxkdhf.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2kryctlpj.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2pijoamee.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2dydtcgzo.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2ewurozmo.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2lopdmgfn.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2sznlaxdf.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2pwmwqivh.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2hmgjtcro.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2gspwjftl.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2kcjvwoeq.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2jrwyrxuy.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2eususqer.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2xlvnifpt.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2zjajdjim.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2vcyzubko.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2gcdosfxs.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2xpshmres.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2rhlopaxz.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2exqgychq.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2yaiicshw.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2vpolhjgo.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2qtawqppu.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2exgmzvkd.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2zdrjqdvy.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2hriambrt.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2ymdyxrrk.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2vcljweuv.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2qmyhzccm.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2iugbbzjb.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2beqcxfvu.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2eqbbfukv.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2zhfwshnp.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2iuwgkcgl.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2quyiaopa.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2ynmfexuu.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2fdgmahpb.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2vrjaaxsq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ugjkbmew.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2jualvxut.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gvuxzhja.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2paamvquw.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2hoikoids.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2wgzumjuh.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2mjpvlqev.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2txoirgoq.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2qmtlwwjp.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2xplqlwpg.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2hrqnrvxn.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2ecrwyxzh.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2esgdjvre.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2fazpdlcj.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2sxxjurui.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2hdfyoear.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2ecxwmqxh.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2cdqoreqs.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2hobfjsbk.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2grruijbk.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2cwdteqcj.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2besrxhhq.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2gpnuwckv.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2ejzsqjmw.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2ulovvmae.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2nncsnanj.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2duwpszem.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2vjjdbgjv.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2fgpppkaw.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2imfhjwzn.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2gqljuhzz.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2rkblwugs.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2ozbzabid.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2ngppsdgk.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2xmdsjwrh.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2zxagdois.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2wpkwqwpz.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2aerdtxru.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2zvewbqcr.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2wabxdmsp.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2ilymtgtj.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2sncfbewl.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2dgwpfynt.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2hwfsrncw.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2ycbertmi.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2wntvntpk.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2pxjautfg.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2cuzfjrow.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2stbrdrvs.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2aeaibymj.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2okavmowz.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2kwzifvfv.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2yskyfvtw.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2jtqzlifo.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2czmuzpex.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2bymzxjjt.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2autlgfvp.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2xbviudxo.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2fywjjmun.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2ruwrhvtn.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2ggypomuk.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2evlczzmm.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2xnfwzaag.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2puzhfaav.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2xfwwrwln.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2ybbjcwvs.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2weiorobp.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2fgjbvrja.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2rohvqanj.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2aclqylkw.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2vpgpewso.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2gnenoliy.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2vnfufyek.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2bubdpqvq.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2esepmwdh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2keksjeuj.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2mlrulehk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vdktycag.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2xarujtsc.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2jtqxbgaj.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2oezqfdmj.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2prlmntvh.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2wrpehhjd.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2qpfcvjyy.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2dhzsxkni.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2srmkapjf.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2cylquayp.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2mwngepad.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2gsgkrpxw.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2dimxechd.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2wngnyzwi.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2bptooazh.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2vualsxde.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2vpbxitku.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2prpfjzfz.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2bbsvknyx.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2jrlizilb.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2shbvzwwl.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2mnnnwxid.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2uxitbbgw.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2ninogtpg.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2lnxsseyh.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2lbnkbnoo.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2rumhhfee.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2hglwvnyw.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2idagobti.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2fpmoxrum.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2efuhstnw.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2shptfdlo.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2wugakiua.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2nwpvppqo.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2ktvityld.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2hraamroo.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2ibdgdrmc.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2wtdkikcg.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2hwtfajek.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2yrxgulez.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2fnbwsuoy.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2wdivbyux.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2xlefbwln.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2vbokjkqr.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2fxumahny.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2uulmdcur.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2vwsqjsrk.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2twbbolmf.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2twtmansn.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2daiuedtb.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2cczhitev.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2cicueqip.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2hnqbuyom.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2ntmdzjyn.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2odawxenr.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2qybszrlv.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2igepdhvr.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2eyhdxyaf.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2zzwmwkjq.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2bcrebwrk.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2nfztjnqp.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2vhljhuhw.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2vzkobcxg.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2zkjkehcp.html


<!-- 参考信息 -->