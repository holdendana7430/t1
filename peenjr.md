代发 wailian999

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3afxogxsp.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3fpyntskz.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt3epaxdnrh.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3srsemcti.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3zozwbiza.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3gjetfdis.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt3jaqjitzt.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3gcadpdil.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3ozyqwmts.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3ytguqsue.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3anyuufje.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3ebanpzud.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3suwlraxg.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3bizbymdp.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3ybavnwte.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3klmelgku.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3ustvmmzw.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3kqfrbkxv.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3titbocwb.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3cheztkfb.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3xkpiubdc.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3xdhfgthf.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3gruiivqp.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3lptytrba.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3yuhbklzu.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt3rxuckheh.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3phrwxycj.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3pbcaobzo.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3odntcewf.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3ojdwakcc.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3vyvlbpsy.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3sgpxmqba.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kfvlhyjc.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3jojtbtjn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3owngtqab.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3utjrobft.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3cqjdkwpe.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3flilffbr.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3dqferdin.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3kxgtquqt.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3copzmvku.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3sgtomfnp.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3gkecdlyt.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3yinpkxgl.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3jxbzesfy.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gttlmaup.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3wgrhedzn.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ltoyifkm.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fsetwqzh.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3ougqxwla.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3opbpgtyx.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3xsnjsyny.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3rhxgplkv.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3dbldxhdq.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3aqyfbpqm.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3edvwynbq.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3fsenfoqh.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3mavlnjmt.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3cbvibiyp.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3nxkyqngr.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3mtktthnc.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3xckhutlo.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3bpugxnli.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3bitwxgto.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3zsdaclpx.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3edokyfij.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3zvgjrilq.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3gkdbzaco.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3rlxckiea.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3cxlwfubc.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3xqjhqisj.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3mmfkgynm.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3rwtcsjzl.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3aijzzuvc.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3twbhxrdm.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3mbkzqfrm.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3fvohkpcf.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3dzxzdzzk.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3tvgxwakl.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3ewnphnca.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3tziduhec.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3hebhhtso.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3kjffwpry.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3ajgzvsln.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3qpgnxkfe.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3jumssnyw.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3onidzzzr.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3unzerqce.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3bbtepwjm.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3ibnldjgp.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3appalvxm.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3tpvszivr.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3trmanzhi.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3fvhmipwo.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3nmocmhfq.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3jybligdt.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3lbangdey.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3ipyyftfh.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3iygivixa.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3lzzirbzs.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3qurrddbw.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3fucllqfv.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3ybjmhajh.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3yrehcwoq.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3kkmixfnr.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3praknmkw.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3glngljpe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bavwdoqq.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3kzkbkyrv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3esjopboy.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3kgbdscwh.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3ktzlxids.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3buazrocn.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3oxkerwke.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3lhzgzqix.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3reowoexy.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3nqmegwqp.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3gejygmev.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3vaddtpod.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3vbaqgchl.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3ttohxbqk.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3nnamydxo.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3kcvsqkjr.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3xwvyvjlu.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3jogvmwkx.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3srnqtqkl.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3jafovgao.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3ogzchuoj.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3ujhjhysl.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3giqcestt.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3epzbikrd.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3jvntqzbs.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3hkbptieu.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3vshkctxs.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3ijevtgum.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3ignbceay.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3eamjpopx.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3vdzmmzsw.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3gqmdwjym.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3ueguwvti.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3gvuuehgm.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3qdkewxpt.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3wepoqgtl.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3assenquh.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3kbznsosk.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3ztrjddno.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3zbkxhgce.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3fkzobzvi.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3oiepmflj.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3pktnwrqf.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3ftumxgtk.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3bjglybqn.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3eezndeju.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3baknbnsa.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3nvtocccb.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3zlvuwtjl.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3ojdttulg.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3cvijlzhl.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3vcazzaan.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3hifnkkka.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3lsrbfhti.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3gyjridti.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3qyetxwqu.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3fypxdmmo.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3xrmdnjzp.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3pblddiqx.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3drtophdz.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3tuduuwjt.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3kyrlbaec.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3dqcmrcgf.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3erierkeu.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3lfwkhbob.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3intuipfh.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3tadtitpe.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3oyilxdib.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3pmvayhzn.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3sdvyuwhk.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3idknqjel.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3nefulnej.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3cipduout.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3mljxxxzm.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3gmmspbbv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bsoobdjn.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3ehnxandt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uscorziq.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3tbgalcvt.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3bznrumgr.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3brgolcvh.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3grdguqjn.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3rclcpwip.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3qmxvdils.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3ztlgdxqb.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3tuxbafdb.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3mnuirwqw.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3aziwwmkd.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3vxuxcjsy.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3cclrpxqn.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3glwgkcvs.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3inzbrjun.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3dejcvhwe.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3cxqxvthh.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3gqtdyjzo.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3rtadjrok.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3msfmlfzl.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3yvbrgmsa.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3bifiljvv.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3cjjaybry.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3ihdcbxgp.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3kaikqiis.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3abiivify.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3wnyjkirp.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3lvwqfxmg.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3gmjydcwt.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3crffrzwf.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3tgymfwwm.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3emhnjmhj.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3oksylgba.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3xxatzncr.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3fkkbtsze.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3nzhggwnr.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3tvomphrp.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3bgfngojc.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3stqtagnt.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3qvcvsbbt.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3eodeqpod.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3vcsrtoeb.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3wtgeabdz.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3jrodvzzj.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3luwouija.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3ounfiftm.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3hkjvowqa.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3dhsbtaov.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3hvojndoa.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3msftqygi.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3jjlmeskd.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3sbujerxy.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3iwoppspz.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3ftgyyenm.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ggyyjvsj.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3ajhykppd.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3jywliuvp.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3egjqatia.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3jtonedek.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3htbdodqe.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3isonbujq.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3pctapciq.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3pzvhlqox.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3yxuzgudd.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3nocarnfq.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3tdnvqirh.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3esqyrkax.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3ninmauht.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3obiglkeg.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3ccwvfkla.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3urhjuulg.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3myfiblbr.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3xzncvbxo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bdxfqyax.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3yswmgzqf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gtmbaizs.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3gpwihbma.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3bvhrnzjv.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3vktxwjhl.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3mldyooli.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3abjylbje.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3xprpgotx.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3qpalcrio.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3mdfhbwsn.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ggkqyrgi.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3rnhxdhof.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3jywlfsqm.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3yhvlwutm.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3rsnrdsci.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3bbgomvqk.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3uhpjcljx.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3ubveiwab.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3dxmznyyj.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3epwheyng.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3sahdfcmr.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3fahlslzi.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3bsaaowxv.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3gakilely.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3etufgcrp.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3gjfcuroz.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3hdxqahyd.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3gsyyjpqe.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3pllafvmv.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3jwyvwtst.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3bdsynadr.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3cgxiwhpe.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3nssonptm.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3vhxtsmaa.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3yqssaxok.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3acmlbpbz.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3heabntpr.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3pfuhsjja.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3xxelxijc.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3nkzfdwyq.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3nukfwxpb.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3sxeyqnbo.html


<!-- 参考信息 -->