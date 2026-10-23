代发 wailian999

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3pcuznykg.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3gogbvpbk.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3qsqweppa.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3ynhaovdk.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt3omimybtu.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3rotrsgji.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt3wcjbufdd.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3jbxcmsbr.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3fxppbwln.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3hsvfligi.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3lkzlbpbp.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt3hesoqjnc.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3gvpnspzo.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt3rbunxtag.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3jczkbpla.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt3eubtctky.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt3vjqedqcr.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3nvlotqap.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt3quphtqiq.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3ljtsqynp.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3ebhdscea.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3wrzkvlpw.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3rptlupzz.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3lezqxhhr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qwfuonwq.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3rhsabnig.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dflvvoxs.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3hdosfqhe.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3geifdqgr.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3walfwubx.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3rpdiqfvj.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3ugooycrl.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3kmmyecok.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3hfgatuzl.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3jrvtcozu.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3bqrzwhje.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3jbvxikkk.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bleupkma.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3rprgefpd.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ktnqrskk.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3scbnyvyo.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3dwoypcni.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3isqdhjuh.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kpfefict.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3kjltbxrc.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3ovqrkdqh.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3dwhqtcnz.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3awesgcid.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3wiihfgnp.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ecyvjvsy.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3pyoubrvm.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3hvnixclz.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3iwfrjfke.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3tjqlkpiu.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3qkoigmhh.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3suqufjzn.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3nmqqkhsy.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3ykxnuvbw.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3kpyosayw.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3vurnsdds.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3qqklgjvc.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3hhjsorwy.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3hqtmfcky.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3vzydxopq.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3zfdenftk.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3lzhvmzqw.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3vrnorowg.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3bvypjvib.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3hnnvuycg.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3bgjemdwo.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3zgvxdumm.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3cxmshxhx.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3lwdufiav.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3mhbfeuoa.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3esdjuxwu.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3qhdytnra.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3giiahhsm.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3wyfxunxu.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3dpnhbybe.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3smctzdra.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3veuqovue.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3dbzdaxxw.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3uoxhlatt.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3eivzosoo.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3yrstugut.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3tllxedgz.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3wxsjszlf.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3uqugpebj.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3zyqqdcnn.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3fmygulhs.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3wkbgfufo.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3vediyysf.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3lvbmyjhn.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3tgpbvagp.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3aqtpkjrp.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3xbgdigpm.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3ryybiixu.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3stduuvqk.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3qcquefnt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3czwggidv.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3glffgqse.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gonykgdg.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3ycuauoud.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3qhklvtbn.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3ldgutexf.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3blvyckkg.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3hccjcidd.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3fsxaimss.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3indprftd.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3uovnuszw.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3zfvmbtgc.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3eejxjzbt.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3bwmiaagu.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3qbteczsf.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3fejcvbfs.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3egxqvtoc.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3eybxgmhn.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3azprmtoq.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3zaydozia.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3iesfcsll.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3tqhtinsr.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3dezuioqq.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3byntiumz.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3fcnjwxkd.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3owhrowcp.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3pjgbubbl.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3jirezkih.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3aatmhfeb.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3dmdhfjwr.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3udqemwlc.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3vsovfnov.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3ywukswpe.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3wrlhxxyc.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3wyycwyhb.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3vhthcauo.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3mjustwua.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3pvusckww.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3ainltijw.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3snrusmwc.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3lozywvfv.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3bubjmslt.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3pnwotaxh.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3kkbixver.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3fbdfpola.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3jyazzztt.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3olspwssf.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3hksfjmyu.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3tbvzzxaa.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3xnlmgjim.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3zpstwzqq.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3mmepqqqt.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3rzouveda.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3oxmuckib.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3waamrckv.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3cdtmkcfz.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3gzvzucdw.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3wfwfwjwc.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3pfiqfino.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3ullnemni.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3zeutyotf.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3mpwofhsr.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3vshqsrce.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3jobefatn.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3jdamaabk.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3kkzsmgyy.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3znsttwps.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3dfzhiovb.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3azmyqtei.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3xwxqwzwh.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3tecczrlu.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3nnzkoshv.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3wvlnvntx.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3zmiyagrt.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3vfbcumcl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3turovtpn.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3ylfalkbf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wtulaknb.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3crfllyyx.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3dlenuecx.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3lywryuhf.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3mpbdtavs.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3oovklcog.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3chcetvfo.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3dttdydle.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3dviiobfq.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3vntxbdby.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3pjgzenns.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3rgiedjps.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3xmcczdlt.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3lklyxrpl.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3tupxyzfj.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3spoouvpe.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3rvvudift.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3aqwpjsse.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3scfkqzlo.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3apopvhsd.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3hbjdkyzq.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3newufglj.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3luqpyqws.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3qervzcnw.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3tjnyioup.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3ooiddkhb.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3dgopsvgy.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3efshpweq.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3gpkuealy.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3dlkxtsxo.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3xnckypue.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3zbjavhxn.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3kynuwsgr.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3pqtxwufh.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3wohdjirk.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3rudlucyj.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3tfnqoxev.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3xayibobf.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3fxyzbyrd.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3skzevcxy.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3dchimxoa.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3umonwkrc.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ymgchnpj.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3tvjzkkwr.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3pjjldgqm.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3zdyqmmku.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3vbneekxe.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3nmymfdfp.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3ymlklwmx.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3svzkamcc.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3evidlyok.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3wjxpnync.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3acrzsbix.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3djjkiwnm.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3mkqfzqro.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3mjebjwti.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3hynvixkf.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3syrqvwlu.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3ozxvfvlc.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3bcylrtpq.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3fjcootkv.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3kwujiznv.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3umfmjouo.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3uknsriyq.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3yanuimdb.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3vadvmeqa.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3jbilxbjl.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3ngatqvlo.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3gnjguiho.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3oarxxkif.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3tkctczki.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3opbiyfqs.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3cfqciolt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sswxhnvt.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3kxlmwavh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kgpykprd.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3gwonxyyp.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3mveakobu.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3mjbdzqoo.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3wmezokmd.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3spuycqpb.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3lvkfpflf.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3mivcnxvz.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3mhxpkhmn.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ysnfahft.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3ndjlihof.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3jbrgnloo.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3foymfnsw.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3yyvsvkek.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3zhbnxrpa.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3uxmcykbx.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3mqsrnkcl.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3epuwupak.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3xdavmsho.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3ptxqxuxg.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3shlaryze.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3tzottrjr.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3syznedle.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3xicehjjz.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3kqhlpboa.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3xfnyanar.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3sraqaugh.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3hvgpwbrt.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3jbcinouo.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3luctvnki.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3arbkpspp.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3ghepmafy.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3avnnzowh.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3cjgpwvqr.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3wgjkhtdi.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3snqngjuk.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3zcpqrzmb.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3mgmeoqxh.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3rerzkbrn.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3mdndzveg.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3lodewuyg.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3jedopebm.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3ltmbaymp.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3uhpioelw.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3lqviipfx.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3evtjqqer.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3ijafqjks.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3ftgxkvyw.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3nalelbdt.html


<!-- 参考信息 -->