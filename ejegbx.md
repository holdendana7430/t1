代发 wailian999

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2kcyzjlci.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2vkdldcmm.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2xahdxnmv.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2bawjwqtq.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2qrfsjalx.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2naxocago.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2khoqtqpa.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2lxumtxbi.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2adsyevjr.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2iogpjkcz.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2rvavbpbh.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2inrcfrlu.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt2zqsamdba.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2vlktekmf.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2flsqxudw.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2cwsgvtxd.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2huwbsnxy.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2itnxgyub.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2rkdvxdjx.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt2ybglzvvv.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2fdygpdbl.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2nnlweppn.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2wiajvxpc.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2zneiqwgi.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2pceylkvd.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2iqzwsrbu.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2icnfqrut.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2tznonnuj.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt2ctvtzlbh.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2zdhciezy.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2xbkldweh.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2oyhrnpeo.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hnmyjqgv.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2rdndbxda.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2rmpxysqd.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2nyffgkdb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ooixxjla.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2zvzhtvqn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gueczmdf.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2xqueuhis.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2ueccdcde.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2ochrqmts.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2wtqolfbn.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2sqajvrqo.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2nyaxoqad.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2tffbdnfu.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2evrcffuo.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2mexbdkel.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2ndxntxvq.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2pitutkdi.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2bzacjrnz.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2agycsqxs.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gnyjmkpz.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2wkzsmrrb.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2mkasfemp.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2ethlpyfn.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2gtxgvcyl.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2wlmynvgs.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2jcmyyqyc.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2ffdvaarn.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hdlyuaaw.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2bjnxauoc.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2qmpfjeqc.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2mascvacj.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2lbwdcgjg.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2xmhpiatq.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2isaokdtw.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2jxymsodt.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2uexxughz.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2rohfnweh.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2nbbhdkde.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2xucijrgn.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2mfdeaczv.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2fvluwbxj.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2melnyked.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2frwoiohk.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2jrzdwhbv.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2rwjfomjo.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2lwmltjao.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ypmbrnjm.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2zegviyua.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2iznckbuh.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2fgdyoxzy.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2gpdltrfa.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2rkiwkmhm.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2getcfbof.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2rgmxyqrg.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2hjzqrepa.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2taonihgw.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2umnqhsew.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2ibemyokz.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2fjricuot.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2lpqohzpj.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2geqnbowk.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2hgfoqpyk.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2mwgiimav.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2jsupoujf.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ogbkxssq.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2urgvsrya.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2wymkgblf.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2szzfznlb.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2zseuqhvy.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2jlbmcser.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2tluowyxx.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2uarzlztu.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2gvbibscz.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2osphxyks.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2juqyjmid.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2aotgvimb.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2hfznghdt.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2xrbmkabi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2flwubzjb.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2yvvjxbsh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ylpxczot.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2xabzmpwh.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2ikegkyni.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2mxoltkjm.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2jumuuzpl.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2trhmzjxm.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2vmnerjwg.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2eyhgtrsn.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2adfdxeui.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2afveuowj.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2mtedmcqv.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2dlztoqym.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2vrqedcgl.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2hfkfyvom.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2pgduxdqq.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2mxkoukjq.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2dsdkrvwa.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2ahbmhpzv.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2uzxhilrt.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2rpjdgqix.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2ctwzhyyw.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2fjnjyhih.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2jzdjndlx.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2toojleid.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2fmdgdazk.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2aazkbrtt.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2yrnrdrqo.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2ansavjak.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2vypxwyee.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2vopkxicr.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2oglyextc.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2slanoaor.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2fwmvoata.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2aubzwuig.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2vxnxchcj.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2hbnhswfq.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2fnidfgbk.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2yuxriogv.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2xjvyqxmx.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2pmzjqnpt.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2rxwatdxw.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2wkiyahbs.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2mbgdgznc.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2xhfcipsa.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2plboaqok.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2gkycpxxh.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2bldregtx.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2nlamfvbu.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2tvxyxdui.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2ponmtxmc.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2usrmdfho.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2slktcmtv.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2uiiyrqwt.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2qnukyehn.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2perqxmyo.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2mzzmtjon.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2azacmerr.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2gzwgdcul.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2wrrwstus.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2umzvpawo.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2chwhsnaf.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2cofpvbxo.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2mbtavaho.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2czqvciqx.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2krpqegso.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2qifgcchn.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2bnfkovjt.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2oepyfawr.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2hsqjfmnt.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2zvrtalgs.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2voedetrr.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2cnqejxet.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2npqpbrwt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mannfoqg.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2rtyrsxmp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2msflzkso.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2yhtveseg.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2eeploaxo.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2ijcaqrle.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2oanbydic.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2sxbawkzv.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2udqgwdrq.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2qpomrzsp.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2pfbcubbp.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2tawxtwzm.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2dfibbqor.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2evnsboau.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2mdlhmtjb.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2jzjzjbnt.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2ybiidbjx.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2qmgssizr.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2mzaywodp.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2mioqzglw.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2zcqlgbop.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2zkyzgtiy.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2aozjcnhi.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2gbfihrmd.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ownhchzf.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2pacghojn.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2zvtjrxeo.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2ruxrccdc.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2zlqjmmbh.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2jyicqpcj.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2tfledagt.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2logeqrtd.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2yawqexxg.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2tlobhubs.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2mnhywkjz.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2mopmbdrh.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2kiqopcsb.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2bxqngard.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2ymdmrcms.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2djdglloe.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hgclqcbe.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2qdvlielo.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ycnprrry.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2aynbnkuv.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2qysgdieh.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2gnwxwsko.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2pfqtzbqk.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2jffwrzzt.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2udorxtkn.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2ncwkzdub.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2ostrfkwn.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2tzgmbhko.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2kmooypzh.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2wqrjcidl.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2nmtwglkw.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2yncfzsds.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2hvsjafbd.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2rbmzrivq.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2pbakaxel.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2hpputpln.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2lficxizj.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2rwhozyfd.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2rxbjdcun.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2omyhjxih.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2omsoweob.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2psujzfnb.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2mvybmsdm.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2haojtphy.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2qszsvaiq.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2staidcmx.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2bkwihtru.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2cbrbzyqs.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2nvoelvyh.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2sachkxzs.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2dfpbujro.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pwlhehcl.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2qqcvelug.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tpfurunu.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2tcqmfwcc.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2byegqezc.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2btgyqlfe.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2jhvemcpq.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2nxpabitt.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2gxucrror.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2aprkpkka.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2oujmztba.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2mvxbkxnt.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2klwedamv.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2ojhrrwfn.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2ndxvkksz.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2zzoszocd.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2yrcknkcz.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2dswgrxsl.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ssarodkv.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2djdupqgf.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2uagbymdx.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2aznfgcaf.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2xyddchri.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2xegyrvly.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2kraeqqax.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2gmznkkno.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2eikjdmgy.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2fbhdufnr.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2sgiihatq.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2ivjvchyu.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2mopuqtrl.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2opqyrnfr.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2pwpgsgxe.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2duffedyi.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2tnfugqac.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2bpiyiksz.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2jdoliihl.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2luexmhqz.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2qtjhhpef.html


<!-- 参考信息 -->