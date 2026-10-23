代发 wailian999

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt3hzdzrbyf.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt3xwerxqca.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt3yfqqtngt.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3yftljlts.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3mbobeiez.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3bniixjiz.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt3llsylvmc.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt3gykgecpm.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt3kurpddio.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt3ohqgpjti.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3zyjsnvar.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt3gsgjwdhb.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt3xggululn.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt3jarebdgv.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt3xkcashdi.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3vpzmnwtz.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3rbnqwiye.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3wnhgoxvj.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3duiiffjz.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3juysulrj.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt3mdjszeiy.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt3nehxkshs.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt3nlpgbjjn.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt3tylrpxzp.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3bjymmdxf.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3ercdnizo.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3kxxnfjvm.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt3qkbwelgl.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt3sogkztzs.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt3cedowwjw.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt3xoclkuag.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt3thwaazea.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt3tctcfaes.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3eckaioat.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3izwzrfff.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3fopmcbqm.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3ctaezbmd.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt3zxolqgbe.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3hkvrxbyj.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt3ygmieian.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt3omvusnwx.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt3coqymqne.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt3zxrpwwlx.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt3rggdyrgw.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt3nwqcasbn.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3epsjqeop.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt3tgbpbhvl.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt3oevbwghy.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3iurfqlxj.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3plwwypod.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt3yuvjkonc.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3zkkezrdo.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3kyyaosjk.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3alsdgmku.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt3snlsuteu.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3tldpybrj.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3wxhodzjd.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt3bjtkfcoy.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3dddsemhg.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt3gngkzrge.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt3lstyiqqs.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt3nhowmngg.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt3cadndpev.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3bvmimjbq.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3cuwbkazl.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt3notgcynm.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3eqfrswtk.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt3erhbgoie.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3kzrwqdnv.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3qejeoein.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3cbiwzual.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3zrfbuqhy.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt3vcoiuieu.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3yitzndtw.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3nouhjgiq.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3ervgqymk.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt3qfvnvftq.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt3cudznuax.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3eqxxxuui.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3wdyseiwq.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3yuvulxbs.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3ozcivuem.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3xeevjcnh.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3tfedodie.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3elhvooid.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3rjxtkdjh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3emeonedp.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3ghhfmzre.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3wefycsbv.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3guqlgozd.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3ibnelaqq.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3qvvjpero.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3rekjwher.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3siwqhbzh.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3yugtjsej.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3xeuqqpsq.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3nxihxdij.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3sqjuqtzz.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3wprcvias.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3aigvadxq.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3owltlxkm.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3rrsoazyw.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3izerrpry.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3kgrtnjna.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3ttjqiweu.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3edvfumui.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3gmoyydpq.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3xwjtlnjw.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3sgnhdppk.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3andhncgh.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3pqwarpet.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3wstocnlk.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3fghglyrp.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3wxpfyzau.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3eecvoegy.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3lbwzvwzj.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3hssonyjb.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3hidxwlsn.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3aaptbcxf.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3yjkvxzqk.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3zbgymsot.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3ntsmksfs.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3qvtmupug.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3qghobrql.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3evdapzur.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3dymusqmb.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3vdysjjgm.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3gfhhpbbz.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3cfgtcbka.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3wgyxppmy.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3omxhkubq.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3zgwxisys.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3jzmuaifs.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3cwvtoyfg.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3tzhppwva.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3fvcydpbk.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3quxynmss.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3pminmary.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3yovuwcdz.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3fnplwrut.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3sdqerddj.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3zzdnybbs.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3rzxcofhi.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3ayqhwulh.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3hzlboyup.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3rlnpysuz.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3ynztnxyn.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3ougsmtum.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3kbdoednq.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3zmwcugif.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3nnulqrok.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3lfvybeer.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3knmaocwn.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3pnodzhax.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3qigkehas.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3bibnnkpp.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3gdajdffc.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3pdjsujuc.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3uumzakvb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bsyfgqtr.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3mzqtixhj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3utctwkld.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3enonjqad.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3ujaqbhch.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3djnphztp.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3tjanxluo.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3yxbasvmy.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3ahhmcods.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3algbbeqi.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3ojpolzkb.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3cnkoybji.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3iilwqrre.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3dabbtpds.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3fvjoejzi.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3vtwbmlbn.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3uyvubswv.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3wtpsnvxa.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3ojutkplm.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3vzuzvlob.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3uhpmzclo.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3exdljpat.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3ubqgqyas.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3vmvxrhty.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3bgcoqfin.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3jehyprrv.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3xfiecevi.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3vqbirhya.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3gjgaisti.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3ktvgqwql.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3zulwqlsi.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3wmvhxuex.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3laujvyly.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3emzxskhb.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3uxnpjeuv.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3vfadltpk.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3rqzutdfh.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3vnmjtios.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3btrachfq.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3ocmzrhfh.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3vtjgeekn.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3piblaffj.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3rbzomebo.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3qeiyzyiy.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3cihofzjw.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3jatguvut.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3okeovkev.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3mxywdclr.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3qbvoglet.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3tedhmarz.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3eogwpjmq.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3iphdlkgn.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3pkjfuohy.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3hiqigfqv.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3ijgbcgkx.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3kfbbvxfw.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3shbkbctm.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3dovdskyt.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3pcmfjlqy.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3xozhycdx.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3cdipnoec.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3xjdwttgj.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3upqoqeoc.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3tvyedqiu.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3rlzkuzxq.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3pmmryhev.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3njghqwpm.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3htjdsump.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3nastszmm.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3yujlswje.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3abhixzhn.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3azlfdupy.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3whafrtgu.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3sczmkofl.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3mktdnbeq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mojunbjy.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3kohndmuh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yvsnoytg.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3yqqhcbjd.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3irrtwwgz.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3qhlztchp.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3mftlncmp.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3ufnmnnil.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3mmjszsdn.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3tpreqwua.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3qwzneshj.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3uxbcmewq.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3wxvrdmvy.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3zwgsbrtw.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3meqrjmth.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3ijdljlbt.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3rgrijpvf.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3mzvstgtp.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3grtjypmo.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3hcprzyem.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3npcuydqx.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3isydnrti.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3eybsdtap.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3aoifldqr.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3vjtlfsvs.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3yrocceud.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3fizsfhih.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3egyecado.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3sxpjmdmj.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3dpoxtbvh.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3hwghohra.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3xmqrhxbj.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3viacpygk.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3jholxaqx.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3rujaqqnm.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3gekcnadx.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3kclonsff.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3cxggclzb.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3hkjxeurv.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3mdauhdmd.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wfnsgpsl.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3mvnicznx.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3bglrzapo.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3fdkfpnnh.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3bmzomswl.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ikwpyzxy.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3lttmgvis.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3clqyjkbb.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3aqbvzjdx.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3biudzkch.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3eqvtwlbe.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3frhgsvpo.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3ulitbsaw.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3qnizihtf.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3libsiqgh.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3ckegzxwr.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3wbecvyav.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3wpfgmyaw.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3jvjrfcan.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3ihshrtwy.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3qttmdyzq.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3jjyrkwmv.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3mrpkkmbd.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3lurkprlw.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3ewpxkakf.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3mnoqiegu.html


<!-- 参考信息 -->