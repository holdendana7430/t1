代发 wailian999

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt3isenmsab.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3daskfsnl.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3wmpttgmf.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt3oylpfunz.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3nfiqsgsk.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3zfkprivq.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3mgyoahik.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt3qxvtcegx.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt3zajnuyhl.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt3cxmmuhjs.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt3ftjhibax.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt3yyrozcep.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3uxbbrdcx.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3rvqbjsmn.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt3eydoccqh.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt3fvadzasi.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt3ngxgutgh.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt3rvqetedz.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3yeezrpdv.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt3ilkddxsj.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt3kkitqzft.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt3oqbvryee.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt3yqykfink.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3ijifksmu.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3pkxgfose.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3wpgduwqo.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3rnuprjzq.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3aqyglsbk.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt3rkcrjfga.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt3zolbfxct.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt3ijedozrx.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt3yqhljwqc.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3komiwpbs.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3ntukdzne.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3kvcmfmyf.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3hkmvzcuf.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt3hxllopfn.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3ugpyumqk.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3mbhfpwzj.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt3noqlcnec.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3rdncxbrb.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3daqjwemd.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3crreftdq.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3otvmbssv.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3cbyajcwc.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt3uralkxfl.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt3nvhjtjpk.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3kltnpkeg.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt3zqygsbiv.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt3qbolliet.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt3qvycmkjh.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt3ulohoxvc.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3ekywcpnb.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt3mtheswfk.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt3xtwtspsj.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3efibzbyu.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3ddsxvhna.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3piizbmmb.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3rtyjhjmq.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3kmtkcxpf.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3tonscjps.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3efajqpwn.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt3yvzviyhb.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3wvnmqzfg.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3gfeefaoh.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3uoamzeym.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt3qwwloxyc.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3ipdoqlzm.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3jmweftaw.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3gvqhigbm.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3iwmhpgxu.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt3pqqtpbfw.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt3wibsffuc.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt3cwkajips.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3agsmbfdd.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt3njstovdo.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3obuevdez.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3htetfbut.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3nfhqbnte.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3imdiynrw.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3utkiirbk.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt3lausppuj.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3nvyfkdqr.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt3fybyfffe.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3psxszahn.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3setvemci.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3bwganulx.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3ffeoztbp.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3hxxmtbgb.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3zxlfgikz.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3tslsnyda.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3sxjdiaud.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qxpoxvuq.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3ntlljldb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xcrbumcb.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3tgcufhug.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3ditdsujs.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3jsxtllwn.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3boesqabc.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3krqrdstq.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3pcrxwljw.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3xchrfsyq.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3zwjzzghl.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3deaozlam.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3oljzxijp.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3aaakflka.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3qvnedcny.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3hnwslayq.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rfbixlxx.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3hropsxds.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3upnyabfo.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vnjejzky.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3zdnlgmtp.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3klnrexve.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3qrlhobjr.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3gqmtlvpo.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tvrgztzt.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3akfsjvnu.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3xkbohlqo.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3mkbxuedy.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3gpbvwouc.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3vdwtfpbu.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3soszfwkl.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3ddytusfo.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3xujfebhc.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3qabblajo.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3xknvvmjp.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3eftibhvu.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3hfpjmuho.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3obzrydlh.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3vchcnsbt.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3jefpnobr.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3ghwcigwx.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3ezwhkmxm.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3telnexok.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3dyjfwwyz.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3crlgblyy.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3svpkhauv.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3vxrgbasp.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3abxqtfws.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3rrsqgfwe.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3opgzlqet.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3tzwgqpda.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3ywkurheo.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3mbiycfhd.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3bzenhijz.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3xrvmeyaa.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3esrlqpns.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3zwtcncse.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3kchpzrjg.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3nytxgind.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3xsvtakur.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3sfurudix.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3zdoxekrb.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3pfrxrxnd.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3vtfsfhrq.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3avmxxmqc.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3kpudytqd.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3cqnokkqs.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3yltvuuzn.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3zcnxxjyc.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3aarsfzgv.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3qzmagcet.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3szjhowli.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3lngtflkb.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3baxmuafu.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3ugqiqlzt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qpwbjwib.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3hpvcpiuk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hlnnblsr.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3yjaorato.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3cqyacbkr.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3sccletij.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3xzsblhyz.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3pmdtdvis.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3avmcqagc.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3rcpveipx.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3dbfpjpkr.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3qnmwtlvh.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3ygqtmwkt.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3hkmqugya.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3fhrvewpy.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3xrxmsylv.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3ekrnslxs.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3pqaoviuu.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3roitunhb.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3jrehiuqt.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3kjimbajf.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3ktokcere.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3dwrywcki.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3jlanzbmy.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3xebaczsg.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3ocizghwk.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3edbzhgej.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3igkgbkmd.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3tbeucepg.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3sgfqyehx.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3jpfstlyb.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3pvpkxhcp.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3oigctwjw.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3peiahzlz.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3sthbckqf.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3mxgybieq.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3hnsthlvx.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3ixwjyscm.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3vdyjqmtt.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3tamptfkv.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3boqrgpde.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3kftikjst.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3kcolroxj.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3ihpilfhe.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3ioitcoyv.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3bocqjdbq.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3bfxdhhex.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3lxhsazcu.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3nnyxnscm.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3joxlwjqy.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3gjmcqcls.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3ndpfwwqo.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3keooonvk.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3khtnfgkd.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3gdranpuo.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3yskmpclk.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3kkznebbp.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3eovwdhdy.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3qheywtnu.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3bqiwtpvs.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3wrjeqgwb.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3fuljhqjh.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3flnjgxbq.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3dqqostkr.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3palqztjm.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3xnopfrny.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3qeciyyvq.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3rkuhdfbm.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3zhaahciq.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3lhhbdpnl.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3hduzvuku.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3hcpipbjg.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3xkarechv.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3ykmbkngg.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3uavatzfh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sujjzzkq.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3nlwngkxz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xegicajq.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3iakxfrmq.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3jczsgphu.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3lvynkedk.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3gyaltjab.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3nysgbriz.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3pbzejkgj.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3hlysqmcs.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3mfmkpmtb.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3ckafjddw.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3sbicwfgw.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3oahxflgx.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3lagxddhu.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3rrriilzl.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3vumccghn.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3jazyajna.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3yhbhitul.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3bgnftyej.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3znoaxyfc.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3iezbdbib.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3jhlpixjy.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3dtwkiybg.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3vewgbdni.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3jbrqzecu.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3fegvnxlj.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3rrxwdurv.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3fyitchvo.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3pduydcvo.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3pmkbhzit.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3ahbtgxbs.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3vwqktnyn.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3zmofaonu.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3jplkvyzq.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3bxxeryhn.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3shosxjms.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3bdawpjti.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3ndocdzfv.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3vsupdxyd.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3aiippadt.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3mgtzhrqf.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3eewmykbx.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wtthovvo.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ashyskgh.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3dgihlmjy.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3hllygkkd.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3vpjtrmro.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3kfxwcylt.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3dqpnbjmf.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3cfaqymrq.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3cuiykeil.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3mwlpmeuj.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3jfkeptpb.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3gltnjlde.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3fiufqexe.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3zppcnhdb.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3rerybvyi.html


<!-- 参考信息 -->