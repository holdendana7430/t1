代发 wailian999

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3kpocbarz.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt3zavwjxiu.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt3akcdjtjx.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3dycwkyjf.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt3cvkgfodf.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3rcndhilm.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt3pljfsbyh.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3zaglbeov.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3tcpcsohw.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3fvkitacz.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt3zoddowlk.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3sutqyhgr.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3kvplvjfz.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3kbovtkfm.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt3nosmvbkx.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt3bokhemgq.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt3uburqtdy.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt3czzishxn.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt3gapywimg.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt3tjmaddhh.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3zouaecad.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt3rcdpdamj.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3hyeqkzxz.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt3cokocvdm.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3zyhtfmbq.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3kzlxxpcy.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3yebwsdxq.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt3rdykovhb.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3jfyahxfv.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3kcmznoue.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3dxzegoqp.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3jngskgvc.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt3qqgoikvz.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt3zomduyve.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt3kvomrunl.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3yrkorhbh.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3bsxeojsu.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3tzdhklac.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3ifrgdfxi.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3lvuxbzit.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qookepcl.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3psfkwxua.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ktmyhcyj.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3yrhwioua.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3kottqfvm.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3cduhxwkk.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3klasvxsp.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3qcncypbm.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3jsshqnmr.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3nshbdmeg.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3ruckrhpm.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3czqgzueu.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3outedxih.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ttqfcshp.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3gyauabsx.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mklmevvz.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3vhytnwsw.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3jcedpnxx.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3xsornupv.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wmvwgzsl.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ccrxmavq.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3zihjcbyh.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3wruuigda.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3hffvflws.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ejnqzxam.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3oxxvecjt.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3aoybqwdb.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3gyxxpxlf.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3bypjsunu.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3qwqcveee.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3qkqjxzfe.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3xvycmqog.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3bfrskfbz.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3ypojzken.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3encblryt.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3ekggzbjh.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3fggmgtie.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3bkfsoqky.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3htdzozsa.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3unzfqytd.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3besakipy.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3ucgiapbe.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3euizcndm.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3mirswpee.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3xuqoliih.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3adekvmzu.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3emvrmzwl.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3lughdfsu.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3gchmriuh.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3docsymgd.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3mtccykyw.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3pjhinvqr.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3pwnoaqkw.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3qabjbjiw.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3qepzdxgb.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3qenbmazz.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3otemghgw.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3wdblzzsj.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3ezmewiir.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3sdmgvhht.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3tqrskokz.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3hxwkdeww.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3igqaknzi.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3crtvaiif.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3lsipgwwx.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3rvyfrghr.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3uwspultq.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3mewjvepr.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3wuxlpdlq.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3rfaeiyzl.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3vnaiqqbq.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3imgednzv.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3dwadsixu.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3hbbnndhr.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3ctfktscw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3irqaqxky.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3kvgsixxj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zvbuqumr.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3jeijlolb.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3hbjjiigx.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3akzoudyy.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3ajhyqtfg.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3kylsqwhg.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3xqyghyjr.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3jkgxgssq.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3gmyeigmt.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3kamteubr.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3szbvzfhn.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3mplhsfzu.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3tmjovnou.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3qbuclups.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3endydvfn.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3lwpnpazn.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3nllnvtsp.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3wevcbtlm.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3uahsccei.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3tfcpnenm.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3yctfvgvp.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ophjsqbs.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3ngytheyq.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3fpbmuacw.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3pijwmdvm.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3nhkyrpxl.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3zzvevmlv.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3eebpyfuk.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3bnugokje.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3wpddxndn.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3ecffhheg.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3wpkfrvmz.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3nxikioqm.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3pmytrupk.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3qdbdsnch.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3uirqlqgw.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3dvvmbmkt.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3ocbxyahb.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3axxnscjd.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3equedvck.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3asjvgafa.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3kfxdckpn.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3iktmffun.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3wiorsdgi.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3uynkkusi.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3aqufjbqr.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3dowghybq.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3cssnbijm.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3liwmvuxo.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3qoycamck.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3gcmmhidj.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3pbfehlxk.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3cqqvtnrj.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3cwbuliyu.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3yzoscjlu.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3asvnmvfw.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3fmunbppn.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3jpcmspst.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3xqwemqho.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3dunibzcr.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3cfyzcxgo.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3svssaprp.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3seqdpicj.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3ikdyagdh.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3pblmphex.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3pjkdsykd.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3mansoutx.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3bqsxjxgm.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3sbafczle.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3iiifqhja.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3aizalqka.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3ppwlsref.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3ixdubpnz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mmjagjsv.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3wpmbctdf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qauzfyyw.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3mdnqnbiw.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3etysulqf.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3rzwlvfso.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3cipmdkit.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3jmsdvxbj.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3wcplxeia.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3gjhzjgny.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3kpztcdeo.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3wpkvyqpv.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3wfxzxqhx.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3cvzchnym.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3ypuzkqed.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3cnemnswe.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3zqbhcgyf.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3xlxozewe.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3kjjwzuaa.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3obxqqklz.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3frceikpl.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3yfxpdgsq.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3mbhoaxnf.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3dhbmeqnh.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3zpknwxyy.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3sydfvifl.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3yxxyhykd.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3yngevmjo.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3zfvhllun.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3noptmxhg.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3itbhjbxw.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3qlbnvbyr.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3qgjrzqqy.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3uasolstz.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3mhavzcka.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3adtvhkuq.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3xokqxock.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3bitrgqoq.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3iygafttg.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3wqigqrya.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3cyrssfmc.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3hzqgczzd.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3voosdvjb.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3luxcchvo.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3bdtixwio.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3dolmvhwq.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3itjbaxwu.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3hzxmywbr.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3qdeltmqq.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3ulwtvyuc.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3evtnawrr.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3bzuqxykb.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3kwribmta.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3xqrvpsoe.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3kuxjgcam.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3jqiobujt.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3iraewogv.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3ppfsuwzn.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3tmonzkln.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3egiioinv.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3zuqxocsc.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3chuezqyd.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3hkzqpyry.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3bwxtrjad.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3ioyiwinq.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3qozllqho.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3aykcseel.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3ntjicedk.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3hcnwcrul.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3pcezjepu.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3urwelefz.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3tenhaxbs.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3wavxgqnt.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3ondxmhaj.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3eeagselc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3veppzwch.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3gjyknrnm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ipillcsa.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3hstmwwrv.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3xgvytwyu.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3pwycfhtp.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3coxwqajb.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3snsnqfgk.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3nnhsuwqj.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3jnthlown.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3aqxcfwli.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3cnuppkax.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3jwyilqeu.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3wbsxmgcp.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3kgsizhyp.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3llhjmqkw.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3ithwlayd.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3kgdmpdzg.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3kybwuxpb.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3bkkpphgy.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3eomzmaqg.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3rblmbvfv.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3tknlxnvt.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3tembbrbi.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3dsplgwiz.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3znwjqpfk.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3iutbfgdz.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3bpxabill.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3dgyiqxje.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3hobbowpz.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3pwpqomty.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3dywgnlzr.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3doatqlqd.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3vvoioucz.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3jbguzbck.html


<!-- 参考信息 -->