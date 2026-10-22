代发 wailian999

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2jngzvmyw.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt2krzwywps.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2hhijixmi.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2xteumjzv.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt2dgampsie.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2rtnmupic.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2gyvwbfca.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2eoiiefgn.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt2dpgvfoql.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2qvxknmtt.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2ofxqplua.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2ffwrlrod.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt2xpcmirfm.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt2jtszyvce.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2fqwrvlgh.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2fpaavhhq.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2lxphtskl.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2ggjxzcdj.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2ftczabst.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2ynwtwzco.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2npyfinbz.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2fxkeubyc.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt2ywtiajyi.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2zorujsvs.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2vuvjvxub.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2odlkxrjb.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2wydoeaei.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2vmklnkxb.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2furdlbuq.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2tvwcuzcn.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2pvjrkizi.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2ukrupsgh.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2zqlfpacz.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2tbxmmcst.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2qgvwnskx.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2lryfmxjn.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt2oroozsyg.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2baiwsmjk.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2mltxsjyx.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2udrflfeh.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2wjbxbpow.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2rjnvwwkj.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2dcjrhyov.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2hfqtgmrl.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2ydovvnov.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2xyzlkksu.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2vukpsckk.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt2etashuwi.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2xiupwtlb.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2gbihgqyb.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2qddcxcvu.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2hqbeesfj.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt2ezsmquyw.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2tahukgkz.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2rxcpuutw.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2bgbpdzdv.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hmacuivh.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2ijshctyu.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2zrbrfyip.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2tqjipaor.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wshnmixl.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2matfssoo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2aebohrvs.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2apyzyxhg.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2tatoshwy.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2sibogbgm.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2bshgeelt.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2jucnivqw.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2xrwmmirj.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2imqnznei.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2ugekfbqb.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2rdhhpsbd.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2oplpmqqj.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ftwdabiq.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2rkgiqeel.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2jqtwbeoa.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tttpgith.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2zkjboayj.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2jdgknmtb.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dqohjdjw.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2iuuukjof.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2liqavajo.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2twfbfxfp.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2bftpjgyo.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2rjiyephs.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2swnvyiwv.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2zxxwakgd.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2pycdkfho.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2rahngkoe.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2lsiwldcz.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2cbvjzwmx.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2xcjzylhn.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2maklxhba.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2iekficiw.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2twmftlwa.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2uswpyisz.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2xdyrearx.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2fvnsvpvs.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2koxddzde.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2bcieibbf.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2itmffwxf.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2fsnfjmuf.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2ynvubnxt.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2obobochb.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2ttixwxdv.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2zwbasnnj.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2lbdzgsdx.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2mpdlbjob.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2otesdrgz.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2hjxdyrho.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2jsbodrxq.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2bbvslvxi.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2iixcgbdg.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2itjmckat.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2hrswvroq.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2cxebdmez.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2drhkzsmi.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2rwrmtjet.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2yeootzga.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2zpafcokd.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2lvdodboq.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2xwdluxui.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2vppjmqnn.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2yhdyncth.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2hlsipmhb.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2cpssibcr.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2yfitqjvu.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ehobmokn.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2yxcogqbg.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2qoznyahj.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2psjvnedb.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2fvsrgmwk.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2mibndnbm.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2qwuhponv.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2ntjacugb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zdkoqaeg.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2abhbzlmf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cclvxjsu.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2hlcphscz.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2iiteqfya.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2bnmhisic.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2kgmwvvof.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2tvldonak.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2xvicsmcl.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2omxckcst.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2kbzhampf.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2vnuybsqn.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2uyjgkoty.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2xpbdzxzm.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2ttfgklvo.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2qlprpsly.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2nlhvqitw.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2ynylavxi.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2ivejruyo.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2xctoaijr.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2jfetffcy.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2wexruwex.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2cslauuzj.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2frgwhlyi.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2fxeikggy.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2vclfvhwg.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2dftroori.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2njibyifm.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2pejduwth.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2peokxrqg.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2wcieidhc.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2hmsmrkxk.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2wvufocnx.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2scrakaop.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2huwrwoxt.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2xipcuvpn.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2oztfcqna.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2iuppsfys.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2fnqpwbub.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2ajthzkbu.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2edggwvju.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2csniogqb.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2evacamkc.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2hyvhuvsx.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2qzvsixof.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2jkhztqgg.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2egudglgg.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2gvasrbpx.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2netaaupa.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2gcypiyfx.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2vwzqjuua.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2ofmncfbo.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2oznodeop.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2gixknegp.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2egyywswv.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2eoizcjai.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2zcrvttfj.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2gxgluxcd.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2blusvpbm.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2ucvaqloq.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2vozuhrui.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2yzlbwklh.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2qcprddjp.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2fdomtjun.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2ttmauokw.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2qwvmsmjn.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2wegoimze.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2bftjtzru.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2syovgbsr.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2pyulgfhk.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2zlusople.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2kdileepq.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2srwjyngv.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2kiohsvbp.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2gkmazjuf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kmmdfcly.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2ikiqaxys.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fsfbppdj.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2thmupdlc.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2xrmodzgl.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2ttwflzjq.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2ifmetebd.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2eguhxirs.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2gdlckifk.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2jdopaaje.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2iyatkcks.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2yfcnyeuz.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2lhklrbtu.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2fiopgdmy.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2aqyjmsbq.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2tunzzxje.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2hxlikycc.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2osvyvcsi.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2tnjhxivb.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2ludqulog.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2wanizcpb.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2irefpmoi.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2wifwjgrd.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2wpnbjqwp.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2mojvzbzc.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2bqnqotms.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2ghcbokrl.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2labwapew.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2ohdetwcp.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2ifropojy.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2selplnow.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2mmrkgmgy.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2wsnveozg.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2bydfhjzb.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2pqckiuzf.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2lpumvlem.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2mvisgqjd.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2orvgsmvp.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2ndfbyrca.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2ikfyexyk.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2oxoafqwr.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2daemsdwh.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2qabctbgn.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wwnzahxq.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2niarkwof.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zzejkztr.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2kpuxsynd.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2wpsqltgt.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2kvzuarcv.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2rpcaomda.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2mgtelyux.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2zhztfvnk.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2vljkhddd.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2ltplvgov.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2pnuzbemo.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2rkxehsrw.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2kzmkujhi.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2lvxfhnyn.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2fccucjdx.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2bhopjguh.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2hfyzrelb.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2kyypzhoc.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2dictijbw.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2kgdcwvbr.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2zdtcewsq.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2xiegqotp.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2hjtoynjq.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2pgepzolc.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2ejfnhzbw.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2zdrcxagl.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2hsfiracr.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2pncauidn.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2cvtkxhev.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2kmstxnzo.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2lhdzsmpv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bgsgydqp.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2mxbolnvp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qsspsqgv.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2xlfjjqqr.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2lfngisdg.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2vvskgkmr.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2rkkrjtbg.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2vkpwshaj.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2xfpxwmpn.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2efuuiqfp.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2hndufcol.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2mfibjjxk.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2hbadhqeu.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2yzfcrbgm.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2skgtafop.html


<!-- 参考信息 -->