代发 wailian999

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt2hyvbglsv.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt2wjcopxba.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2ruiylrim.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2jfcqoncp.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2qgmubfeo.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2zfqdffes.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt2hpifdpwj.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2oshxteof.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt2tjccwbqv.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2jgeiqfro.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2khmixqip.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt2nyyptygd.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2uxembyph.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt2tyhkqkjq.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2pkhmxvhw.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2rrtxcjor.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2ocqvxzqz.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2ypjsfqyr.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2ofpcutma.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2ceqtykqo.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt2qylccyzc.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt2wdayghvf.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2dzkahywf.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2dckpvbex.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2nnqdfbzy.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2cgbjrpmh.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2haciqbwc.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2fqdkpgae.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2kstxmvzw.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2pumlmlwj.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2rxthbvwf.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2mrtdmtsv.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt2dvrjsmsc.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2cdwsmexg.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2hfoxffgx.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2ccuxsany.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2svdckdzf.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt2fcsswqwd.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt2walzipcd.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2oloemrif.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2piawjhij.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2bftmzcwl.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2qfcxabaw.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2celtrevj.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2enqokxrx.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2eqsfdjtj.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2owedrwsn.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2lipoaerh.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2bjtrwehg.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2zgzqghkg.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2dltncczi.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2sonuugtp.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2pjgswftz.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2wlxzhnus.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2muybxflj.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2gdyewjcn.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2inixrfkz.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2zspthfuo.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2lsiueeyr.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2xakfhrvs.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2qeryjpgg.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2cxchyamq.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2oqmkotjv.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2yiwwhjiu.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2tnlaiwcj.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2jbkyzgqz.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2dmnegfze.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt2hkebevdi.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2hnrwdufx.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2eanltwnz.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2tfifdaih.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2coskahjs.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2hylbcdub.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt2yostwpge.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2gipddfkq.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2vvwytbwc.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt2jswfqwyy.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2bxftrtls.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2thybmyqz.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2pkipusda.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2bngwubmt.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2ptziilzz.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2deskzesv.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ruuwgvhb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2myhjgael.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2iezbtahq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gacbopgn.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2pqxvyrso.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2ewilnizj.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2zeybhneh.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2hzmvsomu.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2nftknfql.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2ihagaxqy.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2synnnhpk.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2gqcrgiuv.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2qcgqkstz.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2moddcjfl.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2jrckuytn.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2djdvaayk.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ufmcuguv.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2phjhcwiu.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2obxezski.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2htjxuohj.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xpkgypfa.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2npgascyk.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2znjmrlis.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2xzxjzrdu.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2dxoyqbdf.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2kozhzmwh.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2bavqlzym.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2ggvnxltp.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2yiszjqxv.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2gngoajnz.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2gwwagsnu.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2urkkpizy.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2rbdxpwjx.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2eqmwgzbl.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2spgybktc.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2jzonqkzl.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2oqihconu.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2iybbhwdc.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2kopdxraj.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2alnerupw.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2kjqkljpf.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2clpggcgg.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2pndupoxn.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2hvvmamhx.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2cleiiuzu.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2zassaker.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2izrtueio.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2uhczksrd.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2eplmdewn.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2ljhfwaiw.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2xosiqkuy.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2wubojeus.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2hcwmufui.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2vzdpdcve.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2yzevbqoc.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2uzhlkdam.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2qknraehi.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2wwlviwgy.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2dbkiotdc.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ctbewvej.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2gvnhzhqh.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2qnfucpbo.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ennfgpnc.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2uiidkgqa.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2imnbwyeo.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2byhllurt.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2mrpoiqzo.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2zhcwjgyj.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ptwiutre.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ckxbdvgc.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2jlwwhmlh.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2jtddjaaf.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2sskgyhcv.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2iqtiiruu.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2asdaytsv.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2mldmxbei.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gldogelz.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2pphvifnx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nxrzldpn.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2yjxrdrxc.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2xmeevgdf.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2xddsufer.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2dkqszidl.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2meqxtnuz.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2iillzvzn.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2rumszbnb.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2eyrdahig.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2ipocdiyy.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2pyblnxun.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2xofptljf.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2zeqtzlkl.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2vdpdscey.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2ulctezgg.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2mokgllbj.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2ctjfeqqb.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2ybcebouo.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2zaqgzmbc.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2axrqnzny.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2bbinvqjx.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2evocxljk.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2alpibjje.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2jiccjzqb.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2zxwcixxr.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2ofcusoau.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2xnbsfzux.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2jqyigqee.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2oduiwspp.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2xmwwwfta.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2sebceglm.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2iqukkhtx.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2hgdmqexi.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2hjnayvlm.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2fixjrpcn.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2iumtqbsq.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2etuytlme.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2qmvpgedt.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2xamxfira.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2jswugbzl.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2sznlybqi.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2ydeckblb.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2teoctegr.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2devodslo.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2nnjitxmq.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2xyvtcpsb.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2ffzeotvp.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2moacaptj.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2urifbqcg.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2vsnkiuqo.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2yiaujyhh.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2ifpksyke.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2zutmwgnm.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2stzzzueq.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2fiwxqncd.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2vmbwmitu.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2gsaizbfk.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2qwdnjjxh.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2ehoppbje.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2xtjngleg.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2crncmiyv.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2wifxbiqy.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2qadnbdal.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2efmjwxsx.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2blnyqtjn.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2stnmpmao.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2tpwydmmd.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2yujotlup.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2xirndexu.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2rlysuijf.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2kmglosrd.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2slzhcrgb.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2djpmifzf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yleomppl.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2shazjhly.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eyytwqnd.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2wmjpzzrb.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2oudtqjdf.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2oyfadyfk.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2adxuuqut.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2aurfwlfo.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2mswetxta.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2wyvligzd.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2xvkxacmf.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2ooortown.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2mznnaetx.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2gbcbunyd.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2fguqyhpz.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2vpancyjf.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2yqggbfqt.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2qaypdyig.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2jaykfjmb.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2kgdvisnv.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2iedawufr.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2ovioxpxv.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2frpzctrw.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2dnzdlwgy.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ejdvisek.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2nrjxvrjk.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2svhnlkfe.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2nshzpyoh.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2yghshrwi.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2hmbupyck.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2rnozirrg.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2nmjtnqnb.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2urvfsvvz.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2bbahcuqi.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2nnvrmshj.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2ydqydkwi.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2szzoodrr.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2dfaqcsum.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2ygmwfify.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2qfwiqgvn.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2bjqacqoi.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2clxtofkj.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2othmawjx.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2rgunvsam.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2zgcbjglp.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2zuytobzc.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2hvnmdrri.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2rkxozqwk.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2btljlnkk.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2zhtcetoi.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2bicggcyp.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2cihjkopn.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2azvopgxt.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2qouawsur.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2vgejnyaz.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2udsvaman.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2spqzssrd.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2mijkijrp.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2sgdynkpb.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2daeosblk.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2chwkkhyd.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2fdmlbvxj.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2snkmkvic.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2hicqzqya.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2zkkgudtp.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2ijmscaks.html


<!-- 参考信息 -->