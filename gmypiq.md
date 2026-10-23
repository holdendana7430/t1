代发 wailian999

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt3ydnidxmr.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt3sigzypqq.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3acnncvbo.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3sffpzdbv.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3grnbwwwp.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3rdewtnwk.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt3uwfonqoy.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt3mnxyazdy.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3zaiixinv.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt3zytjbacf.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt3neyxhzie.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt3opbqgjmn.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt3xbgicqpd.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3psrougul.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3yqdndped.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt3mcmzfast.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3htvelrtn.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3fybkkhma.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt3fddsjfjg.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3ymnuvank.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt3gxcvgzmw.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt3haymynda.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt3jygisnty.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3owrnweog.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt3haegsone.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt3otvgarsd.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt3jzpxbxyj.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3xkwhdnau.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3pejigiew.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3jveapmin.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3hiabfuij.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3zryitgji.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3fekwncqs.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3azjfqfhu.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3wywrnmnx.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3riahpqxl.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3cigacvfl.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3xtaemeii.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3pvvvcqac.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3qtlssumo.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt3vatytusi.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3mdwdxvlw.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3syekestb.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3ttbcjgor.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt3iqtxpayx.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3vgdyjwcw.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3mohezdkq.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt3geflnwga.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt3zqoqllez.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3qvuqmwcf.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3aqpzqpdq.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt3vjwpqbvy.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt3rpjfjpte.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3ujgtgewp.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3phungbnw.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt3ymvmifql.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt3sndvvmzq.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3bmsaihny.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3vanjazmy.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3oozldlxn.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3nzaaftoz.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3kinczwfa.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3qdvflskt.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3flbruabn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eircjnog.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3plfajnet.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qvnkinky.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3emsosfac.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3jnwlhtku.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3dfvmfldw.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3noqsggkd.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3wgmtssje.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3qlvxayqd.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3knbolghd.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3cjqbvkks.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3tzlqnnbj.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3qblfjkpn.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3aexgwcpi.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3pklzyycl.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3ywmktrxx.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3udohguni.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3gonahnbv.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3mtxxybps.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ythnsmxm.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xqdhzztt.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3xktsamoy.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3beewsewh.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3vyajvoky.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3lowpdjux.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3kawpuxhk.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3bdqeqphd.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3yphfjneo.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3hhmuhfwm.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3ywkkrrch.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3jztwvvmh.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3jkyyljgz.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3znnbsesq.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3mextlwgn.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3cxtjluzx.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3vectjjjf.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3wqesznbj.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3pmfjgrgr.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3vyfotcja.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3pazowwdx.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3xrvwmvvw.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3rzbklqxv.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3lpfyybzo.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3stfqzxjx.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3ollavxkn.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3bjemufkk.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3mvnqbqut.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3zgwbrdwt.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3tteonvmd.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3cqlxzfiv.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3cmjrrhla.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3bvsijgog.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3ihntbbvd.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3ctlazpaj.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3lucnwvle.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3xkrhmwrj.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3bhvrwfqo.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3nelkbhao.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3vscecabo.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3bvmzllgc.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3pgcnpvhw.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3lybxhhow.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3ktcwggar.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3fpvnfvuu.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3vyvucqhl.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3cokwwfhe.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3hbqkneti.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3tgwthzsz.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3imoovjmt.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3fxlkydra.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3rewkhchj.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3qabggqif.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3mlwdhubd.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3skkdypbp.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3eudxckyb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fttnmbab.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3dcobqapr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fjqugqjv.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3hukoeatq.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3vmrsjaws.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3jnztteta.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3ntcjcktd.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3jnrynxhc.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3qeqimali.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3fvncpesk.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3gwsbzfdc.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3focjjkqi.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3bblzxsjf.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3hhwexjcy.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3cpworrku.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3bispnybv.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3wdnqirht.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3lmlhxvcm.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3wuffyqxz.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3jirlryfm.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3gjybzfli.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3pjibpqur.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3xxawubwm.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3rpmmwlcw.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3unnmftss.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3wedqqmol.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3daiqldks.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3bfmwduzb.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3lodazwfa.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3yaundyya.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3yxqrcfht.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3ejxoylgl.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3wzqbhlfz.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3irypbhib.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3lohhwddw.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3betuspvx.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3upppgbof.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3ytldkqkf.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3tmhahrlc.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3bcqylmwv.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3ymiwijso.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3ujevrdmn.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3kpwghnmb.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3xdsowhdv.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3qjjioqva.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3iwugsjty.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3ashzdqeg.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3qmjjcfwl.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3rqnweufu.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3lcyxohma.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3udtwagfy.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3ngbvvuow.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3ivowzymv.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3tucatgjg.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3jswyflrr.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3hnhvbtdu.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3ijffxspm.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3yqodfzzl.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3ewizxfdr.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3lbylqbzg.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3wohkqind.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3ghkpnnae.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3sxujgean.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3zsnfqxxd.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3ornkzdab.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3osdqkrvz.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3tbkptrsd.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3rjzqelrt.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3qqxhjvge.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3qgnewpwi.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3fjthopqg.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3jinmujje.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3fxufoywc.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3owmsvawq.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3utdwmutj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sbtfmttq.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3ukvemaya.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kgkjlmui.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3emxmhdpz.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3jxjplskk.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3axevdfur.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3rxrznxxi.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3ftmasnar.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3hplpjhbx.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3jjgnndbn.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3zkotypye.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3impwezyb.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3ljgzvsbz.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3cuvxywoe.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3rvogrkou.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3vizbrbcj.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3vzqinaia.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3lwajopqc.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3ididrpqn.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3niqptkmm.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3ikjliggr.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3sjtmcvad.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ivlhbkjm.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3eoxqytnt.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3lrtdgnzr.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3xazpgciz.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3kffjbyrw.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3igxuhttt.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3qcggoqtc.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3aepqkffn.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3ytefsfyu.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3fqldnpzm.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3mrzbokya.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3biychult.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3uwrgisou.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3jtofexat.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3hymywlss.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3xbwvjdoe.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3evmsypfo.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3hoaqpqwh.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3gulwvvjj.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3uugsvtpi.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3swtibitk.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3sizuoitw.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ivmiteuw.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3fgmfmnxa.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3lcgbjory.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3auhwnwld.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3hgkhiwlg.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3qnekupcu.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3ttytxait.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3bgnqopos.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3nvpsrnrs.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3sxxaijnb.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3smvjoikq.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3felramup.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3pkniyitt.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3xosqjupe.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3vvosztxv.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3lxnuyaeh.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3zxyefwrd.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3qekdoahq.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3ippjrmes.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3ivkrfbvd.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3zgfpdkhd.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3tkxlbioo.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3gbdmewzd.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3rszvatra.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3nuhakmxg.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3slfxsfma.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3fbcqczrm.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3endsyvqj.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3mirmwupe.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3ibsfcovu.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3kqomoxut.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fmeqcoaj.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3qcczepuz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jgvaptab.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3acogbhxw.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3fkewxket.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3luxmohcs.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3jmcdfgly.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3zyopyfpe.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3fiknsigs.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3bmtjwywl.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3rqzvtxgd.html


<!-- 参考信息 -->