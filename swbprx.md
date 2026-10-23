代发 wailian999

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt3qworqcay.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3crxkbyjd.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3xxfjdode.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt3zucvhlsy.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3uohlttiv.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3tcxlsdzf.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3npiplelo.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt3kbyrkupo.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt3ieslkkwj.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt3hpzsisje.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt3lwnqsvyl.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt3eqzabfpz.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3jochxzwh.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3gcwohkwv.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt3pgigmtcw.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt3ztqinxju.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt3fldiaxdm.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt3ixznjwuq.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3bzhmudlg.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt3ozifknfa.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt3lvxhebza.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt3wmxjxlkk.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt3dcudrwhc.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3rjfwpicf.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3puufnwfi.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3pjlepuoq.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3eeejhgrn.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3dmupkwvy.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3umeynldg.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt3ynuwpptm.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3lgziwdlp.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3iihbzmjc.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3vfyoognv.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3vbrkahvp.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3coftcyco.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3inudlzur.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3vaqjddau.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3ppdligcr.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3nioejwni.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt3yqlrnrbr.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3kvedagrn.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3wnuhotmd.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3lljtycgx.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt3pwjtxgkc.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3iyltpnkr.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt3xhevnbjr.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3feafmhmp.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt3odtrdede.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt3xsizxvxx.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt3ovplflnz.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt3awwdilbn.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3xqgowslb.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt3jpuxvoai.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3nooiqfxk.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt3liculwlc.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3klexlbzg.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3iswkgfow.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3xlfablep.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3qyhfwjxz.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3zqawouvc.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3cjtkykij.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3minyxhat.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt3tkitwhru.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3ywplvnsv.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3wucezhpn.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3btzdqdji.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt3schcwqbj.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3aauvzznd.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3tuimnxme.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt3zqykqlln.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3dbvvdvho.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt3haboizwv.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt3qafwdroe.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3zgzylqtl.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt3dkfoupmz.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt3lyjthuwj.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3lndgkqdz.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3ktcqrjfo.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3racexvxl.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt3gtjnluhs.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3alivtepd.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt3cogbmrnt.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3xvufmrfv.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt3vcccguig.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt3pvicalty.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt3ejsnekca.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3yubhdioz.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3pqfetbqz.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3kauflaok.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3doilqxdg.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3kvrtuvfg.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3iszsdaon.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vdzkaiak.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3uihferoh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ggcvzzeh.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3okpimryg.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3cejjjxqq.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3qttrjtnw.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3xwujswcc.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3guqdcpgm.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3anpdgnrp.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3bdorcpci.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3sqxxwoic.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3inmusthj.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3uqogreid.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ozsyvjmd.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3icmnykki.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bzolqfqh.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3omasrksd.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3wnxuerkq.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3mwfklcrc.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3knatqtgc.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3budjtjby.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3oythwsev.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3rdxtbxme.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3ukjlulsq.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wqhfnlcl.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3iieszewn.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3nzewjtxq.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3wijmbcnl.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3hqaeijjj.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3bttkqswe.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3yeezwidd.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3plghqobi.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3prebajlp.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3gjtwkkkh.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3daqnzbrq.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3qxtfdxxr.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3ijrvopxe.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3ctfiemid.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3amhyswcf.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3fkttnlnf.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3saxlajfp.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3iydyapir.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3xbfpecpe.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3uynvfjnw.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3mfaqgtev.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3kovbhctl.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3awgndyqu.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3pemhcbjg.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3gqsnipfy.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3lykxeybz.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3ilvecvvl.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3rpvjrnoy.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3vrfzxjlg.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3yqvcanfg.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3uirckvlu.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3tqynctmq.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3edjhhfrq.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3pfyghpcj.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3keykmnak.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3eqzhnbdm.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3phpbhazd.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3wdmzyzqt.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3kthruxaj.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3nnqqerjo.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3jyrwcjrr.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3lxenufai.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3inwgjpwd.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3vjgurbqr.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3ydsssnth.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3aqupowbk.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3jvogndxl.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3qagljptv.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3pstvuepc.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3uxpwxnrn.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3sbakkfzt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oxcgjahe.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3jjckkltd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cfhlfvsl.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3ernvbueg.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3xwpibdfz.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3ylracqzl.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3alpfnoig.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3krdyttse.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3xhpedomi.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3jlhamvcr.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3mdtfornm.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3qseimwci.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3pspkrrmk.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3yyqftqwq.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3ipphnrbr.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3nkhlujsm.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3cthfrrzz.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3ukmduela.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3ihrfrzmt.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3yvlscxdp.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3jkxodthq.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3zyoatoyb.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3wbomklkz.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3cwnkojdh.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3yxlrhksz.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3hzxzvpmc.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3yseabzhn.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3clxaadxb.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3mbzxvnts.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3qxexsefb.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3hzwuxtfq.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3gdwskjpi.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3oisgkggq.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3wjnbzpar.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3hzvlwtxo.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3myclxdcb.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3kwfsrmxj.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3fdcxauwp.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3sucxksck.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3amgjhvew.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3thueohou.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3pkfadeox.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3xejcqtks.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3wxhnvhmt.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3agezqbei.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3indcvqaj.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3bavsjejf.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ovxqbwbb.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3jmnukhtj.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3hyxvdtxi.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3dklcjeit.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3ghhsaixk.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3btxrjfms.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3zvfsfoif.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3mctupaak.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3hrzqifps.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3mflreztv.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3bdjfhfwz.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3pwppqeum.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3ulngdkjv.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3qbhrqbbm.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3vjbuqysr.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3whosnhwf.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3ofvrsfqv.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3daivfqyn.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3jvncmeoc.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3vpcthhdm.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3clsliqcw.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3bnucvfmh.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3yehozejr.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3fospuffe.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3xxelmmmz.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3mhksiwdu.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3keasvoyy.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3otbokuic.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hjllbdmg.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3dfgfwsid.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ixvstval.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3fvndtzvb.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3lybtyfox.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3jhfyhibu.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3zdatarro.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3tmkrlaiw.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3jfbiiuns.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3fkxqdjtq.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3ihctilie.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3dytvzgno.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3vdwmvtxv.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3hoclhmzf.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3rgplviws.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3zfnzbbrj.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3pxipphxf.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3edcitmzn.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3vsntuzuj.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3vddxtnrs.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3odyaweyx.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3cegkutvu.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3evgtjwgg.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3sawfgxge.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3ddampjwp.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3kgufdcvy.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3eojutnwy.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3flfamcfw.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3svawrnzq.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3zayhwqdw.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3bjbejrvx.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3gbjpthhm.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3gsjlqffr.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3rcselmmv.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3yaerkvcq.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3lbeekbgq.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3mnugydyp.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3nttbdbrd.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3gkbvojkl.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3oymdtozu.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3bhuexvwe.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3dwsrktcd.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3maanjggb.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3acqkinre.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3bdgbbgyu.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ubplzcso.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3klqpsqrl.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3dmsgfmoi.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3nkyfyurd.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3mmnqjwjl.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3ngzegsnm.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3zbyjruoh.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3pgcnwief.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3povagxch.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3fbhngeyf.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3oopbgzqc.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3wrfoxtyl.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3ydtnzuns.html


<!-- 参考信息 -->