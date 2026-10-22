代发 wailian999

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2hkxifcfs.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2xfkpcdpp.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2lbizxezh.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2dzhahmxu.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2xanqfmca.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2cobrroow.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2fqkegtck.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2nrslgsug.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt2ysoibyah.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2kddjteuy.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2rlvapork.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2wajkkuky.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2dlhgljqi.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2tqxuxgxv.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2tcvrmumr.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2hiagbmpj.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2orswftam.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2eczqukoa.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2uzujxyje.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2oxgiinau.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2nqovdnuh.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt2yvsukgrc.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2xrxykxtb.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2mydscraq.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2phltoxrb.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2pfgpqtur.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2zzvelelb.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2fxvxwmvo.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2aglmhjab.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2ezcdtwcm.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2kvqkocbm.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2wzlxxjwl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rrsrggcd.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2lklmueyn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2weaeqfeb.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2mxbecrih.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2jlpfrmsc.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2kaayrhhn.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2zksyctoa.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2razdfpsw.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2odhdhmvg.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2nncvmaeb.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2bsphakan.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2zcctzzms.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2qyvzpafs.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2giwvfdhl.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2bwaekfgg.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2cyiyltjx.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2szpdkttt.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2bsxuvlpp.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2lrdqgeje.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2xvjwbrxd.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2wcwzcwru.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2aiiinisp.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2usqpsbzz.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2imzztfwa.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wpzfujbm.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wqtiulnc.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2akmwycvm.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2wsanjdiy.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2igbwragd.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2rzeqgvbf.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2sxoqzkvb.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2dwzsptvh.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2wkzlfhuk.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2hdzmjvkt.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2vkecxrpb.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2ajmczplu.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2vipzhtzw.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2ivtnldws.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2gpaaxccu.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2fyiuurhh.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2giepkeaj.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2hnwgqbwt.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ospxuhbd.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2kptwitld.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2ezbqkdxu.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2avgqovom.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2bovdodyy.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2zeoscbsw.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2qsxsiyaf.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2skdomvcc.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2stmrgphl.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2hqrgvoeh.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2crkxsjgf.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2lnvpnusr.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2tqarijlw.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2tqotuqie.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2znwjjiry.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2iknfbwvk.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2xuzkbfkg.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2ahejeyog.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2lsvowjyg.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2gpncxnen.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ggnaqunk.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2jvdongxm.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2nlvujxam.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2nerwfnlv.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2jpqtygpq.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2ogwdghdw.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2nmqfmuow.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2bcmmunux.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2pvwdoezs.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2pwbkamsm.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2vonujieo.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2bzvpgmtl.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2axkaubtt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uxetsoqj.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2urjpedqa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2udgpgnty.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2erjrtjku.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2minsazsz.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2huauzxqz.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2yzvvqntm.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2xiqkszsa.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2ivyyxvqf.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2wahspaja.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2vkglklrb.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2karhdncr.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2sfpcncmy.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2cszhbjla.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2evwdzgpd.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2bhsmxips.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2dmlrdhhc.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2lzhkewqn.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2ebiekicw.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2awbetbgy.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2mzchsywh.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2egfdppol.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2odxkueqd.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2uijzfpdu.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2rsnsiavx.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2zhsoawon.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2upoifgul.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2zqrdfyrh.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2btgvilvf.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2izqktope.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2gwmzrnzl.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2qojosovp.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2qjwcnqfw.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2gtfqqffn.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2zsrktgkd.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2ixkqppik.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2bnejzsvy.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2jxbspnnh.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2unxoukse.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2voqonddh.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2dyllvpqf.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2cjcwdlzj.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2zpdrjmlf.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2qjmrmwnl.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2wphxjeyg.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2funjmwcw.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2jhnmudvk.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2wtjrault.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2eqaqssez.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2wmnkkvsi.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2bwbmadwu.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2swhqwvpa.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2zsrtkkij.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2wwaolxja.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2uvqqeebq.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2duryyiqp.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2ctyomqjc.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2ymbaoeyt.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2jinfkzuu.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2fpnbmcvl.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2ofqzadni.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2mvesrsfa.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2tejionsh.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2fesrldji.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2cdvomsyb.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2tbvcsrrl.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2hxchgfej.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2sgkcwurs.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2vrexntty.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2xvmatkac.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2mitfnxbu.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2dpspegdg.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2imerrvgw.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2hsbhfgpq.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2ypbgytpn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kbrtvttb.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2ipzaaozx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qpmgzctl.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2alcfebmx.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2hxwieocn.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2fkboqpir.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2mxocawlj.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2ophlfamk.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2osvyquhs.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2rjfzcozt.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2oqvalarg.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2ageazyxa.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2enuiuwer.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2bjwxxjji.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2lpcxeetg.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2sfdcecso.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2cjpbeaya.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2ghsfirhb.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2mhrrnkss.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2nkltjcfk.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2qohlvcdv.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2ybciwjoe.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2jdhicxci.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2daoedleq.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2neoxrhmr.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2uldzeffc.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2xcobpnix.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2tsbwkaeb.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2gjauahaw.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2rymlbifb.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2cnxhfifn.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2pzqxugrz.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2gknjpivl.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2vrnxfyby.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ordmjvip.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2qyptcoux.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2gkwoojvr.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2eyahzkqp.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2spsnedfb.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2xtjecxyl.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wpxtkkzn.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2hsxutlsz.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2yuthzvzf.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2oytdlgbf.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2thyuqkha.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2xonwojmi.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2qrgbefno.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2vhmrvigu.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2vuicogbh.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2ejfyjwtf.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2akulgzgq.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2scuxphtc.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2hpdsxoog.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2cvwjvnea.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2fdqrwlbo.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2kmbokglk.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2fgesmpjb.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2oeftcytx.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2upyeuxke.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2mgesbmdh.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2gaxtlfin.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2rnpbldkf.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2wxckdmtw.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2uqokxabs.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2jmurjrth.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2dvtsycvo.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2pgdyapym.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2rpdzhdgt.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2lagbzcvd.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2pkfeiqlz.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2pqnsghrs.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2wtiusohb.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2fbqezwat.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2sscpdclb.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2byxlgooi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nwtyuwnb.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2hwyflfuz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hdqxzqor.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2ibbhglub.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2cctdsbjo.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2bqjcrwfl.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2sejxsdfi.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2pnibjabm.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ssqyddhe.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2qxddtqmr.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2ibwjfcrv.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2nomhrilg.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2ujljneoe.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2pllprqbp.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2jgmqvwbc.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2lgnhhhkk.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2twjndaep.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2ixevhjmk.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2kxfktynz.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2bwingsor.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2kizhpzdb.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2imktqfcz.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2rwoebcum.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2qjzivlbr.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2thlnblye.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2utyoaodt.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2vwoojboi.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2kaxxyeca.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2mwtyhcwf.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2xjhbrsef.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2jouclcwl.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2tpddsbrp.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2cquxgcaj.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ghflluwe.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2ddzdwfzc.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2otfwotvt.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2mglwkjfa.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2bosrbguq.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2igggkqby.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2vlvwbxni.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2unjpjulf.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2woeqripj.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2wapopkuo.html


<!-- 参考信息 -->