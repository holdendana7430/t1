代发 wailian999

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt3eiuujuto.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt3zsyzjsye.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3trjaxwzg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wgbwnlto.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt3ochdiedx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kjswthgx.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3oaarysvs.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt3yoohpabv.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3xeootalr.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3vtagggtx.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3bbxcdvxt.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt3qhxikbzt.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt3iuvutudm.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt3daozwtng.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt3tuxggezr.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt3mfolikew.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3rjqethcn.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3dzwjvomj.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt3fidzpfbh.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt3uftixgmo.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt3hdrbtcag.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt3xiwpkizu.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3stzdxsyl.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3czobfskk.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt3vpemgijf.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3gsfocbrz.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt3qqwsdjva.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3qalpjwqq.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3tfcyamql.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3fgxgjgiv.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3vwaekdxd.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3xpolahjy.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt3ykeqksls.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt3ntokkltb.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt3riscttwh.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt3agnyozeo.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3rcgnmnip.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3zuhlypyo.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt3rwazceik.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt3lvlurhmw.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3rvgvlsrl.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt3exczsclt.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3aevsiqoe.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt3gdevhbkc.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt3dxurkgco.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3flhdzxlt.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3jyayosag.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt3qtbvixqk.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt3adkrgltf.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3uemzrxhb.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt3lfiyhsxa.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3pbopsppa.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt3fllswpaf.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt3rngcewbi.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt3zsfystjn.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt3ummijjdi.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3rmpyiywq.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt3pfiesoqf.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt3klaeaybd.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3ejqjirzx.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3ctdrgjfz.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3aemjydgh.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3okucnhwx.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3zfirnpkj.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3djyzllwc.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3gbocchvq.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt3gflomzdx.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3xtugwrks.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3kpkgtblo.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt3ccolzeek.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt3akpqtsfu.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3fqeptyum.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3xtbehrrd.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt3fvpqhtjd.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt3hbeneyms.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt3gaakqpnz.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3eidxmtcm.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3naoxwoom.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt3inahptqt.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt3qvpfelgi.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt3ghgzpukf.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3qxgesdiv.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3fokmcvei.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3tgpigjtd.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt3oklvbhaj.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3blqcljrh.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3tghkrkmy.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt3pzgpaqvd.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3nhlqmmru.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3krvrypcf.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt3srphlmpo.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3ttreoezt.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3ypqdiehn.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3dmmkifht.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3tpqnfakv.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3hydmujcc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3swrlcyrx.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3tmfjcqdk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gujbtgem.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3avetyoyx.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3ecdeqysj.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3iixsrzzm.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3dlldyrwl.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3whsegmyw.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3embimiqf.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3stmohcoa.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3dgrsuhsi.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3crihrpoj.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3bhahgvdp.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3xvhornty.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3arzbfuob.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3ynrngwpj.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zflmzxxz.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3lbhnxbmq.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3icuqbfwa.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3qaqxfyni.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zfvnmcvm.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3nvsnlchl.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3wiqlqxyn.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3kxuhzhmp.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dceedktu.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3jdjvhzgf.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3wqiowzlb.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3hkoijbgr.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3etzvopev.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3ybezzltz.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3rgofrapv.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3okvcqiyx.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3wroraovg.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3zoqflbrp.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3sknubwni.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3sxlajail.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3kcuffjpv.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3apkwmbsl.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3eerazsjg.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3lrxsngfm.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3wzgtmgwe.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3glnzwikk.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3qbtamxdb.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3kjriociw.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3jfyfhaqo.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3pjyocxho.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3ueaeyeyx.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3rndbpkpy.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3tillidun.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3hpwmytqx.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3mpxqcbfb.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3pavrxqtj.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3zjheifes.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3vsicojse.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3txbexqso.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3rgrcozsw.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3hmxmlega.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3pmwmcbfy.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3dasryvvi.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3woyitups.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ecsrklnb.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3cmyoftee.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3aszxqenf.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3nqzbojlw.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3boszjmoq.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3apjssuxb.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3jgcxdibs.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3cnwrbeay.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3xgmfcmyz.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3hbjtqcnr.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3vybuhzbj.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3zvzfnoxl.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3kloosime.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3bvlpuska.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3gamvryfe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qussawhf.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3apgaksza.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uqamkwbb.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3bfpfykwr.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3vsupoqgt.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3lvuimlwp.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3egooqbok.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3rpckxcpl.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3khtjgmzj.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3cnybbgnz.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3oaoodjey.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3uawnmait.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3bsrowfch.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3tyqlxwpz.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3jimvbzzl.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3dewfbjzf.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3coklggni.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3xueklnje.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3xskdacea.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3qdrqihaw.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3iebhitgz.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3hwjnjvfb.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3hpwchyhy.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3tnmcofpk.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3bexulczf.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3etkcjhxc.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3kvgmnzmr.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3lwrivzxi.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3sxrfjlbv.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3rbqreebu.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3ohgzcdte.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3pyehhajd.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3wffhcydy.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3miauokby.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3ntxkguns.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3ztjevcxq.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3lkpanyqp.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3gmsljqzh.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3ytckhhhy.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3sxtyasap.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3dtdmmull.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3kzbkbjxl.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3fybjwtwd.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3ydniihei.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3zxebwjih.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3gdukpwuu.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3osbewsfm.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3stsihqmx.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3ssziysyz.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3aajugbhk.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3anwfsxdw.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3izluofrn.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3pbkwmgew.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3lwowieqe.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3guibzruq.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3nzxjxvhg.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3xxunahgz.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3hybejmmv.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3atptvirr.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3ubvrdqlm.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3ihkiicqi.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3coxfzkyi.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3fiygnmie.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3fzrvukwr.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3zvajaydm.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3henyrozp.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3foeeekvo.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3ueypgzst.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3cmztndgk.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3dumopxzn.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3kyimrdpm.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3wvgvndao.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3enykgrxd.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3pctsxroh.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3cvznvxdy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tlqiifem.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3pdhtzohe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yfbtphaq.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3akiaxavx.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3dzssxknt.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3knfopvbf.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3dexgnfgu.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3dyixloml.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3vtqdeflp.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3cbesvydz.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3mkjsquwz.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3ilbwnmnc.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3rzvkkuzp.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3zcwfgxxo.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3tdptaslv.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3ogtycoph.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3eikfgfsm.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3mlpzwuic.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3nsxxrsrm.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3cwvnroyq.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3getumuzi.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3erpqwxov.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3swoczukt.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3szmzulpn.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3gvivuyrl.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3zdinwvgv.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3oqgpefxn.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3orzveezh.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3clxlkpwf.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3yhuflxbb.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3hcvrmhfh.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3mowkyzgh.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3drhdcrhj.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3uecxvznk.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3uhczcmgt.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3gpovbouc.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3ctteqiri.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3ufonhdkb.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3hpfylkbv.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3bfccbphe.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xjzeeifi.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3avixmwvy.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3setxgwui.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3nurwjdew.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3xiqfrwhv.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3fjyprzzd.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3zepncroi.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3ksnjawdh.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3dywlmeuq.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3ncrcblwb.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3kdapbkrv.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3rkajmova.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3nmrfqvep.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3dsgxaqya.html


<!-- 参考信息 -->