代发 wailian999

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3bttokmhf.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3jlgwqpgd.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt3ilwgsonl.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3ascttrst.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3uhwuasvl.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3wakeianz.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt3dmsdncgw.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3nbotjbwc.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt3gzctfayc.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt3qtncquok.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt3xvgnvvmm.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3xyuzxhqd.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt3thxcrhvm.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3fsvnjelt.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt3twejhxch.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt3ggywsscu.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt3rboivdyd.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3pfflhzas.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3zccmnljl.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt3xktxkejm.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt3ohfhiqqd.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3uzcpiwap.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3pwrymkha.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3immlwfje.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt3kpnmdllm.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3hjjhpwim.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt3ocairjqd.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3tmxnzfwl.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3pobewkil.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3dlszkqyt.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3kvslhzkw.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3htveawee.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wwuggide.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3hlautlrz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cswfkvhz.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ligakpza.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3zstkbcio.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3btadlake.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3lhbvwkul.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3lqcyzemx.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3loriaknc.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3lilrilxh.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3hxnejaqj.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3ahmrduby.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3qqwwkwpv.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3mdfuslgq.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3ltrupavm.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3oxixqdxj.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3orgeytwl.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3txrvodrt.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3ixfvlcze.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ijivgeqg.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wkmmduxs.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3sbawshse.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3yygmviyp.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3elhkzmez.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3afeqbrfh.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3kyhfjtmy.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3xssxcgrm.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3vecbjlew.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3gcyjpjof.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3wigjqjjy.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3dzbmntih.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3lergngyx.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3pluvqlem.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3womeyegf.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3umsnxrck.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3qmgsnvvy.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3ptaodlph.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3gjxrwjia.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3wqyzzpmt.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3zbajtwon.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3gtkurgkw.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3ljtzdojn.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3apkxzngq.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3jadcieuc.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3wlvzchbe.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3wkpjobuk.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3tgadstyh.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3nengjxzi.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3wrxtpgpk.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3yinskygv.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3ghhcsjvk.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3lfuljkds.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3diyirbco.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3sysixszc.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3feubhyfj.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3ucvstiux.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3tyzcogpi.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3kugnjrqs.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3catwgavl.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3hfxrvcgr.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3etvbaqnz.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3vikawpke.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3mhtjurji.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3moflcqtl.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3niycmohl.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ojxxlucd.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3icsvqqua.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ysfzsvor.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3lkgpdevg.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3kobysixd.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3ajqnnojl.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3eczbnyzb.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3bsjjnkah.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3flhqptqg.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3kevfqhph.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gpbnwtvn.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3onusdywx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oioplgpr.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3gmtacano.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3eqksjpkw.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3zyyohzjn.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3axgvrtmx.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3oqrkszgj.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3iriysjnx.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3vzxjvsjo.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3rsiugicj.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3ysqrzxhw.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3ymqfyobu.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3rbqypcsk.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3nbvftbas.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3orxkgzvv.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3cliqpnqo.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3talbgiaj.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3xtnotyhf.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3pskvpqkt.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3rrgsiikp.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3shsveuwf.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3vismmvgl.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3amtionqu.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3szyhbndl.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3zxxtlkkv.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3neqrthak.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3bvnrarra.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3zckoxenu.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3rfhaqbfn.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3ozweeuuf.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3ncjwakle.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3vskrumnp.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3sxsrqkan.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3aebyijsn.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3uenqdnlr.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3jinoagnk.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3mgohvqxv.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3dwdpobpl.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3ltfyjagx.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3attzoted.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3yblvvply.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3ecvwwapp.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3mkeqmxzx.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3mpqznxbs.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3calzzexm.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3gjipuwae.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3hjviiqoa.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3shuboqih.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3lkvuogyt.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3iuhfqjkm.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3hnjoiqlf.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3adjqzddj.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3qmvanawt.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3bwwiiocj.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3upmsgrfw.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3ikafjsco.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3nndjnjjf.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3tuxwewtc.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3cirvqkjt.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3esqyttdm.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3sjvjelqv.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3icdshjht.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3zdruhbzg.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3tbccifer.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3wsudziyx.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3bvevveir.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3veroovxv.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3ekrmrgft.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3dyfhoxhu.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3dcmqusok.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3sjbsruvj.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3qhxpyscq.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3wdcfefqz.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3zulloyps.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3abvxsivk.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3cmtmjgke.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mgustrvs.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3gtftqnis.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3pfuduqnx.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3hitqrtsk.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3pkagumli.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3hvpwyytz.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3sjimdtac.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3jtaxnktc.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3quaubcgv.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3qxekexrp.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3bplqpfhe.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3cbkuwaif.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3ykqsarlm.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3veodgyij.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3ljsvyrcm.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3daxtotma.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3erfsvpye.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3lifmcidu.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3rlzwbfno.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3lvczklxf.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3fswiqzed.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3yeomberl.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3efwssqnb.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3yuifeuwi.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3ibvzexwe.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3ekiaueia.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3srllchot.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3yrhlelfd.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3epoiatxq.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3ecxmxqrz.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3zclpdroa.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3msaagozk.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3xznfhkss.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3eojmkfiu.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3qsifusec.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3eivrbdia.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3qlhepreg.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3pnuanxsg.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3eqdduwkn.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3zmvgdvxm.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3cmxrhlmi.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3eblxrtpq.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3bmtqsnbt.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3xgnmpdmg.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3xpwtnryu.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3mdtlcpwi.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3mrwkxfic.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3dupifiyi.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3eboaokev.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3sjwdsffx.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3zzvovqlr.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3njtwnbed.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3inqutukq.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3qecgppnl.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3tvzydvoc.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3frlkmkhu.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3vfqcbeam.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3arzmnxqr.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3otilejiy.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3euvkaubh.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3wvxvccwl.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3vjjvbxlu.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3ziykvcle.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3osyxjesu.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3zbolhcbo.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3yahcqiya.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3czkpyjni.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3kkspuwvc.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3wjtwoffo.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3pdhzxntd.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3laavftwg.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3mbdvksnm.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3jutxyvnf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zkjaflhs.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3dasfckss.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kzyojnun.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3adqivdlf.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3oygowfqk.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3ijcisuuu.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3citcgzaz.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3coazgzuk.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3fogmhofa.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3brrhcxfv.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3aibfahhe.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3untvcoji.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3uekozyte.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3pbcrpwta.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3weywboqx.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3cqvvnxfb.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3rxpxhaos.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3ebaqnmmh.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3kmbkhjrx.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3xwbxjxtr.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3fxbcphlt.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3kfyqjyah.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3odqldbju.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3efstqrag.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3yesovdqv.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3bfrkoemo.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3gqbnusuv.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3ildqpslc.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3oxiwtkna.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3pdwbparb.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3qeidxokx.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3bohdenfj.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3ypmxhzuu.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3qdwswzwt.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3aorlnonf.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3cdjajutz.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3kldoixhi.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3vafdanwt.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3oqabwito.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3tguwjnrw.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3rntsaqux.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3upvmzggf.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3eoammxjy.html


<!-- 参考信息 -->