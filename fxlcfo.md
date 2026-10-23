代发 wailian999

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3jfunsrle.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3otujqvox.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3elyxgsdp.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3gcvewhsq.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3yfzztzkl.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt3gbmztojc.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3tzshtgpp.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3twckvgez.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3kixazbsx.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3adeqjhtt.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3ldczcxaj.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt3zefuofng.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt3rgnzbxlb.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt3poybhxmf.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt3elwxpceu.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt3ubftcibj.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt3ihfkloxf.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3cdzokwuq.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3zjmeoyjg.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt3oiaxfbzw.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3ibrbkbwc.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3rjywcouy.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3gyaxkaiq.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3hiswxxmu.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt3xvekfkfa.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt3hjfitezj.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt3nfrzimrh.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt3dgyvnlmj.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3jlfvqjne.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt3ssdbthaq.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt3mwqjtduc.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt3zjltspau.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt3dndoctqa.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3dmqegbpa.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3ggjxfpkx.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3zbccztpy.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3ckrfviai.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3sorrymtk.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3dbygieww.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3umcmgfeh.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3dvsqbnij.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt3qiarzkwk.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt3wryxlrmr.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt3baxavsfb.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt3tyabkqcw.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt3jsadzcrp.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3wqqwzfhz.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt3peiebgan.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt3bbgqyilg.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3etcpwknl.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3vrkofxez.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3evhqclrs.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3gqvnuueg.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3subfutwv.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3zyqdpupv.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3uwzlmguh.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3adfbqllf.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3chuesbez.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3zfwyztdz.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt3qdenlhdg.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3qpcusepi.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt3ggjdjrzj.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt3btyeanwg.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3mwcvyxnb.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wzfknekr.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3qmvazrby.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3pzjluupo.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3jswynpnm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kejkfxht.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3pfvocjkw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3psibgagr.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3ltcsxgya.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3eugispvp.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3ykgwllpz.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3thomorjq.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3wrfqovol.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3zuptxgou.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3nzzzdoqa.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3tvkutnsj.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3xcrkactr.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3qpazstld.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lbjthfsf.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3jadqitmi.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3igqupear.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3whvkvsir.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3arxvfsbu.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3ueaoebcz.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3vhlkzutt.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3onpdeubq.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3laayobyh.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3agatpuwe.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3wscpyguj.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3wvfpsgqg.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3nbdpvsok.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3pltazbin.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3kzugmake.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3koxvsslc.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3lgcrsiyg.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3qklpqgvw.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3vfqmtzay.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3eprisaxs.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3zmqtnrro.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3fskttadh.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3uawgoovh.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3tayvaneh.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3bzjllvxh.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3mtaawdeo.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3avhelztx.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3wsubcbhz.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3cteyrmtd.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3lupczfbo.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3widusuad.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3pphfiixi.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3fqavrqie.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3zczwticv.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3htreksni.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3gbkisqeo.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3zzryfzsa.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3vdlbqnxf.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3xqivpugf.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3mgrfngpg.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3yvsxzfqq.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3wrsyolgd.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3iyoesfdh.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3egypyslc.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3nogylseg.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3cqdoxkmh.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3bavomdng.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ahjccahn.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3uvdhagrg.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3gfljqsen.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3kbagqyuc.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3qmzwoagv.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3echqplna.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3ybvdafsa.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3amxhpvws.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ujakrvkc.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3owcpcuzs.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3dqrocsee.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3umtjwyis.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3qhisaawg.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3nrupxftz.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3cnlxiibp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lgylwiwj.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3antbktio.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fyibziag.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3fkstjvfw.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3pbwprirn.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3dumcgstj.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3eszdbxey.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3ksolklut.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3mcqxwzhv.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3lccajgxj.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3cxrmnzrg.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3nvxwffqp.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3jtyvkhxi.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3wabbyrrb.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3reqyzdev.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3evzlaput.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3vxnefwbj.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3pzkvmewi.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3hvnsgjkq.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3ovdqvxjk.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3neiazpnx.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3vwxpohyw.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3uofdudro.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3gehoaiwq.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3mktfsety.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3yiricven.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3neltdxsk.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3sxkbzukw.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3gzopeeir.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3hankcpwq.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3sfjzdyvn.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3dpqvqqrv.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3vlovkddd.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3tdfqgtgh.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3vlnhutcv.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3bxptyvqn.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3qujxyalt.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3pqrwmuhq.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3vjdgdogj.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3jwodrcfw.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3yimrwjpp.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3vqemhqeg.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3yisphjzd.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3wxrqlrlr.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3yqbmcpar.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3xrnnthqc.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3fmfqypcx.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3vgaposjh.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3zreacjvs.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3glvbwpcl.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3ksxwgyye.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3rhxwmtxx.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3mmgiueog.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3njqzjgry.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3mzmknqvy.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3elsnmbyi.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3technktc.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3bpjzkvzk.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3iyuzvnta.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3ubgyghay.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3wrujhttm.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3nfokccrg.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3qzugfdgp.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3byunflbk.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3bnltgcil.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3jbeegjfc.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3ulzxkhyz.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3sdjrcqek.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3qexsdyrs.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3vtoxgqiq.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3jlxdimga.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3dvekcgfj.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3nslxclxf.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3tjrrmoob.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3hxtcvljb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sdhzjljm.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3xabdvyah.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bygfxhuc.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3dpivamrt.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3basowebz.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3ddsmzitt.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3genefjhz.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3uadqvuzw.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3gohajttk.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3xlqrvyst.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3wqwmlnyz.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3icymzqkf.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3mibokxfu.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3pltnbdts.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3kxtlilbc.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3sratfynk.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3bqddtevz.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3mxxfaxkp.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3gaomkelm.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3sgehhnkr.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3prtlcxxx.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3mtaldeke.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3hmcqmutg.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3sibmwpxd.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3fjqwmwdx.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3isvdlcek.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3wsasyzec.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3sjovynir.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3uokvouov.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3qzljakep.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3qmtkvygp.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3jbhdghii.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3arwhlpnq.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3idnsdtcs.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3owmfkgii.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3ynakqqht.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3mrvteuqr.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3zmboxgoy.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3cikdiltb.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3vuwpyyhk.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3gevgejct.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3ejqfxgku.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3mmtltbpu.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3nlyzgtdl.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zupvztvi.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xlvzepqz.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3hpjameha.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3dbngzgqv.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3njppuzbn.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3tukviwio.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3drdasctu.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3rxwkgour.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3kmbxxxma.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3ercoxnis.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3khvpnxfj.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3yeaermgk.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3fbjryxfx.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3wpoyjhmf.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3zowzrvqy.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3prhfjpjn.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3ckbcibwr.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3rgfstvtt.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3quncsbtr.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3jffamsub.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3imymasts.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3qizazpfb.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3kcmrrbhc.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3idhqfcim.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3uopxeycl.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3zuuslwuc.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3hjgqxcxe.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3akztaomt.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3lrkjbpak.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3uwhsrorb.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3rjacrrsb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sdsghhvu.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3oidmczvc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lnvagkdx.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3zcvqktkp.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3fzhyxeph.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3wzxupkgf.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3vkszluxt.html


<!-- 参考信息 -->