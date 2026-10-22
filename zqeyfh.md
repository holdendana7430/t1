代发 wailian999

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2oipdthwe.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2kckrkplg.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2qjxpryll.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2rmhadyjt.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2oyqpyspw.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2gsyhezkz.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2jbehlsqp.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2mxofdtdy.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2rrkwhrci.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2yofktoyf.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2vdlmswnn.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2hfrcffkt.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2hranlqte.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2ofmzdsrr.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2bebuiztg.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2xrkxnlip.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2zedigxst.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2kdzkbtwv.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2gbsvseiv.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2tpntvvsm.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt2ybflqrxw.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2fblbibof.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2xjkxmfyn.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2uvlbwnwj.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2pmdtqtwz.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2ldaoyoaq.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2upjyxenw.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2mvrvtmux.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2xeibhoqk.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2czezbyfc.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2ohlzybdu.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2fzrlkvnu.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2hzciyraf.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt2iitqervd.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2dcpeirnk.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2frrvtvwt.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2yxufmybg.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2judekeko.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2hjbqxydi.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ibfiucyy.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2pdrtydkk.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2xaagklgm.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2gjyaqfxd.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2wbryegvw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ixmbwuet.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2ulptwhwf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2aseezblq.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2awglunzx.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2pjzvcplu.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2nwhtyopw.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2kofnmhjo.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2nvohgjqk.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2qvlefclv.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2ihiarzys.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2cechwvww.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2axyotwuv.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2admmggvr.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2zhutrxzm.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2ffhprbkq.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ewwjpsap.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2lxcvyfpt.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2uzkzglmu.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2iikqigpp.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bgxuptnf.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wslbhgcv.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2nniiwpnw.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2wujgffbx.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2qxjwoezv.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2roupxvrx.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2bvbzclwq.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2gxzceuqc.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2wfjxiuua.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2zogcscem.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2bbhppdgf.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2lebbqbyw.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2rtqxddiu.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2pzzufeap.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2aebezlzn.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2jwrgvmjc.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2mtrqzegx.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2qtcyscfb.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2xbhxnuns.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2rhmyyrlk.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2ztlrwjha.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2qdnjilkv.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2uvpqmpwm.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2htcfsbce.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2uwyocfun.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2odtjcqzl.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2kgwlxrst.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2isipzzkj.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2xtknsnsg.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2awkdcskn.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2dvjarihn.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2hmrtqmos.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2mzvhtfjm.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2rsszzcmc.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2rzyylomb.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2bfnbdpga.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2eitufvtj.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2tarekhie.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2fygtyicl.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2zrweqsbk.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2nrwzqvhp.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2khbrpvzt.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2xxmarzcb.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2bgojvguf.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2hsxzbwuf.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2mdhgjuiv.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2ohczzyvu.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2fzxtgudm.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2orlodeba.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2trxmerud.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2tdqzriyi.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2rqjxyuml.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2fsozvlhn.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2smtatypb.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2caxdilwq.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2cxgwlajy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zrxzunia.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2deumjwwi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zcehbcjb.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2dnwyzlxe.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2ozgjiicx.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2sdqzlxpb.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2mwjuzjar.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2xiiubxlz.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2ibyfgoby.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2uqvilben.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2dmrkcdhf.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2gvwimkee.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2xjvtqzpc.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2ypwwrdxl.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2kpwiqrbl.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2yuznkabu.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2wijvgytm.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2yldadjpb.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2dkxenbna.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2doztasba.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2kwfjbibz.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2zwjaymbr.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2dxrsstgz.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2fodmxkpf.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2weoyadmj.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2niqunpud.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2lshowndj.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2jvdjacjs.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2xbgtgxxc.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2tyhlelqh.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2hfssvjvm.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2eebhvuzo.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2dabprfkn.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2agtuevrn.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2zxzeslvm.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2pobfqqps.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2slefidey.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2gpvzfieu.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2hcahubwd.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2qsfmkwvp.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2ymewyygf.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2wuagxxoi.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2bompagit.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2edsjekcm.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2tvxfcjdw.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2mtnjcosh.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2fshhalri.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2czvjnrtd.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2wppmrwil.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2wsemtdbo.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2oprcegtm.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2mgtwhwou.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2vbptevzv.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2ercnxrsi.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2piwcbbzb.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2dypohugg.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2jylgvaef.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2yftsrslq.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2xzgrftph.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2ajalyvbr.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2vovplcgx.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2eddnaxdy.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2oblgtffc.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2vgmdydtm.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2duhaemjc.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2wytwfvln.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2btwkbwuq.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2kuknoqul.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2uvhnoxaz.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2yizgfycb.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2somqfwfc.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2vtjckjbw.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2fmroyfhs.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2bqbnuluv.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2ombmwevn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2phfsrlnm.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2hszdzfcb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2apgkpuxc.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2deuuctxz.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2acuhmovu.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2neottalw.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2fatjinsa.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2dbgfupiu.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2jwuekwiq.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2bjsgmfcj.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2euxojaia.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2amnmzjqy.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2tkuxciaa.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2agmqwbri.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2sikjiome.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2hoaaugmd.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2zcyrfgsk.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2tmnmputh.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2hpqsiifx.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2xkosftuc.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2rapybqai.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2ondaoimq.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2mxoabxso.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2tcttjrpr.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2uuelghav.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2uyudqmbt.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2yuxbvgoc.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2foqnjapf.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2lzfqsnxm.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2mocyxvya.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2rqsxaulm.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2bvqinemc.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2mkkqyvxr.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2kjurpxzh.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ggggnrsf.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2xqjzaglc.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2ohlbrveb.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2omyqvroy.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2fzpqaagc.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2zvkmpkrn.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2rnmrqpts.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2qsuxrjhd.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2skcnmcmu.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2umngbcnt.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pbgagndl.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2stdrihat.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2rbokewry.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2xbaxnhoi.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2ddridpzq.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2prycdspq.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2lsaoaoxm.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2qlrafywe.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2axofvyrx.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2roulitrl.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2gpehtnya.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2ezqhljna.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2uoiuvvzu.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2cvjqwgik.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2flhuyjjq.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2dludhnzf.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2ztxfawap.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2xswxujbm.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2dgswxezr.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2robpcehk.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2juysbukb.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2udyufbdn.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2bcjwxdcq.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2etsoafhs.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2mqvjkwdq.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2cganhabb.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2nvopxyus.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2butuhkzb.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2vcuflolj.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2ivekldde.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2nvfignmh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qyshhlkd.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2oblkqknt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cjzyzlec.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2eogrzokg.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2axgtqbdx.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2plnkfyvy.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2zizvjqsm.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2zuhtlujk.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2iicbxuel.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2hwrbkbet.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2zxpbuxho.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ncpvgjsd.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2ihaqrdid.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2kpddwzxu.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2jhebmify.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2gcweirem.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2amcbvalb.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2bypsolob.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2qthylggu.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2vhvtsqkf.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2fiajyakp.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2pbhnbsup.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2rmhpulqw.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2stuncrzh.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2npscukpc.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2fqcknfko.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2wmworazl.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2vwsjctlk.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2lydqevvq.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2maiftnme.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2ainpvhuo.html


<!-- 参考信息 -->