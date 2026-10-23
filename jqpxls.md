代发 wailian999

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt3hwdzmuni.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zafudkys.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3vjcpxqxe.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt3vzgmzrlr.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3kfpgfcdu.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3wwcylxjk.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3luqmjjnw.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt3quflmzhc.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt3lgymogpt.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt3kmuixbkb.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt3mlxdimhv.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt3megzqxaj.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3hskasymm.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3omjcodeu.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt3gvhstqzp.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt3kjyjvyip.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt3doisajww.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt3qgbjilbo.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3cbdwrkfe.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3sxpcvlpa.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt3ksbkswya.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3cwnnnqfg.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt3suttdzga.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3weatekdr.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3mkwiqrfe.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3cpbydnry.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3digupeff.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3uxyzslaw.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3xkpqqyea.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt3zlwplxte.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt3muovmtva.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt3fvulzvya.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3obsyqmsi.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3uuytfbhb.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3qjcycwdu.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ytzoudae.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt3ounuxljd.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3wzcssrng.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3qdpieoxs.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt3uanqfdrf.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt3rqtvlidc.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3dzvtmxun.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3omaihgar.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt3ygwxzwyc.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt3ysvojfur.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3ttdinvui.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3oksrngzk.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3lhgkmlem.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt3yfiobzou.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt3qsgvspwm.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt3jcazglel.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt3xibdztuo.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3qladklho.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3ltbgatoo.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt3olcoyigw.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt3ddcrmekx.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3xfzhocnp.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3vzmqddrl.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt3ocpzymic.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3wovfyiga.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3efcbyjde.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3nkslcpmc.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt3hiakjute.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3kjwhntjn.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3xhtvqgic.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3fgtmsijj.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt3buozdric.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3zqauidnh.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt3yxookofy.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3mnmlolzj.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt3phzebroj.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3fjglhngo.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt3hilyriwl.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3vwwwsnbo.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3nigrcabx.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt3jvtffral.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt3lyfcstog.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3xpasqdpy.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3mtbsauwg.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3psloipxe.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt3lyaywnua.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt3xdoskuyf.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3cmmdwndt.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt3ejwtjfjg.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt3sukpeuvw.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt3dvfpckqu.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt3uaincwso.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3ojbjwaod.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3hmvlfowc.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3ilroblwb.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3jcpnxbmm.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3jtlukazs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ebqdkqsd.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3ptdnbmko.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wccibxkv.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3egbmeeiy.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3sioifuij.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3veunuuvn.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3xmfaqnuz.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3niudgvzg.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3kqabpfmc.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3htcwsgdj.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3xqhjemmu.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3tfzhvqsy.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3oqlluuov.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zcnfypak.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3qefwhfdn.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3tsexztjd.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3qgoaqqfv.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3mnnlatwe.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3dfxkxaus.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hkskeawz.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3gmrhodjf.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3vvugwimm.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3wywhjmtw.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3mekzuhwa.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3lkidwatw.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3pscqtpai.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ccgqmwcg.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3aunssvqw.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3egudbblo.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3thaajcpx.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3nskqwepm.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3pidhtuhj.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3qhajbvkh.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3pfkjvsjv.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3dhsdreuz.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3niihqrfv.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3fkpizpcr.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3mejmngqz.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3ewxawmka.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3lwivimcj.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3dwdxnzji.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3ozyogjud.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3bsymkmmt.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3mgxstrsy.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3dggzvmet.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3rfieghrz.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3ygemlhtf.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3tpndejvu.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3uocssxgx.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3oohedpxo.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3kpfalygp.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3oylwrttu.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3icxaphri.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3ildlwlfw.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3nnqhsqft.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3ligqnnhc.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3takpqvoo.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3fmzcyrkj.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3jfkbltii.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3jzjwqiuu.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3idijllrn.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3vigvpnrp.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3potpmenv.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3nfjrcetb.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3zklbpfkj.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3tpqmdvnr.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3kawtzizl.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3uwywiulz.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3ykijjhtw.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3niwgkzuh.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3faohniye.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3kuxvqfkv.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3xetwmumy.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3zvuslfyc.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3fxlvexjc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jdphxbvk.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3bhvquveg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xewgilcw.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3kcibhodg.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3ylgdehpk.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3urxezufi.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3yiwooipe.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3aeppwvhq.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3rrugriag.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3civrgipc.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3ytdjxxzx.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3rckitccc.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3wzjnwrdl.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3asnptksz.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3dfyxblcy.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3chltgyfp.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3txigkpjy.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3jhshofeu.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3racfmply.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3lvvgcuzu.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3qoponhda.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3wwqretho.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3ssuqeymi.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3pwjtaofw.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3cnbbxwzo.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3whsuavnz.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3gjfkdwqq.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3lesxielz.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3dcoyjrjh.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3smsqhlxh.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3vuugjlqx.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3owftavib.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3alfukcez.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3jwobbraf.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3crhpduad.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3ulpovtgq.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3upfxezfg.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3jgakiiov.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3nlvsrkpe.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3lalgofny.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3asbjyzcr.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3rhdibazo.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3xzdunwzn.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3exfdjrkc.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3bhjipeqa.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3cygqfcea.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3dssuqjps.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3lbaczfdl.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3vnehcntl.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3lszmukpm.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3ytefvbgd.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3flkwaxee.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3bjxpylyn.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3ldbdufgg.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3rwozuzoy.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3nwnsppny.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3cdhgejsz.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3elfstinw.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3srwnwdgm.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3cltuxjuk.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3eydzanri.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3yjowurfl.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3mcjjafqn.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3qmdcitbf.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3ewjsfhul.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3zsunzbmj.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3fodnuibl.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3ysrwnxgd.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3obcfvqcg.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3fozggdqj.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3fsferfqt.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3ziajrpvw.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3ukirmmmf.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3tuxzkave.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3kklxbuai.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vaindpvd.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3jxzsynvg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dckmbgcy.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3iddgzivj.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3fjzskmhr.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3buqcxehv.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3ctukgndy.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3belpldbr.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3trgvbgmp.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3yogvxwic.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3fywiuhut.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3aashcexy.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3qdtruvwl.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3onfcgvbe.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3lbzeatlv.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3rzpwbzee.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3syjjeasn.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3drzwauem.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3dudfzktx.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3majdrvwx.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3yfpzekfc.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3vmrzixhi.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3hcnviwkb.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3hfsuzmml.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3zfknhzlk.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3zupzatlt.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3kliyitrg.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3sivryzwv.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3vmuofawl.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3icgrjtoj.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3stblsnyp.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3xofztqih.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3bnpkmnvw.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3mxaaamti.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3yckxsfuz.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3kxoygyqz.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3hbsxqebp.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3cakbkvqt.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3tycfgrwe.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3lwdajdtk.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3nnrfqdiw.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3ukfekiiz.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3rpwqiekx.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3xroknvdz.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3oujhbwzz.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zpzdasty.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3xnmvdtks.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3qeuwgmto.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3kftcmamq.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3hfjgrpah.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3bzuvhnfx.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3iekwckxo.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3bdfxhalx.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3mbsdingt.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3owckxogb.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3wclzxagu.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3rfrapbuc.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3ddkbuvfl.html


<!-- 参考信息 -->