代发 wailian999

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2hjdubbpt.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2dtteewfp.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2qfzbtsji.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2nclwzhxu.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2uzcxrcwa.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2bbfwibyq.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt2kfbgjwpb.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2wgonnjbg.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt2hqiaarkh.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2dmrrkqck.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2rossaazo.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2siourneo.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2rpvpgrku.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2iglgcebn.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2hrzficdr.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2ksmmsjgz.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2bvogweog.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2rilvjmed.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2lyvfaree.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2noyfxhzv.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2frpqemkw.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2xqjwselx.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2xoshlnga.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2jiytydxb.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2ehzlland.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2xnrsgmhm.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2dcquznlo.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2taptapkd.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2yzyutcwr.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2syxncoip.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2mocotdmf.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt2lhonltql.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2wtkyjzxy.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2mihnxjsn.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2xpqlfjrk.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2odqehfew.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2hkiqrbvi.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2tposonlx.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2swmsrysd.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2qbdqusic.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2idzysguj.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2nfkhbhrc.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2itfadxqc.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2eresrsnk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mhzuwowi.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2trqwhixr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uknteqnl.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2oyicrusg.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2usuqywbv.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2jftsgqls.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2nmbcmhxl.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2euwlrvwr.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2vrbbfmmx.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2ntaocfmf.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2odssdnpm.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2kuteelix.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2hnaaxzvr.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2esisqrvi.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2gbcszeiq.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pppisuti.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dgndgpfw.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2tirynmuw.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2xcirvtcb.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kxiyvrdo.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gmeglyyg.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2iqttxrrd.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2tzkkashs.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2fmhggsnv.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2klmjxvrz.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2irpadugu.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2uiuyiscc.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2hbbbaaxh.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2uzftgevo.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2fiqbzkwf.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2aixunazo.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2ofhbcuec.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2yalfnwnd.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2gdyquotl.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2uiqhwcta.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2asgsodri.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2moxpbuuw.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2ahbhopcj.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2mxhrlddd.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2sfrlpkvv.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2fxbninlw.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2rzzshjfu.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2zwlkccbc.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ssznkeob.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2eouozdkp.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2shulaqac.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2oqpwquyp.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2prsfbaxw.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2xxzoajgr.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2hvjvxpqr.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2uikadpmf.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2wigpzcey.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2nywrvcgc.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2nhcjfxkx.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2gtscbuqz.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2cxqvjfoi.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2mbkdcxxp.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2kvodlcjs.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2nslmowoh.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2qfvaacus.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2nwgirtoi.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2kgweexdq.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2kcmyfvjv.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2lxwkmiym.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2vmplsyix.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2rznvacng.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2vcidqjsc.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2gzmsntxk.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2oikfxmdn.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2rritxnzv.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2cfaxseyx.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2wvjeeyeo.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2jqmaxuxx.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2ndwayoow.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2ijzjqcha.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2thfdraer.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2byvdtxxx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ahdlklnl.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2raynsyno.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2kpwqqirv.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2zikkvilr.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2qhxnbfwt.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2srynbtrl.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2dpmcpkyl.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2lvjlimrj.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2hafjeulj.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2plxztony.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2cwbrlbpk.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2zdtgzrez.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2eueqhxrw.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2suubsdwb.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2eqepgczj.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2zrkadfzk.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2edafzyoh.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2yxcpmtli.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2ummivjqr.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2lthcbmll.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2kkfytqpt.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2pdloxhox.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2lxgwogke.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2aywhoubc.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2vhheuajd.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2fevwarcv.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2oslrqwuw.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2fmxpmywh.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2pcywlxob.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2ulvvcjbo.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2onuuaxtd.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2kolqlvdd.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2zdusztzz.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2ftbqtftd.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2huagwwmw.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2bwijabiy.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2apvlmzqv.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2dewojlfu.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2dlvykefv.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2gamlrzjk.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2tfksbimq.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2nruniaeg.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2cnqgvcal.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2bblzevsk.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2izwmacpj.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2nrpzgjgl.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2pnhixiog.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2vlrjsunh.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2aeqsqjpm.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2hphmdpvi.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2mgtbjshs.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2gmsiohnn.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2zcbnvioc.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2qpjamoxj.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2wvxyxnyb.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2zcxlwufu.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2awrbzhri.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2kmojcaii.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2sjmxrenj.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2jzbqynqm.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2ytlmabgz.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2nguwidcz.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2qpmdgxre.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2oyhfnvsi.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2zvyvfncv.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2iikwgyhu.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2fnlivcpd.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2wuydvmhh.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2hbeoprdw.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2oryyiczm.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2jmssjwpe.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2ndsnzhpk.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2vupyndzy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eosfypie.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2gvisvtsb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jusyalzy.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2gjnxhqzs.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2yubtvuua.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2vtnyyxwe.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2zzecxkzv.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2lqcucags.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2zoosyfdj.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2dqynnhzt.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2gnzvpzki.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2jhwzovfh.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2ghhzbzku.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2xtzqdanp.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2vaarzuvr.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2gvkqwrle.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2gxtnmjkf.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2pveggkoz.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2qojubdtw.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2ekdpxuvf.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2sidfxsxd.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2rnqzlajx.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2rxovyioy.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2pzowcyro.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ahmbauxa.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2wtyiithv.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2nihwyncx.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2wtuqzmfv.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2bebghfzc.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2odvpgdui.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2vapmxpsi.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2qrhkxhkj.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2zgqninsr.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2fcaqchnp.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2tyrttqms.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2pzayfffj.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2eabpmell.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2qfeysakl.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2henzkoeg.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2ewmlsyrr.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2allhmqug.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2kudtepgk.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2kvxkxogp.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2rumuwrga.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2lalpdmru.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2wvoxctfq.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2nmhhghqm.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2vtjgxhho.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2twxaxpbr.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2pobexlqv.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2crrdqtav.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2zmpwjkwr.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2pvcdijji.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2fodaqogs.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2cclnwivv.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2cykzwtco.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2fzuplpev.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2pwvhreks.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2ptyhgmpo.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2ncycctiw.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2ecxpkulr.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2gxwomzjv.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2pehwrecw.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2fdrolluw.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2gvwnbawr.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2betdwfsg.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2hglhhkwm.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2cxoibrde.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2rqnqtydu.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2ryajmjml.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2jvvgyngw.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2sapzjvll.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2bampogzg.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2krzxezoz.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2wodiylsn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qaggffbh.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2rjgvpjto.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qjvhhluk.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2oworogxr.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2dpjisodt.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2vxzckjct.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2aeijibxo.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2qaccbdbu.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2azyrwcip.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2oyuhhunt.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2ctgpukev.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2jxozeoly.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2yciwgjoq.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2hrxwqdbj.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2fikyoooo.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2uhqxmaor.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2vujkqwkc.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2ghimqqfq.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zakdzmau.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2gmqeezze.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2oxrugdfn.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2bjqrzieb.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2ykphcruh.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2lubyhazz.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2amfsrrzg.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2vlazypsb.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2firktxjm.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2fbpldjij.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2bpfkjxyf.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2cjnjtyrv.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2bkprnssv.html


<!-- 参考信息 -->