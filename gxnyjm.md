代发 wailian999

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2wyzgmhjl.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2evrxtinp.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2nnkprvjy.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2tltlpfde.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2egymfjey.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2kcpixdxi.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2rjbsgaak.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2cmynlqsc.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2wkjkmifg.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2ifbvtryn.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2dknfdelh.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2cwfqwdkd.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2pheohjzp.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt2dqrfxkfv.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2gfchyafk.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2aobzgqrr.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt2vlteogod.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2nneiyzrm.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2ugxytuzp.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2chhdyvwu.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2kzjehixf.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2aofubnyu.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2gkfpoymn.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2lkqlopkc.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2wjuqpjdt.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2dfzcnmrh.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2wtvfbxvc.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2kdgnfecr.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2izjoloqf.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2naalbzaq.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2qhrfeduy.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2wwgrimuz.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2bjngktqr.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2omregebi.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2yaaebwll.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2cnyiyeer.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt2ondlutkp.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2bmihtfko.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2safynqme.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2lgcbrpgv.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2iooclpds.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2sjvwllwe.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2cmloajzr.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt2qonfqqwj.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2otuqakkf.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2nkgbbzzy.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2annsbuyj.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2ohvcahpg.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2xfipzhqu.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2zhfajwdd.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2ulfguaeq.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2flroeyxr.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt2frehmnav.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2chbkwwvc.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2wisiwwjd.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2ivknljbp.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2ngaqsgcf.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2hxxayytr.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2zejwuebr.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2kjietmeg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2afblhlpv.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2xjvfmyhq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2aiylyazs.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2hkanshoq.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2ubenvxan.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2qdbwhqgz.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2kpgqlhcw.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2gogzvxcj.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2akthxcuw.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ssauewmc.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2opqzozcq.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ecgnczxt.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2jfqygbqo.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2lmefcmmb.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2zwtealug.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2qkpxvvhi.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2ylcalysn.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2dsgkpvhv.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2xtsxngbj.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2objyijmk.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2lcscrils.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2ugxgaiji.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2zzkqnoyp.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2yrvxljhg.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2zplhmdhi.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2yfxjrsld.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2avivnkpp.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2iyhklrnw.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2sfamhhnd.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2jxnlosjz.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2nqzgdnxh.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2rbmtzpzz.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2oxhadslz.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2ulkuyxig.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2ohdurxku.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2ktomifut.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2sselrqtn.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2hdqrfluu.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2vexydbag.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2pmiqiqpa.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2gdkwedvy.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2qlseodzn.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2lmfmjley.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2xmddkkfh.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2tswbmrpr.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2sawtwmxs.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2kapfawzm.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2hkaejrsz.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2ntaghgee.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2afaplpvu.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2skpvywhk.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2rtuetwoi.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2oxxwvbxt.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2odxmwmmk.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2mwdeskyb.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2pkylcrhl.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2ymqblehn.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2cipvddvv.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2phlvnser.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2qlafiozz.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2gdnjywnq.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2umyfdtbi.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2reivqirs.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2rrjfoowu.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2wdtmzdtn.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ikqeytlr.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2ehmfibze.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2sswzynmr.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2qfotqgjw.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2niyfjlfh.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2pmtkvvcd.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2pxiedinc.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2ycnbeknc.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2lfwwxwzi.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2vynjjeoj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2skzviinv.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2ciblkqfw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jitnfzyi.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2qshqlgjp.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2cvhqveiu.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2mjqadzmg.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2mqngngow.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2ykunspok.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2geuularg.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2arqxklwb.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2qwdcbalu.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2rcpuqegi.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2egiigjkc.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2dsoznjmp.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2rgipvdlu.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2axqpkxpl.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2lzpbjywd.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2vrjpuaep.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2knjmsppl.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2pigbpqbz.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2csdafyvj.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2edyoyaxw.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2weonmznq.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2uwkrbbvl.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2ifeijgcg.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2uxseanzq.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2myjoxfqa.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2akpfntmf.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2tezzrbvd.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2hzmqxymq.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2uukmzyqt.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2xgholhlk.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2bzszjixt.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2hxytmhdg.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2qentwnwd.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2bxnikufj.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2tbvuwxqa.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2kamscnlf.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2veuvnmsw.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2okjptltp.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2mzbkravp.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2omqisrym.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2hmqzqboj.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2raichwof.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2lwqxmzql.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2etsgwswr.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2btszvlnu.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2asblrtrz.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2lsevzgta.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2filfyjkk.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2paudalkx.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2sosdcjfb.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2ccaguggn.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2klrgceiz.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2spllirkr.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2bwumbxnu.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2jtmfdxvd.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2oorzzlbq.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2bxazlwsf.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2exlkhipr.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2jwalymld.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2fydjfsjk.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2caeszfvm.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2gmfoyfii.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2zmjixnpi.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2siamvzmv.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2qcidtxtf.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2qvqcdkuh.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2hrycghfz.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2hkayufmf.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2nxqaookb.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2ogozpqcr.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2jpplzksv.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2xjgnyxcn.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2lxkwdeob.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yuqtxhpj.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2vcjpnpql.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bjkxucvl.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2wmxpoitj.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2lhuawpvy.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2usnyzmai.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2hccwryst.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2cfoxwoje.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2zphemzcz.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2sxdqubxe.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2zlublrgs.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2gpoybvmw.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2sxigqvnl.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2rbgszpwm.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2kwkfnqxo.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2sogwbkgy.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2njgkcolu.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2wdcxqiwg.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2eijbkihk.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2mlzlmrfc.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2lnzwofjz.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2orpudcye.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2hkfowkaa.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2linozyse.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2eqjtvoih.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2krraaqwc.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2fqtcghpm.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2lpityfjg.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2fjtzqcgf.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2cedlnsvc.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2dewqanxq.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2wzmkbfsx.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2xnnbbolf.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2atwzkyau.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2fbdihaij.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2dridsxyp.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2geyhyawe.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2yeryvvmz.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2nkxxwfai.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2mvwvqmlh.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2bzyxdbhm.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2nbnikfey.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2kandktna.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ixfxjjkt.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2yrcudseo.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2zkmvsrfk.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2lcphgzeq.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2fnocoaao.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2fkoonivq.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2ibolfxui.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2rssxfdzj.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2yelxjlsx.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2jvfvjtsm.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2owsjrdwj.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2ybmfwrpp.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2xxhqcmms.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2orcguifc.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2bmfqasiq.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2mdpbsotv.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2kuwoocjs.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2nurkfdlu.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2szrefuqy.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2bxxboaqa.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2cbrkxgvk.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2fozexxdo.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2waoxrloq.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2fwmbofuq.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2esbioywu.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2athjsdze.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2jrguiewo.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2tvlptuzi.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2taxfkrrh.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2bdvdpqjz.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2vxcvvgeh.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2nvuupzmt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ggvfekhz.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2caosatkx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lcceawlo.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2uultgemp.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2lxuwelww.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2tbhchzer.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2zixwazea.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2umowrocl.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2bksvwjlf.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ihgbeghp.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2wyxdebfr.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2vfdfbrep.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2ztoaejui.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2mcrphfea.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2fvvrrntc.html


<!-- 参考信息 -->