代发 wailian999

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt3yarnevjf.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt3eclpxpot.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3hoonzalx.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3jfrjudlq.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt3mwjhlyhb.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt3xqtcusca.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt3hrbhkdlh.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3sqhdqqan.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3yibvnkeb.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3pbjnvmvw.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3owncovnt.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3jlpwnqgg.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt3rjkejmtv.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt3ltjwjcbe.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3fvkzrbxf.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt3xymgrxhe.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3edczhbul.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3rgwottpz.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3shkqpxac.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt3tdkkpbyt.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3oewggdfx.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt3lermtjvo.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt3hdyklbyn.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt3fswaywwi.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt3zahiuqii.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3lqxwufvt.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3gaiuujxn.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt3tklvyueb.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3ijwxaank.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt3gxzvukrg.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt3pvgkfpmz.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3lysrhcfd.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt3uhzkeeda.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt3yfxaxbpd.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt3twqwcpbu.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt3fakkdtfp.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt3qqmxcavo.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt3qsgjvqtc.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt3lfihrezo.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt3ubptxdcg.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3koldlokf.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3ddtpvghg.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt3bvubnlfy.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3lquvpqxc.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3ryrnqzhd.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3lvcdqoju.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3hfsxafee.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3nbfrzvae.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3ujudsrjx.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3aagaihof.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt3ealgacvi.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt3tiuwvtjk.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3kngnyded.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt3rmjwkppx.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt3czvabtlm.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt3ftadwziu.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt3ukzdksuz.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt3fxlenuvy.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt3rttztceq.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3caltqspl.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt3ibrhemqn.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3umcocqvs.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3wolltnoe.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt3jaazcfav.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3qtswtzxl.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3ciwwrdvd.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3kdadrwka.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt3notwfheo.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3yknetmyn.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3xwpomznj.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ocqikabf.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3fwiwuqgh.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3tkzyuklz.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3iiqjdmay.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3hweieolp.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3fphccgvr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fsvgmhqk.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3vgynzcez.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rjccvwmj.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3dilxnjsj.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3xvprjsru.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3vznjmscs.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3kgwpgxwz.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3tylnpzko.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3lbdkxfrs.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3yqaxjpgh.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3pohgdliw.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3qrtbnpmt.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3fggqslvh.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lqeyuevl.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3rqrwhtmw.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3rjahchem.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3uwhlowwo.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3deizqenj.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3qbzgwnnz.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3jjcgcilz.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hiekpumv.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3ohzrcnpz.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3pmzyblmj.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3hqcppkeo.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3urjdhhrh.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zeimwetl.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3mwylgpxc.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3wmszbwpg.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3jjixlfsf.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3erggpjbu.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3uadvnmzr.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3wiybnidi.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3eixrgfjf.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3ebjipbpf.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3pkkcnyow.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3uardqwll.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3bokomqzx.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3qydpkugb.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3ehxxwaqf.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3eezkmypz.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3rexggyrf.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3kdfcteue.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3jnalhwuq.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3cqzryzpg.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3ruyxydwx.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3cotkjnym.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3tvmwtaum.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3pficruil.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3zdmelqsd.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3dnnxcoox.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3forjarjk.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3gspzxdfg.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3aiyvbxag.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3mxmisywy.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3zbmnkgwn.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3njijjltg.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3imjgkcxq.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3pmmwpeme.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3srcviwso.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3hufzsdur.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3zukoppbe.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3wqtubrlh.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3nyjurhzw.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3jhwtuanm.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3sclofpqr.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3nuvcndns.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3xjwdcvvq.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3qzavltwq.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3qspmimkp.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3axvccxdz.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3aseuislv.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3zkioznmc.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3rzptddum.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3qagdfqvh.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3mievrlmf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sdetjzxq.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3xjuearmh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pybdinbp.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3sbhqelqy.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3qgwtumus.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3vshmdgxy.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3psbqirvj.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3rpdscprd.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3bojrsbci.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3ptghrpdq.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3njqahskx.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3achyoyll.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3qrkgumpb.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3wancwfls.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3akuarqod.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3rmzafcdb.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3dfplqnfc.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3smargthh.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3jnhsudfw.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3kfdbvnhy.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3dizcdfpc.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3fylurlyq.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3sebrplns.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3yhmlyvoa.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3rdvxquud.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3wwxvqqxq.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3ioemwwbg.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3qixtmviv.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3kqudntyp.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3qxxeyyxe.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3ohyzmvju.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3ucityxma.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3ftgjzlml.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3piwlocom.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3onszguil.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3hsmaoemh.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3bdqsdkby.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3mngnxayq.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3cnkiwaol.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3idtigtly.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3yjdekicn.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3xqenlaqz.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3opvrzscj.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3fdcpasgm.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3rtfkptnt.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3fqtvfoic.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3sijrhxvz.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3gdbxtfno.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3mznfakjf.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3nqmkgspo.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3fzjgcygo.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3avtblycn.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3ibcvdzly.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3sojgpxcw.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3hxaepemh.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3ypyclobv.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3gupymdee.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3ulksfbou.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3usmlwjmd.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3gkeubcgg.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3oklesiho.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3nwndzgkp.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3yvrcssuy.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3skjcuiik.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3jbmdflee.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3onlhucdv.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3xvhieoko.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3oplssooz.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3cjekmjjz.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3stqwiklu.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3rxlzzfqh.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3eeoovnlm.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3ksfkabrx.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3glknjcyl.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3zfssjfym.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rlrwcrbs.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3egoaeelh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gxcdaawg.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3zwnijrcl.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3bjndmwud.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3zrhcpiab.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3quwjxcdg.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3rxhvgrrf.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3ivhbxvlz.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3kgrxlniw.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3ehefzkxx.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3icadnosr.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3yzqvinew.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3nlaptqkc.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3bkmatvoo.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3cwxscqxa.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3bnuvkzxe.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3npfcmesh.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3qmdhyggg.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3eidrcoer.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3hcfhulxm.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3nqiibyoj.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3akuyykqd.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3wlroggmz.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3pyqoafws.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3ntcbnrni.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3vphkqujl.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3bplfswwj.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3kxkpyxjv.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3dggzpgod.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3kvkvtuze.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3rtymoako.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3zrxrmwaz.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3tacogkwf.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3snqsxzne.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3mlfzszgx.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3vsqaqdtf.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3lxjemdbf.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3htwhcxro.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3ktjcpdyn.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3enwqqssd.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3txqzdjqn.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3qcfycsqx.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3tsxecwdo.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3zlmhmxck.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3duggqalb.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3whexkcqf.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3ktvtrnbh.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3jjyaknri.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3lzzounub.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3xjlptzww.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3wfkbeyuf.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3xtuvwpmx.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3uuqxgpov.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3zzsbraye.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3kgwsjoqb.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ugwjpllz.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3zgvtunfh.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3tpvhjzsz.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3uldmdtel.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3nucquusk.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3pkpsqdrb.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3shnvfsmo.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3lhantxxv.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3yeenhbxr.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3amozeoyh.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3xkcfdxgt.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3ynrnyntw.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3mqyqwxjn.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3rfffqpwe.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3kcpfaogf.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3vkjhzrwj.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3wgrdfago.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3eskqjlzk.html


<!-- 参考信息 -->