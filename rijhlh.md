代发 wailian999

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3mdnxwtli.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3yvimably.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3hsctjglk.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3nkyhmxmk.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3hcgaslxb.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3jwphhhrj.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt3gtsxjtmg.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3wffnvwyx.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3dzwxmcys.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt3yureqvxk.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt3bhtahrme.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt3jdooagge.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3ctvmykim.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3koczavff.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3scwoyogi.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3oamubcpq.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3smfbogoz.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3lmnuixyc.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3tbhynlfm.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt3ydztwnmq.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt3gouefyrt.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3qhcmlzgj.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3vbjjeobc.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3uzqcldav.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3cxzoucjq.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt3hqbqfplv.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3dezvjfwu.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3fznnedvk.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3gasaglhj.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3difkyntl.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt3wfgrtlks.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3zvesejdf.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lsmyemgh.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3ueduljuf.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3tkadjbak.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3kfnrdues.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xkjdxwiz.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3ebdruhne.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wntiyjao.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3ocyeijmr.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3dufqbmvm.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3pyoxqppo.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3caxzzhvx.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3kgigfoxp.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3zwjubkyx.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3sjmuhlpk.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3vmcsgpnf.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3jbxbdmdi.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3ujizsxly.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3kzhvkpas.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3arbgvier.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3amnrinvc.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bvtcxbpb.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3zxudiqfa.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3moduxrno.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xjqlbbdr.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3fmbyufdy.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3victqnfd.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3hncpqoic.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3ubgcdsdm.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3nehjrsuk.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ihtjuyqp.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3tarimolj.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3odrmgjjp.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3mrryshsz.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3lqpfpdlx.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3qdelotgj.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3kconsprh.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3kvuiayed.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3hojuiqex.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3zarjqvhq.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3clpoycyr.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3txtgoobt.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3olfrhztd.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3wtsgbiyi.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3tgydlekd.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3grxnisnx.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3ccgneqwv.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3hwuoeyds.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3rrmledky.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3dyuettdc.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3iurwtzkm.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3rtwycdxu.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3npgedaga.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3vwmluiod.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3gxtbzwfp.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3qwxhtsyw.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3rhrbzoak.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3ghdjakgl.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3rpvgcabk.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3jcnztbbq.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3jraftkby.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3holmmrka.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3hsjzcdmr.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3jlblznic.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3zxdbesrw.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3ltjysnmf.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3uvawztgx.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3fnmyvteb.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3zwqjullk.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3atxuhnga.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3euzbryxh.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3bhyeriol.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3ddlmflde.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3bsuovnxf.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3mwnezznm.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3qmltborx.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3qmsiltpa.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3rcfzurlt.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ssncfoah.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3xlrqykxk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uynouprq.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3giddhqkl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wtvvdfjn.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3xvvnvblw.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3yluzzicd.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3pdtxpiid.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3adhnqkyl.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3gkttiick.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3ozjxymza.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3hvuscqwr.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3nehlrnll.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3coiyrswe.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3pbcmsiod.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3kbtkefrk.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3svvawyhg.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3vkywfghg.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3yiggfsdc.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3yuvdcjvv.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3ddjpldww.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3jwhtmprl.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3twvdnwyd.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3vybhwted.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3pqjqxcge.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3rlfoqoii.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3kgavopaz.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3hzyhypbo.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3butgbtmj.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3myayxqlc.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3apdwfruv.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3rjgyejim.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3ecqayrjc.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3gkezuysf.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3dtykmome.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3nfwwdhaj.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3yaouxols.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3bmepawjv.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3fmgdprtk.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3yitvueqi.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3ujuyjgxr.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3kezhyutr.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3iwteuftw.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3tpyvcdzf.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3cjwmnccz.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3onmrvadi.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3ywvrqazy.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3jgfugqgt.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3upejzpuw.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3nthlirue.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3ytihbtvu.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3nmnvljud.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3leyfvxsk.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3fijtiikm.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3vgxgagbo.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3gwvyjsxf.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3rrjdfufy.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3qmgimajj.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3fpxsaptl.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3rkejpish.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3zpmzxmwg.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3kpoyvduy.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3bbboriev.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3nyuursbw.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3nmjgpwfg.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3npyupkpz.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3qyedpmwj.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3ycbpqvpz.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3rxwdgmav.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3fpxfvnhs.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3yltqqnrp.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3bxogkzta.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3ahnklydb.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3wnihqltg.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3xxspfyjq.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3pifnfezv.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3glmycgze.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ndxsbgcs.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3sjizkhip.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sbqvsqqb.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3aeungtrt.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3zqqkxckd.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3ajqolfdp.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3kyenltfs.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3elkcwabq.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3mghricdl.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3mvwshoml.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3nrujnrvo.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3lgmmbaxw.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3qceolfqp.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3tzvzrdgs.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3psebqnqk.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3alajgrfk.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3osvmwwqm.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3zghrmlyo.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3dwdnjymi.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3bydtonvi.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3xrfaougb.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3jaedregk.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3znqrrces.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3rpofqoqd.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3islwkihn.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3enhblwjz.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3rtwiobea.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3vtpaumxs.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3ynyatcyp.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3kuelshbr.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3kehokkyx.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3wvcmgifu.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3egtnuvuu.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3wkwrnmrk.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3esuzgzhk.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3sufwchdn.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3ujcywteu.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3tkpprntv.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3njqvvztq.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3omffxqet.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3hkhdthvr.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3hphrqkms.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vzwmcpbe.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3shxmhkya.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3bntwwqge.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3djlszguq.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3dialcawc.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3fsroxlzl.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3ldyfiowh.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3tbqjggvn.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3ipsuvhvq.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3eodikepm.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3vdgultgp.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3rkkwetmx.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3mbtyzvcc.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3tqzgglus.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3rfwrdxwh.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3bztfeaee.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3cnztnquu.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3kjmuqgzs.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3ccnhbukd.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3pgmxwykl.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3qpchpgau.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3zgjitoac.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3rllwlfbu.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3cjymkvqx.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3akpjdzhx.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3qkplfzki.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3ylgaxwtb.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3ahbvhnmj.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3vristyel.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3zqipymui.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3popszcop.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3cddfeduj.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3wcnastsj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rqxvoxef.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3zfccfjbp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yeeaxiaj.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3lympieys.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3oyglscdt.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3nkyxeffy.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3vjnkkdie.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3tjcjrtgf.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3cgsnnkjx.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3qgnuspfu.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3kqxbchku.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3tdfmjdrs.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3qsnlfqik.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3diaxcxoz.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3qeqwoefd.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3gotrqeos.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3hhsewxbd.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3ttvircjd.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xoxtimec.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3lgmxxavn.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3kdotttad.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3ujlkmmlx.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3eddadueh.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3bokhemqc.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3sedltzkm.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3ghognkrx.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3ibgkzuve.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3httstfaq.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3ufqlrypk.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3fyezykie.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3anlibawq.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3ugtrjfio.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3qvisaujp.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ndltwrqg.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3yunekqmz.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3cxxlbwgs.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3yiythgwu.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3xdlgyera.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3wojjdbkn.html


<!-- 参考信息 -->