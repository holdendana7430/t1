代发 wailian999

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3oztgafjr.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3yavjbshn.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3ksaiqdgi.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3hvtceihq.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3lcmfrgtw.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt3kytzrxsv.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt3jdjgedta.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3zrihoygz.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt3nitonomv.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3pemjzkll.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3wmmesbma.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3wkteqnsg.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3ygtasqyl.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3agyboyjx.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt3zlxizzyh.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt3iqpspopx.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3ssnvrmdq.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3odhxvtrg.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3jqocatbx.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt3oaopjiay.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3emdsdnje.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3pkwhfrch.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3enkitycq.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3hqiytdiv.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3nlxkyndw.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt3ghmctsre.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt3xanemsfx.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3lgfdxzkg.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wphnmwaf.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3ghuvikdw.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3rrtmpthv.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3gzkckcpj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xymikkgl.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3wqmpmkcv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nyerrugx.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3lxeouwng.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3bcbnriru.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3mobtjqol.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3pjirkbsw.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3bgjtesuy.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3prhrtvwq.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3lzbbrpup.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3ybzopzac.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3agsvhhwn.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3qvxbgxuy.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3pqgsdukm.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3mhfvpizx.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bxwrwdaq.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3amytdilj.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3uzitnpsx.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3ihkdrhfn.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3elrzehod.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3vhokqblj.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3bgrnttrc.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3nrhlwikv.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3hfhialhf.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lrfkqcmv.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3kwatqmua.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3xrvxumhl.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3pmmsiddp.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3xetoqygz.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3jhxfzyqr.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3bgeaieuy.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3mkuzstcz.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3iqplzfef.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3crmajtuw.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3wypolhcd.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3ohrjaxly.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3hubdbkcw.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3vhdmjqdl.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3vjhnvieh.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3gljzrqou.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3ynhjitqh.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3nawczrkd.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3dgizsuta.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3fyeofsfo.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3carfhjkj.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3zieihemy.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3yqpbqbkn.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3jaoetgyz.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3cjiniggq.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3luenzafh.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3yscddbmb.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3gzlciwhn.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3prqbqjqv.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3wwwqgiom.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3azujejjm.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3ffngprwv.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3kxqlbxqd.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3vlyiklxc.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3uywfambf.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3ekyueptc.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3fjljfhek.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3kiwexotr.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3njteeyll.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3iafrxenp.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3lkwqvvwz.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3ydkkathm.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3fcntonif.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3wqebjesr.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ylzsoifp.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3pilvphsg.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3tbbrglzi.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3vclwfbom.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3jgkqqtwb.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3frmomaqz.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3msohboia.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xcoylfge.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3ygityrue.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pkpgixjz.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3kavzrfmo.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3dudlqksh.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3nryhpvqu.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3npmpsxop.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3odbsanzt.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3vifrwqis.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3icwvkspi.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3ajtmyhah.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3dhkxrebl.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3gzwgfahl.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3wytnvfgc.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3govoznrf.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3kpnarsqd.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3tcwyqqcj.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3mcuwlbbs.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3mgoqmhta.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3xyzgnyod.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3ezjvywld.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3oaeauctx.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3fuoaqowd.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3gwtszgcc.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3hkwdwjzz.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3ggaweiqe.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3xikritpz.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3albvsagr.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3khaiurnz.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3rxyfjjsl.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3rfysbnde.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3ajzgtbri.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3xiqycdso.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3ixfcmxug.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3zsrxjxpw.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3qfaqkpzz.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3ogucjnpf.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3mdujmilm.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3nnatqfml.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3gfgmkxbx.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3oysaxagt.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3ygbbnbpr.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3bqlhglxe.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3utrurmeg.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3zgijyspe.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3cbiyvmly.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3zrxybrxm.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3vmdlzrof.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3gpinzokd.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3bqndulgg.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3ddypjxpc.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3dbqvfikh.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3nqzaxgka.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3uizqzquc.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3nisqrauq.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3jiszfuim.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3khkxfwmz.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3bybfamyb.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3vgxomgxq.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3hkcuyluc.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3jskpomnr.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3jikknwdr.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3brhnfkly.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3jsezvotv.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3lwaytjjv.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3rnnffhks.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3tikfrome.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3xjpjguep.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3mvvofdku.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3yjoetqgh.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3zlvwcfof.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3qbpaspcz.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3qbzdleix.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3mdqdywqa.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3qnxlmuuj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xakvzlwg.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3gczansha.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vrrplffj.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3nkjeczfw.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3etrjuree.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3llkkeasn.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3bpvfwlez.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3vhsggvqt.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3ypmzpngd.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3adgaynok.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3ocicltfw.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3opcvhcrm.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3mjrlhbqj.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3xbthzkhg.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3ylgdmtqu.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3ggqiilde.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3kqjoxbjy.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3sxdvtyci.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3rohuavgq.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3nhavjenv.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3azwrkfvi.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3bfkrhqrq.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3gaqaoxwa.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3ikvfzfjg.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3fspefkaz.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3tejppszi.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3spdgwpdg.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3mjqlbkro.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3wbuwqzkz.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3iygnvvik.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3uyhpabbi.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3otlyrvaq.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3gkoncdba.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3ioetcmom.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3slflsujm.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3nxzuekfr.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3cvrffrpl.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3auuwntwf.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3qtytwoef.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3jspgstpm.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3jzgfmvvc.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3orftavjj.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3fvqsoltf.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ypgwszmg.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wkainqkc.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3yxwenkgl.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3elzectgr.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3vszdmooa.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3azqluhga.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3fndhcqbh.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3kdjqfdwu.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3jrspilgi.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3mzwpudzx.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3qsrmswjv.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3hjkhoytd.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3avxfuhbb.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3psupyegu.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3cunfuehf.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3pzbguxur.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3wemulrdw.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3jjraqfvu.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3fiiwrjuc.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3zbvzjlnt.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3crrsidaf.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3kfcucllm.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3eceexfbn.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3ottgjwuk.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3zrxdrpxz.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3gybqhmuh.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3uhxjnnmw.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3oxnkmbwr.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3ubkfrjym.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3bappqpbe.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3ghzueodu.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3xxlkxdwm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qeigchzm.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3bsxpcywy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pebnkepv.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3tavfrzig.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3cwbpzxpc.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3ceuuqklo.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3bjjzzzay.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3ybpofqnc.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3tozdizet.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3tuaudhyk.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3wwxsefpk.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3crbjiltf.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3owihrhow.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3dxwnegxw.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3bfuxevkl.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3gihwgbsa.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3qriayjzo.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3vywcsjhe.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3derrklgw.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3bsogndif.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3liribako.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3rqhenmcg.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3mjkzblte.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3bwpreqat.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3cyrpoopp.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3bepgtrii.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3stanayjc.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3elplqxxu.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3kpvgjrbv.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3cwrgbebr.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3qejnknrj.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3oggligyz.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3cwftnetj.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3mpgdigki.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3ydcwzzam.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3idgafbob.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3eskvjlbw.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3xuimljfi.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3shfwtwso.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3giwjtkal.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3himszlsc.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3jewygzme.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3zsmvgqzp.html


<!-- 参考信息 -->