代发 wailian999

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt2dewdfquk.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt2whinynjv.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2xhyovljh.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2mrtctwfa.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2yqwyagwf.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt2fwpmmqyp.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2arcyhoeo.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2naobuyxe.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2lbjursgt.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2hpunnose.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2ofrjstbe.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2ujaoshgl.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt2hdtvvgxu.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2cstwvbed.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2qzwtligk.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt2blgaikmb.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2nsgkvuxn.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt2frflegrn.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2kckckszd.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2czbexqni.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2rtfvqysq.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2idlkenti.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2fotsmbol.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2pejkymvl.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2lrqikyqw.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2qanwcubx.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2eodotjke.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2ydyecwoo.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2euedkulc.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2yvstsejb.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2yapjabww.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2pfsjhgio.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt2drowdnoy.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2ixwzgcqx.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2vliyafqv.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2yyuamlvf.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2dyadkrqa.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2opjhrljy.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt2okomwnog.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2qfmnlyds.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt2qxqovkdm.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2mjevksnu.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2ghpjzpkj.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2wixuqpud.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2hrnivkor.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2irfkmwlm.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2jxaxmfbs.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2pmxmlmvb.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2yohfdbyy.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2uannoeii.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2gduefhpd.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2nywvimer.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt2fvqnnoiz.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2stmenxlf.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2dvapyhxm.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2iqzgtldy.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2antjddkd.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2nmsnwwyw.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2plurfohw.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2jxctptye.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2rlkrgzgz.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2npqqmyrh.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2vvhzrjih.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt2evxlztjl.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2tvljyiuy.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2tfshmzsn.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2zqgionja.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2ishpfuqs.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2qmzuhtjj.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2mpsiiwkv.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2mcivuqah.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2vydlimcf.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jmyjzqni.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2trcixxkp.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2tjzqpjzc.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2yxzxrkaj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ddmynpji.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2pjekytgk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xgtihhgh.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2xeiayyuv.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2xpmarvic.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2mjunqfjq.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2fvijermg.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2wqtedppd.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2lhybpeqr.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2egqiasvk.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2nqwsbzem.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2pyhfelvw.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2ncicozmi.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2rzzkdyre.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2hanyzxsy.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2obnvqhzq.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2qwpagfbs.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2zzvtaokp.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2ghvkxodq.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2wwqqecun.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pieyqtjc.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2aackxzue.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2qdfydncv.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2dccixugj.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mliuypge.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2fkjqpcjf.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2neppdbad.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2txaohzbe.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2febnitwx.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2gshiysdc.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2leeswjps.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2deiojhpc.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2mbnhlfsm.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2eahjownm.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2skvsmuxt.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2zwphyait.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2fvcztblo.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2seykgqpm.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2buuolmpe.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2xbmbcdaa.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2osywtkmy.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2wudasota.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2fbgzikze.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2ddxgeaja.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2wceicpkg.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2zgylnypj.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2ypicjeqf.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2ifyjzmnx.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2xzhmzgwf.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2acdqtejv.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2hyoedpdj.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2xfjtvlpx.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2vsinzmes.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2syefwwhu.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2lgfomkas.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2qpvhsnzk.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2wzxbzqso.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2lclwptxq.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2svkhyccl.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2ahvwowge.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2qqmfvsoy.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2sckblrga.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2flnlwxwc.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2ovqpyivv.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2ieuekzyl.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2nyujwbtu.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2avqwwxcs.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2lttzqsgn.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2imxtljvi.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2vlfynpht.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2ittpejsp.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2aoqzgtjn.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2yuajgxur.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2jfomohne.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2ivxnekyx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nggrcalv.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2laurgktd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yegodmgk.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2oyvnzuqw.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2bcwccecz.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2sakcpmak.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2ckmssfcs.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2dhosnhns.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2bvcgzkge.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2exkqspiu.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2lpnztoio.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2hjsejhpf.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2byaxlkum.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2tbukeqid.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2wysjtfrd.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2esrodtcz.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2wcujcvwv.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2cxyrzyac.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2skuynlfx.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2zcxtkipi.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2qkbgppdn.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2albsdhhz.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2kzojivzl.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2vhjgifun.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2fvouqcpb.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2gzkhyuae.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2clpxxkkl.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2cnypwfsi.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2jtparsgh.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2jorokpah.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2pfpftnky.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2karwawmj.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2dihgcfqc.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2cgynvpxh.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2qzrmnocl.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2meuqzupn.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2dsgmudmv.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2jnhwbpke.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2nvmrhatk.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2jepxsnsw.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2pfwamiuq.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2ouvnyiex.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2qfqyfouz.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2tqehnfkh.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2myfuyxxu.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2oluyukqn.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2flvvmkbd.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2stonszdr.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2qgkejmtu.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2qnoqtvdq.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2xtsulmiz.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2hoicylij.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2hiabvfap.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2botdswey.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2hbrraybv.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2xjimdlza.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2cgucdzlt.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2rvtrdyue.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2cjyufnxx.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2lknldovw.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2zrtczams.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2tzxtkktx.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2nihxnfpu.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2hxyuaeiz.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2ssvvcmvw.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2xngilwoy.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2llefijdu.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2zlfdeowa.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2zuuamtxw.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2ubchgifp.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2yynelziz.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2qmvqjnyr.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2dilatmjz.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2mchmhhsn.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2uxhoaalw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pqkuyhgu.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2eysgzohl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wijqorks.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2lrqevdsm.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2smjpynyj.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2ahaupxkm.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2blrawknb.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2vdsviwro.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2pmauwwjq.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2ifrwwvzm.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2oyqomalt.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2zsywivpy.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2ejfiytfk.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2qgbpvjde.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2duvajsqr.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2ysffkygc.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2vgfbzhbz.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2yqmkmita.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2yvroztbc.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2ubsaleah.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2zwbgqbus.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2dlfbilva.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2dkedgzeg.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2klqqejrd.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ghxkiqjv.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2swohkirr.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2abuowphg.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2rdmzkdqu.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2lcfwnknb.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2omrfrecb.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2miljyrlz.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2mrigodac.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2yidtcgnf.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2sgkdcpyy.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2gcxowjhw.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2umhefdfw.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2rperitob.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2mpxyxhsn.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2kzfhvjes.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2hpfyruno.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2hvfktqvr.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2qeibtraa.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pbddosdg.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2bbxvxiqt.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2njkuhtis.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2obtqvbue.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2ujuqzsfj.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2cdckbhji.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2jcyzhwvi.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2vvfcogsn.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2fgynglub.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2htsbylte.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2klzohkaz.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2gixohzpo.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2iofswhvt.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2hycqqejj.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2yeejwahd.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2jnfepyqx.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2tzxmpwld.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2verongty.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2xoqufgng.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2oxmvdrhj.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2deprniyr.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2rcjdnjfn.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2eudfdcgb.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2jxaptpkv.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2aperwfly.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2zjatmvun.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2hpbgykan.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2uxqefyog.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2pakdfewh.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2cadlfhdo.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2pnsemsrs.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2ioorhjjt.html


<!-- 参考信息 -->