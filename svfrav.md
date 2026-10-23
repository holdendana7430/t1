代发 wailian999

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt3oahrsfcu.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt3qlxknrex.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3bjpyqgwc.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt3jdiygugi.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3thozqlgi.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3dxjixxth.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3aoiwebsm.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt3cvlcujrw.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt3jurrlnwj.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3puukbuzl.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt3gecpdxak.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt3yqpmczjq.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3gqzetkpb.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3fzlcexza.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3upstugxq.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt3tymynhzc.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3yazgkdyr.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3zafqxcae.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3cbxryisv.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt3mtmapfgx.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt3gkdakyac.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt3xfmeexdr.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt3wcmgtwvi.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt3jpomlkgp.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt3hbgatewx.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt3mqkcgvnn.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt3xotkqesd.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3idbqauos.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3slmhyusr.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3miunucgv.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt3qnlfgmli.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3xxqifrxb.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3ajldixxz.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3nskewcnq.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3sjmizdwd.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3ipcburbb.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3njrzetaz.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt3kvoxyyll.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt3liapcwbb.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3cnxjssdm.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt3gduvbhdh.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3zmvfchip.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt3nfbjerbf.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt3yswozpgi.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt3xjmwgvco.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt3gbtspute.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3mlwvdyqg.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt3mbrbkyiv.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3yugcfdmz.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3iomdzvss.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3dnjgxqhe.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt3widfcbpx.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3wtagzjzu.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt3newoqjqd.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3shjkkogs.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt3revqolds.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt3sjrhoxtf.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt3werqhaww.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3xqvypfei.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3rutltshq.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jqnjhrrs.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3kzbqokul.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3ovducglb.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3rclmzcum.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qwbyaatp.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3oavgwzkq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tjoloafl.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3fqiquwxv.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3ldhsmcdz.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3pjsypeht.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3wekpejlg.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3gsogxakl.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3cwmvkjxp.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3hepthfzt.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3efmrpxuw.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3ujotdmjz.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3enklcwve.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3xytyevbr.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3uckwqpix.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mjjsftdf.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3rfiaelok.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3fepmznpr.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3jmvfpsvz.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hryxwyhr.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3biynpmjp.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3grritnrg.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3iukzxjqp.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3gknpxxtb.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tgvwlxec.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xoqhxslm.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3jfrxehll.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3fyiusuhd.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3wwovvakx.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3mkrflaev.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3zreoxsgn.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3kxkppvvu.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3esknaewm.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3ecbgrrtq.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3nepswmla.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3kicmyofr.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3qguxwzfk.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3nrfhvugx.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3ugrawmzp.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3plhjvsiv.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3qvgminmd.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3wxrxrhmo.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3rtijnncf.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3tlpymkvk.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3hraxskax.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3odhwjboc.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3fyaqksox.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3qfnwvjue.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3kuwdfgnj.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3qetsoarq.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3rsaivcta.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3tztkrnkd.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3alfphvsc.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3itlijymz.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3ghdfaelt.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3qmrstlpl.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3splnylel.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3xvagvntn.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3bhfylmwk.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3vrisbcon.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3dsssrrxh.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3hljhssph.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3gxbgxzwq.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3ssdezjzr.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3iogqrfjy.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3cfaniigd.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3kbgkqzgm.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3dytlpxqw.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3lgxtkqzy.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3xjpmhpnj.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3vvxaxmry.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3owkoigmf.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3xjbivkof.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3tcxpceob.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3kisraxvi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vxddavmf.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3mwrjgkdk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nbyfilbk.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3atktxjxh.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3vbsjpunu.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3kvkzhzpp.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3vggbsisd.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3pcztsqwk.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3vbmcptco.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3adqddoun.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3vyjabzxf.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3zsuireku.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3lthwzmoh.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3wlvburtf.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3fipqqaww.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3lcbvngtx.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3lckzgtbr.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3dmxtbxrq.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3oawninhw.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3kmyoolzm.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3rusvoykm.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3fxygmgpe.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3fwagwtil.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3zdifjzvm.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3bamvewvu.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3juyndqvp.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3rqengzdm.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3ttzzuban.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3eijezuma.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3fpzolyma.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3qgaafyvv.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3olnnyqud.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3tlfjrqco.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3zruycvws.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3zlhzlcen.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3frcjpwrr.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3fwibewny.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3vsyscwue.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3sfuoalbd.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3voszrieg.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3xwiywatv.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3goidpzao.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3uvcyrfzf.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3xnulrgvt.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3jdzsfdkq.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3buwspvwk.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3xjtbklnj.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3avhpkljq.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3nvobqcpq.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3xmzfrebs.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3zqzidjfu.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3yowgcmql.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3krcxzvtj.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3qdqcumkd.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3wklwsbja.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3cdsdihqs.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3lzlmcsdx.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3gcmnvrpi.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3pfhnozdu.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3lywmtqfr.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3wwvszyjl.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3epynlymf.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3pavqyero.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3kxdxwaie.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3cnpdakji.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3lgxtynij.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3lksjxdoj.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3arrhsukv.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3llbrwwer.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3zktocjcm.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3mesyenvj.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3hvtbekcz.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3pmkjhhrh.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3vuaevxmm.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3sdjttdxn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hzzzfldk.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3zesjcpoc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oihlouzg.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3arjjjjuw.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3ywqadqwx.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3kckmzsqm.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3ghviyeeh.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3hcvugtdb.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3eyeteocj.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3lvyddjxw.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3xcobcjen.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3orcwafnl.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3ophhswfr.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3tfhhyzqn.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3lmozkyfd.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3fqhnkkjc.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3hqanwhpl.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3foqzcvxt.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3zidimkqr.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3ioccilwi.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3xzkbvzbb.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3drtfdvzh.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3clxfbtrl.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3qszqgscr.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3upauuvdt.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3vburdzbi.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3zgorvcaf.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3lfxahcll.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3ugceudzn.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3otakukyo.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3zioyznze.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3mmrgukrn.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3jdbxzvqk.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3jfjoocdk.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3jljolxzw.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3fgwvyiqx.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3exgpuerq.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3txudgbph.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3rdaacxny.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3xuwwzrfp.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3sdlkfgyp.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3vpzmwzri.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3cjxvpwzi.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lxoczpln.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zonrmrbo.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3jnvlctvn.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3eydixowd.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3guweczkg.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3wnnjalux.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3zznfpcrf.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3whunrxfk.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3tjqbplov.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3qrzhpofe.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3glrpxiww.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3qmjvqukf.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3sfgbxlig.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3pcputsnu.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3yzqvkkno.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3jdhiyhgp.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3vaecoaig.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3cxizbnmk.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3tbbmmtbn.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3ndtmukmj.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3becbqnwp.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3nnrzugjm.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3dqhkuuvd.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3oayzvtyd.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3gbcchkja.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3ldyrxrwa.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3amygitcp.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3hurnbqbv.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3tsrcxksn.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3rphylsqv.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3zomvgvdk.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3suzpfqjz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cdyuxqvz.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3dnltvlcg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zpxjlvbr.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3hfnivequ.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ymopqnab.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3nceqqxyd.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3eigxuudg.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3xejxguos.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3gptvxtcb.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3pajmbhuv.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3neizogoe.html


<!-- 参考信息 -->