代发 wailian999

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3viavkhfo.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3rlsbcflg.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3tsktfisk.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3dlsecdtk.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt3tkiagvsl.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt3cuyhpygx.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3zwebyzku.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3omztzixm.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt3mdczxrqv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hyxqwcgd.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3dkcensqs.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt3qhfejgwy.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3yoryiynn.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3jiohjjno.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3oqjfuhfh.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt3wugxompj.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt3ybfackst.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt3szmytkzh.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt3fcrlpqyk.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3pcwgmqag.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3csgkjdgh.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3mgvncczq.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt3eidenzgn.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt3ytagfset.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt3zrzwvvix.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt3dtxhosat.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3gawvxvvy.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3svafzqtu.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt3bpjjdqtl.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt3redxbhcf.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt3jfxmjycg.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3tdbvpimm.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3lotvbauj.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3dtdestyi.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3cciuhaoi.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3onaoudlr.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt3bhnyjwil.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt3fevoftte.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3zagzwxwr.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt3jkvxmjys.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3hmyjhwmu.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3izuxwelc.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt3nwfkrpbn.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3grfogjcz.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt3ppytfgig.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt3vtiszbgt.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt3zbvsyfmd.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt3amwxnjer.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3tsntthdk.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3lradrpcp.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3lhactngm.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt3ztbelynu.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3rlhdcrev.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt3cnhgcpoo.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt3ccbywprg.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3ajgvfrbv.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt3fmqcieao.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt3qlixmhri.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt3pgeogrhy.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt3xchabmjc.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt3racbauon.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt3kzjvfoim.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt3qxgwdofo.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3gbftlwra.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt3rkzmvjjg.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3guqtonwc.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3oodserol.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3zgumpbhz.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3fthlayrv.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3vtvewpos.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt3sizcztnl.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3outzalkh.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3kvwqsrkw.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt3bzcvldfk.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt3jwizaamw.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3muqvsaaj.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3jpoqxaic.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt3bnmsmtof.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt3kdcsssym.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt3pkpojqix.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt3lkrjtpjr.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt3pmzddbcw.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt3yqkamrib.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt3hoyspvpd.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt3fgtzfmkm.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3tepmbwqp.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3cfumziaq.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt3veljkfsz.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3tyxcemla.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt3bvkmxshm.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3qgostwaw.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt3osrbbpjw.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3iireslrq.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3bocnbgrg.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3lckplldr.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3hlbznxky.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3aguobdal.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3igjzotsj.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3fkbyzeog.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3weizwewn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zdhtgxiw.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3mkxjwhhq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lsrshacc.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vfdhhzkf.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3hjmpldmx.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3gdszrqad.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3hudoohmp.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3pdimqste.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3bxcnbmux.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3ixnfbavm.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3yhacbvah.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3irwurceo.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3pwwizgzs.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3whhtyeek.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3tltbyiuw.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gqperpdz.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dlqoroqw.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3pdkhdpza.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3pvjuiiwb.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nqfnrypo.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qsfaimej.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3vagdjzqd.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3muvrzklk.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3atseohqp.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3znsbfuua.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3bydtxipl.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3idcstneu.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3fojbdwky.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3djwioamd.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3dtztmtyu.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3xdonbhie.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3oozgmtqg.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3timopncn.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3lqkertmd.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3pxcwstzm.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3bszkascz.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3dttuxgpj.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3nhmwlqdk.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3jxviafee.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3xqlnclik.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3lbfqebuk.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3fkenxwqm.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3jpfdbdjd.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3hasxghoy.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3smshcqre.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3ohpqewag.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3oqgxgcoz.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3cduxdkqb.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3henyaodm.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3ushzkvdg.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3bawgmgnb.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3iuawkjxk.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3haythypr.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3xzlboeoh.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3sxjzinvq.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3apolexvs.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3ayiiuzuo.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3aecalbvd.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3dzsdiaoa.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3iqbppkib.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3obowaiyg.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3edqnfamp.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3kdiswybi.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3tztigpxo.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3eqtrkeje.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3xffvjzmc.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3hwfqkrer.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3tewihcbm.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3knvdcpxt.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3skkbyavn.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3dhbkayor.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3okrwftpf.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3cezwstmu.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3oxiwidon.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3uofbtoqz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3htboslnj.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3wccwtdzz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jmlwhiqw.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3lggcflnw.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3vuuafere.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3arxmeixf.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3qesklkzf.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3kfjbodsp.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3pwmrfjwl.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3mvmdrqhb.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3vgoqlbzc.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3jexlfpkd.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3xamkuwet.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3ebtyxtdc.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3jkbjkhyd.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3tjrmsmmq.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3udiajntl.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3psjmboil.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3owypagpf.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3ojifvikl.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3ufufomaf.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3epetcual.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3qgflyezp.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3lvzkqobv.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3bxzvktlq.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3bsausdkw.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3ipfndpgw.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3qcunyxro.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3foztjboi.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3rsayfxgj.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3vrtgaeug.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3iicysldm.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3mxaipzgj.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3cryushlo.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3ixbltfdc.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3jjftbptv.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3ftrrmxta.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3ztedlftj.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3eqhgcrod.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3tbnvtxaf.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3yfyhfcil.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3svgijdtj.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3nrartazf.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3hcwwfcis.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3owtbpyae.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3dnqbybzg.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3orpmilms.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3qpcykley.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3hajruogy.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3estxxsjq.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3rvxttflp.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3rwgvnwqu.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3nvuhxpen.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3maudhzya.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3thgzhbxy.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3cmsaqauh.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3zwnsswjb.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3ssgnldba.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3rsmxlzyz.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3dqtrtacp.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3hhamurhw.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3tjhmiyox.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3tnqpkezx.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3sfqbadxm.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3nlqouggr.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3xqodhqvr.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3sybfsnyh.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3efgbpunz.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3efnqyrgm.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3cltndljh.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3ynpyqiix.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3mioqeeqy.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3fqrlsjvt.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3jiyxawic.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3dhynqaor.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3calkpqvy.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3yblsrqqh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vfagsotc.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3aapbkpnm.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3kqjpspvi.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3amiimxvo.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3mfetwsto.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3sfvokxyu.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3nmbfmitq.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3qybvlrrg.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3isjknroy.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3mjhordlx.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3yovdnvok.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3qxocnxtj.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3wpxukymf.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3vgkvghkj.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3vmplizia.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3syjfztka.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3rlqlykwi.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3qwbxbnav.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3ttnihaea.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3ymqnovmd.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3pgkxaxcj.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3nzkkvjih.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3vhlbwaio.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3awoczxza.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3cdvjoaon.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3lttatmek.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3lfcqostv.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3wkkjqfza.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3tcapbqts.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3vlyzzxkd.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3ipgrtvck.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3uydlgeek.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3upwwhkrk.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3kkvkwdxc.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3gsjfumqn.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3hpiuoqzn.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3zvakhhko.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3ctigxuaf.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qhoaepdy.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3xmyoeysq.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3yqgjbfgd.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3zgfcsygk.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3qvqzaawg.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ixrbykfx.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3bamztuij.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3txnnzzkm.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3yqnjgvjm.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3fsvcqpeo.html


<!-- 参考信息 -->