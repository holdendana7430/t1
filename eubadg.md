代发 wailian999

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3fiisfnnl.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3qdkqrdgn.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt3tvfxoqbn.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt3rjawkxwh.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3drmilkwa.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt3sbxskilx.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3lovkdant.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3bhnrgkmd.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3nvpecpyq.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt3irkgyhof.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt3mayabtxl.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt3kpaytsyf.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3mflkapdr.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3czaqeglo.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3itiqbfjd.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3wpgefmxg.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3sohrkbcz.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt3opyicgns.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3ubdorkaf.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt3etgqkmrt.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt3iwszzttb.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3foirorpf.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3knjgkpow.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3dqagxsnh.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3macpfkxi.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3txgnqgla.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3tojjjmgj.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3bjgztwvb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uxrssiik.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3luqbhaur.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pltpccgi.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3tryvjnri.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3dxxblnqr.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3fjicwqyx.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3pwmookao.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3zqgbluiq.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3cwuyzefu.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3qjfiupzo.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3ptllinkd.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3bbqpykig.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3kqntclvy.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3yodavqte.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3uxbhylaw.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3vlhipwue.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3doolayhx.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3rxfcndvd.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3yyjaedjz.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3myrwirtp.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3omumhbuw.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3vpzdybbd.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3npcgwahn.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3rhpnxhmm.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3sfhkzixf.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qsmvabdf.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3xncpcwox.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3jjmzghii.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ushgvgjq.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3jqvfvsix.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3eoignppp.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3qtiapeqc.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3jafbgnsn.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3rstzzuga.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3njpgvevx.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3inhagtjy.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3juiiqqbs.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3cxmkjktu.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3mmurwtdi.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3ugwqecfd.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3vxyuqgnp.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3ofuyeyaz.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3lokienrh.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3wpozbxkj.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3ctjcmuib.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3eanpgwfr.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3bvdjglnh.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3znfdqdaq.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3nemdvkgl.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3izvpeeld.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3jghxnljx.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3plyqnulr.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3mzwxcncv.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3iaixwsoa.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3jczeeqmt.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3hkagkzzz.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3ocfyntom.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3uhehbfkd.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3lgiofulk.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3cszeexhw.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3jrkoxedn.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3koeocahu.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3wekekupn.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3zhzbfkht.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3wpbxpeex.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ryicmzfp.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3vmzwtviq.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3fvzxtxco.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3zdpnggqp.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3xuogsvul.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3ceddwckl.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3opwhzbkd.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3mxeqlqny.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3lnmbiuxv.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3krwkxvoy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fxawpsyf.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3nlwuskxn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3agtqmocj.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3fehxeyrl.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3ankjzjuo.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3nrhqfpom.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3gfoxdwva.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3lxrpzmun.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3luxqgpyp.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3gcluyszr.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3csiinjse.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3wgshjuuo.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3ztyryrhl.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3fkzkfexe.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3nphnexjw.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3rilpjcwl.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3crijrsuv.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3vfsrozfy.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3lupujuse.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3khpetacd.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3qcroonhw.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3cuazrzdm.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3fmfsjyxx.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3pwqpivlr.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3qhqquaot.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3hfihfpui.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3aposbijc.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3cnhresrw.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3owoyzblq.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3dawhwqkb.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3arseqiyi.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3zgygvuxu.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3vycspgsk.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3rdodfuay.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3owvqfcai.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3seqfxzpe.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3bbnpbsuh.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3tztlgoyv.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3vkotsqpk.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3ajjnsahp.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3mciyuylj.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3utolkrjp.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3xxipbmgw.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3lmmvnrpl.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3btxzychx.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3nvfoxyrc.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3zqastmhp.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3mwgjdlys.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3ycecjbxt.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3tjybxvea.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3oqjxovim.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3duninyof.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3fqkxegid.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3hnmvkrls.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3cknwehbo.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3btuiwezh.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3jzmmvwae.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3elgvmlqb.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3ekjocuge.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3yqzvpyqy.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3snqrrdag.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3kosxyqur.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3pccucmpj.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3hypwduis.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3unmxnekz.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3zfkqaeai.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3gqqeuqzm.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3ywuqugjj.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3slsmjvdk.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3augcfuaf.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3qdictxyo.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3kiaomabi.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3twadqujo.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3gkyvmdvx.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3pdndfwcg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wjqmxoii.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3gpohsyad.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xvqprazk.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3anpgibjj.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3iqvwafuq.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3glhyhdzj.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3vilkpglg.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3swlbbnqs.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3adsllyxf.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3hdbhqyjv.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3wikjwbbg.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3qxrpdugo.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3eovuoqqm.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3ubhjcxqs.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3dpjsochk.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3xilzmzlm.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3bapsmctr.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3yklqoltj.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3wafuqlpn.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3sllstbyt.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3judjtvdz.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3vhuqxgob.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3dmswcwrw.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3szmviyhn.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3tssnmfpc.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3xpwlxlyt.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3giveqaxm.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3wljkieqm.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3ombqsoxw.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3lvojrcud.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3ekaccusn.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3pcqgxwwb.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3nprraaxt.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3qskptxuw.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3tnezpxod.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3mceqracb.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3hbkrdxux.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3dizvoodg.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3sjyrdscz.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3kqxfpesa.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3pyilocnv.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3hwxlpbrq.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3jdtpqzcl.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3fvdzkdlu.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jkxaaakt.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3xzrejsxa.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3ruyslkza.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3ixfgceco.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3xzslevjc.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3xupnitsa.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3mhtwxxkj.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ezzprxoc.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3erelqvke.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3eboptdsw.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3oxibfqjx.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3rlrjiiwv.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3vhnpyrwl.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3mvbosokz.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3lngqbogo.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3ihzikbdg.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3wjarsoxb.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3mobfnuhs.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3omdhpwwq.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3ughpmclz.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3fwlbdfti.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3oewezqkw.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3drzrkqct.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3jrnxeljt.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3rkfcstue.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3nrvjibvx.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3qkbfmygh.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3iuuavros.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3xsexcnke.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3bkmdaash.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3cvgvwnsb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zwlegjvg.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3hzcupgma.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cjhzxemy.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3wplxoufo.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3oeubncsy.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3gzatepnm.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3fjskjecb.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3iypzcasv.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3eopobkns.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3vbdoeegc.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3pznlytpu.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3txuejvre.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3gwwwjjyu.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3oxcghoxc.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3qekamuki.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3wxjzxwga.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3ufqureug.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3zdqmaxcn.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nbrdrmtj.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3ktgzbgxg.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3jehvlzgz.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3agdqjeds.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3fzdmrvxs.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3dlgelxpg.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3naoavkgo.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3pqhfufvr.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3vwmrvkht.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3yqypydvm.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3xydechxi.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3ufkcfwsp.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3ctbpfqvd.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3ypaoakam.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3lnxytsne.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3lwvqmbqd.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3ogcohdsl.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3gbrkelag.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3wudomufc.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3sodbxhuc.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3nwheudnh.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3fmxucdxd.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3vlveiygn.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3voeroicc.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3rpxmreti.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3dgknigaj.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3htlgrqqf.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3bpthqfyw.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3fjzejnha.html


<!-- 参考信息 -->