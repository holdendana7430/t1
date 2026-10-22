代发 wailian999

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2ywiumfik.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lrzkaazx.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2jysvqxgf.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2wckzhumo.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2mdrmppmi.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2hsnvcmxc.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2ydseyfhx.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2bmkiboes.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt2mwmdnxor.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt2bfaricag.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2bhouuzys.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2dvefmbkx.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2ykvswrye.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2qpbmfufu.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt2inprisqh.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt2wmnvtmob.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt2jnqiomva.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt2bfcyzimq.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2ghhogwhp.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt2syoitxxw.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2eeomueds.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2jnkobjod.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2agmncbwo.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2ufvbrjel.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2qgqsjgqw.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2xmfgivua.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2bnjoizlp.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2vjlwqvgw.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2jaikynot.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2zlzccafk.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2grzyaexg.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt2gwzbgydv.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt2zqmnsmlb.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt2kakrefar.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2hmynxony.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2hoatyxms.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2fadqkcea.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2ceswfdff.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2suwebxef.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2fqarwkda.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2ywgwxvww.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2ewwiiuzq.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2kcfwugzv.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2odqjydav.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2mczmyiqa.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt2oececxqm.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2yupcmtal.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2dftqzfes.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2fwhmlkai.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2fdnaosfk.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2tsiagwdj.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2vagwgtpc.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2sejonbdr.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2ttayghap.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2lwjplvcu.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2xrczpifh.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2aorfvlyr.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2naeywffw.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2dirnkqeq.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2vplxvcpf.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2pcwolgfc.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2hxaacauh.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2wgbmnffl.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2tdzofnvq.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2scuwxpvy.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2ocutmjoo.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2qtswyunc.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2wuhadvio.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2nxbmbswb.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2ayscnpnv.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2tdoimezb.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2jqczreee.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2vsyyrqge.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2eflapjmu.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2huuocvvi.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt2zucsghkd.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2hhrlsmog.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2tbjcyiuw.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2azggtisj.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt2jbkrheex.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2ocdrfiwi.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2iaddafqe.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2skqhmldc.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2rvbowhqr.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2cxjfkbdt.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2lilvqtjt.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2hyekejep.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2yihpzqli.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2gnoufcrl.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2cfsazrvv.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2sxcjacsk.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2lckfvxij.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nwpnknrc.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2ewrikmck.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lcderrft.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2jrfzksvf.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2hvxfhiwx.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2mtdgerar.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2pbkzzjrw.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2fcejtowy.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2xuqlbmys.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2nfapmjxe.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2mmhbkczx.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2sqgjxyhc.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2ciyouchg.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nfrvwjpw.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2phhmmzqw.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2uwgbfdxj.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2emliwwoe.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2nkluhziq.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2idenzqmm.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wbliajnm.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2utvmglwd.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2lyxglfer.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2ngmybrxj.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2uthxwbha.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2bgnbmsed.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qkqxymuj.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2dpdziwrq.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2atjgwaxk.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2bovckuyo.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2sdwnydgb.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2tzsuelod.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2jzbblpgq.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2zvowvzwc.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2msxhddza.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2inzdusym.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2nohqqdvg.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2lmcrgyqh.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2fjnqfqbq.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2jvyakyti.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2awubagnf.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2gxohlueg.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2fadcgtyk.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2kiwjfjyb.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ywcwsmvc.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2jgzfmfzt.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2bhrpemgs.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2ooingzhu.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2ttearpil.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2gqoeoatm.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2zypaygzf.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2himqircq.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2cjugehjd.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2gobohgbr.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2omekgfla.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2pftezxxn.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2rmygevhl.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2jimqmfag.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2lncgdljr.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2zuieqkzr.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2zuywxgjj.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2oayqxfqx.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2arwhzieo.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2cryzxusk.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2zegxtrrq.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2ejvernit.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2xpwbvxhc.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2bdssgbyi.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2mmeopyqe.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2ixliocjy.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2oepqybpi.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2vqlrqycs.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2hwssdkdz.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2getxhdry.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2dhqmwmkv.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2xgdssjxi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zcvmbmpx.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2aicoaxkd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2flgheocb.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2juyybkua.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2ksnvgnqh.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2xjqihlqf.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2yuavhhpd.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2cmsrugzn.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2gghanexe.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2hyewdysw.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2zuydzxyk.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2hkfxbfco.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2ygcbyxxh.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2fpgjmjif.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2tzyhregf.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2ehdilvvc.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2kxgyahyd.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2wtkzwtkb.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2ptkihrei.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2xwrpdshv.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2swzutxuq.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2rpnviesg.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2eggzhnrd.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2pqitmied.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2nvznuxqf.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2wazjpaju.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2ytwcnjrw.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2tuouuvgd.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2rbzuqjfo.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2zudyidcs.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2chpxnnwb.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2gxxuunlu.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2kofkqlhb.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2sooibvji.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2tfovqzcb.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2vubnxskj.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2xorzziti.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2fzrnguyk.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2pstrefgb.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2nxvmhqsd.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2jehjgdqv.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2pyyopufe.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2hzxnmfwd.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2betpdedn.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2nyvcuucr.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2dzolbtvf.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2kxlrutmu.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2nbnuvtas.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2zvienrzu.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2qlcvyvlw.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2ymatzeyv.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2aoblhlez.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2dqrghrro.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2udrpvezc.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2knckzqcg.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2qrzbudta.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2kqkrqkfn.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2ajwnfswe.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2anuhbkux.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2cdgbwiyr.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2wkcxviny.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2oiraftgu.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2uovtcuwg.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2vtpbbqfl.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2kdlgcnbv.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2nmhlybsd.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2vvxljpwr.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2zxotejnc.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2gbkfzeay.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2vlmoedxu.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2fyztwfwa.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2wzbueipa.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2mfohmwwv.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2ivbjxssf.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2nywfzuyp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gdccafgf.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2qgngjwsg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ogkyjpth.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2sbxeezlm.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2ljjxguny.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2entdvkbj.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2uyzrdqlk.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2ntzlueci.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2ccmueedj.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2lnwtcahp.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2jppalhlq.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2pldyqovh.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2jvdnygui.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2rrdqepul.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2ohjvlevw.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2wjyyuyej.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2hcvjyqso.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2wadoxqlh.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2gzwqbpar.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2tppwnbqd.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ypjfymuf.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2mhnrkcqv.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2navgqpsg.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2erxrgttd.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2abtsfsgw.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2qdzzilhp.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2psybnzxf.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2ibhrbaxd.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2mhrbhpaj.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2ttsurnsx.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2zduudgjt.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2nwqszjfn.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2ursonvli.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2xtxudbgg.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2ijaeqvwu.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2eqafuury.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2hlrteeox.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2wltwiubq.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2tpjndidf.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2umdmcwmf.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2tzsekjxq.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2qjzcmbju.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qgsmxenk.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vtmceulo.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2mxbxxogs.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2iysldlfe.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2bomarmte.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2pwjnxepm.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2vhdbmwzd.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2nrmqjutb.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2llrbzusp.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2aufnrfkm.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2aagzjhow.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2unwqzwks.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2lazikdgt.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2blrzuczi.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2sicghpeb.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2ovvilqlg.html


<!-- 参考信息 -->