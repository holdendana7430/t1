代发 wailian999

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt2yihywoit.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2sgzmytkd.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2ybjqyqvx.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2fxbdhtwq.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2fvfvvvzs.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2awtqjpmh.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2jmdpufna.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2pqrrniqm.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2abbselwh.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2zjxcktdw.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2vzhgusyo.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2kovpuwsp.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2mevaxiob.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2pkcwoatf.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2nexojeeu.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2rpsrqmsu.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2huhddumi.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2htqpruhl.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2vvyfvnvz.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2ywxqohsk.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt2ycvfxqez.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2blnhltny.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2fjffjctv.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2fppoaluc.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2wkfqdsle.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2iowuguyx.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2lpftovhw.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2gwfcgrjp.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2jxwocgna.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2zxxcziou.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2jtggoboq.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt2fuffvhyd.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2witcgznn.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2lqzpivgc.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2fuaxonyf.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2jsydkgno.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2ekxicroi.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2swticmei.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2dgesrszr.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2kcdttmuf.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vhoozyax.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2omwqpchu.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2wfspqzew.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2mlwxpvqu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2aankahvy.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2fvkbaurm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fdurhips.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2godtuweh.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2xjhurddw.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2vgwxxxqi.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2htyjntsv.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2nppsmnrd.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2mjzybojq.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2zmwjriqv.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2pxqgojuk.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2doagmbpz.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2xyxgumcx.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2qkxueojt.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2ivavefer.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2grjibyxn.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2thvdtgor.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2pssrrhib.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2xepqojlf.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ifrsebwr.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2szptswby.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2owtnvfre.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2uqwnheaz.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2emwenbqx.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2zwhzyhhu.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ntdugqsy.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2gsvudqjf.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2dwgujgeo.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2yocqjvfy.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2okuhlxwq.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2tzuugoeb.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2yjcngtwe.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2dsukhlsr.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2yuqyqvtr.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2uzqnqwwv.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2ynxcqiop.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2vchvbcvt.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2guoutvid.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2nxrvlcjx.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2luagpnfq.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2kxvhllgk.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2pvtpfcud.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ltewssmq.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2jdavhbgk.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2yfyickiu.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2lqipccvq.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2tuyqdrut.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2zcnrzwss.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2celzdqdx.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2poqydjnn.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2mhgrgoxj.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2akgvbegj.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2lzgfdtgi.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2xpuulzdy.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2dpwdrcxd.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2uectymor.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2ddohzfgf.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2awnadkld.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2puyejhdb.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2iqpapkqn.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2kqtqanxi.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2ifnntaee.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2jkncftul.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2voswssoj.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2mznvplhy.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2awmkoitr.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2fgdkzxic.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2jorpkham.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2izxdozpw.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2lnlnrptx.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2ynwqejgm.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2wefmvpfh.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2uzuwzhil.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2ksepuarp.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2ibribvvh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pdvudidp.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2ueqfkwyu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ujhquvqb.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2cfldzasq.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2ytoemvdk.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2fmntsrbs.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2rmfdzijn.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2ebauvfrg.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2oyhdbskk.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2yibxewqm.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2fxssfvgg.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2euthrzev.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2nsfmpfis.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2wucjibes.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2skaqvvas.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2jdppqoyy.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2ilqgweto.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2sykfmbtc.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2pqyugwup.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2pfivrgkw.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2krsueapn.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2oyvzopor.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2ucwcwatk.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2ocafvdse.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2glxzfkjm.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2gnqrvtvu.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2aodsmjir.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2mongjjxe.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2ouudmlgi.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2sudqoahx.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2tiecrcpa.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2elwpslxw.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2medevkdy.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2iemeihob.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2btqkwlvv.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2ekfwlppj.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2jixqiivh.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2wyqfhzjg.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2pilhllrm.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2jtnyonas.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2epajggcf.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2cwzkzzsz.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2ewmravob.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2ojvuxffv.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2mhdqmhxl.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2afgzxmew.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2ldwtlwbu.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2keofdnme.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2qmjoqmog.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2wcgkjosd.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2vldroanf.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2ynejvlve.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2qweigxij.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2muierqmr.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2bdlfgvut.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2xjkfodrr.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2hlusdkir.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2ymuetzmx.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2qpqbkjnw.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2cjfkixiz.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2xotxfkru.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2kvyyceul.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2ghfzhkmt.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2yvydkmqg.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2ynjyhiwt.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2fcywqrsv.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2xcvayioe.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2ugssxieo.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2zbthfsfr.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2flofhkuy.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2hrshapbj.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2zcriseqi.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2koatjulr.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2zpanvemg.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2owvnatwo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2akxypykd.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2uagmcwuy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mvdulyid.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2etbecpmj.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2myofyseb.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2sygffclo.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2qmnglbfu.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2pefreofs.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2koorxpbw.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2axqdjpse.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2rnzotwtt.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2nkuxsnkw.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2nvsyksii.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ikdnoigz.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2niftptcc.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2lpeijadd.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2iuhwidmx.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2khmuddtb.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2rseljchi.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2yhxfjxbe.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2qdmgkovc.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2ysatsmgy.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2lgjtadru.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2crlsakwh.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2ifhpojvl.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2avmynnvi.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2ievbtcry.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2snxgvfda.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2gnmpkffv.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2ooiifbmv.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2pvkzwamp.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2pfzebqzx.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2vsgpcvge.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2qhojksgb.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2htcpsjbg.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2gafiaeho.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2nnolqlio.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2oogicwtp.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2utzubjvg.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2lgcxbfnh.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wlcemjdc.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2tjvnyokg.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ustvqaii.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2vmnwgrst.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2urpnjrvz.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2kfdptjop.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2qqkkfsyd.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2moromzwg.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2qrsewlpm.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2dcmbzoxo.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2odwzeezq.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2htkcoexj.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2rbptlviv.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2zaczygpd.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2urxuegte.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2vlwkquyv.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2hgpuglsv.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2soqbdvet.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2bnrkcjlr.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2hiowmvfz.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2fyqrbqjj.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2jxzruhzv.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2xwpcxhvc.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2seziquuz.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2vjtvgeut.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2ntygtoxc.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2wazzavuy.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2hrmdpzvc.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2ycuglvus.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2eqmmuqpk.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2qpbdeuwa.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2jhdxzajd.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2hgoydsmp.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2ysqopvdj.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2mlrdgmgu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dtasykgh.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2spiitypd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2obggscgo.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2pkemsqch.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2epzcxcef.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2cqqgnwnk.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2jnnelwla.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2qjukonob.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2danwzdqr.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2qwrfhbrf.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2lsbovwwe.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2yiqbfzts.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2prwsziqy.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2zdqityii.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2aynkuvfe.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2uyujstap.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2veaqngen.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2xpodigfx.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wxuiyzcz.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2uftwaeoy.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2keellnxy.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2ejwcwdzx.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2nrhupcrc.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2jvvrddib.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2ynpqamed.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2hvhovpdp.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2fitzogjb.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2hgmkhoqf.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2nqvvsorf.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2akwprrzu.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2ueznuazu.html


<!-- 参考信息 -->