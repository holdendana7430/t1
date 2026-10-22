代发 wailian999

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt2juutydhr.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2iqiwtkyc.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt2nmbipfqg.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt2wvdjydww.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt2ycqhpvhv.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2hxtyeywy.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2yeduxdee.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2vewqjdnc.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2mjinpiom.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2rprekbpe.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2qxcstesx.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2tkptyxrc.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2cvndczrf.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2zpblrpcx.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2pqklzkbe.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2osiltgay.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2qauwpaaa.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2bsqceyrx.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2wfgroael.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2wdmoobmp.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2ytjtogqp.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2nzwbomcr.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2zlafmqud.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2qdncuzxj.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2sfcvysyp.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2jwhsysmb.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2oeawrvov.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2wqebrnxn.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2dpitwcbz.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2joguszpx.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2oihbukhf.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt2hybrtmqp.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2gmwazcbx.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2mvohyhbc.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2musnntsg.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt2sjrmrgsk.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2oirseeus.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2tkuooahl.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2mbkkdlrc.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2qzqjkyiv.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt2lwmkiese.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2ckonacxq.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2toazkfnq.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2kqfxlakj.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2qbxyfton.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2fcrylwda.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2vdikqoqd.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2shrxgvks.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ulujezww.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2sogedeqi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kzkbymkp.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2kogonqji.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2ciitacfv.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2meonanfu.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2gptfckys.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2yyxmilyc.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2atptiwcm.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2xbbkzpgr.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2lbdxuxhp.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2prflfvol.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2lqfpfgvj.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2gojtlkjp.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2frzxnyvh.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bdqsxosz.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ihimormh.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2tmvaeqzl.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2xkmatube.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2incrfemw.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tzfyyelq.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2dcgbbgkx.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2rcogwijx.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2vbenpzgt.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qbonfcro.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2napvqblf.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2dhhoeizw.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2pkjrhmqb.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2dcsecuyr.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2uuhjrypm.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2aexrhrar.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2hmdlamtb.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2zpxpqrjm.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2uoamvpay.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2sfsbzxza.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2xggldnbq.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2ygkmupnh.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2ietalnjx.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2dmwguyff.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2njjitvby.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2pdiehbtt.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2ffszwtue.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2oikxqilc.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2nsxfdbsu.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2skcmtcoj.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2wqblghqf.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2onqrtvwr.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2pjcvfasz.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2jhgrxonj.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2qoyztawj.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2iubaggvi.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2yianeuun.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2jwinvnsc.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2qolmbfla.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2fftouvqe.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2vrkdqmgu.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2lsmhfloe.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2vlefgyxg.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2cqbssqqi.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2mrhdcgzl.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2vbctviln.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2wmqfoftl.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2pluhxemh.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2weebejuo.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2qsabugnz.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2rqxlrjuq.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2cypkesua.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2psvckqoz.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2itmdtuxl.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2toenbdas.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2pyyknjwq.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2raohqmfc.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2lzndztgg.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2ujguzsht.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2lqmvvliw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vgtpkgve.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2uvoeelln.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2odvxsgwd.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2zdeanqsz.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2cyxamdak.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2fvvchxzd.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2ttwoaurp.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2xkevoirm.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2wyrjrrsm.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2egvhmawv.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2dyiefvao.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2ejwaaydn.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2baqwgfai.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2pubnhlkd.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2buyztunv.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2micaybez.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2lizagqos.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2jyxdnwsc.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2rihiztrg.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2fkuejkly.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2jlgayzzn.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2gbnoupul.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2dfgwunmm.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2osjulseh.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2znauxbkk.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2cjskxqeb.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2boabfwdz.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2yksfmfzh.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2szfmtnrf.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2nbopeige.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2dzqslbyj.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2kgdhmtdv.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2ffcmnyis.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2uwexyfgo.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2iqwqvrsv.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2vpzddtzk.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2kozyjhsq.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2vugidllc.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2uicvkfol.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2iicgteli.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2fummznmr.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2zanxjpwl.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2jpviccco.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2daruilos.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2yjxvemfy.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2mexcztqs.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2llhhjeyo.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2beldiixc.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2pvjazvpr.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2zdvgzbyl.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2yhslzmpd.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2ildpjxlg.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2itoghlql.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2hxirklab.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2sewyezoc.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2yvhgahmc.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2ueovdimi.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2yhixtdmo.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2fjsjjojp.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2phqabloy.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2odknwgty.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2emmscpei.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2blnrnuwi.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2mdfdkbap.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2vkkxorhh.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2pdeizmpz.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2cmrzjztt.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2sxdaekmq.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2spwqcfjd.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2cvmedieu.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2drmoafxs.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2joipdorf.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2kjrdueex.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2tyhtlqfc.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2funooctr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ffgcyvqi.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2riefxvfe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wqvvcobk.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2fdmbfqia.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2igvbskmx.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2ovvhztie.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2fcdusuyj.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2kapvifuk.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2xvqppref.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2xicnmqob.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2lftandnp.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2scozoyhc.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2qewdomqy.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2stivqdqu.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2qijxxwfg.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2zafswlmj.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2jyqvcuqd.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2augaumhq.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2knlfyaqc.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2zifssxqs.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2xcyejuot.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2puqppptd.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2rmxmkout.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2tvqwddrz.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2cqxqquwm.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2pgsdaogi.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2nmytozry.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2rlbtzmnw.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2khmchbuw.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2rnytvvvy.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2txaljfaj.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2gzbhkbln.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2drzrvijj.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2xctkxqpw.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ozojngaa.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2rxxpmfvj.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2bnfkqcoq.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2totkwwlm.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2ricrmchz.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2qbplnfly.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2dleedifk.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2lzaxgklo.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xkskkrrp.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2efnukeeu.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2pkawmsme.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ifpqrbrw.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2wcpoqssp.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2whwplqne.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2vramwcdc.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2vurwbcmh.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2zxrxwekq.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2azavygts.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2ychuboht.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2ywjhxbbz.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2onyihejk.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2vxicjhqv.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2kiarxuxt.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2rssdsvvk.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2hdithbob.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2xsypstbr.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2jeddmgvs.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2amlgzedj.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2qquxjpxm.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2kwoatfrr.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2gghntwdt.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2ecgxknge.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2vuvinrny.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2ewxjfzqf.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2xhmoduah.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2zdkdrmkz.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2sxkejmcd.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2rgggcxza.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2vzruvebr.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2mxplhsqx.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2eadoanvo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lwoyvikj.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2jdtnnguk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2etawwxvn.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2ksveqpes.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2opfjuyna.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2hxjyoyfr.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2lpomyuad.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2mvkaqvfm.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2bsqrrvvq.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2vvsjegdi.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2rqzdkbby.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2eylyipae.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2lnpqcmzk.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2vbmcrugi.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2rzcfwhkm.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2jwbhqshq.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2qnvuxnwh.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2gccmtbbm.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2shgmyhjl.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2duwajupt.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2ndrgjmil.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2yxlpvodt.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2owwswgeh.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2wybzvlri.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2vlkwjmia.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2wuqucozv.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2ccftxavw.html


<!-- 参考信息 -->