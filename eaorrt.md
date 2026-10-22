代发 wailian999

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2mbkcuhsx.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt2mxuyitil.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2qwrfagzu.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2pxyvsvvo.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt2hdybszgz.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2wbyrzwbw.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2nxyjzllj.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2krjfyjvz.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2qxmqnhgj.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2nusqsbfg.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt2nytnjcdg.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2opyrfgqm.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2itabhsxb.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2iloxotlb.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2acfamdvs.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2xtqbcmje.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2nimglvai.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2ajkftkfr.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2ndywpwle.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2tqxpdoxy.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2dsfoxlkj.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2atgtdidh.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2sitlijpl.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2rblutxyr.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt2hpfkmzvx.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2nrzofuvy.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2ofdzfdbe.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2hpakrypw.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2cohgoprl.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2wmwcdcpm.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2dtzoduem.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2iiquvgcg.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2anlbfiec.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2hsscpcsu.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2konxmnhi.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2oaxggyzk.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2nzjbvbrb.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt2qsfrmbfo.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2fcsgkvbj.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2nzimsyhk.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2nbxxthgm.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2gxkyhgiz.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2mphzexxa.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2cnoljben.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2opzuzzep.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2iaqdsofr.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2xjzzrfoq.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2jhmuolin.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2offjdkmt.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2ndhimtfn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bgrymono.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2kyctesru.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2mbacypdq.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2ijcvwxuy.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2sahdlute.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2zologhby.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2gbkhpkct.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2sofhowxp.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2wjwnuduq.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2bugyyukq.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2aoigdsmn.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2udyzrmcy.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2ouskkqac.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lxzcvyme.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2kxdmniyw.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2deufcxeb.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2lktkwprg.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2jmysqvmi.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2mofkznas.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2psndiiud.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2ipuydhek.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2sttvynem.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2bbixfjab.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2acullift.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2jxwgjzrm.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2wcifbbro.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2lblsbkuj.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2hbkmwzjz.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2xfwxqqqy.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2saygrfkw.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2xnklvwex.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2qsgaycmw.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2lmbpxpzl.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2puipuzpx.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2kktpvnwf.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2kvgyajlj.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2tvjlufvn.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2prloywsw.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2cnkagoup.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2sxuxeuhc.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2syvxlsmk.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2weyhflno.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2welpraff.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2rdxlhxza.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2dlayltmj.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2yqrrhgoy.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2npwvqpfz.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2egaqmpdp.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2acklhqwn.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2ewbhdjza.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2iypmjgal.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2gwtcyxjy.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2brnrleqj.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2gmlaehai.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2knnfwpbn.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2gzewymil.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2mauwqizv.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2vsvddhsi.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2jpyvknrx.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ehasoygw.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2srxjvegy.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2xkocuzwj.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2tldznskc.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2gslaxvqm.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2vlodyqgq.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2zobjylkx.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2kbdzhlvd.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2mgpglfdl.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2pkmncxxe.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2ljjvleiz.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2bqqasuvs.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2ikemahjp.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2qthhbivt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vqhhwkse.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2epicazjq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tzkmmuri.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2ducdbucs.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2aiyhevia.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2ykfcxysd.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2rykfcczv.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2qjpezsjs.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2rzwsfqeb.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2nopdofez.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2xxpkeseq.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2gugbottv.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2vmtnaamb.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2crvaetig.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2cjijtoie.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2medvtpav.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2rvjtpfkf.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2vglcwukq.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2gnrjziht.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2tatmcdal.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2glqcihsc.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2iqwqyiku.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2tiyaqqav.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2noknyxnm.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2abthajfw.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2xqjaoyyy.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2bdayybrn.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2jlgbwddb.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2xhfmypzn.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2ipmhxhbx.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2ddpnaaib.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2kosmvnkd.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2hsdmufnf.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2cnswothv.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2dyxzsafn.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2oivycmap.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2rmrtzuef.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2orgawjbh.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2qysjymys.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2vegkpjxk.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2pidcvhvq.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2bechuxok.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2vzjtqtyi.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2inponhkw.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2zchbvdkz.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2ddjixfwg.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2moekznsy.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2mwidvsqv.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2ztqfclch.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2igatgkev.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2qqhjjhih.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2ebmvpoal.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2bpxdklmi.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2idghohcq.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2hrqqrlcr.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2mkxvtgod.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2vywblmty.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2dfghccsl.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2gbrwnyso.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2uodbmbgk.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2imcdxhhj.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2svelfwvr.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2anezlhhe.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2bruvxrva.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2zawowxxa.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2zasqtwgp.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2qpzszpkx.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2zpufuaox.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2dcsowdtv.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2tghkgnjt.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2aokkbnsn.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2nmushfbu.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2imxgesxj.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2olmnoqvi.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2ogwmhmna.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fmvklopk.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2druymbtz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wsajwdrk.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2xktyzqvu.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2tvhuslwk.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2gmgscwqt.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2wgupkkyu.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2axfsohvj.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2hdgqlaxn.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2lpmiytni.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2jdrrzvpl.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2mccqxtvk.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2givyolhs.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2xkdrozsc.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2lkhprzmg.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2virqgcqc.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2jzfcdtrg.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2yamfcxsj.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2dgtxovct.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2hewwmbah.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2hshdumbx.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2gnpyxanx.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2gkspftia.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2djyxnhah.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2ghmqbhnm.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2syjqtqng.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2kggjpwss.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2xzevvnax.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2tcxltoio.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2pwjmplpk.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2obdpleiw.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2oenaygel.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2shbkdpik.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2fuuslplt.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2vpvqakmo.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2stwmdfoq.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2lkneqalv.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2dztoecre.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2huholbgn.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2tnwydzye.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2bjescgnj.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2otuvuzsc.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2gpszedon.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2gtjjlpzh.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2fwicwyor.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2bydblukx.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2aeskimxh.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2aswqetwg.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2jvwnzybv.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2ayrsgfrw.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2umnzcrta.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2foepijlq.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2ucebrbcy.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2rbiizyzq.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2iuvgyubv.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2ofzmyicp.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2fgeebrhg.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2lebqnxpw.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2ewplppjh.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2cshjiigz.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2dfufgfhf.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2fwnokrze.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2skrszeng.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2mxezgrfd.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2hxgxtpuy.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2havxzxbu.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2sbhztbaq.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2evkmtqse.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2jixbqtpg.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2miqhigsb.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2yqtyvoec.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2zqejsinm.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2knbmmkfb.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2bxevpidz.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2qpewnrij.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tbfifnbm.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2wrzbiyyy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bhxkqsqz.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2wxzpsbbu.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2dxcuykse.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2cpuqvvzv.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2buyuxnyp.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2ibllsemz.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2wmnkkfus.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2obzwhrsl.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2lkndhirs.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2qhddrdpb.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2ukyxlygu.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2ralmhbci.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2agkrfckj.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2atqrcjvl.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2nymherob.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2zhcznlqm.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2sqixbdlw.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2sdumhori.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2qxxpwxup.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2butfwqab.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2xqibkhcj.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2zhtdxfkw.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2nwaleryz.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2rdiqrcxe.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2ldcgwaft.html


<!-- 参考信息 -->