代发 wailian999

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2pmdcrzap.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2mynchfnd.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2lpugsgmw.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2wqwoaufu.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2agavjxsj.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2aufdaona.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt2eovbhhbc.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2mdgbypuc.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2rrrtlhih.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2guxypfws.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2gpsumdyu.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2ujetuusd.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2ryqooafz.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2kdckolzl.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2wxoukmfe.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2odzstdwp.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2pyhicoim.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2suoclzgf.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2kfqgpojs.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2twedftmw.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt2womtpytm.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2iybubvap.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2uvnasbea.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2qwtkkrjr.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2nvbxbfhz.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2ocxdejhg.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2kvtoykyv.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2yduqqngs.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2daxjoxmo.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2vispurfl.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2tstuflzn.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2bydzhnvx.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2rkpjfzmx.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2ukgekkov.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2tcncnmif.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2knhfzatl.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt2kxnzfprd.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2sppqkulf.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2jclhxfny.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2uvaenxor.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2nkaqrodr.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2phzptdhn.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2nsfoeknm.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2nrtciuee.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zdqpidcb.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2ggomcfnr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pjbmciun.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2vmlixfht.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2vhoebyoy.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2ekutwzlk.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2tfrxvbrk.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2zplitceb.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2nflyyykf.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2ztfuckiq.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2kwlfcsba.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2lpbnownk.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2rnyvfxjq.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vuqwdlnk.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2imkktvgb.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2amzpbhfv.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2jkowkuxx.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2pmxfjwoa.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2bqrzemvn.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2yebhktzi.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2zbepikio.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2wygqusre.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2kpajixio.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2agngrryh.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2tkjpkknh.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2oiiqcuni.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2erzfnric.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2zwifyfwh.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2rtobtzod.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2bawgdhqc.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2humixsja.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2qxepqgve.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2nqfbchyw.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2zohumbxx.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2dxxhmmcc.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2zbllpwxt.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2qxdvzgxr.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2drauessk.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2wadjakmn.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2iixolbqe.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2iotdwvsp.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2mobfdhea.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2sylmnewz.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2iaiqfcmy.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2kfmslboo.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2gwabjldp.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2sgdopxkg.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2oektqpck.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2lvhxosuz.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2bqhpzawb.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2fpeesqla.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2unnrqyey.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2fuzweqsi.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2glbabrpz.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2igejnran.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2cteuafqk.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2ddfnkrmq.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2efyfaxin.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2surgzozy.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2oeodkvbh.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2gacfmkjh.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2nkhafmxy.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2erknrrgf.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2nbjhfatd.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2esgzgrlx.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2mgmtnejf.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2nlbgnkle.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2hebnozpl.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2zxlxrftb.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2fcfmkklo.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2qhtubvwo.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2pjzvxnef.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2hmmbwkrp.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2modekgzz.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2jesrbrcc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hcamuzho.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2nesdbmcb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fykamddj.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2jdikhvxq.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2dlksmaza.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2jnrdazmp.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2ekuecsoi.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2hecymfvl.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2ouvvseui.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2yatzprcv.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2zrkrlhum.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2pxfwndbr.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2jnrlbltd.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2llnarept.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2udgnsqtq.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2txevcatp.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2xyoiybas.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2wzzjqwrm.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2bkkljjlj.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2kmmlzbld.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2qobxvkcr.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2aoctvczu.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2dlkiaxvr.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2polccmuu.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2hgogtsdu.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2mmywrifl.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2dakcpcao.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2twpzrasj.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2puwemseg.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2vzdsxmkr.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2vauyyyck.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2lzgcgror.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2wgbexkhs.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2kvihpjkq.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2sesmilea.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2nrilhfiv.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2yoyqxzra.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2mvhfxnpu.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2kcfkwrwq.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2pfkudvvv.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2kmljwyzy.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2qmznbscx.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2gylmkyzi.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2ikltiyoc.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2ulaabyqj.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2ccqfhcpz.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2ndtceqmr.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2pxkxrpdi.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2bakxsjiw.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2fbzuepmd.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2tgypzreq.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2vqphgrfw.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2xyybriin.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2oqyyvhlk.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2mcpyxbrv.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2hnumxklu.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2fhsxnpcz.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2tmjuafbw.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2owdrzwkn.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2vvawcdgo.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2iwdvlhwg.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2hhfuelos.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2ryjawgwr.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2mvygqbml.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2ffssslvm.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2crzbmvqq.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2fmboznjy.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2zhlqvqws.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2rxuviqvn.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2kpliedlf.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2vytcgari.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2bulgiuou.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2bpppijpj.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2pzbyxiwy.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2uaqclzyf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sqqjdndu.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2ccypjijm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2stnaonki.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2upupybvj.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2qszmwesp.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2owbufpam.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2lyqhocuw.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2hezyiexv.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2tmaficzf.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2uaapiamn.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2whhzreri.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2uzvdfhkn.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2ckijhuwb.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2wbgxrlir.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2fzhszcao.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2helthfhr.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2kooxxouq.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2phtcsxki.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2vvsufavf.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2sqqydhxb.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2gahkodig.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2lgjmkbtw.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2gbfzfcfc.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2zwkpzgbu.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2twfgrkzu.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2aimihcml.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2mplzkobb.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2cqxusnxy.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2smbnbdru.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2leexmwzb.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2wzndrndm.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2zalnqgfs.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2wwzhgkgr.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2rttqgyoc.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2lspxyhbp.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2comrotan.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2pfuseaem.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2ckcwbrsq.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2fpiffnzc.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2ybihcgqc.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2tvnkjnxx.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2kyplqkho.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2uljyjeac.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2baupzhwi.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2extuslfq.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xajrjaul.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2yiimljfq.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2qcaugdlu.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2nyjtqzec.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2jiyhgwyr.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2utsnfkwo.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2oglyoccr.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2glotomaw.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2vrhtsqoz.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2popdvhgd.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2mlxaqmcb.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2wvpjacve.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2eialygpy.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2zdvkoljb.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2jlyzpjmk.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2eosihyww.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2vschaevr.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2maeqkwem.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2qkkgttvx.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2xatukxtn.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2iqryavcw.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2dkgvwsof.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2lfbrbchd.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2xpapyrie.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2suoccacm.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2txmrldpo.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2imahfrsp.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2umibuhif.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2mmylimar.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2jsmwggxk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lmaujrcy.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2sebvauxh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bvrvypjj.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2wevgxflc.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2pzumljdf.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2ruogfrtz.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2pnosmlau.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2gwegrgah.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2wdybxmvg.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2cmgwkdzg.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2gbfpdxhj.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2agsdoptj.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2tpinnpfy.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2xarhjhlx.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2eavphdjv.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2gxclrynx.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2pkyzdgpw.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2warkicay.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2navvnlyt.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2rffqamsd.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2phvornui.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2lykmvdwd.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2cyjiolqn.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2fxbomgnx.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2mrhhvhkr.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2spanglfs.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2tsbsofjy.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2oklivkfs.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2rdhyrusc.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2hwtevpok.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2nteaeott.html


<!-- 参考信息 -->