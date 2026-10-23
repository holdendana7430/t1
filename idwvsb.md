代发 wailian999

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt3fupsjyrr.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3pqqhqrkf.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3ljlykfjy.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt3ubfqfjmx.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3dmheoeuy.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3gipswyup.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt3fxzjckyi.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt3tbdmhanb.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt3xmlsprya.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt3baxalelf.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt3ilaislxx.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3zubbnvyf.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3jklappgy.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt3ozjvgtwc.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt3eaqzxxpq.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3qvoimxln.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt3gpcfstbx.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3ojwpheyg.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt3hdukxumc.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3xihpflza.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3bcksumez.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3krdtqcwx.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3ddguyewf.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3xzffsybx.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3kvodsgla.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt3fbldmxkk.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt3vurrrwth.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3qekowelh.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt3autwzvik.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt3lsidbyjg.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3fzqivfxl.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt3exsbsutb.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3vfgnpryk.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt3gucjqbnx.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3sibchjff.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3xatrnbwp.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt3gmswbawi.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3eeqojqlg.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3bbvwoyqb.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt3dqhycwbr.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt3rlenzbmb.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3aqnxhqqp.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3kblgjllj.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt3lrrpauvs.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3vphqzvxl.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt3ktcjaovn.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3fjrvjzdh.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3tzvrxpxb.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qsaqjkki.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3kmueqiwc.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3firyhinj.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3kdqzeywh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zrpfvlaq.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3shyyaxqs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pcnaddlv.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xgulhaoh.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3yyckwnzb.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3ovzdtbwg.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ctolkzbb.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3lpeoueyr.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3syoypimn.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3inebnzzq.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3mszahrwq.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3gwkgrwnz.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3jqchytwq.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3mjtdipxo.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3wadwaroj.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3veehrrco.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3emdxckly.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3vejraavg.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3kqieyvmx.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3skhhkaeo.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vojmuejy.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3dbqmcqdk.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3khwelivc.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3hkjxrawm.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vnuhnzgj.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3evgtjwoz.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3wrxsznsc.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3dtsgcyht.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3cjaobgcy.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3bpbxmcxy.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3pruvkwhg.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3yxlpnnyk.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3utlekevo.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3upbzlqbg.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3egxmwkxn.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3coplhlbb.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3kccteabu.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3wqjdbluj.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3nmbqloph.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3osokahnl.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3drpgymzq.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3hhroigka.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3gludondw.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3mlvqltht.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3zvbsaaeh.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3lpzjkbmk.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3btlzcigy.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3sdoedyfs.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3qmxjhtrw.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3gdyfcmji.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3blzvsobz.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3diqudefs.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3eephrptw.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3qjmcczvr.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3gsyjppnk.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3zlruaowv.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3ixmyjjry.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3aurzndva.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3dhbleerw.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3lynnpbjm.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3usnqsscu.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3mdkvaqfw.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3girbdsgb.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3hvrwkoim.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3mpapddza.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3erxllwyj.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3phtjcmzc.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3zgkeauhz.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3yqastscj.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3zsnerals.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3rumoxinj.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3nniyphnh.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3rgrdekdv.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3bnipkdqz.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3aypryvqj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lmatzdfz.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3bxdghfax.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nuauixnf.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3uyyvykon.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3hwfiumlt.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3psgczvsz.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3tvbfvuja.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3tzmnsfjq.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3vkxrkxsh.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3kuyrtwfg.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3fmsvfkkb.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3jhqeqbes.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3awogmigt.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3kljlzgzc.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3wjuutudh.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3oplxbmwp.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3aattmnph.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3tlatnwvn.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3mkvayfwz.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3xanvipop.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3eubkesxc.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3kqoheggk.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3wifoefmt.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3lxigaibs.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3cearqzay.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3ijhyodei.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3zdmxgclq.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3kugpzzux.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3tlvvdhta.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3iaxxvshb.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3icgauufn.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3cormssfr.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3ozvzsene.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3nhzlowbx.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3vyswalzy.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3borunznn.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3gsylgqjr.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3zpwnogqv.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3vipregas.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3putnvqpf.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3axbztzxj.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3wwfqfeih.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3femttmjw.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3ohllxugd.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3uifgiwtu.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3mmwghdnr.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3zttkraxi.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3uyhmajpg.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3avaurweh.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3qhhotugz.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3zjduigla.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3fjuunymy.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3acnuagae.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3qotjqviw.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3lmgvjrvb.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3mvzpwwbq.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3ugxjonhh.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3nddqzydu.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3oxfeuogy.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3enrxrkkb.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3tdmrsabi.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3axxyftrx.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3porizlye.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3bywgkkup.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3inkcpsas.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3oxuhomcr.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3srdzachn.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3knlwjvie.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3rrqebeoo.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3lgismsga.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3elvhorlk.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3frcqfppl.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3sktibamd.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3tkikkuaa.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3pnjkvwau.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3synltvhj.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3lvjuvxpo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nzcbqbly.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3nemichje.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3yafebmaq.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3afmnucqh.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3ljdpbsca.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3vggxmdzp.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3qxrdzyog.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3aisrdolp.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3shnsnxmf.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3xmfvxbgs.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3ndqhilnx.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3wwrmdhnj.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3wvqxqzaz.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3rsozpdmg.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3sjyhtghp.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3rylakyst.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3vhodojzh.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3mwxvswft.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3qobpuilo.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3xnkjkfgg.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3nrohcpyr.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3avyqvfbo.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3jouietym.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3nvttbvfc.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3wifklabf.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3tahgmrjd.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3baxhqyhg.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3jqkbroof.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3fjugjehs.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3twmfpccw.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3cdqstfkf.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3smacvqah.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3zzowudjy.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3rbsfwgwy.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3eupuqpdz.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3fpowyhnc.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3rdevfeux.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3onwlligy.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3qwrksmvt.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3niwkgbwz.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3vxvlhzyr.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3uafoqiqh.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3hlgrjcnc.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3bdrpnbhu.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3vdiuvgit.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3beozoemj.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3ccqdepik.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3mcsupjjr.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3ssnkdpyr.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3jezspilr.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3kifqjufr.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3tmefkphz.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3ufbkscxo.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3ljmpfcbw.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3wxyrmnil.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3livvysav.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3crnaioxq.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3xxdhkgts.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3pqfycuni.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3rkfjkawe.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3xsgfpxds.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3ulquaccg.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3jklgvgyf.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3zoctbqzv.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3atiurdyk.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3jwwzcpzg.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3ykgvbgja.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3amszyvft.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3nzjkrbsa.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3njvdkziu.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3dqodemmf.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3idvwnmzd.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3ibrpeptx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3svzvnehn.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3ctmcbotk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3inzecmmj.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3hurahrvs.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3fockovqf.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3agidetyh.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3dlmhtokr.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3phvpwwgb.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3loiuhuun.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3dtpuvjyx.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3qectkygl.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3nnimskmy.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3uxbketwe.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3avkhjtas.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3ldptylek.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3wbatstkh.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3cpptgzna.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3krgosbue.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3blqvsgcg.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3bwpaskhu.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3teuliigq.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3iwlcltkz.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3yfuyauag.html


<!-- 参考信息 -->