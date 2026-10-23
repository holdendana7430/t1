代发 wailian999

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3bjbbhhzl.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt3egncwzll.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3ajxfpxpy.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3pityijki.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3zrihepkn.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3pgrcwrds.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3rgjcohyo.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt3exxedmas.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt3pexblckp.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3ohpxewjr.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3hrfrcili.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt3vndmxrjc.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3eksolbuv.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3ioreleci.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3lqjnoxox.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3reflglqz.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3pgkpvtyp.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3ygzvzmup.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt3unjyvfiu.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt3atilbizx.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt3juwvtrjg.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt3fnbbcncb.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt3riondgrs.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt3puvxrqph.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt3sjynqmeq.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3qojcuhti.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt3bdbouflk.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt3tunzfery.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt3fnwotkez.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3escqmexz.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt3tqklcsub.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3unohzrks.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3bgeakerf.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3jkflvvfw.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3xleuaili.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3vuzhcyxo.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3dwmuijzi.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3maukjrcj.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3fqzfdeee.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt3uamdyrbd.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt3zmsmwotc.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt3yulqajan.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt3vxjyrjma.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt3qcuhedug.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3rndncbjc.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3ibkoomrd.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3bkpxlxog.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt3vjkjxxjc.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3qdlqqcjg.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3wcjabppt.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3jxcrvsjw.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3bbzlgbjq.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt3kqukemfx.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt3fosnvjhw.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3khswmiwv.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt3xbyjnjcq.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3navlqcaa.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3ijoardgf.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3rjuvdwme.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3lypouuxi.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lpdkwnzq.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3gubdjens.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3hkgaumdg.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3qlugkapd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zqzacrda.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3qicsazuy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nchbhziv.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3katwprdq.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3inodblip.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3qvwyqxme.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3shsutnhj.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3utkemxwv.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3zyhepkpa.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3licsykbn.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3sxowgotx.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3gdtipdin.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3lfsjepkg.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3ydikylhk.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3kwregiwi.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3zdgovxfb.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jvbgxnhl.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3qydfxfey.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3wauysjwd.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kbmxgtxk.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3knrcundq.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3ucgrqlir.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3mljgsdnn.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3hqctkora.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3hqonqyal.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ulsuixxc.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3nsvpljfc.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3betmhyfi.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3hptdnskj.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3ijzkujgb.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3zvqgknmv.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3smzspvyt.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3zavpnczq.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3xrwhmfhx.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3csjodujh.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3pnxpdxre.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3kvzmihsp.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3nphxbnhq.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3douwtmxg.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3kwfurwvy.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3knaftanc.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3vsjhjfhz.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3qmepkrco.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3mgsajsbc.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3xvzdlheu.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3zvjivsgn.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3idqdwupi.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3yingedkc.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3omvfmyga.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3zfzfoejz.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3wrnolyrg.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3ooxdutfd.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3bzwsftea.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3fnjrcsjt.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3cosumzqx.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3wfgirsyg.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3gqsoajxh.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3cgpgcuik.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3srwbrgre.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3sxoqupzz.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3xujamiyd.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3rdpmukus.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3qcbdchea.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3summroyd.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3awwmnipl.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3agxdpmvi.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3ffsltewq.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3vwzugsna.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3vaaldmml.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3tkbkcckf.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3xfalzcuq.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3eqzcelep.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3qyohvgjx.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3hmwnncoi.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3wgnfzfhw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lsxwibmk.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3ertknrjb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ycsysrqs.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3xcoawoab.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3jfrgnqkh.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3tgyzukgr.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3wonkhoqw.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3vjgjcgkp.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3idiykvpz.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3yaavfzth.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3zojnoztm.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3hsulhtbg.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3qyrekzhx.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3zaxrsdgp.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3oxzxbubc.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3cajxkycg.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3malalyil.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3hngepozw.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3fsddywod.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3zauihadw.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3hczvguco.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3pmcofabz.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3vrrrtwew.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3msvxjhlj.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3zgbuhpfi.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3hdgornqm.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3dccufenl.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3faicsayz.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3tnscyfmq.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3wovakgyt.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3nfjxdwep.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3owcapxmt.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3enfswmbi.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3ezgnxxpu.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3zovgubhr.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3mbewhmlm.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3bymiiqby.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3uxrdfwsp.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3izwooikh.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3wvoojkea.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3gvuokrja.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3unnqljak.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3pflwivvq.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3drukfspx.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3kilctcfq.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3jdenjryd.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3cuoivmla.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ahhuvvmm.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3vucdqvvt.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3lejxmxul.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3akuxkanz.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3iiomrmua.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3fzezymmh.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3yiyqjslm.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3usgjfcxc.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3gdqaquac.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3dnhdisrv.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3fimlghrj.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3kslpnshe.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3grdxytvq.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3dyemgdjo.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3ozknrzcw.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3nnspgtuy.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3bmfopuri.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3yebcijny.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3asaumyba.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3vsvzvzax.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3dnjyyeoc.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3zlhpsefe.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3suyuuhuh.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3hncnctkn.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3qypvwzxu.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3tiuxlzgq.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3qgguzvqf.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3fxwxosvu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ykfqrkis.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3skksdzij.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pxuvfeih.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3zybszdkh.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3fdwzvfop.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3lbzgsdfm.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3mumrioem.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3mmsjmzke.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3zgobuxwh.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3porxxzgl.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3linhfpul.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3ruombsil.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3geypdomb.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3ovfhkuwl.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3xfogwfca.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3xmtfmfec.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3dvrmikag.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3rmjfjmtl.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3sibueufe.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3hykjgjow.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3ptugvqqx.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3sykxpdjt.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3pqogpqhq.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3ctlfmvye.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3dqjvbsaw.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3aftwgvgz.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3gonpzryl.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3pvrvehew.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3istmsice.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3lfpyzcjc.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3qrgyboup.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3kniuuubo.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3hmokcxws.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3rozahsqe.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3btdspxho.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3himjyvru.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3zzelhvef.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3stdxuoml.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3zefdtzrp.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3zwmsnhoh.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3mcfnsbtz.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3yxnfgzvk.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ncpyrcgt.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3vbbprgbl.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lvooyvdp.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3hlbqdusm.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3gjpkjcfb.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3nvwgszsk.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3xfhftbsg.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3xpsbkexy.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3hfmtkgaf.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3llahgtmp.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3bhmjbzuw.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3kuyaarnq.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3gdgmyzpu.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3ufcpjxdx.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3pzwuwnqv.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3sqsxgfbu.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3zoqokqab.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3yeaetkfw.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3uknffmnq.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3snrqiybt.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3eldewgcj.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3gjsxiyin.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3ylupilua.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3zovigpkk.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3vwymrpnv.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3pndeqkuf.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3ecvydiwq.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3muabdwwv.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3ayucohdo.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3scqtfhmd.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3mogaiagj.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3eyxbqasd.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3umqtjvlh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xivgykbu.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3gfotyspc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3onestqdo.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3nzynmwpy.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3phqzltkw.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3tyjqirxr.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3gyqkhdft.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3boftzagr.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3qlxfwoga.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3zpzgdycd.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3xsnylyvd.html


<!-- 参考信息 -->