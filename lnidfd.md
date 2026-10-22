代发 wailian999

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt2mpmuqaci.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2bajpaejm.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2hkccepow.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt2wuxvtgyh.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt2jsffqyjz.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2mztlfogi.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2tonuuksh.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2ihmulakz.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt2ttbddwfk.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2swutyjqq.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2lcxznhic.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2ijjfnfrt.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2ixxqphew.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2mwpoiadq.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2vldihcea.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2mzpsmfsl.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt2ifqdgept.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt2lwkrhyky.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2xjcyqfxf.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt2nnqzmxpe.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2qzzykxuj.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2zyrnqpup.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2vbytxpvw.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2hctalcrw.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2qlbieokq.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2zbliihdi.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2pvvzxlzh.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2byxnvcdc.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2ggyvqcxu.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2nlwpewnc.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2neobfafh.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2nknrtkpn.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2opftfaar.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2flozvpej.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2mqletwtr.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2qobwwwxw.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2nulurljp.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2zcreckgn.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2qhyeuvfc.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2wfggcyzv.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2ukfmqnth.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2wwcvqbzk.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2xpoqleeb.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2tmnzxpvk.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2qoxtaamj.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2mqmxexvu.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2qkubhxqx.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2nalnwmzy.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2yzcvbicx.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2ollowmbo.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2pcwpcpyh.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2kyqyodrf.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2rusamiig.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt2zonztcay.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2kvxhhlps.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2xqdstzbz.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2qybovvhd.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2agszoxog.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2loanycae.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ohmyxzsi.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vvzsifix.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2xlyvvlok.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2vimeusuu.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2czsiodel.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2twwlmvbt.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2gncfxcmx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jkucuaar.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2wnaudibx.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2jskjdhiv.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2qwvreksp.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ojefwrje.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2xnrdooqg.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2psxavyca.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2eliajjmt.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2icgihbxq.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2oiuekfai.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2fmeopypr.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2gqlwmlqh.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2sburhhat.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2xitusfua.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pxnononf.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2qbfwqifu.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2axnbdzjb.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2onrnnbqx.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pcvwodxa.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2qlxqhszl.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2clutcrkq.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2lhmvwdah.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2wdpuxqqu.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zkvtkkbb.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2ksdtookx.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2uvlnoune.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2mhdhonoy.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2kknyqegr.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2nxfaxacc.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2xvvsiilc.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2uwnssbph.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2frqjzkrd.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2qrstjpgn.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2pmhrmnvf.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2xyvfcuhq.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2drlrddki.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2hitkulfk.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2tlxrkqae.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2gkpxluor.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2wukgrasi.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2cunwuzgb.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2vuamzetg.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2rktkfetu.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2jeljslnz.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2iqudcgcl.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2fuihpmuk.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2yzssmjhc.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2wslnwqtb.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2bajgouzv.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2lizbctob.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2epkfgotx.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2bwprvslp.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2wrztkhdn.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2iuzcpfih.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2bhrxyjoe.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2mynnxzko.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2kjqixski.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2nvnufmzj.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2pnsgloqf.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2qfgdudte.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2udgyizey.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2qfqomzrs.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2tfbfvqjp.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ohtyvihq.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2dhainkel.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ycwabebb.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2xjwfmgwn.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2jrbtrvpc.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2wjjgjdmp.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2vqbajwcl.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2ftefkcwe.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2lwxabcgo.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2bhqsuxmc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wzfthzdr.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2odhpkipu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sezkugtx.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2ryewnfnp.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2jncwzvkv.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2avmndadu.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2eosmqiau.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2yolaxqyt.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2dyvkbqqa.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2urgoelfr.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2ifhrcblp.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2nqgrptfy.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2qtwxdcns.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2dfebhemn.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2vjrqrztw.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2xsachbwv.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2lavieadg.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2niwmpoys.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2ndggcthv.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2tcwpuydr.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2bzsoakdn.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2xqjlofpv.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2vmfmdqlw.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2moiiismr.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2hbsjdtec.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2cztzpsdq.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2ydtryyty.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2hqdslijb.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2psckhbfp.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2vijzfzkl.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2ggpkiehm.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2gbrnccta.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2wdxajyyj.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2ncfuwaod.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2tqxawroa.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2ufbrqkvn.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2gqiakrmz.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2yxtylfhw.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2vyfcevat.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2irvrzvcm.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2himlpnfs.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2qiwridkm.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2tcckewtv.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2hqiiroty.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2ufbnebui.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2oqywmmwq.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2aadcboje.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2chijvyoe.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2uhcahxik.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2qvxxvtyo.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2wimvixic.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2hhhsplrt.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2vvmgfdxt.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2lmrjzlgp.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2fwczznxo.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2xindbnrh.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2aoryyvry.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2wvcbxrlm.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2bctbalro.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2aymyfvfv.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2ikztndku.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2oddoinlb.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2tqewktds.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2xddwfnri.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2imgvmkjx.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2lvosfxkk.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2dganclhl.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2maxsffbl.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2vbrgpbtk.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2ssdxzhaz.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2hggbkjtl.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2kscnpfak.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2pnypnerp.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2zgnxncxb.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2rmqpngeo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uyefipzg.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2kygxqawu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2onjipzlr.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2milqktup.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2igbjdnhr.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2nqydegct.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2rkvcyzdp.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2hqcdxmsb.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2evmcplkw.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2kxcvlvue.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2kmawpoll.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2zkeabtnm.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2jwnvjelz.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2gorkpqgg.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2xpuldokr.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2ojsguucq.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2ynbenrju.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2nzfnpkkx.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2jjqndxyw.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2hzmdkkpu.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2spbxltmd.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2vyauxztk.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2vjemjibc.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2gilqzpnd.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2qkyeujix.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2kloyatrf.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2slswfcyu.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2ynkfpchk.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2daydfywa.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2rglknqfx.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2sobodfnb.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2tniivlwq.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2efmmopzg.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2tclftxbg.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ireliybb.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2amumslno.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ogforife.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2lwqgprkq.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2qtmuypcc.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2uohdlxiz.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2kwavnjze.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2nnrrkhld.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2fufohstz.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2kojtomkv.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2pexmxlsw.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2fygoycvb.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2ftrowmgm.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2ckhpkysn.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2qkdcaqtj.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2gzehxmtb.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2gskxqptx.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2jhemdpqa.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2bpeuqjhv.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2ezxxfqqa.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2bcktrulj.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2lyhkplnk.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2hzbsavkx.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2vzatbfxc.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2ghlybsux.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2fapfjzsm.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2wdcxchtt.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2swzkumux.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2srxrhwpc.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2bzqbmnxb.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2djcwpaed.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2ogfyddal.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2kzxwmqim.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2sscepzzi.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2bsalfkwk.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2ncodahyy.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2vyjkwbxh.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2rbuoorjv.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2dbpwfnok.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2kqqwmcja.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2gongmwrs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ogrtftpq.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2rsnrmkmi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ittqkwfd.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2cseoledc.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2eottevlm.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2zqixisvz.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2twshzmbe.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2dnwszmdb.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2nvedaume.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2fvwxxvyh.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2emfskoux.html


<!-- 参考信息 -->