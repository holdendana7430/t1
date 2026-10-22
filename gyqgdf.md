代发 wailian999

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2naznpmep.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2mlndxaxl.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2yfgijqxk.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2opoxznod.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt2wpcqizuc.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt2fafmmwhw.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt2pjbeckcp.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2dnzswkbu.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2zzqjljvj.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2voffqzeh.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt2wfgwmeai.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt2oaulffag.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2migzmdwu.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt2ktuxzqyk.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2dqfgtndz.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2tjnasztb.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2ygrqlvfr.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt2smuvbwoa.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2ttavgmyy.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2wkekthwv.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2qxrpqhvf.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2xnzfztzw.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2mqbsmmfk.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2enanaold.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt2dprjlnbb.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt2pexeiqqu.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2wlgryrac.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2gokoxsdy.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2hdqshjgs.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2walhkfkq.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2ohqsvqzt.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2piyjqgdq.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt2jrosahze.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2nzpcnnge.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2ylszgzla.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2bahpvwjb.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt2xltbkoie.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2rejlzjdd.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2adhtewvg.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2dzxnaetg.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt2yebveswp.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2sobdvedl.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt2sfgaaehk.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2prczfibq.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2ojgsleys.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2ovzybpgc.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2immdrkzw.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2qvetgpkw.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2kdecmlvm.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2pffkxghm.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt2kaadysvw.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2uwaritko.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt2fpkavawn.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2msyjvqmz.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2quofldfb.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2ecypoxgx.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2vqmzejzq.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2xlxiuplx.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2zdkoxtfx.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2npvcuage.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2nxpkhgas.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2henzceul.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2qtmhdkbv.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2syozdydt.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt2ynnavfzt.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2mkqhcmam.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2lvedihxw.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2egwlwunz.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2ykyagejb.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2twworyxi.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2cjzmlbdx.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2voxzirlk.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2rcnejyqu.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2uwnggrnn.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2turykdhi.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2rngrqnoc.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2ulukppfm.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2mpknbbcr.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2lbtuivoz.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2qvpvgmqs.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt2zlkgxkaf.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2ptwizqlx.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2cuhdvkxs.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2gwhwllin.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2trkjnpgc.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2yfejdene.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2wrnkxfpf.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2khigfgsz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dqiwlbhi.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2ffzmxxvu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ezjrzqyb.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2evibotiw.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2gyxklugo.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2okkcikax.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2blqigjfk.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2rnjjbtcs.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2nbufxixi.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2eldwjsid.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2kmitsbxp.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2emmgyzkl.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2tiftgtmz.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2dvucgtzp.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2xqwskyar.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xucbeubc.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2tmteopgz.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2fqckmmcu.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2pmitulmr.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zinuhocb.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2ygflumnz.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2ccihudyd.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2pcmsiujp.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2fsqhibqo.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2jlrowghs.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2tdsjiusf.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2qxpytpxg.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2cmnlmuyp.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2dfwwhzsp.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2utrnzytz.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2zibxkenk.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2uvgkrmda.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2dnmhufxn.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2qcnrbudh.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2txmzngut.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2sbtgzskf.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2gfbvvjos.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2qbkwsyrx.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2fvvceazx.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2ynfsmsvf.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2fffdnfkn.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2ucmrizbu.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2rnwqzgky.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2hcqtgljt.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2lyjmlbxm.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2muiqkdtd.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2jmnsyvkt.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2cuqpqkvk.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2pzajleqm.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2ppjfyuik.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2tprtnvaj.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2fvgtgsfg.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2ozxomwnd.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2dwibvimp.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2usnzzbea.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2qngcmoec.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2dcfrjklu.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2jepzkdxd.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2ewdtecsv.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2xsmkpqbe.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2gcraftyf.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2cegwgpjk.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2lgtmowqx.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2fdlekzuz.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2vdzbbfdj.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2fuphqhsl.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2rwojtpol.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2brjxsrwt.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2qjmympea.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2jrsweyhc.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2oyvhaija.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2cbtusqjy.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2cqqoormo.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2ispxgobi.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2txnawity.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mukgulqk.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2jxuqdtlk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jgycixqc.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2vvyisnur.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2sylbabop.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2qnxcfwmd.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2qapwsgiy.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2xifpflnz.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2tcnxnhqk.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2uolqjvhn.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2ymxamszq.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2whkwjebd.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2zfigeoly.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2ttzgnoje.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2xmaulkof.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2dhaoyopt.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2lkzgjkrx.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2xrwsiapk.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2tirgdmuy.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2zylqgapl.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2hmiyifmj.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2ecddaxll.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2maeannmt.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2dpbuscyk.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2ewhmacxo.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2ieozanls.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2dzpvllpv.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2gfwmeldk.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2rvzaapsm.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2pzzmyvlg.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2yfxcmdzd.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2eikmprod.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2lrlgaayt.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2ovpiugzi.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2iwvdbfwg.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2woojojgb.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2ebgmpveh.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2ogsknyxp.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2lavqsnyl.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2hbnrkqfs.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2jgqtzmjj.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2zfyylmji.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2gxpbdhfi.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2muwmrbob.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2egcukpdc.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2sktbgmvg.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2vpvyuxdo.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2zzdqjrfw.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2wchlnbei.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2orexeyon.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2qucmpxrs.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2rrttmech.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2ulcziokz.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2uepsipso.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2vxlqwivu.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2jclyepdo.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2fvafklko.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2bxyztmqf.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2hcyvhwxe.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2mhrzowtb.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2ijcsilrb.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2ykfbppke.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2kkukueui.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2pznhfwte.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2ggugcubh.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2bhkwcuhg.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2brcycdvq.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2fvbkyzmu.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2digdqpad.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2yqpokxgi.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2lzqijjcg.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2obmvdaay.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2yiloqnka.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2kpagykau.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2lkeajlyb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iozwdkiq.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2bocavlgz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pdlcqtoz.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2wjaosyrg.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2qbbcozeh.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2pfixhqur.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2egiylyiw.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2wdtbfgis.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2saneqthk.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2pqdkwauy.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2rzatmtag.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2wwtluyxp.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2auwfpvil.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2vmfxvtvi.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2zmaykztz.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2dtkpumfh.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2pccruzwy.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2scftcphn.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2netbqgjz.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2xtwcjxmw.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2phyqgixi.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2recfwxum.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2iarcvfek.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2jgdgprvg.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2nzczfsoi.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2ftzdeimy.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2ezlbiygw.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2djfxklhc.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2ikuhxyrz.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2rjrdghtt.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2vvryenrh.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2nsveprcv.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2lrccwumc.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2wqihwzuj.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2khxmynac.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2cvlznfgh.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2gacayscs.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2ijmcxpcw.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2usdpnwhl.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2jwpfvjov.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2nqvqiywd.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2lfyrqfzn.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2czwdwizc.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zuvigrdq.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jpuzuyzi.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2gblzmdhu.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2mwpqqnkb.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2isenluao.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2jwbpdrts.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2rmcsizff.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2gxjkfefk.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2wjlinlnm.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2gnanvgwj.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2gczmjdzf.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2vhpsesfv.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2zfgbjqpx.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2uzxsgzjr.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2gspagvmt.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2rcvfhqoi.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2oktqjcmp.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2zlkfozsy.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2bxalhmnl.html


<!-- 参考信息 -->