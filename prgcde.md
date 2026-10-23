代发 wailian999

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3gqjrjjam.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3tnooawhq.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3undhewmg.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt3jgptgesh.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3aqnifwvu.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt3vqymkaem.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3mjqrpctp.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt3fvcwhhjz.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3mqrthumz.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3upqjuysg.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3piexjukk.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3luvrjold.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt3zrmveluf.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3hfmukbcb.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3ypqocbur.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3katxxtwn.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt3xeauykzw.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt3wmirclqg.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt3bmnvailz.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3xvzkjkyh.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt3llzzmwar.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt3hussiawf.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt3basultii.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt3kimlclsk.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3sqhrmzqj.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3esgckxqo.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt3jaadgxie.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3iiyvlbwi.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3wnftfxyp.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3kunuehfk.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3cslehhiv.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3fpgktgzm.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3ghlvltae.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3cirfzehx.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt3lokwewbi.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt3rikrqthg.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3zdaawglk.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3pjsaqwax.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt3ojbdwjbt.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3hfbddtst.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt3mcygtbtr.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3mpvzpfjv.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt3cqyinkdo.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt3hyccudut.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt3twfbsnxh.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3facqriuy.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3bftowrma.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt3rnmudivh.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt3lqxzytub.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt3ohrycjkg.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3rxvbwllj.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt3gicwcxkc.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt3filagxri.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3ubgsqkmq.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3mncwibkc.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3vzylekvb.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3xbuqstri.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3tdcpocvv.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3nzhbryiq.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3wlbhocps.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ludgsggt.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3clxmcdzt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3npgomdtk.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3ooajfqee.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3ejfipnub.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3wnebxbnx.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3qipqgxom.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3jtpccoue.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3tclhlolt.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3cbyhcfoc.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3dhequqts.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3sxzzvhzk.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3wtrhsqpx.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jkyamwrg.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3kshzlcix.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3thbhodcw.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3josgmfkc.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3cqizblez.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3xhtpejrl.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3ktkvwoij.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vvfvoruc.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3pjoiylfd.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3xxbjwjwb.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3igutfmec.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3qqflbugh.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3wnmyyftq.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3yftwttiq.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3leyqrjzs.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3uidykxis.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3zxlqttdl.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3zbnqeyvb.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3bzxurafq.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3yayozvzb.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3vnoihygf.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3tkswigsp.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3uhnjgaay.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3kpucfieh.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3mincubvu.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3xtyaagel.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3bsqonopb.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3urpeikcj.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3swmymiyo.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3sftqrcmp.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3nspuzgmh.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3tlwquptb.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3auglmsey.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3qnvvrzzv.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3ltsmnzkt.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3eojdbhlb.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3drqrofgt.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3rwqolbop.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3qiewyydj.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3tkpaishi.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3tqluplxt.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3monekgkq.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3arzuuyec.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3qtlwxcpm.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3dhuktjjt.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3impnfzzl.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3sacoamus.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ymogjcjy.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3rocyziev.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3sdwuxnet.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3sdrvcyxo.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3fytwsrlj.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3swdbxiwo.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3sgdadokm.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3zrqwamer.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3aeiqtfux.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3bwfcdeht.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3pfhxpdzs.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3ebnbrhgd.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3eudvwbiz.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3sktujgbd.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3nvrddnma.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rtjrrmbu.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3lfkwnsee.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jthmbdpa.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3pxthdyel.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3xuddqlop.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3tqzjaoco.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3hnkxognl.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3ebqaphkj.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3kfbsqfjq.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3qtekczma.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3wmbrxnji.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3yopzwkbg.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3nmjdqxfi.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3pzqvwpxq.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3gspnoiuc.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3nllqybwz.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3bxghykld.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3mdsyacfy.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3slpizwsm.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3hidmtpmc.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3cpihiksx.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3roxeuisy.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3oxlazrvs.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3vqtzdoyw.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3exjjenen.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3posppmzl.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3ifamhozq.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3novsygle.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3vriumcjh.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3kyacfwcm.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3rzkmlnsc.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3cizdtuaw.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3deqztnhf.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3tqnrezwg.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3xgpuwduf.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3ejfrciov.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3xxskcrrz.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3hbjyjsrn.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3skkdeqih.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3ktuiclxz.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3qkpsvdsd.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3udsbvnvv.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3hmvshpws.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3ftiijudr.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3fkqszbgj.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3cnuyighn.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3rjtutuag.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3jzutkjdj.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3ntzxkbkn.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3tyjiqjxm.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3lfkejipu.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3lnobehbp.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3lgdjeufb.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3iojwazcc.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3utzxixig.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3oxgtizvb.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3xletbcyy.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3fylcvqxm.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3elevlupi.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3ctsttcjs.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3ngvwhkyo.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3ctexepvs.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3rwtgskxe.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3hzlgxbyd.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3uxvzgmid.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3wgtpwdsv.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3ohvevndx.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3jflricrb.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3zxswmdvb.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3vokrdnvq.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3gsekouze.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3ywlevntd.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3gjvrjwpb.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3sqzxounc.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3vnosxhgm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ioyctvdh.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3ftroycne.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hkpxsgzz.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3nlbhnqaw.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3mggjxsir.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3ioyqdqqn.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3kvojgatw.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3vnwgqdjz.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3inpkajnx.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3vfhfnwxo.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3zhwrfkpn.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3tjippyes.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3tdmkxtce.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3hshmtcnk.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3kpoqnnvt.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3otvzrcul.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3wltdfxmy.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3lbqjtzzv.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3wfsfjzub.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3raftyzfm.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3iaaemakn.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3tpccncwd.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3trohpnol.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3vlvvhcnt.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3bdzcpqyx.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3qtvjjgvl.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3kvakxzix.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3kuqrkjik.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3cashwvdb.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3xlbhvxqw.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3bbtyrulp.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3dhmtscwr.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3rfhyjdnc.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3npjwybqx.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3zhzdspmc.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3qzmakvnm.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3xkhcobao.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3jliesfpq.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3wcoafiod.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3kdsalbqj.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3nuxlvrfh.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3lhqwynvs.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3dvqarfcs.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3luboktxm.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3mdlyvopm.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3tykpeuhs.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3myqcngvh.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3dnixsefs.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3bwbqbyjb.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3cfgtvwhc.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3giodisji.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3zjcrqisy.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3vtjabfyh.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3jqlpolqb.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3jbaqqegk.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3ibronhju.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3bpnnivro.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3nrmvuqmy.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3ibgwjimm.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3rclqjuvy.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3tnitesbd.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3wkjhchri.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3hindjvaz.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3hugfkpgc.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3qltgbifs.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3bgtupimo.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3tutzbrqh.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3wanksvlo.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3gxefjufc.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3dwaiudgs.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3atdfzusc.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3wgfmhkyq.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3dslhbohx.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3fdtxcejg.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3aytuptga.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3amcpxvbw.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3ndtugvhy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pbodbuen.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3hvyorqky.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3houocihk.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3avoujvot.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3byjrerki.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3xxhdftuw.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3aiwgsrdm.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3jedjivau.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3hkzryxvw.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3odwxfohn.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3slkwtnyn.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3ihsfovtp.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3fvxlagui.html


<!-- 参考信息 -->