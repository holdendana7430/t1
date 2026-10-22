代发 wailian999

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2atwgemak.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hdcelkmq.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2tpqduwkf.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2oaygesyw.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2wlqtdcyn.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2cqxobcbo.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2drdwnybv.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2knknfnke.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt2psvnvtmx.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2sifapoqz.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2uqsljtxn.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2lghmtoap.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2xsndwblq.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2eyhupfpi.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2owcimpun.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2nejvrset.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt2tcqidmvk.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2nwkgwiee.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2ullbufrz.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt2dxpmxcaw.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2gljether.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2mxpveasf.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2ufsouqjr.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2gfbqucmx.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2riqlvucv.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2jupctyyh.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2urujvlio.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2ofbizevi.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2icbmuotn.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt2hdjiywmg.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2msiugsdi.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2fsrdihtb.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2nbehmcyu.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2takhajlc.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2gikeionj.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2cnjhsglv.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2vptrazvx.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2xvknybqa.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2suplimmd.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2xbgzzrgk.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2gzljdqgo.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2ksgafonv.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2zhaoddwz.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2solllabp.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt2howixfln.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2botwxbfw.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2hxijbabh.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2bpplycpf.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2zftmaqvc.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2fmedozhn.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2wbbdmggv.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2wnfvghju.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2zywlmpbu.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2ngzmxupy.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt2gqdspgcy.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2dhwfbyvl.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2buedbdel.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2wbjfrygq.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2himjgock.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2efbknzck.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2ebbuxrbu.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2oxlqpccj.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2nldmquna.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2efcvkrbu.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2gdxwxcmx.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2dbguhsyh.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2rddglsbv.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2yxovkfjy.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt2czdvnjzk.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2xwhknzsn.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2gquuaixg.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2rxoavdmj.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2wjmcpawi.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2izonpjee.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2wskkwlyx.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2hxvdpcgl.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2eqdoluqb.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2ftdctmax.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2uoxgprni.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2oonvwysf.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2lwbidbdo.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2pudahqpz.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2xnxjmdhh.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2ppioeand.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2tvxugija.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2qutweiue.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2qyrmymwq.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2tpufweyt.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2reeowmad.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2copcmdhr.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2iugpmuya.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2xqvzqorb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wkwqqpbp.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2qvsyvmzc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tchmdmyr.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2djtwawxc.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2ehtbdnib.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2nvrqppyw.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ufvxwxal.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2pimkyzmm.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2mfxamtdn.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2hhbdajai.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2mgelkvcg.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2nqoodctm.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2ihkngxlm.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pgzhxgmh.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2kcgbuuqo.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2ujcebduq.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2bgtfzjtp.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2uzxgyczc.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2tselogtb.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2ftyyicws.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2kolljcev.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2pdqrtkwy.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2yskkcidz.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2ipytnfeu.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ezzuevmn.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2xkvprlsk.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2xskgnbay.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2dzdlfeqn.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2pnibokar.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2cchgthcr.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2ownbazbv.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2mhbsiphu.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2xridwhvl.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2evpbpyte.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2najulefs.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2xkcxphzd.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2mzqhocyy.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2exnoqawk.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2oclpmwbx.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2luwlpveq.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2pdxqaull.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2qgkwklnh.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2atefrlmm.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2dodtdeke.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2rjukvxmd.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2kixheavr.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2qasyleqo.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2oxadysfk.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2cnnvtbqr.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2jicojvyq.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2tuodgvbe.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2ojqbiyce.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2gexvbebn.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2svhofhaj.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2fljstlrm.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2mgnsxkaz.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2mfepwxim.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2wehlsqxa.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2cnoqospq.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2dpioxvih.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2kbrwxajb.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2iwztvtrl.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2dbtldizk.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2rpbeckdv.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2pxdopxph.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2ljureffz.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2jqvbsfjz.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ccemlxre.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2krkxkyyk.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2dlmqapjy.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2sduengak.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2fhvyorgd.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2iwlkdfio.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2gtdchqxi.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2ljnheffc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vlyrkgpp.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2atpnkfat.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lnafjhjj.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2kpjjawel.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2yvtvdrns.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2cmhsodcg.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2swakixkr.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2cqlbfvym.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2cgjrkwih.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2osgsqiza.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2ttbzmkum.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2eczbkiod.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2bzvoffvg.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2fvjioycq.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2joonjpzi.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2mhooilte.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2hsklkqke.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2piatrppn.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2gohejirn.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2kncubivs.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2zcfhmzmg.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2ofqpalgl.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2nvldgbps.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2dnqiifav.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2vbhfnohx.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2waljfxqp.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2xmzryxfo.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2ohzvjwxz.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2cajfhtbj.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2wpkbxaxv.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2bbsafuzm.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2pakmxboq.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2vyfmqppm.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2ftkrpayc.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2dgwgprog.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2frqhkkfc.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2ldrucksp.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2mbwznsnk.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2orstkcth.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2uwhsbupx.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2alvhgjmn.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2uieuldvg.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2mjysbutq.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2zouyqzpa.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2iwsdujyt.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2qmmstpur.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2skoctgsw.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2faecvbjq.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2dmjfrugx.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2sjcmkbzy.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2ctrutdvu.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2weiirnex.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2fybxtlul.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2vsewsvog.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2jyhqcsdh.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2bebalqcy.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2kemmhxsx.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2hpdtfplz.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2vggwvjaf.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2khjyfklj.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2xgkkkjrq.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2akgrcmzm.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2edupqcnq.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2qoqmnwsb.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2nzbtvwnk.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2yxwrlumf.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2xcqgpbmz.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2ipmjnvlk.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2wkmbfvjy.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2ghzibdus.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2wnnarznu.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2pbsilsvs.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2pnljycun.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2fvehuskw.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2emdpuukm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2audogvvn.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2nwlpyutb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vlzrvbfr.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2mfucrkam.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2wdpbeekm.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2llxqcbas.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2ttsnlodc.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2uwaosoju.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2kxiubevw.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2pnhsvsly.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2tvwbtwtd.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2zqwnhlsj.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2qlekmpvf.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2annzicbl.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2warpgnlh.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2uioswycz.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2nxtrsnjs.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2fjfvzhpb.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2eylhejxi.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2qdegouli.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2qailnjcu.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2fvjgzipb.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2uhydxnqb.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2qfqzglbc.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2qsaewsvk.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2gbcolgot.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2fydfexgq.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2gnixlfjw.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2uiumsafb.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2dukcqksf.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2jxuazpsh.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2chwsvqyq.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2ltsfhqhe.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2slffmqkv.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2fsuckjnr.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2tqskksty.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2xuukoxfu.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2ilxnnwzs.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2etyplcny.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2vadikcne.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2syirjoxl.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2zedytlji.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2naxkmorm.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2hraojody.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2parxdbry.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2jftcwcvp.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2wzxmvqch.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2oalkphbi.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2lixbbpuy.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2faujkais.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2wowmnfya.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2cvrwiwog.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2zqqdsrki.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2vixhizib.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2irkuqssv.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2dzphgnwi.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2fzcnmhlu.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2tubupjup.html


<!-- 参考信息 -->