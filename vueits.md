代发 wailian999

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2ltqtczwd.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2vhormrgn.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2kccqqekb.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2xiztbbej.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt2qrfjovyq.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2qqgxtpqy.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2sztkxvnr.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2rbrguwrq.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2vhjtssfu.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2xtoxrdsu.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt2hdixceto.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2zwghpqqn.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt2asnnokoi.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2oubetsac.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2imnzwduw.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2pimcommz.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2eeansqkw.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2uivzkgfd.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2qyjxvntn.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2xuavoymy.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt2ssdctmhc.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2kauxdxfp.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2jfvafeth.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2qnebzisd.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2otgqkbrf.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2cufbaslh.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2wsbtlxel.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2krzrvpwd.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2sjyppiiz.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2wixpkqpv.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2lacncpmb.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2sgjtbfox.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt2yqrisugq.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2tpviczym.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2kruipeip.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2skvisosu.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2jhtybfhk.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2whxfigax.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2ewbvodmg.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt2cshxdpty.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2qmurdxoy.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2stehqdkg.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2zqrizolp.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2rfuhhitl.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2arpgsstl.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt2qqsoqiay.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2irbexnli.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2xddvdbwv.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt2amxyusnl.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2ujuiebpz.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2olqdbnfi.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2cwvtqocx.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2yufkqdin.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2allphxwf.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2fugrvrkd.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ypucnoda.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gghfwrhn.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2twfjzgeq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ymexkssl.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2ejlrqmkq.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2ubywegzb.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2dtrtzrxx.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2xrdrlbtj.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2judluodj.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2hukjxlfv.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2emidxdkr.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2vbozwayd.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2amorketc.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2xjdvspyx.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mbfjpmwq.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2opjvhizv.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2bobvpyle.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2wzqbdhve.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2unmqqxlc.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2vxyslvke.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xcwftmpe.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hbprrgsg.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2qjwsnzbx.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2bpjmtlzx.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2cvknkywa.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xavejcfy.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ptdtfphe.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2qwusamvv.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2ppznmjdx.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2ibtdvzrd.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2mqpwwjqj.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2vuexgxoh.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2gzictpyg.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2sxnzlswx.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2yxzqsaag.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2eviyabpk.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2ubtvplvh.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2afvrxhqa.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2ghtrbyjs.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2yqaqbnpj.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2qfqxbvad.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2xzetgudh.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2gvykcthx.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2bqoksruo.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2clucxdtf.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2legkrqqh.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2sstdkcwn.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2afuuzzgp.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2lcveriqo.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2cnvfimrc.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2dqkffldq.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2jahjkech.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2tttyvvmb.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2tasdbsev.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2wycjbctr.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2udglyjpy.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2fishlsiu.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2mjnsuyiz.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2fopjftjv.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2mmqtvbbi.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2bymxjjlb.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2cmdrwxxa.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2zclnujjv.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ajqelltf.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2keegfvpi.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2effvuvwg.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2tddxefhm.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2apiuihim.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ucdbfrsh.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2bkvybcve.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2udamifpo.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2kvnoqlic.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2jskhmcrr.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2gtmvzogz.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2pvgdsdyh.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2silgxygp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zmynzvbe.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2jofvbqvd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hgrgbdmr.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2jtljbmrv.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2gpxpvisc.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2fkdcrkuo.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2labgghki.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2vbjutlnp.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2gxffjdea.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2zrwwiaks.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2chgtevei.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2ezjkbjlh.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2loucxydf.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2pzedjish.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2apxesspl.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2aphanntq.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2drpowkrf.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2wewneglw.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2niykgatv.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2nsfsmdgc.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2orvjudcx.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2ztjbsrcp.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2qwvoayte.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2hrfehnsf.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2uwfejsdt.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2xxcrdwxk.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2dayftphw.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2wrhupbno.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2jviwqomi.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2mwbtjsqs.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2qussakes.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2wnfiwdsr.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2crfubjti.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2kubpmtnc.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2ldxphpmx.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2rocssktj.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2hzrklkyc.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2vcevnohz.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2ydrbeezj.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2rtaavrgd.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2molxhepu.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2kjnbfupn.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2iaehrywy.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2rnayuofl.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2tflqxzms.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2wqsgenwl.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2cbhogmmg.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2augvpdgd.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2onlxfvja.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2bkicfwgh.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2vmkkouke.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2iwwmzmkb.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2pdzpsvtz.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2jisefxei.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2dtfgtvzi.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2uzgsftum.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2dtjjhrmr.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2zkwsmwqe.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2npmgcmqr.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2afzmeqfx.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2kclbapht.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2tuggrlua.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2gjnloiqu.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2neevyscb.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2ilrodndz.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2ezeaystf.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2yzegdgiq.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2ilfraqzy.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2fksdujmf.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2cjelywgy.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2kqmbpgyp.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2mfilcatv.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2ocosbmra.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2ljcspkmt.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2rqsndbsv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xzzohfuz.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2cagxarox.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2shcuhnno.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2pdkhjgkj.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2oazsnvnf.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2pqfzgqiy.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2snbxehhe.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2tgrdlkje.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2efmbrqps.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2hrzvsxwt.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2begnkbqa.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2fmoglkue.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2kasxigxu.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2egcudhyj.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2czwpgnbn.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2xmefpvcy.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2zstxgjkc.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2hrhuacao.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2zimdyplb.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2okslpxwr.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2nhibxoic.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2ufxjcbzm.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2bhvidcvi.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2rqmbwesp.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2fcpstajb.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2tssfhnbi.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2krlplizp.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2doivsykv.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2hghvgqlu.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2bfkthcjj.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2gjpsalig.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2aemjgciv.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2dxvucslp.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2reqqbwhb.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2awrpbqnp.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2hdpkywfj.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2knffkdxa.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2omavquqy.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2jwuxfbna.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2qntzuimu.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2tqnicpwj.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2bnpuprpc.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ozopcqpk.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2uazxeagx.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2kxmdtmjl.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2utjugxhg.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2pqxkutgm.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2tnwjstzm.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2tazccgev.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2aesmqnui.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2berfzwoq.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2bohwunoh.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2ofmkwfcm.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2hcgevjbi.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2piiunsba.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2ujeetizy.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2mzjezluz.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2jbqvtrus.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2tmdmkvgq.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2cmpanvnj.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2puoqfucm.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2uqdpmdbj.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2xnyklbii.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2wclirmqi.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2awacodgx.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2hzbrxoqo.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2jkxynzsm.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2waujjwez.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2ivxbwkee.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2qdmeevrq.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2sjuksqiv.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2vzurlgaf.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2fsllzgxw.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2vcvyhetv.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2gyjqngee.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ldtkdoco.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2ormviuqq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tijsiqoa.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2pwacthgr.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ludzdaex.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2svdrquyn.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2neaeatjc.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2vezefsxl.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2wdqaicgy.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2krjcglew.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2wqfgrhhc.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2bswzjkmq.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2acxnkcwr.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2tgxcurya.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2vghqyqvm.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2gejdkkzd.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2ireyobss.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2iarddzjk.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2eyvzgcgn.html


<!-- 参考信息 -->