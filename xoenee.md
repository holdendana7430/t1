代发 wailian999

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3zsiqugeh.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3qfagxioi.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3riewinke.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3ajudulur.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3rivmnqci.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt3bftvckvg.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt3thuhsnmp.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3jqxiaxwi.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3qzhchfrx.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3ycicdvee.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt3idsslzio.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt3aekfqlho.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3zzwtyiqg.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt3cgalinqs.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt3zpnvnecd.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt3wruoxghf.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3qftmztbq.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3mwmjxwlr.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3fgghlycb.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt3uvlwumqo.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt3oigaysxr.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3oecctnmt.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt3ewgwmoki.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3qhqjpjox.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt3tnseaiqj.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt3poykmguz.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt3iexxxqfl.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3xlryranz.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3btgjowko.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3soxfiazb.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt3ivlkrvfn.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3iafvknvd.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt3vzodxxfv.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3jifeczxg.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3fcwfkvsx.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3jydhzook.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3touwilrm.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3rrfvitlj.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3ydxocdbb.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3znzpacjm.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3dakofzql.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt3avioevnr.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt3ukyupwsk.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt3jbeaehxa.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3vozvkpob.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt3pfraxvzz.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt3ycetaozn.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3qqptotyz.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt3vtsgvypr.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3ftnkdwya.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt3sgroszap.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3zrqcykcq.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3opbitzqg.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3letmyxyc.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3mdubgeur.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt3vlhpjwhp.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3rwwjnsle.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt3nculaogl.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3bwasakmb.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3dwzxtulj.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt3xfqkvuks.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3fcgkxabg.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt3btxgohmv.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3osouprvs.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3yzbvqhpr.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3ukqfwdhd.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3ljqmpqhw.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3kjogvwon.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ilgnlscg.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3ugwaotan.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nmnydpaa.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qowzysxb.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3vtodwfdh.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3arsncfty.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3seznmuxv.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3kufscvjb.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3bzxuzoyk.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3cnylokjp.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3jdzyemos.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3yfzihhai.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3stkeoxah.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3ecbjmzaw.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3sqbmgtil.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3gkyzloni.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3wlalhvyy.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3pgrcvnhb.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3ihcfurxi.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pzhqlviw.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3sxyiapvh.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3gqjmkzxi.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3lclhxrai.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3prouuvxq.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qeuegrqh.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3xzwizhee.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3tmgajvck.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3rcddsowa.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3hlefqime.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3rpthoogk.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3gzyzkegr.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3jhaoaokb.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3rytygnsi.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3blbmyhfv.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3kqikquot.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3nsunsnuq.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3gklamohp.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3aietkqyu.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3tkidvekn.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3btkpycub.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3xgezcteu.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3cgrevpvt.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3xfdaoqot.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3ybnobhoz.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3zakgfjjs.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3juzoqgtk.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3euwifjgh.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3ycmwghnv.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3ayifhcnu.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3phlutoiz.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3ybnjznya.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3wpkcmwsy.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3qfcspcoi.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3wshduelw.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3exlqjnsj.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3vmvubgkg.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3aqkzwets.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3itehoufr.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ulcnxrlj.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3ysbpycjv.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3oawaznay.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3iyvqzjcd.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3thibshlb.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3mgtnkynr.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3ykmknoou.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ylwrxyzj.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3hbwwgync.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3tdrdtbem.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3acyohbuz.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3htdalkzx.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3ycfjdaiq.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3ocbdwuyt.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3fbctdhoz.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3zsttivxy.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3untwddrz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3thlegemk.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3mjqfhfmt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xiagfldf.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3neaxbabv.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3vofqprct.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3rxhxhhpe.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3typxlobc.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3dopqnbli.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3nzbajlev.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3kokzzrvw.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3lzcvbxdn.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3azduckcv.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3izrwnzqg.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3nusxsjuq.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3llirhxfe.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3eaknnhjn.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3duuojdwc.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3kuiffcgp.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3dtfbvhvy.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3awbihnjg.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3uhlhzngu.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3nchhqxaa.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3viohisvs.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3mofjhuch.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3pvawzlin.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3wybpbkiy.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3ztcbfhmk.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3dlvaqdag.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3sfqfupia.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3fhqmufas.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3bhsnudxo.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3erwkzkfj.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3kykkeoaq.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3dqemcwxp.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3ryzjmlbk.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3henutikp.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3oyhxecld.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3zklvjwoi.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3qvvgodcb.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3tyvhufpd.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3smhzgpta.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3krzgtjom.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3mojlshnk.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3antiepdy.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3wyqqpdsm.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3ntypmkke.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3zbbbsutv.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3puvtjkld.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3bvjlzicd.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3keeorzbr.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3sywgsxfj.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3yaypsman.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3kuwpwpur.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3ctugfaud.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3rrgyuwiz.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3lisjppih.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3wfmrfetg.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3cfbewwvn.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3nbtqbdxd.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3dpmufihf.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3yzafvwol.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3exrjpdcr.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3klfdejzf.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3lppfwbey.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3uvkfglwt.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3bdwriqcd.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3cjlqhkuz.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3nyztewxh.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3ffuitxne.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3pvsskkrt.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3rrfhmakf.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3wflrhjwr.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3zmwhxaqw.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3mkavutvt.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3ptrhvyrm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fjdtyrvg.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3yvwivgsj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fqwiakcw.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3qvcxpsvy.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3xvtdqtpt.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3jhlagyos.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3vgjhiyte.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3aypzxtsp.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3xahuskls.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3ialewsbr.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3qaihopwe.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3yftetzgw.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3uqfjiziq.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3qejpsmcs.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3lndkfttg.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3obbmntcf.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3nxjyllxw.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3capwvivb.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3apznzicr.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3rmobhnev.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3ovhbgueb.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3lpslvmym.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3fdvmnafd.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3xwdpwhia.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3irmqirkl.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3vdmmoukn.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3vlfoftul.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3zovmhrbd.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3udjkskun.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3twdfajiq.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3nnhmeznr.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3ptrldjtz.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3wptkrctj.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3opzlvnkw.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3monnflgp.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3hjacuecz.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3safwrfvt.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3drhtkixl.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3rrxprhed.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3xpprkjgm.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3bapkqbnm.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3jdqbfnel.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3izffinlo.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3miwoqxjp.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rkvhtghv.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wounceux.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3slutizcy.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3slapklpq.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3xjiiviin.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3imuiofjd.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3fpuzcwth.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3pfklrvet.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3xqviuskb.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3jxbzkrpp.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3ctnjkmxv.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3nmfznues.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3iudfxcrz.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3cttvdwpp.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3qozyelbw.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3oejssevi.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3tnzfndby.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3ejffkfwe.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3cqinicnl.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3nmkzjxak.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3bztkeosd.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3diatgtpx.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3ewjoqwvm.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3mbmxomsy.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3zstnlwua.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3pfswfltv.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3qhckvffa.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3ifxzrjeh.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3tzutvpcy.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3vhkugwkk.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3gaigfuzk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wcuuifsn.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3gebxebtk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xigwnlhm.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3vpjsaatf.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ftduleuk.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3rslhpatu.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3czwpadgv.html


<!-- 参考信息 -->