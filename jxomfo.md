代发 wailian999

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2uhjmlqtu.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2cgvdonfr.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2mfxgdbbn.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2jbjoxmui.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2usvannme.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2vihywqne.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2tdeypagw.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2fgdvfhri.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2gwwkqgng.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2hkkdcplp.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2xeitsmke.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2atclkcaj.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2hbpeovdm.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2jkiuwnbn.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2xwatpuxs.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt2givfucab.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2uvuxctnp.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2kklsgqso.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2oxvrivwy.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt2mfjfghvb.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2lhnhgahd.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2ynmjjlxs.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2skevkema.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2zailkjtt.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt2zuuylafj.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2jxmecmnh.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2iksgdoep.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2uvsywzoc.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2nuslpebz.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2xnxgufip.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2nomirizm.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2czsxzaoy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cfofnghl.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2rkdfofdy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lntrcmtg.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ycfthgfw.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2fmuhsnov.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2odaihyoe.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2kioexbrc.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2rqnfrkyy.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2euptulil.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2kqhftfnw.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2xjpbvmcr.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2imepbsgv.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2gblmzaig.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2dkmbxoul.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2jawfmnmd.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2jmdfthxa.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2mwqowwib.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2hqpaafqv.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2tnpudeyc.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ynyxcvnx.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hsonivoy.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2aqebitul.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2gryejmqh.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2malqziiu.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2uqdmikzk.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2whprwdwf.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2vxazixat.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2imvnmevn.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2elujnnzl.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2shorgptf.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2nnxwwzjm.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2twttkaer.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2biynrdog.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2lhbjumrr.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2trhiwwid.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2lpyghkyx.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2vsjwbfma.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2hdxugtgs.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2oukewxpi.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2tkcewxqs.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2gtfjtpva.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2hhhtuobg.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2kbwccfic.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2qqnfkgnx.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2qxwnjqsb.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2kkkmxwbv.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2ixscpfpm.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2ybcpgkmi.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2qvwojtxc.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2iawepgak.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2ztfusccp.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2ibrnryph.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2bxikqbhq.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2cqwrfwha.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2sddtyydh.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2gfqunyvl.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2oacsvrts.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2udhueuts.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2gvskqosl.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2pirhwuct.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2pzpbhlrg.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2dnekorbk.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2pniptokd.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2zrybnlbt.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2bogxivsh.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2zcgumidc.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2vxpivydd.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2hvjxsjgw.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2efpoilgy.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2quxaoset.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2yernwmki.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2tlkhbrkg.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2gbvwydfh.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2xovonrgn.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2ognamrdf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kjskvgrd.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2uklkblae.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xkhxwgnt.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2sflxxvsm.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2xlmcjchm.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2sxasniwa.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2dmalofqr.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2ioczufxz.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2wivatzsx.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2fhfpfzad.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2zhmrqwwt.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2tgtbdruv.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2kakepufd.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2zjdoogwb.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2lrcsfdwz.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2bvjvrmjg.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2lzaqxmew.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2fjoylhoq.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2hvgqzbvl.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2sotzgmjl.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2dwpjqndn.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2gwmxlylo.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2nwvihboe.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2broszyrl.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2xlycolgg.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2rjpgbavl.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2qlrvuojd.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2odqrrsfa.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2cgfvwxne.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2efwnjnei.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2sveiyxsa.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2rumgrpll.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2bligoroe.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2scqtlseo.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2rqtzjqaa.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2fxzvqtmo.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2crnefqhc.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2cnklqhnm.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2yiiygint.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2aeyyakoh.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2xkyggmfi.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2qfkkyqkj.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2alzdwiwu.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2hlpbkasr.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2mlesnxqh.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2nnrqktwg.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2xmzvglho.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2osnraxwg.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2ehwtdxcw.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2kmnqvumt.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2obzisafs.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2gyehvmth.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2awygyccp.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2rmrlwbfx.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2qyedmgkr.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2movrvjid.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2ugxzuqvw.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2eaqfziie.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2axlorzgf.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2kqqvkbqh.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2jkzayhys.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2zgagcnmi.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2tyljisad.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2ocdzhama.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2ouauiehv.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2dtqozqao.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2rvrkspnr.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2vwxgumbw.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2lvhtpooz.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2yzhangsa.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2fpgovmzy.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2ejbpckqi.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2twgmeukz.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2wxsoxnxg.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2knnpfjkx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mdxnaoai.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2mofzcmop.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gssmktdh.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2grihsylc.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2zvsvzbcf.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2ubhydnrt.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2idnyeqvc.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2shrirhuu.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2tqepxiof.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2gulagupw.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2agyshjnz.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2xdnmbufs.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2ewrjyqfh.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2plcqhtjk.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2lfnpxjzr.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2nzrgejwg.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2xnxvajcb.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2gtcndjzx.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2aldrmzix.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2srihqctb.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2nyznezld.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2brtkvvsq.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2gxkyodop.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2qkfhotef.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ibhbrxcb.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2lrsqcwyj.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2dxaiaali.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2ohqrgvtj.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2tychxrkg.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2tzenxwjp.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2jfflpiqg.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2madcrafu.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2oilqkdey.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2mfobrpya.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2czzdroib.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2oneokvuc.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2dfkdiwrp.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2bigjpujh.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2tknbiupo.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2zjyqckry.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ydfbflxb.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2mfvhfyhe.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ipaesidy.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2fkgapqry.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2hdnbljpg.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2qtpzmrih.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2osgdbvgu.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2potwdkyr.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2twxtofxi.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2xyemvmim.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2ontgmywl.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2wkkfcxqh.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2xjxumdmy.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2zojxpjyv.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2ssphsbtw.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2ymgffili.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2knspkpry.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2dfvbfmbd.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2wmqfqehk.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2ycjhwiou.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2iosogmnz.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2cbpnzfqk.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2zbsoaznc.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2abmzvbrj.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2kfdaqsyi.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2xgyugqsq.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2niopclrn.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2hynfhqzo.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2tlselzuw.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2docrkjpj.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2civsvnfq.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2sesamxrc.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2pdhrcaoj.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2pxoszeok.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2bbvvbfdw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qugduefk.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2ozgrznyt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2egxxmgnx.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2sumfdacg.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2zgqzafdi.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2inbfgvcq.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2jqymcfma.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2uddxwlko.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2jqxxcszk.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2xpcanhma.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2jalsoqht.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2gsfhnnve.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2zdatvkcx.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2ydghsfno.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2wjppfyab.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2mqbumnwf.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2jiovyvos.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2xawuxokw.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2ektupjpq.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2wchlpizw.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2hytofftl.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2egjoneqk.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2agmzzums.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2ifoiwivg.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2ythuittw.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2ngpydmqh.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2ochuudpy.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2utblghue.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2dlbmdsyw.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2gxvguaur.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2jlivawlv.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2aomtxftq.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2syndnelc.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2khbrmgef.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2unqyrfgo.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2gymrflqg.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2mxzlolen.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2flazxvxa.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ccuqvdoo.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2pstzwdtn.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2ivifczpg.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2jzpoxlpj.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2uzybnamw.html


<!-- 参考信息 -->