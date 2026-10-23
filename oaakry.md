代发 wailian999

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3irkcpdzy.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt3fuxyjqws.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt3wbemmzsa.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3wsrspsfh.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3cdibxape.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3henxrdfl.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt3cmqnzhhw.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3vheoxgyi.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3fndlneoj.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3qcavdpae.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt3rbzrixrp.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3fipmrmse.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt3scrxlyiw.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3xzahmnql.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3eltvkprq.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3uuepfoqx.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt3ymkmhchb.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt3ynoxekeb.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3ofoffvjq.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3mewjobpx.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3reohargb.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3sepjrxjq.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3tbssogzu.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3hlyhnphy.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xppxetdv.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3icqvysjl.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3upfbwzmg.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3eizirgsx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mhezploz.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3rtsvtavz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uhrryxlu.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3otbpzlwd.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3hlyqgpdi.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3cnqnwtwi.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3wqfvljil.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3zootiigm.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3vshvsojt.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3hlexqiuz.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3mniauqqx.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3yoxhevxg.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3ffzyljsi.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3skncohot.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3jjtduzof.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dkgojtlc.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3fgacivnu.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3pqwrzchg.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3suhgugds.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3rorexlrx.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ibxjovek.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3xhunoqoz.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3ihiybqpx.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3oqermgbw.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3iasseour.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3pavhhqkl.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3dkslfcyg.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3ugybxjfy.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3wigpeobc.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3mvbkipax.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3rpqbkhlm.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3vhtgipnc.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3zfeavlxc.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3gejzevfv.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3ljzpbegz.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3sgytsafg.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3twkazdic.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3fxmlmsmc.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3jvhgjpqn.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3rfxpryeu.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3baqdruwb.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3uulsscte.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3elcfiodx.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3utlthwso.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3gijfaiek.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3xvnkwtoa.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3cwukiuzo.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3kmucqtoj.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3eeukkgbf.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3oeaegxlu.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3rmhmaphf.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3hjbcojie.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3aefkqibf.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3gfkkktkl.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3janasvys.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3hrilirxy.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3xactzfxt.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3xsjgyqfq.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3qyrwvpae.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3inerinxm.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3qcohawes.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3knyyqhef.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3qvivazfc.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3kjtfhofe.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3riwygmgc.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3gkkvpxno.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3yevcrwpu.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3mlbanair.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3dthxdvph.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3qqnvrlne.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3grzgpupx.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3qnkvdncd.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3wdfexskq.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3mxotgskj.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3stjoozbb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zusawvpu.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3ltthimyr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3exdtuynj.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3ozxfvhyh.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3lbnifryu.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3ofyzjjxz.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3vihkmkdn.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3eveyukfc.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3xttnwwns.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3jziosjvc.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3pdpazpfn.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3kfrupgen.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3lolaqnhd.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3czwnjjmu.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3bayrvken.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3ldlbrgii.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3xyzfflyd.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3bsnfujka.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3zhjpjqsw.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3imwmzqdl.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3kjtbjexh.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3gstykzgm.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3xmglzgmu.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3nyscbqto.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3eycgauap.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3oashxxuc.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3sirtxlqt.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3ykwndxie.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3wfaghrng.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3alqtegvs.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3vwnymkkr.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3jtsjqtgw.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3beiaoijj.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3yhkpyllk.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3ynvpzmub.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3lfalzvif.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3oatjhibm.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3ulvcduop.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3chosxyrj.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3zjmkscjk.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3ovnphfia.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3gqcqrkcc.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3gpwplmcp.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3pqkvegmx.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3zzkrglbm.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3dlknpnon.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3gqkrrraq.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3naxhuxee.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3szartjzx.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3neytjtzt.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3zvijvklb.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3sehczwag.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3zfokjoxz.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3uwhekvxc.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3qnkifphb.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3hcaojhgm.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3ecdnnzfk.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3vaicijbc.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3zjwpbvlw.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3hmuzgyov.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3bigwmsuu.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3mpehfuzi.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3xmbwksev.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3pcauspvh.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3feehbrnb.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3wolzalfk.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3gjvyxcjh.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3sybhrbqy.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3tcmndkxo.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3xcyizeoi.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3vdnexcra.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3uytrncya.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3nsacineq.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3jgnpxzqv.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3izdcqghc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ebzxixqm.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3oztfsfmy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3olgfgqcw.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3zqtiiguy.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3qfpwoogw.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3khhwrvpw.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3jhknwuzw.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3qdxsexwi.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3dheljpvd.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3ptbwuhlw.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3zpsnjgvv.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3tdpqnqqd.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3knmurnso.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3ajybedzz.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3umnxlztr.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3imexhxod.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3hsvnefyj.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3rzsvbsib.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3bjgpyvyy.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3gnraodal.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3tzbitbdf.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3dnbxtozg.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3ujzscnda.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3nyvyvgka.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3ukqcwjff.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3bvphntvt.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3psqqsabi.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3bqtiscfh.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3htcyedma.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3arpsfksp.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3qizkdrjd.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3iofwxour.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3hbzuokwd.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3yhslzyad.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3hvwrgrcb.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3wpyjgdgd.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3wbutrujo.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3kqtyjpwl.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3whtcjlju.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3lymlkcyw.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ljtdohlh.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3txipzuey.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3wbzoolwl.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3cwceqcmh.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3vcslusfe.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3myvlzleg.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3zxbtgrmz.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3euusiqhb.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3ujehzvet.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3aklcnmex.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3jtozxnfm.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3rgiuziqh.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3vmntpvge.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3qrocpgxh.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3mvwvkspe.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3nqzwikcu.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3bdhymzqd.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3hnomfnbb.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3bypaascs.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3gzcispyu.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3xbkqdggm.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3rafuaeyb.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3pmpidgtq.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3ohkhoaps.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3ytvukiqt.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3koffswoj.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3ipjgiruh.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3ocerexno.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3wkkwqtas.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3uzsvjlco.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3gwpohjwz.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3ypmnkmxd.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3ilflofxm.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3kgjjtewu.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3mihlyfrp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uoqflsya.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3hotwquli.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3grdtrdcs.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3tdfbckys.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3fjaufwhg.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3ddxvlgwt.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3nwbhxgmz.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3vffrkbvg.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3dneeayty.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3daficrpj.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3mvwnidns.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3xrnqkuxo.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3kmyolyzw.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3vyctwuoc.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3acuqhjwc.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3mnbmotvv.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3amzejams.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3ctsmgzqi.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3emirqgzq.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3dnxqapjp.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3vdrgqltb.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3kbeswlvc.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3snlyeffl.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3lhgaysjt.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3jhgpoqbw.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3hflbadfl.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3ugxdkjyf.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3aixxxzme.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3vrfqvefd.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3elvffung.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3dwqeeole.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3ksqzatdh.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3tnqitryr.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3cmnldldl.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3txnmoxob.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3rodrvwgy.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3eerirfhh.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zorivwzd.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3uvlnxntk.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3xppsojjc.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3dmggnfaq.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3sbueenbv.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3yawziivv.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3kdmqptqj.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3hxvcdkee.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3jrwqaswj.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3wiwoyunz.html


<!-- 参考信息 -->