代发 wailian999

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2dxobdnye.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2klkqoqbn.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2uweqovfz.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt2cqmlmuju.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2awobowsm.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt2kkdxoffn.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2rpxbstrd.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2scycobsw.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2hhoxsrvw.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2toimoloj.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2pbsbkytg.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2zrfiinwd.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2ohdmxfif.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt2sgezecub.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2gzirwoxg.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2grrixahp.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2mdhdttdc.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt2tgjgdynh.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2rvbrnayh.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2vctydrzq.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2umowpehh.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2fpaurcfq.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2ndudsvqw.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2hmlfzknt.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2tuzkcgyn.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2nrypscdl.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2cbubgouw.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2aaaaadma.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2eavjebdy.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2txgyhssq.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2ogjmwcwa.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt2vveifbcm.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2weoambin.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2quwicqjt.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2jlwecqkx.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2yrkimdln.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2xkxkxzxs.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2troooatp.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt2emxvhkym.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2nlktktdi.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt2ptvekefb.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2hujvfffp.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2juofkfdx.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2jhmeypow.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2nvthswvk.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2qcrttjwj.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2lkqrqyjh.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2poedwebq.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2tepyccyi.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2vyyzosih.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2jwzwymjw.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2ocoqxpqv.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2msyrxcqv.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2sfpumymq.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2gyjkxstk.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2jhculjig.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2hetcuqop.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2fjewcmem.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2wgopphel.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt2aycajzli.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2gvgyvkji.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2ipmbmpgx.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2qufoflvl.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt2spnjtuxu.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2qjnevbkr.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2ijtrsalw.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2dysyfumg.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2zinndukk.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2lhswelfj.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2etvzsnld.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2fvhzfqao.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2oprbvzdo.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2nbuueift.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2maginylk.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2eoomrnfh.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2tgiqzhsy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dkhaamon.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2viakibnn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pskqgsvd.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2nhisesgr.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2jyouarnt.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2bwcsgvwh.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2gpbyeieb.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2pvreiqze.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2aenlijqy.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2xrmrarmn.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2vsexoavy.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2dsifxzqz.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2wamjnzxq.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2deypshwi.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2nekgpohi.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2kzqsheqx.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2ucecpxkw.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2bhyzumws.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2hdljvdvj.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2iwjxksph.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2wdmeapxr.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2xbhawnhn.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2cvefargj.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2vpkkiojj.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qvbntxoi.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xykustqe.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2syhrgwfc.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2xxwxsvuv.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2fdhtgnii.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2ojezwcbi.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2rmmszijc.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2duifhxqs.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2bxvmdlgd.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2herqmmzj.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2utuzxxhf.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2bfzvuvav.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2teitvpnq.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2koljspue.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2eztzvthu.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2pvlzkfju.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2hxcpztnt.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2lypgznhu.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2awkbuozg.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2waupkqss.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2mhlymelj.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2pjyhzoyu.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2ejxrrhkf.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2hmqhjojz.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2mkfdacmy.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2wgqearmi.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2cjoogkue.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2ktvdqzxi.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2tzexyuvz.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2twxzimbu.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2dhfxfoop.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2khsqtnoy.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2sifylasd.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2xrzqondx.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2xcwfqlta.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2orpgomye.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2mocgcsir.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2gbpuaqvn.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2fhwplnfx.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2gpobeafe.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2imfdytjs.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2rckyhceg.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2eklmflau.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2lsogdobp.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2yfikayyn.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2gcgjrtzw.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2qxvwkpzv.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2hakfyaln.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2brtbaheg.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2yrnqluiz.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2cuymmlqu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xnxwzwgy.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2nxlifxnc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2izpqjuyf.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2trssmlzt.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2cxolbzvv.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2opfpttdy.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2tepeimoi.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2rzzlaffm.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2tnbdegpx.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2lbajfret.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2pwszhaqp.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2hyuuczdh.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2iwpiooxw.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2euyoylzi.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2kmzwfirq.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2phdrxpum.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2fbdhuktk.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2qwsfunzc.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2hxpbgxeq.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2qfnxzifd.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2yzqldspx.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2tdmotpys.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2ewzcvbap.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2luoeuyiw.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2xgbzsbmq.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2yqnpcgdc.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2zlavjmve.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2bliesjji.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2zzzbmsyh.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2tpeyykdj.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2qbgslvcd.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2rpgwttju.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2ssuffcvg.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2mowsabzt.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2zasshteq.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2ifehwpen.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2ihzcqkxq.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2iowuloqu.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2tawkefpl.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2juukuqbo.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2cmzczcxr.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2ncqpezoo.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2hfdpujig.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2idpbhcig.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2ncxqsojj.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2nfcwgsdp.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2vgtwdyon.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ttgpkasn.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2pasnhqes.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2onqhnxyi.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2wtlhvrse.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2froqsruv.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2zufyjamh.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2hqovyyoi.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2wpfhrjmw.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2ibnfvbnu.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2pxgxsvgi.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2renjbjps.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2sdtkdzes.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2kamxlawm.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2ffakzahz.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2tjnyvhlz.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2mrkxzeyv.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2khwbmusc.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2whwduzcw.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2jurghqwe.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2nvsmtxeh.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2cvbvvazn.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2cpxfnmlz.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2yizzrdcy.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2juogmpbh.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2qoqjdhoc.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2tkfnqqng.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2fgldcxfr.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2tipodrry.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bjvhzpco.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2bspeagdq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2neokveth.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2wotyrnpb.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2wrdufuqn.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2omruldsu.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2myceszjx.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2ndgqiqfa.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2ihcsggtu.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2kbmbjkte.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2izvjnlaa.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2jopvsfcm.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2mmeqesli.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2pcorkgjo.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2cfuwbzbs.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2uqhpyfxg.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2ntomgzff.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2kgpprowb.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2omnbfmpl.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2rbhpmjst.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2tqecvzts.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2lojwdpfg.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2perwrjkt.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2dqhxyqhx.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2iigecrez.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2mqxtutmj.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2gsmyqqlj.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2ghwilkpd.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2sfdyjwnp.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2yocrrqok.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2uwtsmqrq.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2zvjzcupt.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2wcuutrby.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2dpiomqbo.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2zaiqtxid.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2plrodaqf.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ozjrwzpb.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2zxdlkprc.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2dttpfzad.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2pmvjpexz.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2owrzkyll.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2ycicvqdd.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rcvjpbqg.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2kkskkrql.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ifzjptmd.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2lnxwudav.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2ztcucvvj.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2zwzlftkn.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2oqqofudp.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2jplcxrvr.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2jseogoal.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2ggnurtrx.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2icqjfokz.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2jrcgquyt.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2tuzogswg.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2frwyqwbq.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2whoakhew.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2uymashjr.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2cllkjcmf.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2gfwdghvm.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2eidzljcc.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2ekfxoszl.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2vxclvwjx.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2mkkdxojm.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2lmbrlzci.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2penbdebp.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2czbiqxvq.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2ypopkaam.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2amkyjfvp.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2zqgenvse.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2mwfapait.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2vjtzqwri.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2anowmmrh.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2zxzomiag.html


<!-- 参考信息 -->