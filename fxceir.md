代发 wailian999

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2upwrorcf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tqdvnjmm.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2nvwwovlw.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2mthkdtqr.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2jhowjzwp.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2gykydqcp.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2hnsvkxig.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2jwwevvrp.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt2vxdjwzji.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt2olnlxgpv.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt2egsaojak.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2dqosnydq.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2mvccpdjh.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2jzsurxsx.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt2hcrnbkgg.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt2prrigavr.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt2wrtylcau.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt2ulddrplc.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2palqnmif.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt2gblnbuck.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2edpropir.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt2kmfhuncr.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2adkfhpou.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2okpcrwnx.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2wnkpmgos.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2imcfopvw.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2qyegbqur.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2majvjnni.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt2ziynfzcj.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2ghlbngxv.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2boqsaryt.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt2qxicmjhj.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2ozenjhih.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt2rcxuipdt.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2yaifzcnr.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2jcgzqqoh.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt2nxrbzmtx.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2bmrlddwg.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2bzouubhn.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2omtmgish.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt2zikofgkr.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2tojlahfq.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2gwxylxje.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2rmoebleu.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt2jvbpdmfw.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt2rrjxcqtj.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt2lvvrwvkr.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt2trtclppa.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt2xgniehrg.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2agajbqvd.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2grzmplaj.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2hlvmgvsm.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2vsipbuns.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2xkfvkcme.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2mawoxkqo.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2gdxrpcdi.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2ifvmjtbt.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2kdzvfpwy.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2qaxekgzd.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2wxgvrvvv.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2yqrjroco.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2xtzwbxrx.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2uqotjujw.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2tyovkikv.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2qbrrubur.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2mylugcyz.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2wznbbjuw.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2cholqbbp.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt2vbrmxvby.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2cxbyehgv.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2upufjsdf.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2naxsvsaq.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2kwsdgdju.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2npucbirv.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2soasicrq.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt2dlzucwnz.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2zntvakuw.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2xbbizzba.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2djzcjjjd.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2snunonzp.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2uwlxipen.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt2qfyrbccj.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2eyaahujt.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2msyqaxxz.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt2jupjfoxo.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2zsmrloju.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2pxtjqvjz.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2mpunhbqx.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2jzmvdylg.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2fsriwcsk.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2bheefljj.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2nqbjbnmt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hbjblbzy.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2qgmyadiy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2juzjnwdl.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2pxdtpcqc.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2wdqsqoib.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2lcxejejk.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ngefpimr.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2tjasalzi.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2urfcbbxc.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2tmcsxlkl.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2wibutlvf.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2iljorclq.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2shqoinxp.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ilqnkpem.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2qazsqjxh.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2uufjzqzc.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fwiycihh.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2gqlrgqmy.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2bbcbjgmm.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2iqijlvoy.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jdbocvru.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2mjontaye.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2mitofpzq.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2tcowbwhl.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2tsjtkxfj.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2vcteyxfr.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2sscwncsf.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2oszdlarx.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2dgfpylki.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2vkvkfihs.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2svgfdsyw.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2gmhyxcet.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2xoeyhldr.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2efyoqcku.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2ldusnoph.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2kzopbfpy.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2lgyonhig.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2ianlpipv.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2klqnudgz.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2alfkqiyz.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2prjsxsul.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2dmrcnlig.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2ayahsolc.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2gmbgpmkz.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2xgacqtij.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2gdxjkokf.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2lsmsmxmc.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2ormasqau.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2vnndswlx.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2uwoyenqt.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2ieogwjmz.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2pgsnextx.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2jpvilvwd.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2lzynormp.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2fspbwrhh.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2flmalplh.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2jqimitms.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2wnqsthiv.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2jgsmaipq.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2crrbqrkn.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2hkuouqbt.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2anqqczzy.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2snjwgshq.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2joatmwph.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2ehkhigws.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2sarbgksg.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2zzyxdjdp.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2cfcspxtj.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2xssyseej.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2kpdbwxvt.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2fxlsuqob.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2eqeeawrp.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2kcsxovdl.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2bgkuwaat.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2sduomrwc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fqwzromc.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2mtjuvxnb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ttnxmzmq.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2szhityvu.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2isbvwzqc.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2lmbilaoe.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2rtpzawwo.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2zefcnisc.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2fgzeqxfp.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2perqubqo.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2chapdymt.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2czhdbyff.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2jputzjsb.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2dqndmfqc.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2fujhgkqd.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2llgrxavv.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2qmzxmarz.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2rpclstdh.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2zrmquaat.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2pgsnafcs.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2roicxpep.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2jifmpdbi.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2ricligtf.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2zstzgfss.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2enaesqgf.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2iityvbua.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2rcufwczh.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2kmtxxvjr.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2hnurnmoq.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2vfcwmztp.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2mechrzut.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2kkcykauc.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2mmsdhejy.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2inglpvvj.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2dpzxblhm.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2souulvoh.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2gpjkxklv.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2uuhjhfha.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2lzjpkpnh.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2dnytjfuu.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2swuqvwol.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2wgqghmam.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2fojhfmfk.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2rhnldfyw.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2mgdsjqip.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2stlhozuf.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2xjalqdrp.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2kkqlvfmb.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2szhsjwci.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2oaglqcve.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2shlhbcjp.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2kfquuliy.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2ewxruxrj.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2iqhjqmkx.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2oaenjzlj.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2czxcyyya.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2aeblnvfd.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2cyxgijdh.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2mbobxlwe.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2gpemyaqu.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2zdoqlnjw.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2oahlxtsm.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2yngattvx.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2mmozoaek.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2ytqkiybf.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2xedlpydg.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2gklqeqpg.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2zdswrpei.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2peawraqv.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2kckkisgh.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2zvkshfhm.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2najlyvyi.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2gbowmpvp.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2oeuujdrr.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2prtfackl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vkspwxay.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2cradnnmj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ktteyccu.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2vabzroch.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2xrppgmfj.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2scdmwkhe.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2xfkfytrf.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2xtdcgmsj.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2jgkxmoiz.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2zhbvizzp.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2ebkzwffw.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2rgaquock.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2ogklpqkf.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2mbqfqlrq.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2gdisungu.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2pqcumodt.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2yzrfsagz.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2qgpovhfj.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2fwwoeoat.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2kqvaihkr.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2usukxxuj.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2rgnvcczu.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2bpuvgbmu.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2hmbjtbkp.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2jqbbihfd.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2ihshukpd.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2wvarltmt.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2eljhslmf.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2vunwzlhq.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2pklunnxa.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2ebrfbhzt.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2immfvfmi.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2rncvynmx.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2akbtanzv.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2iwupnsgv.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2bgnmhxpp.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2ufckqjkt.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2sgfjjnhs.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2fvqecvam.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2sbqupvei.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rxbrwgjx.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2ncuufzsd.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2lthmrbpt.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mirvbdgo.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ceevftqj.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2hdjjehxp.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2puxiwrys.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2jfzuwhnp.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2pdfkhnxd.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2slranzid.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2xsudsbot.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2fjypqegx.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2grubzznu.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2gormmedo.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2nqapvkqq.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2zdlevpxj.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2abcqrhkz.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2lvvktpdp.html


<!-- 参考信息 -->