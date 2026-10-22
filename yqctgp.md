代发 wailian999

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2rrijbmgz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bfziswjl.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2fwxatpso.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2mncudifi.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2utqcxgjn.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2sevlyvaa.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2whjeuuda.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2mtyfrgjj.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt2yjqicycj.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt2wrbmeumi.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2pxetqsgs.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2pzmfjarh.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2sfgdgsdh.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2jsxvcwau.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2rgcpzcky.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2xfqznufk.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt2jzimgskf.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt2jkqcukkn.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2ngbsvwfg.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt2jtaaqnru.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2zckxkkhv.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2rrpxbslo.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2akdcozok.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2mpdzilne.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2mefbeklm.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2sdltflvi.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2bqtsixhv.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2nkhyvxlo.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2eycivegc.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2gzpzkshn.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2vzfgckfe.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2mlkphqai.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt2muarsgvg.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt2yuiveejc.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2havzhgdv.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2kwzxxuhg.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2ohrrwnsx.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2cayitbpb.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2qvrafmor.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2fektvwwv.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2cekchsyr.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2zlccdhre.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2xvyyofrr.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2lenkuxzf.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2sdnnwztr.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2rzzufaht.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2gjtxjgbc.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt2jstdtxxn.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt2niioqtxp.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2nkwfuxgm.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2vjaysfyv.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2wduxjonl.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2arxfbcfj.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2avfbldks.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt2rdyslocq.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2kkgpmiwg.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt2swflsljt.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2yarbrwwx.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2riwsqfdp.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2maxjjesb.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2tfgpeedw.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2fcmhctpg.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2yswcbzwr.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2pjaqnkft.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2sxtnbpac.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2kzhurvch.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2kgdmzsfv.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2pfmnxnfy.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt2xkkyyspy.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2pswlmyij.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2ifyjmeem.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2renaznoy.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2zoztmbkm.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2jwbywtml.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2gyaajfii.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2lieduioi.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2pxykgfhg.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2tphybvvg.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2whfrnykw.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2xypovakw.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2vrxkzrix.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt2fitxrkot.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2ijznnmon.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2pwxrjnrq.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt2vfuobtec.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2kdalmxta.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2nykeekxa.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2hiftffrg.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2fixyueky.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2bxgiltzh.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2bjqhbsmw.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2cyefayyz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ylazplni.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2nedjcgce.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ltpacmir.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2qcesvzbh.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2segtmvig.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2qtfplmmp.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2defdctyc.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2yatucekr.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2sfhbtbnl.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2oqrjxgcp.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2fzgpdrbj.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2marazxpk.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2cvobflnm.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2gehkcobg.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2ukjedtvh.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2upreygwu.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vtehivmw.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2mhkfhzxu.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2adckpwqh.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2imsrhqth.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lnoeywek.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2bhphljqt.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2vrwlncwd.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2kpbqjybu.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2smknsybm.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2kqllvycb.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2xbvujrvu.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2tavbaiuo.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2amvqqcqx.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2dsoqtawr.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2svlrtxms.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2jqpabesq.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2fqdnyflw.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2sbhvcntb.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2weksvawx.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2lyowcnsj.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2nmfuouek.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2ugziyrtc.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2cliahfww.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2gjdfzski.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2gmazcmhf.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2skthvzlr.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2eachkqaa.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2swgmofqv.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2ivqafykt.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2rpdzpoet.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2ujhpmdbl.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2ojvisnmg.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2nvcntzpv.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2pgdrodmi.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2mgklfebe.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2wdvxpkqd.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2tljjvlaq.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2lcpilyod.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2cwelrnpx.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2bcfqjpil.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2ugkljzip.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2rqptaluk.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2vvmoctyz.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2egbjrmdx.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2fwoamosc.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2texljbjy.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2wdyfxsts.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2zainyqlz.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2ldqtuxaf.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2opjantqq.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2zyzwxwwx.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2zsikfdiz.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2hgzlwaco.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2onwzifoy.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2spzeudco.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2jmfkbcca.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2hpuatlay.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2mtkxlula.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2vszylrah.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bbivmzkc.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2ustdrtuq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ijclgdtk.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2dqlfrbfv.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2kjfoczaj.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2lsyepllo.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2gcsnnnce.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2ocgnlpza.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2wkjpwpwu.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2zpnvtqnb.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2fpvaakpe.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2ftryfaxl.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2yicyrkaq.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2bjaknyck.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2nxxnczvh.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2hakfxtsj.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2cehwchqy.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2aouxthxx.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2wnvjbydo.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2orzyjonj.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2ehxaiwex.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2mubmydet.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2dptkvrwf.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2irukwhac.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2hrpsegid.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2qerqyinu.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2nvmfdioa.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2wdcwoteg.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2uardztrz.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2wysuzkyb.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2zaocvtib.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2goazdyss.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2ovmwycgs.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2vrisjfnn.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2bxglzrta.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2tqbtzvcw.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2zgjxopvl.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2yuzbhwjk.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2noqjjzgc.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2keuzpflv.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2yhjgpdjl.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2xywpngmr.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2srhltbsf.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2friffttm.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2zphwgwgw.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2rknbxqst.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2tagefbfo.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2hasvtdac.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2fbuaaugh.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2gibnstfh.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2iishwhdj.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2mxvjcxsy.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2dxcbapnt.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2kuhhqvaf.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2vznnppdt.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2xeqftmbe.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2ptddhtua.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2uwiegknt.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2qfmmawtp.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2icwmyuif.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2waqsrvmo.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2rbtdxzjr.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2piaxwwle.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2hfkofmcm.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2ozhkkxim.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2uldurdly.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2eaucexgp.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2lfkzwacb.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2kvaopjeb.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2dkpztddk.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2tahuoblr.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2itigxbdg.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2chfghbja.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2ocefbrwt.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2xhnxxqej.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lwlljzbj.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2qnjyorsz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wgumlbsh.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2hufgvehc.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2ygjgdpbs.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2quqegzeb.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2xodfmoea.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2xieyubdw.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2gkspptdn.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2tymhmwxk.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2bmvflvyk.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2iofcmtsq.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2pccloafa.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2mlfanepx.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2wzpramvx.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2lcjupxod.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2xzvmhphk.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2dhjkwrpn.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2phpdmexv.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2gohtkzmv.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ruulwsse.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2dglkbkhx.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2scrvmicw.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2tljsyxbe.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2jcormkid.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2clpptikl.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2vwrdyfbp.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2dkckjnlt.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2ouoclufh.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2dctjjzdy.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2oiqtvddj.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2csqeyyxk.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2weenrlvf.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2jnalfqfm.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2alqxbtuk.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2ubxuatov.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2uipcouli.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2fqkilowt.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2oplvzuws.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2mkymcigg.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rnaqhcdp.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2gqmpvrrw.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2lnscbthb.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2voiqpobi.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rwybceaz.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xameokvf.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2znpshnut.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2pcqugrou.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2ptidfqof.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2gdorqmhi.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2qhivgwui.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2xpfxpofi.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2ttxbhtar.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2isjruhcp.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2exranegt.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2wdqyosrr.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2nuspjyry.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2vzorxack.html


<!-- 参考信息 -->