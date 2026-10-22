代发 wailian999

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2namkktwa.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt2qyuogzeb.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2vpbfwjbd.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2mgeooisb.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt2jjfgwhao.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt2lsicfivz.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2yysxeenx.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ackzqkrb.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2ujxwziha.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2dfwbhifd.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2plruyurb.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2mtrirnfc.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2pnncvxch.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2gbykbdli.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2ermeiiqf.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2gmbpkanq.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2wfztjslt.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2fzhbmkqu.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt2hhswuaiy.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2xsomwyrk.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt2wrpfldbo.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2dohspzwq.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2hobzpgpt.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2auvlclcm.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2znjeqawg.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2vdacmyal.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt2kwtwngtm.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2neyldagl.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt2xbyxkxdo.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2hjxycxsk.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2zpuxpbve.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2niihvpex.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2hpauffmr.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2lkgtnowr.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2rncpplak.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2neizlnlg.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2xqfszrvl.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2sxjvsuwy.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2dtxavdjb.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2imropwoq.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2kkkaffzd.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2juamwpyk.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2hvgnkxcq.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2xdwggvnv.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2tpecocpy.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2ideksjdx.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2umftwdjf.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt2aqvlirap.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2uwueahwn.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2fhdxaetv.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2daozkyzi.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt2nihmvjfm.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2weoosmbw.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2jgpdanit.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2pgnjxdwd.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2ikgavvqc.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2ofbqvuun.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2vitdknsg.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2zowymuha.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2aywklgmh.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hjdukedt.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2pksyeglk.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2twiyffcd.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2lfofqqcq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eixcmica.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2vqgbtsut.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oalzzthb.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2sqnjlbnj.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2ygvxjjkg.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2vkwknbsn.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2xmtvjzpr.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2dbwganmb.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2rvdfkijt.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ranwetoo.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2wkswbcir.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2iwbosnrv.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2ksodasdj.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2pidrujvd.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2ifhotxej.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bxznddsd.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2ajrlsmbu.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2azqditir.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2mtbqekzm.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jvzohjrj.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2fbjssjbu.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2dgszszsj.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2tebbrnus.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2wjwuhobm.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2nkxnqmsu.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mlgmzxrx.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2jxhucric.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2aojohhrm.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2mxrllnis.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2tswtuwfm.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2jjgqrosz.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2ccwwfswa.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2seeywzjf.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2yblgfmyi.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2elqooljc.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2wuhzfozj.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2wrzkozzw.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2eydbaczt.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2lbkpzawc.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2alxtsqiv.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2wvllwyan.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2dcwnzymr.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2mneacrpu.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2kyyyakqk.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2yhelyogk.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2ydvldwmy.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2xnpstmzl.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2kozhfajn.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2wvkjzzum.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2qduqimlw.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2ltgjxkjk.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2dkynpncw.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2torwtzpd.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2caxogcqq.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2lbqozlxa.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2gouumijm.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2asqchwrn.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2ievqnzkf.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2ictwupze.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2luprqceh.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2oabhlwpb.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2qsngscfh.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2ijncqmeh.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2nodauztb.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2hdndphwi.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2doinvhxk.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2xbewntqb.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2gnzctjwu.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ueoocfsf.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2xjguocyn.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2wozoormc.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2cbhwgiij.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2vjlazirv.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2wbaacmmn.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2bwmnnmkq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xifypuif.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2zidiamlo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2skpvtzhg.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2hlpmxzcg.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2dbdgvola.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2rogmfnpv.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2snaxjdgj.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2bhtlrjof.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2bbnuwydl.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2otjhdjfr.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2rfkkdych.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2oyuqrdqb.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2wfegaord.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2lynawcjo.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2hmfhbyxg.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2junmeile.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2cjwpflkd.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2mnynhvks.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2jmnipkmy.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2fwfezoes.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2hyfuddcf.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2lojaigqw.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2dmkfwpjw.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2iyyugtpf.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2jcalogvu.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2gmxqmczy.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2cmmfnysx.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2cvofonnl.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2vkwnaguf.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2htzzhife.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2hffysuop.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2skgxtknm.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2vajeyobz.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2uaemminx.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2peoqjwyv.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2wjmzrcds.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2wtesoqje.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2wqbvmqss.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2roiigkgh.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2iijdmjze.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2vdzfoevw.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2ywfythig.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2tdbzcbna.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2oibbtxyr.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2zicwdnfl.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2swqrjxqc.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2rsesgfdf.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2xcwjqvdr.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2ivprtrld.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2shfzofhx.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2ykdvafhf.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2qxgysrlp.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2crjdrzjf.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2jxbxzgjq.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2sgdhrqng.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2vfvszcth.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2whtbttap.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2yrhphkqw.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2oikfvevk.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2vvlegvuf.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2zwekqkdp.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2gnbqfkej.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2bvhcfdkh.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2gkmrusir.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2ktjoowax.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2ijwgtabp.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2ygkejjdl.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2tqzvocxz.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2znhrzbrl.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2xxbxmngj.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2mvkouzlj.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2nmsbsfrj.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2bjfqarcr.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2cdbwwqwp.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2krmbfgpt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tbtpfgil.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2gxgmaqvx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2utpyvasd.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2ppieygdj.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2gyqfbqno.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2nrgqybdp.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2kakcnexr.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2ytwpipdg.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2wzeigkee.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2eyirwpog.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2qrffizpq.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2menrasme.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2qcnkosus.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2dbxwyzhg.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2bkhvsjte.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2bawqqgrb.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2bwggtcjx.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ndqeoymh.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2zkirxjuy.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2yxatjpie.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2wldigake.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2smkytufu.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2gayocnem.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2bikoxjfc.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2dqppopwn.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2uhwwkzhu.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2pdrkianl.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2akuowhyx.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2yfcuucfz.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2rjmrlkcc.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2eyrgmwjj.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2rglzyybw.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2ufhghqbj.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2vmsqntyp.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ccnrsvfp.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2mkkenudq.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2kklkpixc.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2sdmrxqyb.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2twcxtjcs.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2bhjoanzg.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2nibmjirz.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2uhvhwljq.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2phsosyvv.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ppjsppzb.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2jijblthi.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pwwlqmas.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2cqwfznnq.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2ekvumphq.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2kefjaplr.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2emhsgxaw.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2qjbdakoh.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2kkynoyyf.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2ippokfxw.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2ypyqkumm.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2eundiate.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2tlxbsvkq.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2ioqawdvv.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2pcxcdnbi.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2rxfatcvj.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2xsxbwxkb.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2rndqtleh.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2xojpaqal.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2zpckrjwg.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2uztpwmkj.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2jgqpfbjq.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2xtcokkob.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2nprzkbev.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2lcvcilxt.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2gopymows.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2kqytuieb.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2wravfrwl.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2sgtpvgxd.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2eykpgxfq.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2welajvyf.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2pognbhih.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kxaeafcd.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2nqvbmhzd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hsjcojjx.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2eiqytozo.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2isfgtwxe.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2lvekiomj.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2npoisaom.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2yfmpsnvm.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2wgsxpmij.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2jeepnbbl.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2agegffgt.html


<!-- 参考信息 -->