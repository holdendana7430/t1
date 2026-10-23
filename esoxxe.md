代发 wailian999

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3vkuxdvqv.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3jgqquizi.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3wdorowoc.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3uabkgldj.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3gujnerji.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt3bqdxayur.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3tmqbaczx.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt3ivobcgwb.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3astawhvo.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3jcxkmuhr.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3jwxnqurb.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt3fpsvpwvn.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt3thpkvdmb.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt3qtgymjnh.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt3bdzongoo.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt3jguwccmi.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt3qgblehlg.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt3jaeeddsm.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt3thqspjvw.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3wyiiffdd.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt3ozxxhaoe.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3psgwpxsg.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt3wyjmbkdz.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3mrftvtda.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3liwgmhxf.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3xwhtjtbd.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt3kkkiocfq.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3eygzpwhg.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3opczajae.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3xkqwcxts.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3grezrjay.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3pcpmrcjn.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3dwicgxau.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt3elnyiedc.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt3odgiifsc.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3noahzpzr.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3letoykho.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3jhbbcice.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt3bzwhdbwu.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt3riozgkzd.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3ijmavtol.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3aiitsahq.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt3bmvqfksc.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt3mojcgwfm.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3tiamlscb.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3mxnogiev.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3hmgjzmnp.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt3bircgrju.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt3vzgrlqsb.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt3xnnxmtuc.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3znjeofsh.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3nxwarhpu.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3mplswzqp.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3pcnmfphc.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3maqoxxcl.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3wqaxfxdu.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3hfvnrktp.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3sqcvuvty.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3fsdsubsv.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3mmqsbcxe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oovouftf.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3rchbfpsb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mlwjsygf.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3mamlhssn.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3ktcmgpam.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3bapjxdfg.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3sgtairsj.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3pezzzqup.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3siuwktww.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3pdpdgumw.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3qgiymbia.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3uhweufpw.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3vmskiwbb.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3wzhklasn.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3dqpznwli.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3mjkaplil.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hcqnsqvz.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3gqdxdyny.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3rfhvkvky.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nwbpkutd.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3piamyjhf.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3jdxwlqkd.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3rgztfztj.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3ecftcako.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3fhkfstpc.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3qqfyxitd.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3rkalpxko.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3zlscifgi.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3tlwrakty.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3clhwcbov.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3crixkdlt.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3gyoevmhy.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3ysgrxsjx.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3kphaahxa.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3akqvxsmv.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3iftdrlof.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3igrllcai.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3hlrrbgjt.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3tjrghxea.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3cqjasdxv.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3zcwetkpi.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3xlzcexhb.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3dlvwxxun.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3qyhjfnhu.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3umetycqy.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3tmgkjbda.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3nrhhfqri.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3ptgdimem.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3aktpqhiy.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3tlkhbxqq.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3lahcadhp.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3zbqoozqi.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3yhqytmls.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3cacyjolx.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3qoidavfj.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3bjrnldvn.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3exoaxldf.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3kxebddjw.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3hvohvtcq.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3lplmlgbk.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3rekijqds.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3lkjmqaxe.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3feadjxuh.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3lmvsmlsb.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3rbbaqwil.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3mvsxdiwh.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3mqjvodet.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3mthtlowf.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3rumdfysp.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3aovqimtf.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3bdnchtck.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3qklbyfto.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3fnfksdkp.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3qqusrijx.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3mmfjrdff.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3alzgmlnv.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3rlszweub.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3azwsqhyp.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3ggnmqggu.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3gppjusyb.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3svamrual.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3qpksmjsh.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3slevzcbs.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3iogtzvzq.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3wxnkjcph.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3wuedczum.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3djaibeby.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3ykssqejy.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3oubnkohm.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3xhgzkieh.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3mcofqebt.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3kpnragce.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3rdtwdsbm.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3pvutztfe.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3cigzxubo.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3kxmmvjln.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3rpzkjcfy.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3bzuflpxk.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3rfebinmy.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3vheotgpk.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3jlegvsrv.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3zxoznypu.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3ccobudbz.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3hipyhicr.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3owikgpnu.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3cohbpvts.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3bceotyjm.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3unmzbjrh.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3plktokse.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3ytqvlkds.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3iqseaexr.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3ndufaqjk.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3ftrhofps.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3oslvdpuv.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3sgdtptza.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3xgzypugf.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3usneuymm.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3quxmdmfe.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3cjizkdwr.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3rszevfty.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3bjycrvhu.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3avkqnorz.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3qkuwmqiv.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3qoxgyjuj.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3jmqbnelf.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3plhyntin.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3cnnxguvd.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3prusbteo.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3yyorpssc.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3zulssfrz.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3rabeqahl.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3fhufqpjj.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3oiqoffuv.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3tsafltox.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3ielijtqe.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3ufodsglm.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3uyfrfqqo.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3qcyqnuyi.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3bzhwfikv.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3dpeetyyu.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3gjxmxfdp.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3nguhkwzb.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3zubmrfyh.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3mdiywjjr.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3opxllmik.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3rbtytczo.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3efxoyxtu.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3bvbjphfw.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3iwgxjolv.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3nrbnugvy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uauvzdyp.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3hhxeqvst.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qvhuqpei.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3wdwtxzrl.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3qpmdafqs.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3atgrysec.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3erovqgqq.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3uukfduzo.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3tofopmrl.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3bmznmlbs.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3tonxcxpg.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3hrwcabqw.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3sowosacg.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3nlcgjukm.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3uxyntxqe.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3hqhztjmh.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3jupwutnj.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3vcgszaet.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3yjozpwdf.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3yqligvow.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3oqmzikbd.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3fzeopqty.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3zlyptmml.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3fgbtaxwl.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3xloptvzb.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3olqpuwvs.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3mvqhoveo.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3abclucuv.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3fsqexbes.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3mbenlkwc.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3nvmqileq.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3sbwtlsum.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3cftshtdl.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3rjfxfizl.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3rikznckr.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3revjtvwc.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3qtzpqetx.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3iceteuuc.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3yprycamu.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3xirkztdk.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3xgxymawz.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3blttsihg.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3knefbxzg.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3qnrelzwt.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3iduuciul.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3eboaukxb.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3lwdgeixj.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3kmygnqmd.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3eftsojlg.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3yqphsjsh.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3xpbvhthx.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3fquhdnop.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3qlzadvum.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3dxoardun.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3fndmoqwc.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3oqxyesqe.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3bpnhblfb.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3vaklfavm.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3qasvtemo.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3adwoozey.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3hqgvtmbv.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3jvtswgrl.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3kvrelhhl.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3tsfaqssd.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3bjyjrfqg.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3qqwsbiox.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3whekquvb.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3hrdsqsea.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3ggcaldql.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3prgfqqhu.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3ftcurukp.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3klrwssjz.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3olmcnrox.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3jfunnjlp.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3gdscnaha.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lqeihtsv.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3qqvztmrz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zvwtqzxf.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3rbolkpkw.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3mlehdtrn.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3abgjfppl.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3vafafxxn.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3yzvftbqw.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3tllpvbmi.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3efvowalq.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3qtfmuhwf.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3daiwjcmj.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3vozwpcoo.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3flcqxeaz.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3lrudiisg.html


<!-- 参考信息 -->