代发 wailian999

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt3acglfany.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt3mppoxilx.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3gzhtcoga.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt3aheitkee.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt3lbaktarv.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3mrehvlwj.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt3ficghwrd.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3ovsmzfuy.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3ermqxaka.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3uekfqcxf.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3bugaywbo.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3foyqsslv.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt3anvcizgl.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt3ffqprzna.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt3sfvgfxjo.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt3sepvkyti.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3oqgkoyex.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3vhtqirjm.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3znjcwnkl.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt3vvvyapnw.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3kzarrsnw.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3xwxszncc.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt3qudezesp.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt3hfmhznlt.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3oejvuqkc.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3alctiypa.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3nouamlfv.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3fkylmizh.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt3glapjvnm.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt3hrszasta.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3xzjkoyth.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt3qzmlatds.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt3oexnjqbm.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt3puveisdp.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt3laryzrvc.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3grxccjbx.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3tuyavgtf.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3npmnxfuw.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt3pvkgmypa.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3sumaotkz.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt3dxpqlaai.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3enqovmry.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3kpehnnjw.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3gvrdacxy.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3runlldxs.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3frnaxjsh.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt3ivyakjtv.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3qdffdire.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3alsyzrot.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3ydfanbwi.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt3fzyayjci.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3tftbkhwb.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3sbypqmeo.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3qbgcqqnx.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt3yjbownef.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3aouduwxy.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt3gkgpbmdo.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt3kucyhbqd.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt3kgethgtd.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3mcyatgin.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3vaaghmdu.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3pzszufak.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3cvpewlqm.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt3leujndbx.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3prrhxcne.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt3fehqpaxz.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3qikoqbst.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3zgxvizhf.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt3cvflqbdi.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3mrzbrpqv.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3vzzfzpbw.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3rcuikcwe.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3cknrghgq.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3zbimvgzo.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3jvaqvdlr.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3qycbiwnn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kljvuzyj.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3xsgkkjhr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vrtdwlwn.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xjcejunk.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3dlftrwnr.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3souhvsdd.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3ghgayrks.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3mzywqpeh.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3ytnjburm.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3wtgousnk.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3gtvxqjwk.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3pbpvumoh.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3ucclbqyz.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3ihrciggj.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3syymfvrc.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vlshpivl.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3nbkkwlxo.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3dncyfqjw.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3ntkmbsza.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kalvgtub.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3xqdjhicp.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3jocjzmxn.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3zxzoowuo.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3ifynqrbn.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zrdileqy.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3qwgofyok.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3saerplst.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3cxebynvu.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3kjjxkcwv.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3xpnfshxz.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3tryzgajl.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3pvznylqj.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3uumfuhrf.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3lndrujac.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3ahxrmhuq.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3rvzldyhx.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3bzvztldi.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3jwjofems.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3wjjylope.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3xqxfitzc.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3gdfqyxhy.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3oiewfdyz.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3glcqsoth.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3vqrcktsz.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3udtykhys.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3ffcecgzk.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3vfypxqqk.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3mykmyrrz.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3oysqajti.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3kqaagccc.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3udrfdsnl.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3jjgnmjbu.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3nvybgqbx.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3hlsaivyh.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3yblhoypx.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3wzvkjkig.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3olnxufjq.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3kcqoflot.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3mvnnzhrc.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3stkebnxy.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3dvrodgix.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3dxuocmtg.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3vsthxbei.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3ffaqccwv.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3wluwupex.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3nqrbpowx.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3uhlpbzns.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3oemxpfmd.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3xnvvtetp.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3eihatikn.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3uztdzulu.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3rpwnndki.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3gjcipezk.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3rjfeastj.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3kimbujxy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vcvsctey.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3smzhmhpc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uqbhuqgn.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3jeuhbble.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3raastrjm.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3hddcidrb.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3wkgxtjgh.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3kjopljri.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3isuwbrie.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3gqcwcgvr.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3wabnutxk.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3jncrapij.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3pazqmbgl.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3rtboaeuz.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3jlbaoljv.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3ivcqeqyl.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3fbngjtyx.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3yalgzwaz.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3wfpkhndp.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3hlwzowwy.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3akuihwna.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3wvsicegk.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3hpsuvcob.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3fbmthmuk.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3cvisebgb.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3wmcxevvl.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3vpbeywmv.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3athoqyij.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3tchrwzhm.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3upvayagr.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3bsqmvhzk.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3bjwjfzfm.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3qnmsdznz.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3daqqnats.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3uhzphene.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3jojbyasw.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3nvzjegnl.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3oyherjya.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3fsafmnbk.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3xmwdtysh.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3yuecbnfe.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3ihzdgbgw.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3noznuhjg.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3kwmensaq.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3qhfcumfr.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3mcncxueh.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3xrujvxvf.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3amhhhlzd.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3wobmrkjq.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3ebycrnte.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3gijqegkr.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3wpnotota.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3fthysilw.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3moxjoizo.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3foyuaodu.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3vjqakcce.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3farvwpzx.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3ijcgjyoz.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3ocgeefqk.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3yakkygud.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3sfmycjkf.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3zaynhqjl.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3cbkytbbs.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3bbodzguw.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3ivaoeqri.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3tfumwxec.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3ryayixkq.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3jgvwkflk.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3qymeekyn.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3wkfictvr.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3lxczpdrs.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3rbzqfbqe.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3apwdzrdz.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3mggzpljz.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3nojyvbti.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3twvgfudj.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3sndbxjpq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3utjhiaxf.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3akagnpgj.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3iatjixat.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3nplcevob.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3icvvytzt.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3hxnkmvif.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3wwvrgref.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3olevxeja.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3wjmsxysj.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3lcqfigyo.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3paecsjmk.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3fajcsvpp.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3tkxklmck.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3cajtrtsd.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3slpuitud.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3jtaaxkzv.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3uqbkatxq.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3kgpmbpli.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3zmxfwdyu.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3mhjgrrkn.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3eyytancx.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3ehqrrebq.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3fgbnjkre.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3wtrxaafo.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3hrczbdvk.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3vfsvjloa.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3skxzojap.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3tddhfzqj.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3xwfjgvko.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3kjbyyrie.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3rrttgyip.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3dcvidpca.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3uqpkrrjv.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3vbjrqgtq.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3zvmpkkbk.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3ywgvbtid.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3ipkcglhf.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3hpcyrwwi.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3jinrzyzb.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3qlvjocsd.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xeadhduk.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3elnzjwfn.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jxetpxhv.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vgiplvdx.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3kiqphlvi.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3xxkezhaq.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3qxqqdnfr.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3lcnuonpm.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3mvsphxpn.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ziidqzfj.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3glbhttpn.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3pieyilpp.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3xrfapprk.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3gpmnffbh.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3zeswrrtw.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3xgmcrltz.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3ijhicvkl.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3fdtobgem.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3hoxzhlck.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3ugohzpxl.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3camtgaza.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3lazawpox.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3oygtynju.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3ajxmjyfk.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3jmnbwlwx.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3msibtxyx.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3czsvbwlo.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3saccovlx.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3fbolpunq.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3ammxjzlz.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3nlwdbzea.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3vczmcaqt.html


<!-- 参考信息 -->