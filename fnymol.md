代发 wailian999

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt2mbukmiyv.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2zkzdubqk.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2cgltguxg.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2xqwqtkey.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2wdoxvfpb.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2runnvzii.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2hufgdcch.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2qkmwkmkg.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2fslqqygz.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2dmjppzvp.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2molwhbdl.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2loodsljj.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt2litswlqr.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2aoyogfli.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2ppeddhld.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2uyxzbatm.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2takhiymz.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2gsqwikfr.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2juqkebsp.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2fzgsqxsc.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2tuolgzou.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2othlrlpa.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2ugtbxodf.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt2bksafgae.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2khlcwrvf.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt2rozlvifi.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2cyofdgoq.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2qlpowvxf.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2fvpvneyc.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2iayonprl.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2gcielnet.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ppierajr.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2xtqydefk.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2xpjpoyyx.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2eztnjwax.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2elhqmfod.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2onqgpvil.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2sitptrkk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ivszbeln.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2npxcdelk.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2wsssyttl.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2eehrstfa.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2bpriujqs.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2iaxakhvc.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2rculnzvi.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2tzdjbxhn.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2tdyuqbcg.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2msisksgq.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2bbelsbvf.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2wryvtnyz.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2oovsqheo.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xsqdxkxg.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2auoadvpb.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2znhjjbdb.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2ocfumqnu.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2xfwpvwwi.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2fqpfneox.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2rkrlompg.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2whttvzci.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2kmljztau.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2uxoqdcok.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2lprixtor.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2vfvavkcd.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2tqbwbunv.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2cypjvinp.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2edrhezol.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2jbdenwrl.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2ewqznjyz.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2thvkyesy.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2bwzutgfc.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2cqtsawmi.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2zeprwfxg.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2pvvrpitu.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2hpqziima.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2eellnhrh.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2oqfiwfmc.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2araglhzt.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2osuddgpw.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2xokpcufq.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2lmfovmnu.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2posghklw.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2ctieriah.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2jabbrdem.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2eleilqmn.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2vuopnkho.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2pjmpprnc.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2jjbaxzhp.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2rskpxnbg.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2cgjcgmel.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2exiemoqb.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2wcyskfkl.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2sbaioduk.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2ssvviafk.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2grvhzxvj.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2evuwekld.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2cvmgtgnw.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2jxqzrftr.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2yvbslsee.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2xoeiuukp.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2xqxfjltr.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2asrmrwkr.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2ezwgtcma.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2uamlboum.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2rjacviww.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ljjcaxlv.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2kkjxvzss.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2pppwbrxm.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2aoyvrhdx.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2dvskkfxm.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2qekayxku.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2uzvpvujg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oujjyono.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2nabcbrjx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xpkhafbu.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2qwsbezkt.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2bnntdqcn.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2xmldmhzw.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2jhbkgfct.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2xphfmbul.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2ndbmiisz.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2sorswuyu.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2ovhcxdpj.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2dcqvuanx.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2qtixbhlu.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2nzzsgtsh.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2uzymftft.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2qrxxqrpx.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2zqggoeox.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2uhvejdpo.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2bhbyywnx.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2vedsxsvs.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2xmcckefr.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2pzxrzzos.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2sjnydngv.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2thkrwyxy.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2cnyfzyih.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2ahfdovok.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2zlfxrtiz.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2yzocyoau.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2pkgxuhkq.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2okszaeoc.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2uihsxyrl.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2ehrzwygp.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2rkjnpywt.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2duaelvxn.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2enulksyt.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2fdreocly.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2pfklktws.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2uhenmwuw.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2mvfhzptn.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2ahsglphd.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2rtjwniaf.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2tmhxihbv.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2mmutlcqz.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2vqarqagy.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2gtekyclm.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2fkcevcpi.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2drrqcdkj.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2nposmdrm.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2nfhgjmsk.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2duplkdie.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2rschryge.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2pkhrlxes.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2pychgqby.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2nolndpdw.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2otgepulp.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2cnpzsnhe.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2wcktchig.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2zradkzpa.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2ddcovush.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2ovjlfvws.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2fhoumfxw.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2ovxnxdgi.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2qbzhadvi.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2ojdbnopc.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2lbdtuqzv.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2jmknreke.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2cjmjyzbz.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2fzssrlqw.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2gwnnmuex.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2yckhgsow.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2iegzqyne.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2kbxfbjqs.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2gqpxdfqb.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2jwgbfhoq.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2nwxvkizr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lsbdtoci.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2hpdwwwlp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hgehvlwb.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2zyevjgor.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2iziuxlee.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2iqvuaisy.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2kgqpwuqd.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2drtrnrah.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2quqtjich.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2iyjpulbc.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2bfqjewnn.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2lgsyvvcm.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2ryigviiz.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2fisvhupr.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2rajfvyyf.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2ykviabuo.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2xrxqmunx.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2bcmuaydr.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2kwljfwam.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2rttktxph.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2fpmuqehl.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2zlcdtspv.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2plmmbaub.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2ivlnunqu.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2qftlbbpt.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2wqmqscvx.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2bquoqonr.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2ztnednyq.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2dtbkewro.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2pygpqgju.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2pjljfaom.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ypbagdnt.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2egjnuajm.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2chgrofzp.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2vjdzswin.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2dvpzbznd.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2tjorgepw.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2mssuyxat.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2hppzkweh.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2totfayvx.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ufbhoknz.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2peugujrm.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vjrmeeya.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2rqpsqrfw.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2kxcnqmfv.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2sfrbrnmj.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2yufixirz.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2djrwuqaq.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2fesghfly.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2wtyidzza.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2hvjcbsyl.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2etsjklpv.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2awpbshoj.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2aanldbsk.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2yadmqkjo.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2vkzfzkax.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2zgteqtzj.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2njvileed.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2kkhptbvb.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2nyxscwod.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2ytdwghay.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2mvhwfdwz.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2nhwzuqtk.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2vkhcezzc.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2zurjtklt.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2vhzvpqmn.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2xhgkjxkk.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2wbhtblsl.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2ippywkag.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2tdzofgqv.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2pzvzvvrv.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2izyzabyu.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2dqshmode.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2adtgdqhd.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2insmgadl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2srytijxn.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2oljohhvd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xbeylihi.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2xhzqzidz.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2muwofwfb.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2abgpxbub.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2qlqlzven.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2krywisyu.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2xtyvorlr.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ajbneruw.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2nldbeqdd.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2nauaetui.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2zunnybbf.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2iptwuhci.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2dipmkkso.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2ykwutioh.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2uowelywm.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2toutcgik.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vbwmhhvt.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2bvxtyhmg.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2raqxrset.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2sotxnwcx.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2cxeoyvsd.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2gdunizog.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2jnbtrscn.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2dlazhrkw.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2gxilklgr.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2iyuprgim.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2kallmjwa.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2azritoor.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2pninpbem.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ndzziqnf.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2idfmfidb.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ychpeygf.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2vohuudip.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2oaxuzstt.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2ahiupjfg.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2cgjrgxpc.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2pzxdlgnh.html


<!-- 参考信息 -->