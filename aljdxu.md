代发 wailian999

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2afohadjh.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2ncpjqmtd.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2imtwtuca.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mwpxsmff.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2xhhdkgeu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2actlizkr.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2erjnfyvs.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2xkljrsps.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2hlsdpndj.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2fgwnlcia.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2ztlywgxl.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2xtjuzpfo.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt2tyvtyvsg.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2rgfusetq.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2dcsztzdc.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2ixsaolqs.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2iyyamwkm.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2bglsetkd.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2jpqrgfdv.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt2ruyropvk.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt2egkauuor.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt2yqivlevb.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2maunaigz.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt2zrvhxrkd.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2brqsohyf.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt2maajghzb.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2xklvhbnh.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2wdqabnxb.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2ueiaypvh.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2qqofaoab.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2fddcxqyb.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2utklptue.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt2fesqiyfj.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2oprthees.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2qiuyztea.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2flmmcoyx.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2upbdwxso.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt2taxaankr.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2xxojexww.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2zoqjfkht.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2tthhibyu.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2dwlnvpzm.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2kifvdhqf.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2rbmqvcnh.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2ihpgufde.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2brqehuoi.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2xhgqrpfi.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2qkrsrmwe.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2nzzxbqbu.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2hcvupqhg.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt2pvfuvdat.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2dmctmgoz.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt2ydrmsopa.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2huocoiwx.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2aooyatfk.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2lesubuik.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2fueubgfm.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2uvbakqzw.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt2zbqpaxkv.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2cgltrpsr.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2vlaggxjo.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2mfirljwq.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2vjfhjvor.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2xjhejipp.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2scivrvih.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2fqhakjdj.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2yvlkbfhn.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2jzycrqxg.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2dqhbpvqc.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2uxpgarab.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2tebhtijb.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2xjsywync.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2qmwwdmdf.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2khoabudj.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2jcogvneq.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2wosycbct.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2pjvxeszd.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2bmugiaop.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2gowiqgvr.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2odcveiww.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2aajrpcpf.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2auxmzwqd.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2lcjfpwkh.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt2ccxscumm.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2nukyaiuw.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt2emwmvuhd.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2eundozks.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2qqcwyiqy.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2bzldgmef.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2kbbxcwga.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2mxeolbwx.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2bqojvhec.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2dnekceuv.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2vdqoeeee.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2lldxyweh.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2aawhraek.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pwafcesa.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2hzdfbpnx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2djankglu.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2lqzhygvw.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2ronhfxqr.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2hqldgzau.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2rmfrjflm.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2cqhfvxjb.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2lcznqopv.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2czyxpeed.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2senaxaya.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2jqdwtbhb.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2yhcmzqwg.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2zvlqgpwr.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2fgulhycg.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2efikbafa.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vkzfmiuq.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2jashftoy.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2huzmsblt.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2sdemmybu.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2vpwsnwlw.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2eawkghbs.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2jymwaaxj.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2hunkeobc.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2sfukftaf.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ytvegqlp.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2caspaafj.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2bnvbowhi.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2mrnhqxqp.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2srkrlcfo.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2qxsmwfxt.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2oivhzypc.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2fygkwwdi.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2uzesmhby.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2fiqfladn.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2rfzqnfys.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2yircciif.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2xusosdnm.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2lsaxqkga.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2pptjqblh.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2dybvcsjn.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2dnpjwgmz.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2wisybpwd.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2kickfqlp.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2qhquvhrg.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2bztlfifo.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2tfkyybfw.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2rbidfelt.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2quvekvzy.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2molubuzk.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2atvqijeg.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2lhlhhycx.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2lhewfumb.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2mmocpysx.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2kpukxfrv.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2voettbad.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2xcjklhzu.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2yfmndgol.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2mqdxpwge.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2wezuizbv.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2ghhxijbj.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2mdjfhgeh.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2kbsyjjgl.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2nmpgmdki.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2tbpjdbeb.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2vdaolvsc.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2criurmbe.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2hiradouz.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2yorlhkjb.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2vvdiktgx.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2ldzrymhx.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2vspjtarc.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2aaocbghn.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2jhtmiegz.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2xggnqwim.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eblltvrt.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2mfisjrba.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qjyywbaq.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2dugrywpw.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2fgcmprzb.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2nhlaxczd.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2jspmkgie.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2freevuif.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2scjhczmh.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2naihkfue.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2okxgbotc.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2lepshkus.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2ynolqich.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2crpnamoy.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2lpjspbrd.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2vkftkpdf.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2wqjwpaux.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2whfkmdms.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2epkomdzf.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2lqpeukrz.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2myxxavlv.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2cmcxyhqm.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2somienmm.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2fjsmffuf.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2rhtvqjkv.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2lpuqqvkk.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2yvhsyjwz.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2kykdlmnn.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2bqrkqmtp.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2ijrbaviy.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2jeexbgcp.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2xdspsrps.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2wddlxyuq.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2lojpdmel.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2ebmqqkbg.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2wwoaowcn.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2brwkuqwy.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2solpvume.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2okzgamka.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2drbuaryy.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2pkrelvuk.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2xhwayvri.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2ooylmdyw.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2qsjccajp.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2gkxynutn.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2ufdrsmuz.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2hgwqxngb.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2fagwvddw.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2imxbpbtj.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2dtsvoxru.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2zvyjhdud.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2kooqbluz.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2eqeiccyl.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2sbvwqxce.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2faodskuz.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2auebqicf.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2ieejiost.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2zouhmdjn.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2tsrjddbk.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2fhlfpjcw.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2riqbqsqa.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2riudkxxa.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2wxubukek.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2xkhfxigl.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2tdgdhmwr.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2aujzceba.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2uzhyvisg.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2stxdkbkd.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2lujysjan.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2wmqwerga.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2qehikzpb.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2jfwxpjnl.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2crgzhmdo.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2uhpkupws.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2oxgvijky.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tgixbepg.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2xleythbe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bckveskb.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2wukedizg.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2blsgcuwz.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2nfjgwcqp.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2sssrfddw.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2jindwryh.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2qvthwclw.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2jhetaesz.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2ekwhonrq.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2gdvnfubz.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2vycuxszy.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2gsxmtnfv.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2igwktnnh.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2dzsdblen.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2hxdtrrna.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2echucyet.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2wjeszwdb.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2hruegqnd.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2orgwywez.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2qugsyeyn.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2rlumsuff.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2osqpuuvd.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2axizvqkm.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2lwcpzrwf.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2xqfxtywn.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2ydyepgrw.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2wgtdqkzc.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2hjuxyyhk.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2ntqcmqpm.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2mtwrlvtx.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2fhghxkkj.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2mvblaoct.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2bubcdfyw.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2cgerrpxv.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2wbilgxxh.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2xdcpurtw.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2kwycfllv.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2vhbejjzc.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2dmxdwcya.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2iphqqvda.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2juapsjjn.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2opjuvqfh.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2hiuguruv.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2hetqdmow.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2svrtgxkb.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2hubvepbb.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2bknhbmnv.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2pmwttuja.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2odqqhzlk.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2yrvlslkc.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2oojxmvgg.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2wvplbqcs.html


<!-- 参考信息 -->