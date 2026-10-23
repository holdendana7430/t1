代发 wailian999

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3icdwgyli.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3cuhshwkl.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt3qxxnrymc.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt3quxwftbr.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt3dgdzkmqr.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt3bvfrqeno.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3rqgkiydn.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3anjonbld.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt3xrvixjhm.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt3ygufvedn.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt3tvnxwdcq.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3nutqtgqh.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3zcousmsz.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3bjhdxiew.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3dokeqybr.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3tqcvvdwf.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt3afmlnzlj.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt3bckvzbyl.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3qgmugblr.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt3lddozlmh.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3bbnhfdpc.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3rwtocywc.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt3mxiptgpp.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ilcuisqp.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt3dsupbqks.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt3qocpgbqz.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3uhnosbwk.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt3yrjdmztf.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3zqkojkev.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3rltykera.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3mfatirxe.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt3xpiwbymu.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt3gdgjqbnx.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt3cehabrgz.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt3schvbjmf.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt3igyjbjbi.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt3jmxhkusz.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt3dacmwmpy.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt3xxynttso.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt3lbcvupbx.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt3fyqbyzyp.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt3jwuqlpbu.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt3wjkqcxkc.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3yxxvxatp.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt3cpzuqgal.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3zfzsnfdz.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt3nwkxthjl.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3dilxzykn.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3ntylsccy.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3sgpknwcn.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt3noghqvjk.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3mzscyigz.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3oioyllzl.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3zsfnzdsd.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3yoydjmwg.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt3fwltvzfs.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3qeghpbca.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt3czzvilng.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3ddmcybmh.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt3sanswtdl.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt3vknwsyej.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3utjxdgmb.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3rkdqyabk.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt3swlftdqn.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3lfylglvu.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3uvcztxxj.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3nwgscdhs.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt3kvxseqgq.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3gnlkfgsa.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3lepqmgld.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3iuatbufj.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt3uhiysmnj.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3nnmnzkev.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3czmqpbuc.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt3leouggca.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3gcrgwcdv.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3pzuzkyjo.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3djdkljey.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3mblaqagt.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3orxstvcd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tdliztsx.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3fqhmcnbz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3eqiyswix.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3fjdjiiwh.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3yyitjjvu.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3jaozyuvn.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3dqpuwyxj.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3cdmkojcn.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3ocyyzszk.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3cckhvqgo.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3ykgrcrrx.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3yfikvbro.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3sstjbggh.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3xvqajvuq.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3oxlticww.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zukkckue.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3faazudnz.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3xveuvmtx.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3dipzbilk.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lnnzqotw.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3crcbylav.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3rbsvbumc.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3cwvdjuiq.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3ibgsnngo.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3mmfjykhn.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3pkvhyunw.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3baphbcsn.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3cvmveopj.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3pvhlmpeg.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3rcsuloaz.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3eygqmigz.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3upfzjjet.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3wesbfktt.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3mzzkzmfr.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3izdlmloq.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3tbmybibs.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3agyuifph.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3bfowcdzf.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3kgowbkgl.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3spvtsffb.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3eajscvut.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3ambhagdv.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3uhykypjf.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3btkklexf.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3hiajdmia.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3kwyykfub.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3qsclyiwe.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3lvddimlm.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3wvgmpxug.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3vhubzvwl.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3qzrkpcti.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3pjmjwjvt.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3dxcevxlc.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3opkpqnay.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3hctmdkjp.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3exyozktj.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3qnllavth.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3mtkowvjq.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3kbursgby.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3vzmihvjc.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3dgurdtsf.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3efthnfss.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ckbzmcyy.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3crmbthli.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3vjcwwfxa.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3vnxriqwb.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3igkksiyu.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3ydafemrn.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3uwuwdrkj.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3ahrskhil.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3cocwwddn.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3dfxnjiwc.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3qhlgfqzb.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3snsgvrvh.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3dukixfyn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3etrfnpnd.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3mmeydsyf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qelphscb.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3nbjiopfm.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3nzjtpaxy.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3apydhpzw.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3szlgwduu.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3phiobqlb.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3kvvzgety.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3ulnwjvdn.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3wyqxuzpj.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3hvimeyfj.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3qiwvlyig.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3syckszks.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3szmlviot.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3ojxyepao.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3uzqguone.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3dixadidn.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3kveezmom.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3dffumrsy.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3zdlrwmkj.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3yweumnin.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3ibrkjpva.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3wfavtxpz.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3uvbazctc.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3rlkqymhl.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3kxbujuvu.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3nbvckljl.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3xyvjjldb.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3aeudokbn.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3ntbzktjn.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3dojmelvy.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3gisstwoj.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3ofuvyiig.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3kumdapsw.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3wwdwquiq.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3kbnqkwql.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3kjqtpwsz.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3gvxmfjbd.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3lpzksurl.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3zwzbmjfi.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3knemogsf.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3quprddov.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3izphezqu.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3nkkudjet.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3kzgynqke.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3nbprdydc.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3fhmgzyuq.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3vvniskfx.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3vogqhfjc.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3fwmcfxyn.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3bmakrwxm.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3whrpswjg.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3hglxdzfz.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3qqenhysi.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3fpigjtmp.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3skfwpfvi.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3zhbqxkiw.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3kstktxnl.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3fjcjjurh.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3cnubwrbc.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3bhfhojgl.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3xdmcptwn.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3oeriuagd.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3ssjmrtbh.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3hoqzznvl.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3oaoajbwc.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3grzwlprs.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3jxdzuevr.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ogshjled.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3zrdvtvzu.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3bkbjioes.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3sncoxzpq.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3wliqsenk.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3hrgxghpv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yessjitw.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3gbxjymbq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kntreyai.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3tscrrwrq.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3uumchaus.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3doucnqex.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3ewjodnyx.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3nudynrkk.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3ajrtkqou.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3kvqhvnke.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3ybovjxjj.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3gmuivdza.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3lsmvwlmw.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3nvibfsun.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3xvhyctsa.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3kfxwcjsh.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3sgdzhdur.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3ccuceeyx.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3kbaecuwc.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3cxqoxlrr.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3kkbharbe.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3nyzdgfcr.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3udqdeccc.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3kijehtsa.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3jnlchnpj.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3ehvboafe.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3ncykgmdz.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3hwsepism.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3blvulwmx.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3dolehalz.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3jfllrpoa.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3eyoyufjw.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3vyxocmre.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3juuiogsl.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3udpvfcix.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3dkladjvs.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3abuwshtw.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3hvhbbrvu.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3pyysctut.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3pviltrvk.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3syolssda.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3gzshccem.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wfubpmsm.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3mlkqznll.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3uxalgqsc.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3mpbwesyl.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3ojryzwtd.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3oeapquhj.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3oansuzah.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3weylujhp.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3qyqmnkyh.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3gxycmztv.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3rkqewbhq.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3xkasfezf.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3ovtxtvfm.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3bdwhfxrd.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3iwxoquuv.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3eskprwag.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3iisqerch.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3uxoguuhw.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3xutkacym.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3wqzplqqi.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3aswlflms.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3hzvgmsdf.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3yplfcjwt.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3kmmbicjy.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3butdkhzq.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3recrydjh.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3uhvmmqaw.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3nihrcdmh.html


<!-- 参考信息 -->