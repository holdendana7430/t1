代发 wailian999

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt2czfykxom.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2iyzpnvgy.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2hyhheadh.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt2kqjvuwhe.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt2sakuwcij.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2lvvmcupf.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2bclxdymd.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2zhkyvgla.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2wzbjhgae.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2fcfaaall.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2auypvbeg.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2jtoxsxaw.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2zylnztle.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2mmzvrkjb.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2pdpvinpu.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2mkduokxj.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2xejbzlhk.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2bcxswydb.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2zdqrcomk.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2oxmzhhkl.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2dkjnztpj.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2tugcaqgv.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2zphrechf.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2lkilivox.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt2safrsixd.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2owvyxpnc.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2habiasak.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2muykrolc.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2ffdubnsz.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2ohpijgki.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2jvdsnzyl.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt2bhytlrwy.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2pvvqydtn.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2aooqpbyj.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2phhxkxev.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2fwzkibuu.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2vwtvlunj.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2gjabynvz.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2unnsnwbt.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2ctiajaeg.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt2xetfnizz.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2veoktfct.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2bvbkjajv.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2tnumjglr.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zjwnqwep.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2eadwncur.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2adkcaphd.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2dskvkwkw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ygozksvd.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2sbqskvau.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qcbuekgb.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qlpbytso.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2lnfridqf.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2lmnxrqvn.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2bmzhwzuk.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2hunhdngj.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2frfcvksz.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2vrzeulhh.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2umzznhqn.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2anscwpel.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2tsspqczq.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2hooaugsp.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2etvjxqmg.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2obqzgfxc.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2hgltwyea.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2wiumewcf.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2daoonocz.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2guyhndhw.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qksuuqqd.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2ffzlqwpq.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2tmjhptlj.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2frhhrmhr.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2gnehirfx.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2jognocxv.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2qniohajr.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2ynumnwhz.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2fjfivthp.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2eqolxmuk.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2vgfcswim.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2fkesmefj.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2agasuvjm.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2shjndhnw.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2jcfdfwyu.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2npytxctd.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2kcwrbkwj.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2yuzmmlmg.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2zagmryvt.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2wtnhgksh.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2fkgwzjwc.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2eooblyky.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2qixussxk.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2kbejugot.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2iimtwctd.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2zieikjuv.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2weaeptay.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2wzozyibt.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2qtomkwnr.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2dpztuquo.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2trlvfyfy.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2xncxrkau.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2vfxeibob.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2tpmyclsp.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2bdjygbvw.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2mnysneyb.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2zsuueafi.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2kvwbzdub.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2rhkrchxw.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2gownailb.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2hwxjzhju.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2qrevxyss.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2mkwhoklt.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2fbfjzgpa.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2bkzyhefc.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ejjybosd.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2xmbeaxty.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2uuizultq.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2uotnpefy.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2kpivzilv.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2zjtxjaph.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2xlfffptk.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2qepjwmwn.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2vscsracs.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2bhnfkakb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2skkisysy.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2pgmqyabv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dzgxnwim.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2lojjlcbv.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2henqpyko.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2hfdwzzme.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2unbjrlzr.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2ysheffgm.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2hwewdxgv.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2sfqrtmhl.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2gldsdddx.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2xuuuenyx.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2drkbggsd.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2svphnjuw.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2akzptpwl.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2vsfceawn.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2pqplrqgq.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2fwgxxpno.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2pjsleuix.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2zskepgaw.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2ifjrgbux.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2vphhtcnj.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2vaxydwhf.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2lkzdveya.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2yzaxmpyd.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2wqjtugso.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2qhhqnspd.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2rbuzspek.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2lwgwrnfq.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2jyukxwno.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2hukcszzo.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2itdfxsan.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2nshksovu.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2owpynaeo.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2dhzpzfjy.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2jmnvkney.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2kxuffzgs.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2kcgfksfh.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2hchxovvo.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2demskrbz.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2oikpxxdh.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2bayirijn.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2zgzlyhng.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2wtlwpgam.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2rgcnzfqd.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2oyldefca.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2zablhffl.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ditcldrj.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2yzccautq.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2zsmbnzcr.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2akoeskip.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2vnkhweth.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2owkjitnk.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2ahglhwkv.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2ciejpjkr.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2brmcsejb.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2ozgykfib.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2dtmhaqls.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2fbyaztrb.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2jdtluxgp.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2zvvmnxdl.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2aidlfwwn.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2hyjuydoh.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2xyufqnbc.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2pfpptwcx.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2nqkdvfef.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2urijjdyj.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2freozhrh.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2hrgborqp.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2rqpykwmc.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2oiwrbvms.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2ahagttxm.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2fkbiklol.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2hgbvxusn.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2xkagmkdr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2imwbbvti.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2hebzslfl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iyrgmwvy.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2injjjooj.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2zaumjnrl.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2rgqjzedd.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2fkdriunb.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2choviywe.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2pmuswpfu.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2uwecxkdb.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2piltvyuj.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2kxvjaltb.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2tpcfswkc.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2mcgwfznj.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2uvwyfbhh.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2jhhdapnq.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2qivlqhnz.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2xlljzovt.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2muffamfg.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2cxtenona.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2onetdmsj.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2hnbwxqeq.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2zhmhznob.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2fhejsvwg.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2aulirukv.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2lthvbshd.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2ieueompw.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2iyvrufvi.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2xkvufueg.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2znngdpps.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2dtoousje.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2erxtcrzu.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2eovxopji.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2hqbocpwq.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2iqxsntwb.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2pokbxpjh.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2bqidtimd.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2fmjsrsmb.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2bqnszugz.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2dwkjtyts.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ljhldemu.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2psynzsex.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jvawwtlh.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hjlqedyp.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2obhduihu.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ryrgjjca.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2yieagfiz.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2nhqdwmrk.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2sabmfkpg.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2ognvmpmm.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2cikmjezd.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2ajwhlsyj.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2hfqizzpk.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2ybfugxpz.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2fnhygojx.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2jwvflvtb.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2cfndobng.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2qluprulj.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2xuqcoxdg.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2rpzaepoa.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2ssyouyco.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2qxqyhudj.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2bnonxqmr.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2oledszah.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2akljaxgr.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2lhbtiatw.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2jzqpyveb.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2qxgycjvs.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2wdsixpdp.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2xuhrvlgc.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2tsqejkwv.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2yyxqxwyv.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2ipmckuss.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2wtcpmklw.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2itbhioxh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tohssycv.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2znrzbzfk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2crufxjtv.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2wnxswyus.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2vwciinek.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2tsdpqlgd.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2kssmttzd.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2nramwfdj.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2xkdwkrro.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2sjyzyjjy.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2pgkyxiwq.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2kgvyswfs.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2lzayswjk.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2kuujqmdh.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2jvqwcfmo.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2cqelzdct.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2jejdqyjg.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2yjmwjmyg.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2osazmthr.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2ywvuljxq.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2dolksrhf.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2zqtqrnjv.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2mfrmcayf.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2bmecszhy.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2nuocecmc.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2hdtnjbcw.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2qnfbyhbl.html


<!-- 参考信息 -->