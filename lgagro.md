代发 wailian999

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt3uofwzcrs.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt3ylnsmpzz.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3xbjnfgeu.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3zunsrrdm.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt3qguvieqb.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3jfhnllks.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt3ktsffmnf.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3bbhofnta.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3ovaliaak.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3luofsuvq.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3vopshoxy.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3ikzunujf.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt3vewsbfyb.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt3ieuzpkty.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3ltydhlyf.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3ofmbktub.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3lzfnocbd.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3dirjippt.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3jundfuff.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt3reuggbul.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt3covocsms.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3pvpaczer.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3ogfkfaie.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt3rbnsocja.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3gjdlmpzb.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3ftxrnrrz.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3bnvgfyrn.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3bqzaxpww.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt3pwkhpuxg.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt3legrgjfd.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3xcbbnmvs.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt3himmmllg.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt3htzsycpm.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt3vvsiuurz.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt3xjnfxzqg.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt3dpdscnlm.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3kuxhewim.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3ydxgqbbs.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt3nxouuhmg.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt3kamrsfxt.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3vayrowrf.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3xmhwndqh.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3lodceibw.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3spcnkzxa.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3hmrpebrg.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3wuttgxuk.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3mvhsknov.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3pguokmbx.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3pigwrqnb.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3ysragqxw.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt3krafbvii.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3xvhjmjfm.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3dfvigowy.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt3awippjpo.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt3wbjrhqml.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3ectdwkfi.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3wciksvne.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt3odzoxmge.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt3facffbnd.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt3ilbmsbjf.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3myaqulwj.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3trwidreh.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3whteguqs.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3aviqssha.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3qkirrpri.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt3vzefgohe.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3dxfkrchf.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt3goqvczqt.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt3ntkyyrrq.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3ebsyzfkj.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3wvgofjoy.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3mlsmqktw.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3juvcjrcj.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3lsdeclvh.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3epjpuynw.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3fzlcinyq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lcmrrfzq.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3wmeovdgz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3azywqxjd.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3jabzhadc.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3esejuhcn.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3lwfdeihx.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3apejvals.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ztwvpohf.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3mmumqfyn.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3shlzbgjg.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3yweliwav.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3yqkudlnm.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3wphbwmnf.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kvfnuchf.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3tbianaxx.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rpjektpv.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3wlmhcaco.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3emjvvktk.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3czvyqykz.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bzjgcorn.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jkbgehjm.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3njzbiggg.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3vhhhztug.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3uwpkmdud.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3pswosquk.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3sbkrzces.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3bqgvixbf.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3xgvuhkfr.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ycudjazq.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3tzawobvh.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3lpymkgyc.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3vjzdrygx.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3uktsmxui.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3aosojtsn.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3wqxdriir.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3utxbzdrv.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3mhudsnuq.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3alenjphl.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3omsijchj.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3tzinjoct.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ubnwnmjk.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3tchkanen.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3selstjht.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3gsllrfhc.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3hgxpmlvi.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3dlknqcxq.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3njnfeohb.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3ubegowvh.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3mvwqiqoy.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3gprjcgol.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3cjgtkgdd.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3jvkooxct.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3ynprsabb.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3qrfkoncm.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3trgnnlsa.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3eocujdcb.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3tqzsijfq.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3wbikjhma.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3dhcudfmv.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3hjhvahzw.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3lxaymnga.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3fjlczvfi.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3ebfqczst.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3xwayujow.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3cfefzezq.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3vozfynyc.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3lkodtstt.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3wydwweui.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ispxlelz.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3zxcmjcxc.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3bavoluyo.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3mahrnrsp.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3zqozcwrz.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3dfjslyqp.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3qlxnjrem.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yzswsxgb.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3vrolhazh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uuggirnd.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3ijiglspk.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3gochhqnm.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3quakesdh.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3jytuwajt.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3lowgxekn.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3utdetnqj.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3jpzjurkx.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3fllavwzw.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3xrjblcqr.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3dhhoprxc.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3kbkfwmad.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3tqutzxeg.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3ttumojwc.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3lksklpah.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3ogllqbgp.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3jslxtiqr.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3nvtawgrr.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3mjkxoejn.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3zzhnxdbn.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3bzlvcrse.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3mnkfeztg.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3eutniiis.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3piwdrmzh.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3gfmnvyzi.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3ilrohurh.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3zfgcnlck.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3ujgnwzfd.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3kpcqxnqa.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3usjzirty.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3ihvacugw.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3qztnrpcl.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3gzhmoyla.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3gtdxhzfu.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3rrytqecw.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3daavpqst.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3gbuqdwzl.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3jrnleomx.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3luwjofwa.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3rzmwqhay.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3qqdawymw.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3lcljeoad.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3dzxaoxcm.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3soqfsxlr.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3rngijhmh.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3sdpaeirn.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3abnfdnri.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3zmsxbvod.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3yerjmkrf.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3oxslnwjl.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3meddcxeg.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3dhjesjwb.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3sbecgehk.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3fjrxkatj.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3wwoplisb.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3npwjfzpx.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3ymnmypsx.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3lewombzn.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3dilufunl.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3jhitmuca.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3lpkbbvav.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3jmsbsvfu.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3jzfibydl.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3uppzriqt.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3rwxctwsz.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3lblennia.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3ccpjawjo.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3tygvdsgo.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3rfurxwyl.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3yetoooyw.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3sazjctnj.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3iuubudcz.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ihcvnwov.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qaonijdi.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3rgypacyb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gkeiblnj.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3vxclshpy.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3deswijnn.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3mvddvouv.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3zphwpkmr.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3dgdnsavp.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3lqidzewo.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3zhdukmbp.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3yzabfclc.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3vrkajhvf.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3bmiwlped.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3tgptegea.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3qmdwezjd.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3oxckxder.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3qslimchq.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3mswirdwd.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3rbmrgmnd.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3jfkojllr.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3rzqfouui.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3fthkniaw.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3inuaexfw.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3nlpyhtkj.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3zdjwhjdv.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3luhjnpxz.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3nwuhdrif.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3sqkkqvdp.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3hkfqslhw.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3ewcfulil.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3ydiqmjni.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3zsrchext.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3wpvtnnmp.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3jzudhrtu.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3iiybacsn.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3ausyrajx.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3dhrdjcrx.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3xjkrwozm.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3vcbwnhyl.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3egnhibmz.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3shjbmwkx.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3goksrzjr.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vhuvmotd.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ysucayun.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3pfxxwvxx.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3osuzwbxu.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3tdbyslpf.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3ayxerbin.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3hmvzflsa.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3ovdzwkir.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3ejwligrc.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3zgbhyvcd.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3zcymxltr.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3ikhsghra.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3khbjtftc.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3uydpsrps.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3twydtltx.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3mghnugqu.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3hcwsvyzi.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3juckibii.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3ryuplvzh.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3pnyweizu.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3yfyyvzbh.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3qiddswap.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3dbnhvgbn.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3fjnzevih.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3tgpzzwlj.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3oisrqbyx.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3ergobmlk.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3ichomhok.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3whdiroqn.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3odlpemwn.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3ictowzul.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3hwcyassb.html


<!-- 参考信息 -->