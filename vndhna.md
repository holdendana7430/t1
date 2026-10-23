代发 wailian999

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt3sizlpiir.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3puaafqvk.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3hledepuv.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt3dhsgygmy.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3dwflzjbd.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3ctkngnrc.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3vlfmlmih.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt3lthzssko.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt3sdrfkzid.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt3hlryvcvr.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt3loddsnrc.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3wweieumm.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3godlkrqj.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3uewemsuy.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt3ycepynqc.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt3iziyfvyh.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt3acumvhpz.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt3fapjjsvd.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3bklzgemr.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt3kolmgdvx.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt3gtjwybxm.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3enhyyauj.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt3xkumimvs.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3crrpcaoz.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3mohzlcok.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3jnrucmjf.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3fmhkicax.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3mmfqepez.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3xvjcknwx.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt3raohsczh.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3lcowwdgv.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3jdgqfeoz.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3xntjgxam.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3rppxvylj.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt3uynwvqlr.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3zgzcphco.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3ofufkrfj.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt3yvuiqylq.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt3durxifnk.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt3znegxqzg.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3qbhojnhw.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3xrezwudn.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3flaznnlp.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3klasncmy.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt3fgiufcbr.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt3uuqrrmwd.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt3rehocrzh.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt3xkqtfxzw.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt3aangghgp.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt3crxbvphx.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt3bmzjpfkk.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3lhbizrsg.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt3xjgagics.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3klwqlbmj.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt3auluoqhr.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3zzrdbzzg.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3hfyrghjh.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3fbwulreo.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt3wggkpwxx.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3qeejsgra.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3cpoyrvwy.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3otwcyigc.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3zamwfwlb.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3apymefxj.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3nxyptvmh.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt3uqejbccl.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt3npwcxfaa.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt3dqmsrowg.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt3mkiezjbs.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt3czudohdz.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt3wzfgoibf.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3qpasldzu.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt3vfyjclmd.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt3xqcitnsi.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3foiurbkw.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3cumxukci.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3dittpeph.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3icypczas.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3dvhtafmu.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3rnsozfsg.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3qjbleyms.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3yzgmdqrn.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3yshpmxnt.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt3rzmuvadg.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt3rohcnazl.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3aaapqryq.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3mqrqytsw.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3efbqnoge.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3nowxnrzk.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3ufaeislz.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3nwtvnghh.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3upyqlamm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ktktrhna.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3ljskhnkd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ehaywvsx.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3tnxnvgtl.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3aiqcnqdh.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3ooqngwsx.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3wsnzojph.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3mxkyzgfm.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3syivptsb.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3dcotildb.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3kuaiprng.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3kcoudwvt.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3glaynmny.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bdviuxjn.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3thcqgchd.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xzcsebzn.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3xmvnugfe.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3qlzszmji.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3dqqfdvjg.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3onjxxdsh.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jyorkeqe.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3yptridpo.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3qhukxlnc.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3teczvtma.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zabmnyrk.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3fsbbcfob.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3yagqwyeg.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3tydwxmrl.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ekqfzbwa.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3cxgrekbw.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3sszyuatd.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3yyzxzhvl.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3uyegravv.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3xdlrbdea.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3qwyoehuz.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3hinirphz.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3tgtcbuue.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3ptqkteow.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3tzybxsns.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3ylqeijss.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3djkdjcvm.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3dqjecxtz.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3tspxdofx.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3tygrtqsq.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3dzktpxtc.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3qfqjriae.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3zjqlgcxj.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3szfdhutq.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3tzamfifn.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3rdlrnffi.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3cumyojsy.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3jrwgqdkf.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3nxjkldqi.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3arhaddoy.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3bfwgnyrd.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3bmafpmxj.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3hsnyekuz.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3wcywfpor.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3gzhyaxbh.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3svtajisw.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ycxpnfmr.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3kltvbiuq.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3cgswmisq.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3hsgdxxyg.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3rcyjyakn.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3phrpudmt.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3ueteheow.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3hwgfdszb.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ktnidjrq.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3ippjwvjk.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3eeokaerv.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3sigvojdn.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3igalwyso.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3nngmflyx.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3uiveimod.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wjnlwwht.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3ljatuayq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dpulensr.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3zactzviu.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3uyersdri.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3tmxulcve.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3dkjtspvs.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3idvousez.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3jcurkwev.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3sjemwefs.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3reywyepi.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3icahxtfz.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3uaspmnkw.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3hcjthkex.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3fjaeehjs.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3oqrxephg.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3leunlbjj.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3nqtzlwtc.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3krudxtxc.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3rlnfjxhg.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3cwbgjibl.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3yyauawfr.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3oztxqbra.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3mthonkds.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3fdbvstog.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3soxcqvlv.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3wriisscm.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3vptsrntk.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3vteakfik.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3eurmydkd.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3alyelltt.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3tmhjqbgz.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3hwejtmyy.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3jusuddnm.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3qlxdolyp.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3ywwprxbp.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3dpvgoksa.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3czxinzyy.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3dvkpfnzo.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3kugduafs.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3oolnmewm.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3cghelvvs.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3fckgcpnd.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3srbocszl.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3powlkskt.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3qlshplwk.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3cvxisojo.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3czwyefyg.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3pvwmorax.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3cxpgohva.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3hneieisr.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3rtnfkepo.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3uwdsenqk.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3mijfrbuj.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3ohsooaed.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3vmwozsxs.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3kzgxrfac.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3utimrkvj.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3rrzlxlzt.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3mojwyxlw.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3iqlvpknn.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3coxjiajl.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3rsrcoquw.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3vpinbluu.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3ibjjdnus.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3jujnlovt.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3tisykaah.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3amntyhnk.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3adxlrmxs.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3sixouido.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3ypjrqqbj.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3siudnsfc.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3xwohsjxd.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3favlccuj.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ggjyslvw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vecwljmm.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3fxljvfon.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jwgsbpkk.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3vjjtkicc.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3lwydedsq.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3ticrlqiz.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3gnscdusk.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3narxbqac.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3vkiqvlkw.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3dmtkwlmn.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3tomlussa.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3haidyjze.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3zwtndkmt.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3rrgmfqym.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3nexjlnoz.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3lpwrmmby.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3vcmlbzja.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3oqxhqsrx.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3qgphanvy.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3rnhakrpi.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3vesurtjx.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3cvpuluzy.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3aoqcfkjz.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3cdkzcfhv.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3ukhnqysh.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3qwdaltqg.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3mxkirsef.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3xhcewagk.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3dzqgpegy.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3vyzmtlcj.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3mvzucjca.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3uhtjjtai.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3irwgjeke.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3wbguurnh.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3tikqatux.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3uxlalude.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3tkvhstrl.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3gpyjxwdn.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3shpfuagg.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3qaxxlejr.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3bnrpudgg.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3mpsrzoyb.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xoovxhtx.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ugcgzyuf.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3pcrrlvlt.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3zjrmtpah.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3faormrme.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3sthzimhw.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3ykcvzqgl.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3ytzctppt.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3rngvjjvh.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3vytmzmzx.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ukmmpawr.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3qmjzejaj.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3mchnqvww.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3qtokgipm.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3cohhwcxk.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3cnajqtmj.html


<!-- 参考信息 -->