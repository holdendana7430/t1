代发 wailian999

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3wstpnqoa.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3feegexkn.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3hlimxjrt.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt3rojdugse.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt3qfveuopn.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt3lymysrnw.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt3qwqqfcvr.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3zlpcqtyt.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3wsraslhc.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3frnzuyde.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt3gaqvucbp.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt3saatkriy.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt3pbrosnrr.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt3vpgrrpxd.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3popsxdkp.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt3xxhqbbge.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt3khmoyxlh.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3ctpvybit.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt3eetwhyyk.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3hdhdxtok.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3jcmvrdri.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3qzbmggim.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3ffhgsdkc.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3nmqjwolr.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt3stboqovj.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt3fjcdplxs.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3cwfansjh.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3jsepjvqt.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3hmzwtzph.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3vvihduhj.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt3tewwxtzd.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt3qasljauh.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3wujgunmg.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3knxjszko.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt3ttmvaprx.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt3lafymnmr.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt3kxtywoww.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3hifpbxec.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3cgtaoggz.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt3mkbhaowm.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3egwaoiae.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt3zhekapso.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3uxpujytv.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3mgbntkka.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt3leepkxhl.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt3rpxmburx.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt3icibsgqb.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3amrovaak.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt3ctwabwzu.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt3cxzntpeb.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt3bpspyari.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3zkpwomgm.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3sxpqrknw.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3sorlyuoe.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3fmkclmeh.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3ypfufxgm.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3lqilmjbk.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3ycpupwef.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3wgjxcoad.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3rglhltyu.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3aiajdxnd.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt3ulgdacqa.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3tupvxahi.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3esencyfl.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt3neirqxht.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt3itlkoztb.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt3ixqtdxxf.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt3gfdunfbv.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3qqibznje.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3vdizlwke.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3pzycaqdm.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3ysvxufje.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3fxkvvulg.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3onsgrgqx.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3pvflblrx.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt3abgrmhsk.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt3tvpsluvb.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt3hyoizxat.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3uonepiwx.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3amradfbf.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt3dnkpvbzf.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3kfrircjz.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3uwlzzeth.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3addcozgj.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qneanrdh.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3aiekkmop.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3wuojtoiz.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3xqtvsxvd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3muxtcpap.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3tlxewqsu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gkvbvzyo.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ueempxua.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3vmrfojkz.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3algvdpqf.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3jqhekgts.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3cfempmoi.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3bgacjspc.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3myccvify.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3wrjudmlp.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3crumigse.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3ololyket.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qnifchqb.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3yrckhudx.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3jlsyogyh.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3tmfbsqqk.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3uhzffnuk.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3bpswdbjv.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3sbylwhcq.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pkotvuuh.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3qdwvklxc.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3ijtqizeb.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3depokmfj.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qtdxqqjv.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3tvrbsbkr.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3btaxrypt.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3arabkqtj.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3ltbsneny.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3ibnvaeea.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3klyqljat.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3pkoskzav.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3boanhmue.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3jdanreaa.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3iufqnskd.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3svjxrjag.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3ncrmirel.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3rowhyiqh.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3sihpxcad.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3jbktowfm.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3pjwqtgej.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3hduxriuq.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3obfyeqob.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3jxwhexaz.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3avpxjvzr.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3zkpcnblj.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3mvsxpwdn.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3vkgpdcqu.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3lkpvtycl.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3numxndbe.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3bhrhflah.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3svhmsdaa.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3bpjozmvf.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3cfcrltow.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3zkkgfklz.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3myrfsudw.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3hmzhxsmu.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3nmkwiixr.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3mxgrrtcp.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3qnkmdbyp.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3cnbbvktq.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3ufcefiod.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3kslyvucu.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3mmmlnayt.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3oqhkcfvf.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3weoebogh.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3opmsyepn.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3rxejvsek.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3yiuirugw.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3etoqdiry.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3cinupaod.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3oijjfdfi.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3shfdruhn.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3oxvmowjh.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3rafgjdgz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3glijqljh.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3fzbchvsf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fkbbozpf.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3yvloocwz.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3jqqkmxvr.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3dtzyivnz.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3liaeyffz.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3gzefhqhx.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3pdklsopi.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3arbozwgo.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3zdvbtibm.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3llbplzis.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3kzmmgkjg.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3jpvvoxxl.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3bvgukivn.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3sxfcxauy.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3cjmjsktx.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3dmqzpxbq.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3pehimqan.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3zjorrjmi.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3uytkvpnc.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3fxjemggb.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3idmsrkeg.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3dyuxzqlz.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3qaybgbyu.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3opuiddav.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3xyjrgkli.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3tqcmfljf.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3vznqftdf.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3nirlcdfw.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3rpsopkxb.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3kbksoxay.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3vyvqamdm.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3fqrdgsrc.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3haunaszl.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3jzhietzb.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3gebjtnyx.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3zjynuwnp.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3qvhppglk.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3klvwqbdy.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3onxkgjsl.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3ywzuopnj.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3pidxdrms.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3flqairyw.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3mijgqdnd.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3amcjbiwu.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3pfymnhft.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3frvdrciu.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3ujqcajdz.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3gwpflden.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3gbgetsjn.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3nueuexnm.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3ggcwvzbl.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3spbewjit.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3hcwnznfi.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3vxkhfppd.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3qbpfghlz.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3udpkpflt.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3ijcdfjph.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3msiuzyrc.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3nmwanypa.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3mjemzyvt.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3rwhamoka.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3bniijlxs.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3ekpirkbh.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3qkzhowpa.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3mpfgcozb.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3rjelwstx.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3nwhfndpf.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3vlnuryia.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3tgtjpqaz.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3yhxoktya.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3guuldkpd.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3tnktidgi.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ikndcgdq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3crcimofp.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3etulgwfh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kqbkdzat.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3pnflvhbk.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3zzbpkfvf.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3tlkuodtf.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3jbyirpbn.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3sdthbxgi.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3ibompbir.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3divpalbj.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3eriwerbd.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3ettzorgu.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3llsudsqb.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3ihhdfhkq.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3qwwfkhwv.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3ztozhets.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3oogdvzfd.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3girnxshx.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3lalrndtb.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3lmqiuyrv.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3iiqkyfos.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3sszgxmzx.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3rcbpsswv.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3vbtgzhve.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3ycmfkriq.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3rpjtlcvg.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3fnlsaevw.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3pihmdqmd.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3sxnvzxkr.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3migevrib.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3dlrdqyqy.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3hojosmgf.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3houtyrxv.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3tueenmgr.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3yydzgcwp.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3icazeqbj.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3jzjwckln.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3butflgvq.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3znujezfk.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3vfjcepju.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3tfyukdbk.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3yotttdxn.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ufhaxvmh.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ixygpvvd.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3aoylmnei.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3uknbnlzg.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3fdjgezmk.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3mmqxvcsc.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3cdjqsnio.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3qhwpxkqc.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3lazbonpv.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3dbomvuyh.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3sghtotic.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3phsptshp.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3oahywbxh.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3qstmvygq.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3iyratpel.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3nixvjhkn.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3bbpytqmt.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3epqqamuc.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3jnijlrfv.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3btzxkgjj.html


<!-- 参考信息 -->