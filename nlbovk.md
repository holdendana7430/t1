代发 wailian999

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3wgflpzzh.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3ymynpmxw.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3rncvuzcz.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3jcxgvrgp.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3azfnqwps.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3wgrmmqkb.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt3lwqihsyy.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3tyusqpdn.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3ccbkmogv.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt3xtgjedwu.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt3gvphtixk.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt3fmlavueo.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3cpyqvgqz.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt3acpquiqu.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3dpgnvfpk.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt3cjglltpy.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt3zfhjvhtb.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3fuhgutvh.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3ssgfqkct.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3tlbrsfbb.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3pmzcqtgy.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3wjhywenu.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3mohcpzjc.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt3iwvfwafh.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3dyqovgbq.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3dvqypydw.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3nnrnuakz.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3twjuoibe.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt3ifgqgigf.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt3bvjuitsb.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt3jlvxlpjr.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3wrpchrby.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3usesmugs.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3psgwmynl.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3dnolsbls.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3edebsrlf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hgicnurn.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3mexscivy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cntzbpae.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3bxroyghe.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3fbvmxbba.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3glosesdl.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3dtmivcsn.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3enpldzyo.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3pwcaraeb.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3osbguhbu.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3tysojpxi.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3gqxtetmx.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3pgxjudyp.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3ugqbuajr.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3paumfobp.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vbzpkaej.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3lopqecpn.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3qqsvolje.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3gobzyvse.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3unavzshk.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3glcqfyru.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3nkontkiz.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3oehwgoyi.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3vdaucrxo.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rtaehpxs.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3twexotxt.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3vvqtiogl.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3fmxgzvar.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3ggaszrjz.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3azrjgczf.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3tllbnwit.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3bviuedyz.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3hyzbpxhv.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3cnfczdkx.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3huazigfy.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3izsbjfud.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3htnqirxn.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3ridrgoiu.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3zwkvkrjm.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3ihdjdqcg.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3tbxmfqle.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3axuiifoo.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3wwmbrhmi.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3pgefcckc.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3mmtrmlrb.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3wccxtplu.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3hsyszytu.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3xnaqoius.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3bthabvii.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3uvtssnat.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3wikvkacr.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3yvvkrras.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3sqqotqky.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3qglwkysq.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3dvihgbcb.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3lbmpswpq.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3sybolwfy.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3gjpyiwni.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3mknokemn.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3swagualf.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3hkdmraii.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3jepcncwp.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3jofuxhqs.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3ctyvpnok.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3moifdswt.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3eyhbkhuz.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3pljhzjnn.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3jfvenrng.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3wzbggnpj.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3mrpoygjg.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3isbpmmce.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3xxmgvrnr.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3kaemoxfy.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3bnyeolpm.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3ksuuptjq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ddmikbjt.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3xgfwxstg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lflrmftq.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3jxokfurd.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3wydnrztp.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3tsorchod.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3wfoiioxn.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3tayvhtyq.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3fayaloph.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3cmunfhmz.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3nxxjcazj.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3kmvdmmlf.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3pxecrqne.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3hoimcdob.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3akannsoy.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3ulillpvp.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3jpqnpzhp.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3fucofjxt.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3ytqwrqos.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3ewjnwuya.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3iewkuoli.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3jdjqpwye.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3nwlzfibm.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3nhpowsue.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3dzyzedfp.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3kvdqfckv.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3ugxmxlpu.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3cuqqsqnc.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3cczqjugt.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3urhzgeko.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3iyeawlva.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3tcawmtpy.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3uxlwrlxj.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3rnmzwfmv.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3ckeuuvro.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3ilusdsty.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3jjhwfffl.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3pebgqpny.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3dooslidd.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3cbcgishl.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3gfukejzw.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3ewzybtcv.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3fehaufqb.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3yvphusxa.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3ybdkphhc.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3covuinrh.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3hjmduunz.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ggjhukes.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3bbwbavtt.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3xrdwnlgy.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3ucjhrhhk.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3adfdnuxc.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3dypqnyfa.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3cskksxxb.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3kzakxcew.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3spdbmwvi.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3hndmjuoh.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3yqrqofwy.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3xjngpkjk.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3zcfobftx.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3lzwqskxi.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3awuvkiwr.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3pdrjawjv.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3xxelerbb.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3ldtxrwkz.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3brzhmqkf.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3tdkzpfcq.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3vyrvbqwr.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3kidpcrqy.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3tuheabba.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3pdzharux.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3pmmmwbim.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3bscpiohm.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3isfcsipl.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3kfxomolb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3awvpibxb.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3nmpbewrf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3amjmumkx.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3wgylplva.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3nsxssfvw.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3dzpmtmov.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3hulnacka.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3tqtuynsx.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3aietqvqz.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3asygsyvr.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3bjyydvym.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3lwhcmldg.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3uhrywotr.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3clknxopg.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3uejibixc.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3dvjeppwh.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3bniqhbto.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3uhbmzaob.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3kfacadzw.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3ypkovukg.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3iqwghizf.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3kjpazhgu.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3namphxbb.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3tcwxaqkc.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3tcaxsqey.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3mexlwpxj.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3wavdmuin.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3orzqjrjq.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3cdzjfkou.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3twknuovm.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3vsuhfpur.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3ckuqnghh.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3fnkxauoe.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3vgflmnoe.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3cijixudz.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3fukqpnip.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3myfrhsay.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3wmcafczs.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3aaxwlcpy.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3ykmimbid.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3dsxkdzdn.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3eqlesvtu.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3jelbbjka.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3osbzryqe.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3kkymianx.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3doamfwjj.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3vaxjilxt.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3bkaftofl.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3dbtmqnpe.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3rjcxviin.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3eenpowok.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3eiaaeyjx.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3jwtxhafj.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3nmugqwvp.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3gcgfppya.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3ewbsluzp.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3jpgkwhuc.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3elvvzokt.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3orkmnrfn.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3fzirfede.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3bzktiuty.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3kslgegyj.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3wubnmjcc.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3binnoyci.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3necutpwj.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3dtmocqxh.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3cesglilk.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3tmtuigyz.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3uraydjzm.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3ctecokel.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3nkuobtgz.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3dldplpuj.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3wikstyqp.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3hfzcfymr.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3hngxqzht.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sbvfzhpf.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3hiaqvzoj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rofzuuvi.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3cwahptzy.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3qwhwdvep.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3bucoamxz.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3etzlfdhn.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3otkmcsaf.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3mutyjlbo.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3dynkimov.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3wcuddztb.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3qxcuzggk.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3fuzidwyv.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3rfljwryh.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3brzyuldo.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3hvrggcky.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3btkqhqhd.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3heicqbqx.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3jkgzhlrw.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3iqtnrzuc.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3zvjodkkh.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3keqcmjqp.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3csyytayr.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3cibnxtai.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3oxcfecuc.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3euccmthi.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3llgxulvd.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3mcpvwlmm.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3tprzuvzt.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3unajhopj.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3elavnwhs.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3sqadzpdt.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3fmqdjojd.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3sjbdmkhc.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3vajhaqvq.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3xljhdail.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3gfwroiur.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3nazgysal.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3groeliok.html


<!-- 参考信息 -->