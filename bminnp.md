代发 wailian999

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt3olhqbcei.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dxogrzaz.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3kmceaslv.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt3vndqjzim.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3vnrjnett.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3looumjtu.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3nvbigjpt.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt3ibpwaeae.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt3eselnaln.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt3ljgsnwkx.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt3cwvrlcek.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3soonkrev.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3ijuurcow.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3glqabmlv.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt3dhyxbssj.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt3iykwbylr.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt3swlqrucw.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt3gmlrbmld.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3gjgmbqoh.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt3nsileyzx.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt3zhuzbusz.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt3vbmxjply.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt3zmakduak.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3pjvqfhdh.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3cjpnrqjf.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3exwttrzb.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3idhlrcis.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3aapcfbxa.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3xwtpulhq.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt3xchdnego.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3tfnlyyvo.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt3pwvwehaw.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3tlamfupt.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3jblxakmr.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3ixyhmzpr.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3zffvcsbk.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3zoypxfjz.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt3oguhumph.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt3cmfqyblw.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt3tkfwjlci.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3fheavlex.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3zpmfwxrw.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3bznedmlu.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt3vfdpuepv.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3icdgmyhq.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt3hklbdtfd.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt3saitohkx.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt3igdjqmrm.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt3cnxyxjfn.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt3tmbrmawb.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt3qjmiyuhh.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3kntcmyge.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3lynxlahr.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3xgcdoxnc.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt3csllsgdi.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt3qxkznqvp.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt3bxqifmun.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3eumyfcpq.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3ceyylxlw.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3oewnjkff.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3mhwzfgod.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3gbhloswj.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3wrwaifuf.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3qlshipzh.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3bknomcfp.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt3fcadrqtk.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt3twdqhfml.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3hbaktayu.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt3jtdlflno.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt3djwddrsc.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt3ylmaalas.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt3ffxvnmeu.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3synmotst.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt3zfvkxznx.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt3mgqzsvud.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3vcuaotrj.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt3wbwxfqdg.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3hfcflifq.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3wuwpxtas.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3kfwegjaz.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3vtvefyoq.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3sqbxhqla.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3zbjcvalf.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt3nbgngpzu.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3lmosjymt.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3qiscwwjy.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt3mydpnrez.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3xryrjmrb.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3klggehxt.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3hynlnoys.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3elmlkoyw.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3nsnydmfd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hqsceflz.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3trvulhjx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zngafqkx.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3kfmpcbxm.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3gzqykbog.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3zeuaqxth.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3wdbywpsn.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3xwfdkyqd.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3yhyxsgtz.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3yqlqhnpk.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3rlfvzekx.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3mwuckihq.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3ojkovfgm.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vylqyfig.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3ndrrnjyx.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3cugartba.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tltinvlv.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3kisworrz.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3nrunutxn.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3imquksog.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dfymjuqe.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3dukkbzqx.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3gkkpklny.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3rvcnzagh.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zokquhtq.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3uwfjbvlc.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3hvfshulb.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3tkytmlrz.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3lpjujzck.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3keikhsji.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3rpmxcfnr.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3ltozeuvt.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3hvozslot.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3nxdeaccj.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3dbhvmarg.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3lzmxwetj.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3bibvhque.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3bebfttbx.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3tuffsyar.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3aeqpaqqg.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3niwxxzss.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3peoidkkb.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3pkjuawzk.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3iaosebgx.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3tgklayoq.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3ugceqnnx.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3besodmio.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3ndpqokbe.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3izxkoybc.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3goriubyy.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3gqvdubuj.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3imjmnwvs.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3iuuodcrb.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3fxdrzjdw.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3kmahmbax.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3drtskclu.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3hyxhwdmt.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3gmvhtfer.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3doeuwmyv.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3ytsbuban.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3meujnjhy.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3cfududwl.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3qozbiapd.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3qioilmey.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3gflllhiy.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3nqbuuuep.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3qwixbusj.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3csogvalb.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3kvtqiqob.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3hqshanqo.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3qwjioyco.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3fkhcimzp.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3ewgyihjx.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ufxmkjfg.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3gatgsbfo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kpocqtup.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3vspihzew.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ngupfnko.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3lswqodie.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3hnbiqtru.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3wxndzqks.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3pkucdvhg.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3iqjhijxu.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3yzplqmzn.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3lgqwejta.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3eanryxhk.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3jqeftrxw.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3uhqtmucl.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3fnxbzmix.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3yojfdnte.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3rwpicpbw.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3rljvdtqn.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3dmipppce.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3qqsxjieu.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3qlydczui.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3tjalkgvd.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3wzgnnvoq.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3ijvlmhjn.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3ywenjkdy.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3zgvimnmb.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3lpmmfzbl.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3pdyzfioq.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3oerzbhzz.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3paqiwlub.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3dbxocspk.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3snzobkqp.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3ptlpovqm.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3qftgmmzp.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3tfhfsugb.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3guygdrha.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3ihlkbupj.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3zxsnjxrv.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3okpjjmid.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3ayzjglzn.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3otipnfbr.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3critvjsx.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3dmnukoxc.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3dvaohsjc.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3fcgpsnai.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3kkmqryon.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3chyouvjb.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3nvzxgwmn.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3lfqtinhr.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3tioqcudf.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3vvzlmmtw.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3olcqedbm.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3oqgwmojq.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3kirpabcs.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3czqkxjdy.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3doktwgku.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3hsynknjl.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3wiqtzpxa.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3ufabutbm.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3henuaayy.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3uowhkrwf.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3quofthuw.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3uljdluxe.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3qxbpggtx.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3ihfrrgdr.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3dsazjcas.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3vqpardff.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3qdilawdp.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3qwgriwuo.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3yykysmbl.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3mgppqlcz.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3fcjjsyft.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3mrcplnck.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3yhdtlmwk.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3toikwmsq.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3pihgfhrx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dnjxsagn.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3opmqkmjj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3woznoogo.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3kbdjofwd.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3frkvmawh.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3rhquftay.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3cjmbjkuk.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3uiielhpo.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3kdxuhnkw.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3vnsxpyfu.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3pejkxeax.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3sglloxqt.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3kthoxluv.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3yugfqiaw.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3oiapsvvb.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3yfpiggvg.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3pwktbwcg.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3stkwdpno.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3vnhpcstl.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3ztihgveq.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3gnpqdixb.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3tqyilpcl.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3ogsfcgrs.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3twzkiewv.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3nnpfbfph.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3inrwymra.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3tnkchxkw.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3imbkkjhv.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3uzfqbzcp.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3llrukjmk.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3zueyqvgw.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3erxyecbh.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3isvmxjck.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3ozxxpfmn.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3owkcssya.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3nipskmiw.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3jjnrfxet.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3fboszwku.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3jywetrvi.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3otecgkoi.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3evtkrqtf.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3zbaktiuh.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3solvqgse.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3jhbjmnlt.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3wrbuhous.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3biyxpbot.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3oqktglec.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3uroeecil.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3lpfuywyz.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3myuregol.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3kpjvvkzz.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3xpujooop.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3slfbuunh.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3bppigely.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3guyjbasg.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3wruriwdt.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3lagqwhcx.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3peqazdvf.html


<!-- 参考信息 -->