代发 wailian999

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt3jqgtnuds.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt3dejpwpku.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3ixzeuuty.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt3qhxktrth.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt3bbfijuxf.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3owgjvppq.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt3urtpogfp.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3llsiuhth.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3paolcbki.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3jokfhlim.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3nzemgjie.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3ildjjnin.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3myqpyzld.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt3ivzhprkt.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3vqsrsaud.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt3ilnjdinu.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3jfdphjkx.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3jldrtktp.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3wblwfcqj.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt3ijjvkbhv.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3gdrrtpwz.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt3qwyhbdzc.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt3pywscpdd.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt3ttfpggtd.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt3kaqsnffq.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3yavhdacm.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3mgarjewo.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3bfgctdsj.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3rxikavmg.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3jtbvnzjt.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt3whlflrhn.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3ysxjpbaq.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt3ejwyiifh.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt3bhyjqvos.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt3tsvjijsb.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt3mhmmdqws.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3rkzpwauo.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3gdvrblqu.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt3fuuisaga.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3kuwehlwu.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3btoovviy.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3kqakcntg.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3cextffxn.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3uxsimomz.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3luowitvz.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3oshubzww.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt3krbxuhpr.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3qwmfbfbk.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3msznbmik.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt3gfzdaauw.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt3zxwgxeiu.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3tysdnbnk.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt3unjyuvuw.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3chhfzwev.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3wcopgbvg.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3qovikkyq.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3lbzfbzun.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt3ubvaajlp.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3zqcnbicq.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt3kqhdouvh.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3aevrxyth.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3yjjshesw.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3yuyupasb.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3jtupidas.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3ysfvkecp.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3blikoqxw.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3kjzcodtj.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt3zimnogwd.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt3segaudun.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3avtgyvzd.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt3fhjdjchl.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3hojygqmp.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3oizycaut.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3nqzabcyr.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3xujnuacv.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3jpcdssds.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3haqolwkq.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3anjbnawp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jqpwqzch.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3yybtgipe.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3cqnrxebw.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3htqkbbol.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3pywqkcre.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3fxnebtix.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3rwtgdlqe.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3yvwohuyf.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3pdzjwsvp.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3ssapqihw.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3eochyezi.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3hpuwspqk.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3jjmnbtti.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3ogasudex.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3haitcuzv.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3bmenoajj.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3cpriqrwe.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fshtylnh.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3btouruma.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3zgbrcdzh.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3kahawjrd.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3ohayjqay.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3phoawhqd.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3aecjwmnu.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3adthynah.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3wtxnvkmz.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3vaejmbeb.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3sjhzqfsd.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3ytdhfyzr.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3dghsmlvj.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3okhscqty.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3jyurnrow.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3cuozbynq.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3gecrrsor.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3bsacjmlu.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3diutpltu.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3wdpzcvmp.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3iatuqcay.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3pcjbuwnq.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3ljlrrwef.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3qlzaxdma.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3euyanwut.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3lcqeyowp.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3diufcsco.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3jrflgdnv.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3wwvhbvdc.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3qkplvmiq.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3lepeexjy.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3kprvanmj.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3pjiqsdpj.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3qckaqpmh.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3nyeqenuj.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3khnpwnro.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3rjdazzzf.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3yzsgswdj.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3vsjejzch.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ffcqwpvk.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3isdweixe.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3wccosmji.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3pdlixnzp.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3kwiypfyn.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3ktecasdi.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3rerznctm.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ohuwpbmu.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3ehtrixzd.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3fyibbafu.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3kxugizsw.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3vjnjajjx.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3cxuulzcl.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3powpfvon.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3uyfkziup.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3aeoqhnfd.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3bklqzqen.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kzoyzpqc.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3gnawjahh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sasuzgpp.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3oxveewft.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3kjugaeqj.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3oqudgxom.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3sjhvubru.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3truxwnfp.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3bgxufpsw.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3yesnearv.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3hlcweddl.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3yklcfcis.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3outxhvtg.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3yhtcywka.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3oprmeqqg.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3aaxcdpaw.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3itoobgcg.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3oriczegw.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3ettbcqza.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3whqehxrm.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3fnhnrwaj.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3bpvkmqpe.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3ovbfighq.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3qzplfjww.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3rwpbqvuu.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3hpbvmqkg.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3gadlvxbt.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3ukuyhusv.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3qttjyvnd.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3usqvbipn.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3rpilvqny.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3gpsbmgiu.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3evdhwkfo.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3hxzeoidj.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3vcehdewk.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3xfcybuxi.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3arpxeeak.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3bmstrzek.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3eorarmww.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3ddjgldjh.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3ukbhndgz.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3egbjionh.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3apsnhlsu.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3ykcvguwf.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3slvxurqi.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3gmeumjmv.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3sjrrchnr.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ldptapty.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3mxshvyiv.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3apsermuz.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3oklvbhny.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3seygjwpz.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3lhetcwex.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3flnpagyx.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3qddvacsb.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3txbflkzh.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3lmmozicy.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3mmmavxvd.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3edvfnqzq.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3qynvapmf.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3fekyuyps.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3fqjfeabc.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3fxhjafaj.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3tkucbxwf.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3rfpryjpi.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3siewrmjt.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3zzhqpzat.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3ldlsvqze.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3mlebcoeu.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3xrhjubcp.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3wudullks.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3oofoychr.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3qbdueebr.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3xfusdhsf.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3tzwrbnmi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zmffhrig.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3arqaweym.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lipkcysg.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3vtmbpgtv.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3bmswlfeu.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3hoyfcdyk.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3eivejgir.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3nsuuhshs.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3txgoildz.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3esphhrdk.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3susmdybb.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3qpdcthlo.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3kbpmpmss.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3jrsnzxfl.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3kgrryvnz.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3almecqsb.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3wurczyev.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3jivoyigu.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3wekeexfl.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3wazfhbwk.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3qwltjocx.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3jpcwgiao.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3mjoltdtg.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3htuxrvfb.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3jvfgfcgw.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3nrqelnnf.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3tfuwjdsw.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3ylxsuueb.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3lcrhghqy.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3tfqztphk.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3tkquegsz.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3ltperfds.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3pnnkvrji.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3gvdvwskd.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3dufzigfd.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3tityxesp.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3tjvykylg.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3bujffeck.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3iswuadfp.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3ccxncrqd.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3yimwsokv.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3xdflxvsd.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3hqjpvvgd.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3swuohxya.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lncghysd.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3yfednbjt.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3fxmflimy.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3umxjonni.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3azhtxibs.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3abowkaxr.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3nttalyfc.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3vdcgrdqo.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3zhgoegix.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3bnhefdsx.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3gvgkjxem.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3jznsbbcr.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3bmjdjabv.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3effeomro.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3vhgahbwb.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3kilrnxaf.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3btfvokos.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3bchdbwlv.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3tnaravlu.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3pooghzxp.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3vtqopyjz.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3sysdhxkv.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3wciclbog.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3uuuvmcfd.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3fghahjwg.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3nmvwbkkv.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3hhnedoav.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3xdfxnohp.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3vfyproqg.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3objkpkjk.html


<!-- 参考信息 -->