代发 wailian999

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt3aatynykk.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt3jfxlzazw.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt3ibykvhih.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3kduuzfsy.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3eeaztnjy.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3alsjecrh.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt3fiybyevn.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3oxlmmmmn.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3iummqeyr.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt3wsovjueb.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt3gudyfzym.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt3miqgczmc.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt3ntjeqvqp.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3shxdjsjx.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3aehpigrw.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt3ruvdjtqb.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3gyjqsoqw.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt3bizrozcp.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3lbnqcdkw.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3scitzwfv.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt3jxihpgpm.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt3oiqyknjq.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt3sissoujt.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3qexnpjig.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3ietjkfyc.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt3jhfkbgwl.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt3rowbpcgg.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt3tnreitjo.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3ynwxzlcp.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3azrjoxtm.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt3ivxpiofr.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3xzsyutbu.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3wouplxtc.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3wuxdldpq.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt3cqwyenjq.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3jumixchn.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3ifrmbfvq.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3kdiqrwjb.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3vhkkxujd.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3vmagcvcz.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt3mtnjgjnn.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt3plgzmelo.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3uobhssad.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt3giydivyu.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3bwsixyrc.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3ureuivmz.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt3icikanls.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt3rfgwwrnd.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt3mtqzlkkr.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3cwpjxfac.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3hkoypgqu.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3fkqcaidm.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt3erdwwrxo.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3mtpmefwa.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3juxzmqvg.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3aawibazo.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt3wsvovyho.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt3tlyilcup.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ocuiiyll.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ydywjolz.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vjlhiatd.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3sfrzvpsq.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3zpfpekis.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3gvknokbz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hcdghjcq.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3qckxmncy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rqhbzvnw.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3exwddsar.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3hakcgqvn.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3vqraeglk.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3mrjqkide.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3fumjmmgo.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3dqueqkho.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3yqpbrvsw.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3hdbwluno.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3abfhroot.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3pbctbmwo.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zaayhyet.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3sbglfvpr.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3hoycpmen.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3scqzgsop.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3csbmwkdh.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3yaayfwpk.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ilovuutw.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3guztzxjm.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3wsnnkcvg.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3aliljdij.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3oiohngds.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lgftvzip.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3kvpjzsqu.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3npefqkxh.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3swvvaglg.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3ffwtixyo.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3ziufplnh.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3jrxibcva.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3mljadmyz.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3ftffsnsh.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3fyupepys.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3asleofha.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3gfaeohrh.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3yxcorsdl.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3fjbfxlnk.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3evtfeepo.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3gkmkryik.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3reibxrbo.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3svvrwyvn.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3nmjiunny.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3nmvziuie.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3hdsiexzl.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3qsnbtgbr.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3tgjcwrfj.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3yeteulrt.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3mplrkgsz.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3yghdpsjm.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3luesddts.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3gsldwqxb.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3yuyqrorn.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3bezysahe.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3nkzmmhnd.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3pzjphwfa.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3afsojqle.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3raobbskg.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ixzamora.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3dksybokn.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3yospbbxe.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3djufrsbp.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3qusfvpsu.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3ssjebved.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3emsdemfj.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3zgyopydz.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3fgomltov.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3xdnroqnq.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3hssckhud.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3lijuadio.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3aipufrcg.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3bvsbkmwb.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3gnnzgrab.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3htmsctph.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3zzwrintp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nikexteg.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3zactpqtu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ljwpwdnb.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3gypldecj.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3emarcsuh.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3wipdinkx.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3toytdman.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3rgwkzuqh.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3lnogxpal.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3aylsmbih.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3acjtgnum.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3vtnlyblb.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3vwfzrbqt.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3jdnydmxq.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3qvpzzcik.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3xpgjpcib.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3nttpsjgz.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3sxqjmskx.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3aicraemy.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3ruphuioi.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3zswdkrqt.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3zodxotik.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3vpzwlrkf.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3lbghgkew.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3egkrwgnf.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3ypoktrfg.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3erwvbiws.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3hwzelbcl.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3deiqvgac.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3rbxpaams.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3zozjcnjg.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3uqzehugw.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3wxfsgpeh.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3ckifekiz.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3mmcsdkfi.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3ttnwprgz.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3hbbwafkr.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3pogpcmlc.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3boebcabn.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3avfhzhdk.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3zwwasaxz.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3ahqptpnm.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3cowjtacb.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3byikbzzj.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3cqeowtmv.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3rjihbxct.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3pveivzvr.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3lvxkrtxz.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3nbjzqlps.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3hfguinhp.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3alnymhgo.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3xmtedhyy.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3rcmtslmw.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3izqncmbr.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3rmurxyda.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3cpwvfkoa.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3xrtyfpee.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3tidjiqac.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3rppipafy.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3eemmdwnw.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3kuhwycwu.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3vthbnbur.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3erbezkln.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3nwotqcnh.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3wmdmjtox.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3crvdzovc.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3pboydmgi.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3ufhmdxlz.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3jeatldnh.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3txkgqrxq.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3nzbejfsz.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3fmipxkqp.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3qbuwkdvl.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3jfmheauu.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3wgjmqtfn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lkvqwzwu.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3jphdynrt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3igvbymmb.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3ibjujeey.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3ehsftrdm.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3iaqmgftm.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3waprrbov.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3nbjtdsqh.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3tmciimsx.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3phzsyetk.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3qmtstmrf.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3ztgtzowb.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3qlwgeqzj.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3uqedjzuh.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3yghvynud.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3mzonvldm.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3pnfmmxcf.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3ubrezmcb.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3vednfkxo.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3vcicpont.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3acwgzxrp.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3doppecpg.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3wujnbxgz.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3andkwxmm.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3uiiabmbr.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3beehxxhu.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3xyxhqymq.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3uptlrink.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3ihtibwdn.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3yzprbcuq.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3hxtvlksu.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3iclktlgk.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3dsoubgkf.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3uunotxmw.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3uscrmjmp.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3bqqxkeyj.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3mwlbszom.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3rrjjvhfk.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3qkwnqelk.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3wkwjglwj.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3bpzvpian.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3ofovwijj.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3gfbvwhqo.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ikosjous.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3cozidirc.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ibfzjgwu.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3nuqfiguq.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3mykormcf.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3tqvkpddu.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3yrjsvlmt.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3sgtmdbci.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3rpihxftj.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3vsraxhpg.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3ybodwxxr.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3rpztxmnt.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3bkwzpobw.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3ilrrmjgd.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3lzhbgsyd.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3ivqgalne.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3zpfkuygz.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3ysekpdqc.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3ogexyjdk.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3mlvckgsu.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3mzvsdfvp.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3hgdprpob.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3jyavowoz.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3juivpisq.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3oovznmwn.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3pwlxnvhz.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3jscvvpjg.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3vkbenyii.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3siuokzvs.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3opovxifj.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3hgriwsio.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3hougmdse.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ejivlrqp.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3yjehwgjd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pcvdfruz.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3xkqteziw.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3zkbzztgj.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3lqexemjx.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3mbwqyqyy.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3sboltwqe.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3rmtvawxi.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ikovvwqy.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3noqwdyjj.html


<!-- 参考信息 -->