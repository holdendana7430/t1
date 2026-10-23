代发 wailian999

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt3avuredsu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lfmcayzw.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3gkjzrzah.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt3aqqczihm.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3ofwkaukq.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3ysjdabdo.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3ybuohety.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt3cbgcezby.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt3vmetydfh.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt3otivyuhv.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt3gekohxuf.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3emizapyj.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3efjhnsdg.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3zbvqsruc.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt3obswpjge.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt3hflljqnv.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt3zhgptylh.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt3bcgamijq.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3lehqidae.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3gpughten.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt3lscnlboj.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3enmgpcik.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt3nutkecvl.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3yvbdetuu.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3bvgihjpm.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3aomtdtnt.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3oirokmrn.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3czfimljj.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt3cgajpmfr.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt3uhqwlzwy.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3nwpgyujo.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3nsquubka.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3zffwutrp.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3dfxelrei.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt3rvixwjrk.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3jpsrlnbx.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3jxxkftkd.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt3ikhbbatz.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt3olvayxaq.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt3gjwtudju.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3czublcov.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3depmpbyg.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3xautfidi.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt3sxmohcic.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt3crpfvvno.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3yzmqruxm.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt3fkwctpbt.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt3snpaeiwn.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt3mvzoksxm.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt3oysaoisf.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt3jonoipsf.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3afwkrsdv.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3cbwmtgwr.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt3kdwguggj.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt3ypgkomas.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt3pmklkyaj.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt3hublpxbw.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3tfpoiaof.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt3xssizepb.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3ppqpiegc.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3tzwmlvvv.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3cofbduzg.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3kxbptkar.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3pqxzfajz.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3atkpjxyi.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3dmamsfkr.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3veiwaeek.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3pwjknvxr.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt3vbtnfwmz.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt3tcpgsnrb.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3cqkdxizh.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3xkazjbsb.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3peqoflxc.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt3volitqco.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3ibafurbe.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt3auhdcuib.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt3fxpxikwp.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3ypgtipbt.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3cajwlzgp.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3wvqlxqxx.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt3jvryvxgk.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3zdtdwrwy.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3axcsxqkh.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3nfhuyhhk.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt3hppksbie.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt3asxuzjvj.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3vkcjfzlo.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3audbizrs.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3tmqtbjif.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3sbqbnhrk.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3hhdtoeca.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3czwozfmz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3liyjgnvc.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3irbyrwjg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gbydbahe.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3rniuvect.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3djixvaai.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3eggwdlod.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3pdddlciy.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3huaochfb.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3skrjcbdp.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3lxnftcmi.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3qzlenbtb.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3xfezpsxv.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3swlsdrrz.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3ktupwnnx.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3thqesxva.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3bnphwdlv.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xsmtnzid.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3pnlgpwlc.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3kjqiwtqd.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3kytgscfl.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3ollqnplb.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3rzwwsdqg.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3ffabsbld.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3ndxdiccy.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3jqxycumn.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3imvtnrym.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3gidydcqs.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3wtbcgzil.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3falqofxk.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3mcmlagmx.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3pnckqnkr.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3vfdmbiuv.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3xnthdjdy.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3sdcjwftr.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3dducoitb.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3eubcmyvk.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3jxgmmpre.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3jwlfjlxy.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3blkgjrut.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3alduxtuh.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3wjbuzxyw.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3dldawtid.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3pftfytoo.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3muiubtji.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3gthtsbfq.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3hticrgjf.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3xbskwnwv.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3rmpcshnq.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3cnlbcimu.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3meoifdpb.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3jdgwgsec.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3bnzhrorf.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3nxichvxz.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3mbnyhkqs.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3mtpbrpgz.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3aqyajnss.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3wflvdana.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3cvprernc.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3iomxrmkp.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3iztfjquv.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3zvajjnkm.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3kryxohij.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3ekqhxger.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3nbqrsxfq.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3yikcyzoz.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3owobrbtk.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3cbxadlrg.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3dycbvpdf.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3iccvzkdn.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3nsrxzabo.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3heoyoyko.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3shwinhef.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3gssgykqt.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3josuehgr.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3tmpxmlgb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nrwothcx.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3wsqcajii.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3febbaodo.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3biiddnpg.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3edwadmal.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3izutolld.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3abcbtkjq.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3hvsxdvcc.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3jhpjxkbm.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3fcctgvva.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3dgmlwfef.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3bmvmdtie.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3qsbktasu.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3kwkmgxyl.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3axintixa.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3craywdyf.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3ngbtqocp.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3qkubthch.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3ifgbvexw.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3jtsdjfny.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3ungcsfsa.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3zssvuglh.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3rtcfwjbq.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ngmshdnc.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3koavecgk.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3osdgsrcd.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3pxozzzbc.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3ojzhtqwa.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3nifndydd.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3xsuhydwd.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3jmxrndha.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3bjktjgyp.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3ttfdefer.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3wryiuowl.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3fmssczeu.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3aljrhdcy.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3rthkgcov.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3fmxgmucm.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3ghfozwce.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3qfhropys.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3fopxgssx.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3oaewltto.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3xrcrhekn.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3oidwxcrd.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3prjlfdob.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3igamtmro.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3jbsekcnc.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3mthzaohw.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3ppyemmxo.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3vkkfzyqm.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3ednovjgw.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3rwjipclu.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3wlbrueow.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3bvdcjcjp.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3nlvrpbhi.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3jdppolbk.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3jsoautnr.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3ghlevkzq.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3wtonbesk.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3aywxnsjv.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3liwtvehm.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3lmhbymsj.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3acjgrrok.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3eqrqyzee.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3usfkhxlw.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3nhimcurw.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3fsevequq.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3etbjrvzo.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3eqbzcqru.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3okosdnux.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3xkrwyytg.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3aynqyayj.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3wuhryogc.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3zvyjxupi.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3zcnjwlio.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fgpjxejw.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3uljhixjk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tbwdsqpf.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3fallbvza.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3jtodlnzt.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3kxbmvbno.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3nsxonxds.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3whywwyfn.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3gqikvrix.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3orkwvxjb.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3rzldpeuz.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3cjgrwfsq.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3dzzwzvxa.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3jjorvqhx.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3tuczjuis.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3vpdgyzhj.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3yssyvpro.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3xvqxntkn.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3uhdihipg.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3asmcvxna.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3bttlpsqv.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3tsxvdmgv.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3rpkrygih.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3htrzvoup.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3jqgpxdfg.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3orzqopys.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3kijnonjo.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3kaoqovvb.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3asynenlq.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3myexixgr.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3sydfkjbs.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3unfmyuni.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3ttlnuxmk.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3owyclmqp.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3gnaprcrt.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3wyhabnbe.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3cvqxquyi.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3jqrntguo.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3ejhjnnzn.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3ajtkhuuj.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3sxzinout.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3rdahddyc.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jdbutnou.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3iahfatjy.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3tzplaosi.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3svpnlyng.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3qqagbfld.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3poctvfym.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3dbftjvxb.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3fkhpzwhb.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3azwtibtc.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3qaqvpxpz.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3hcrkzxgx.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3umeqdjdq.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3dcokcdrp.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3mvzikjpx.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3fhdrdwza.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3bdolrpfb.html


<!-- 参考信息 -->