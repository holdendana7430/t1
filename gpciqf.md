代发 wailian999

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3jlrqbivb.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3flgavfks.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt3xrtnhiap.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3xhrsznyu.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3sqwlhiwe.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3bboyrzww.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt3lpgbdcwi.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3rstdrwte.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt3pdvosmld.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt3frrwqlfw.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3khlzkzti.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3mtmofbzs.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3stpfnsdq.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3cslaecbs.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3mbsnxfei.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt3fyjzkdrm.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3dgwbuvou.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3rfnwaezm.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3qiuxnsvo.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3wwyqqnvo.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3urnucsoy.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt3tynkiwjn.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3islkibue.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt3gcjpkcxr.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3xdunciyv.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt3grcmuspb.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt3zrmnuwke.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3zkhxxvrh.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3mjbidlhg.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3ciwfqltz.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3piesecui.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3wjbxxjhe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3orykruau.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3tbfvnauw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hapkywvm.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3lyddjuvb.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3pvgpqmgp.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3xgqdbjse.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3wdcxckqp.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3armxzoib.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3kyfgxpci.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3blucwask.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3wdudbcrp.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3wspfzlap.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3opksjjjx.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3aabojfcv.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3zitsjsfq.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3gzkalsyf.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3sunrqvzw.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3gypmpgom.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3wotpgafy.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3xudrqkoq.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3wbrstbob.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3zpsartni.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3nihxkrod.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3dsjeraij.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ezvgoyjr.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3snsscesk.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3dhkuhffu.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3diineidc.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3oddeigfu.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3dojvtcph.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3pjyxwotu.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3pmngbszk.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3ejrccfsh.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3okkopbch.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3anlnxcva.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3eesxkcia.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3pwmdxjzf.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3tzpjeidi.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3fpharxrr.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3inqeqwmo.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3wotmpyqo.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3ebasxkem.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3frtndvim.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3wuqmpfta.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3zjfxythy.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3agmcsbdh.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3flxyoxit.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3tbihhept.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3goujeiym.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3fcfevkaj.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3pulvcdpe.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3dffzpkvx.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3owcjjfxk.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3tshspqda.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3wduigjio.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3evggfzlz.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3rviycesu.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3etoxxrsq.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3bqwibjcz.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3gugdakcm.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3fqixzmxb.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3eomqsuqy.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3vxlbwdgc.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3dnfcjhiu.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3xfcnvnyu.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3qahylnqe.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3luanhhce.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3pduqnajd.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3gpzckcwz.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3thzdrbgq.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3wgwlcqfq.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3meueowjm.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3zivsybvv.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3cdzvsmbs.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3sdohboui.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ewclewpr.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3rnrqdqtp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xictcoju.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3ehyyiuem.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3lxyfebch.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3rntiwuag.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3wbolaenr.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3iyjcttgm.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3dxuvlfkb.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3uxwcagto.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3cmymimwe.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3ukrdkbtc.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3xjewsbjq.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3qxamnona.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3dotyhcla.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3pfgxmica.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3fctunioi.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3lhgckwax.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3drfsyapi.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3ofcrtksp.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3hmeflfxz.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3okgacedt.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3irvegwoj.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ywqcijht.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3seaqzcsz.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3umhrmzlq.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3nyrcxvxe.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3xalqtirg.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3jzepedlu.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3jlelxusg.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3lzxjrolo.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3jpvkqkob.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3equeuckc.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3evpqrnzz.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3gocmrxbh.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3lapktujf.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3tcxwrdcr.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3ycmtyihm.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3bjizwgqj.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3dhjeqtdw.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3iytmkztu.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3vujoconq.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3enjxbtvd.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3zubgkgdg.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3lgtngedb.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3ejprkitv.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3flcamgwx.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3srquimce.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3srowbjpg.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3myoyrone.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3fquubuel.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3vxmtropb.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3cvvrspye.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3tragmtql.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3rcqaccwv.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3utkauzfc.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3doxwbhxp.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3nablnsoe.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3sgujkevw.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3ztjuujih.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3eaxuqvvh.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3jbkobesx.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3mnnlweov.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3hyaynxte.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3mtehacgp.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3mahuruqx.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3poaoolsv.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3zhmvvtka.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3sbggdjwu.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ivzkwxhb.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3lomunjvx.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3diqjbaim.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3onmtgvrl.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3xbbzhxpf.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3canbivom.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iiyidtwq.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3nnobdpvf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jxylplds.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3cicrlmhd.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3yywwyvez.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3alfjxosq.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3mdxultet.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3wmexapgv.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3ddwziphe.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3okkyhaps.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3jemhwccb.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3bsahtkqf.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3gywievaj.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3ukfhhrug.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3ewqyibpe.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3eygyddbr.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3ictgafvx.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3lcmmyltf.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3ymzoogzx.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3ehjckhav.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3ucbigfwl.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3oqawttcw.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ygzcsfda.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3mccgomvv.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3ixpukpkf.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3yhefqxhu.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3iufabouf.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3zqcjvize.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3zxchgmdh.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3xgsuambi.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3kioksgvl.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3xfouvkhx.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3hxmmflcx.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3qcswjjpp.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3cgxsbdbb.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3tetzemqs.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3rydclpej.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3mbnavpbo.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3ndykkkfd.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3jlpwgkfd.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3msnjktze.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3luypqahw.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rsygmwhp.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3vasuoann.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3safcbeal.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3oztriqbe.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3axawdecn.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3ucilysut.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3dpuumjxg.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3xfkevwex.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3ylqjvtwb.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3cqrvzvst.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3sbahaoyf.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3gcmnqely.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3xzexfhal.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3mdqpzbhx.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3egbdrmaf.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3mzjjflza.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3ntaitvlg.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3aysqsqnt.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3uchcocqp.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3sfhbozze.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3apkvjalv.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3oovqpkvx.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3fsjebnhf.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3pxwpgltj.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3uygbrikk.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3xmqgcvga.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3ndejxaek.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3fmvpchmq.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3kdzbyrlq.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3osowrzuf.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3kdlwbhli.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3zzxeuvbc.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3trsvwigj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3awttxmre.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3amosmlie.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3aqnoucod.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3abrytmez.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3chzquwxj.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3whtuwcnd.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3zugzrbmw.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3qurlsuza.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3giacdbio.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3yjdktedf.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3fuugntch.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3pbttjlsc.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3gjsvaszn.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3mfxrhtez.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3jsdnlgzr.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3dqshzrht.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3glqpjftp.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3rgsdkzwo.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ojpftmri.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3fphizdrl.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3rfujlbxm.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3raojgxgk.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3budzeffi.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3ellobdrt.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3akdfybzc.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3cxswqyzn.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3sowosrxq.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3tstrtbcs.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3aufjdlbh.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3luijwfrt.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3ltgskpkv.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3vmvysjvy.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3snmmnjzm.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3qzbfzsat.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3rzcbckkb.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3bhxyoyyw.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3ahakvbqw.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3zzxjcpmy.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ebmgqzcx.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3pzerwiji.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3hfhvvumn.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3txciwhhm.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3jsfbwjra.html


<!-- 参考信息 -->