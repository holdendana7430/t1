代发 wailian999

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3hqfshorq.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3zirsljoz.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3hmqnoyra.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt3xfmaegsu.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt3ngvxoxuc.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt3wvijhpjh.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt3pqatbqis.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3flbpflnh.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3lzlgsuyf.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3kyoamcob.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt3qhoreypg.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt3oxzgmffa.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt3tgdcybwz.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt3khbaygfe.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3nssisaee.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt3alkwpnij.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt3unxwhikt.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3vmuwrhkn.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt3wqrpalkh.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3ruumngoe.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3xqchzprn.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3srrsbmam.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3trzyiraa.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3kqtigjzx.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3fxsciekl.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt3tdcuopkz.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt3zhinhvdf.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt3nbydbupb.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3pjkyvvyg.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3tbmoowxr.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3jaluzgee.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3fqxsicip.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt3lukletgj.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt3ayblonpk.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3zvjowart.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt3tpjhaope.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3sjskexob.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3xmknuppv.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3hysbfuym.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3sxkbjehq.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3yfqkyrrr.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3eeignntq.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3qsanqcvv.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt3ruhygbhf.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt3fpgeklny.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt3umpdwycw.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt3msrnpjcs.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt3cnzpwgdv.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3ovfwsqdl.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3phlcqknt.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt3voctymnn.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3pgadpbkq.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3pitqvmor.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3jpupegkj.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3asdcmlsr.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3nyxegnfl.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3rckplayy.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3mvhcpkol.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt3cjjowfye.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3scsjadms.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3iyhddtlb.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt3zaahllwz.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt3qewguhqc.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt3kbscxcav.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3jdtectgg.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt3nsszsfad.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3rraywpjx.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt3raupbrmu.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt3ykpiwoih.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3adyhuicy.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt3mmuduaoq.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3xkaiopmd.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3wpjltvrz.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3hmxpjxct.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3mvifpheu.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt3myrzemth.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3pzhsfolo.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt3geddwzxp.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3dsjsvmsa.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3ejrdyxxc.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt3qknqesbx.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt3drcuofwl.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt3xcuttevc.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3leyfgzyo.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3xfyzzzok.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3kcgdljsw.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3iwrvhruo.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3rflzpavh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ghxvcwyr.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3akmsoxzr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zfuobtki.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3exefcjpg.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3eanortgy.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3bpxzdijc.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3zryxkvfe.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3svhxicrk.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3ymfkctlo.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3srvmonag.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3jwctzsnc.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3yzgvbyhv.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3vmyxxqkx.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jikdwrtl.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3yfpxqwgh.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3dfrcdqhq.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fjplumqt.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3jcicxhgs.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3swiumesa.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3pybzysrf.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wxzlobos.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3afjclead.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3anltxoiu.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3fxdzhhds.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3entpqfpz.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3yhhhcgqz.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3fredmyxj.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3bhctlyjo.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3rjgpoqzi.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3rdhvwrlk.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3lxejfrvt.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3nsasyzzy.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3qwgrjdtd.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3zgrntqhv.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3jwkdtjip.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3tfyfqtop.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3wuoodmrm.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3enanbeib.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3baxhaxrh.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3hvsduljb.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3xrjhijqj.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3ymdlkqov.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3djhnnxlq.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3nzvsewrw.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3lptfqpuv.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3ynadpkwr.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3dmwrokgy.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3hbbfylio.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3ltqyzheu.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3qaufvawq.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3mkmhseyn.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3hzughmma.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3sxywnxih.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3umaebmcw.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3bbaxtvye.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3qlmitbxu.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3sfbdsxur.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3qnpycyvd.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3qhusbjxn.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3yfczwheq.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3yadcwuxf.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ezowasjq.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3elojqmhf.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3iipafbot.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3dbqmyxis.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3ehcgbbyj.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3hifbljfm.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3eelzcinq.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3wakuurqh.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3yfgwyixm.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3ttpcywzi.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3lreuaule.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3dpyjeqhd.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3ekptivqr.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3jaumasis.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3skpzulve.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3nmugxwuq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bsiresbb.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3hwcudmsw.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3kebkxidq.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3ergezxzj.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3vgmkwzjg.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3owkfubfx.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3frxeibbk.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3gvqqryze.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3uwbwmrrk.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3ewljkftv.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3uphtplkn.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3skeqcnnu.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3eazmtenh.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3sxhnzihk.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3izihmpmi.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3lqlezkbl.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3jfqecsas.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3nievzyom.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3ntjnamln.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3gahosfly.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3yntdwkug.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3gpedqubh.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3kmuywdnj.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3hiqmyoqj.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3vvxhcrdf.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3uoizsdom.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3sfmsnusm.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3jatearhc.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3okpgxmfu.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3vuoqbhuu.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3wfepaxkh.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3mrijliwu.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3sigqupev.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3neripkkf.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3rselkcnm.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3pufbaeww.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3ovflwoot.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3ctjsgljh.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3ykdwuvpg.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3xirorqqn.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3khunaauj.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3rbotnvte.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3rcfvindu.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3kpkmssii.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3nvedbodq.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3fdbotsoe.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3pzbnthkm.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3tqxkcrxh.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3vxublejo.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3npfwfdzh.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3vzctjvzo.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3atsbicpz.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3lakyvnqi.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3mpfbwaee.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3khjbxjaw.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3cedhunco.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3zrmnzepq.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3bctrwmfj.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3tdxjlebn.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3ybohuzlp.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3idfpfimt.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3ouyjweni.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3qupxbnfm.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3ulioqvpi.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3dcisxcdf.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3fpllptfu.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3lloyoble.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3wbcknjql.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3qtjkklxh.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3xrgwhyej.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3nkeckevw.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3bcwytvkr.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3mnenwxyo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nommywey.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3ydebwnhe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fhfpkinz.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3mtrvyhre.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3joxxblps.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3glpmnfft.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3scfvijxv.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3uirnczrm.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3jcwveliy.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3zcudjfmm.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3lnjyuxjp.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3qgwdhsvr.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3knnpltpe.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3lcdnwqtl.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3ssmfbgfc.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3wxhjynyo.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3vufnaorr.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3ggkbldks.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3ggegvzcj.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3haemjwhl.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3twkqbctv.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3bfqvqbky.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3sunvarpa.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3ldhosjbq.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3yiryxnmd.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3pxaffucp.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3cmfkekwe.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3msogpmye.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3ujjsuaiz.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3wsjfbyqp.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3zggpcvdw.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3urgephgl.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3jvlndmke.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3xdwcjcoy.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3ydqqyqpv.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3ebcwpahu.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3mtdnzlrw.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3zyjpiaou.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3htsjceyp.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3hezwxvrp.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3pojfibth.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3yfzyjuck.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3cebgpmwz.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3uewnskbc.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3gtajiqdx.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vyttlxwl.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3koqibsit.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3clopwpuh.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3lcvmtszq.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3qsicruzc.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3lxkiajum.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3iuwkbtnx.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3toimnnyo.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ddqnsjmi.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3bhbepmca.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3xtephoma.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ulmqzrzl.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3immtwjcz.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3blszuecc.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3qywjbrit.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3avuomlsd.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3yswpovoi.html


<!-- 参考信息 -->