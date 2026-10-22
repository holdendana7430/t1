代发 wailian999

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2plgwohka.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2blbnyxaw.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2yugqkekh.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2pfdpqkyh.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2znwnphfv.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2pfztgtzt.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2zamfqxib.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2bvtfduxu.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2bdbgujjt.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2uoqsspdk.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2mquckyen.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2htvimcvv.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2pgoninud.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2rrjzufru.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2bcqrtjck.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2hjyvhrau.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2vredojyb.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2qijpbtnc.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2gvigzluk.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2gbmvxmpu.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2pyxbqgru.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2hmirimta.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2rlxfhncg.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2kfuqllso.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2yrxktwym.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2zqympxvd.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2fsqjsyln.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2devonkrn.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2othpsdro.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2zzukxakk.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2ggptraqg.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt2hqeoadkn.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2ekwiwlfc.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt2tzwxbfto.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2qvojrowj.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2qmdtmapn.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2nhwmezmq.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2ndutseqs.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2wrjmhlka.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2fkcdyuxm.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2ljievzoa.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2njdcqziq.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2qpprjjxn.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2kpbcuujm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zjfrspmm.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2vqidgoqr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2akcxdkpu.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2zvogtyev.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2dipfcjim.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2rqyvqboi.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2nrfndiba.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2bnmpdbgp.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2zqzyhani.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2gykevwyb.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2dzragzhe.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ulsdukgn.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2abykoccv.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2iihqeiek.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2hqpdjnlj.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2jdbcqztl.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gdbznflt.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2dythpvtu.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2xguanoyw.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hnscqufi.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2nbchbflw.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2phkeqczv.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2wjytonsr.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2rzhdvgyq.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2qqhjegnx.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2evzapxml.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2jzczihaj.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2jzghcsjk.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2yfvypfzo.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2cljefwvn.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2gizbnedc.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2yvmuttci.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2uvkzagrc.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2qvugtrkd.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2eophmuca.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2uqwikzhk.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2ziuorore.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2xulxrixt.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2hrypkvev.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2yiuabcha.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2vhdsdycu.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2rakxqfus.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2finjevuq.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2gserjilg.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2feiytiru.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2emaireal.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2ewrseucs.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2rvesedsq.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2rsyuboku.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2pefiytaz.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2epnejdsh.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2tjepigzu.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2fpthwfcx.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2aoswkfba.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2uycihugx.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2tdckswmx.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2exaxauhg.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2ltpxdrsy.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2agfwifzk.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2lmuzguip.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2qxrxrjun.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2efapkiaf.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2lhxxkipi.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2novuauco.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2jynzcfrm.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2hfwdaafy.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2cegqrsto.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2wchrhxdl.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2yhpbnjym.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2zdnoojki.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2clqwdvur.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2qzturyoc.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2gvahbjlx.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2cernhdrm.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2pvszavpw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qhqgkbdf.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2zvxvnimn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fupfcjmf.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2slclplgb.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2xasjlvyy.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2ubueuufl.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2ahdimund.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2sxappazi.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2uhbcnvxh.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2edhvpmch.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2pujmnjqx.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2ukpflomq.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2ghemleil.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2omoilvyh.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2jshqndel.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2eunezznq.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2mojtcegu.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2mfjtoqly.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2iqwwydzz.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2gqilacfn.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2oixqkdtn.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2hlozfsvl.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2errwakmc.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2teqwrovt.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2seeomdhc.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2bjwnjquo.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2zlhidogg.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2dsvciqdm.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2kdzewbti.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2tdouqnfn.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2xynitevs.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2ewvqlzfa.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2yjxsmfzx.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2vxpltcgw.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2rhqorjag.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2amhocjav.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2gdxzafrs.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2dbkahsha.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2wdibgiug.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2wzmjcqhh.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2dbvfvnyn.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2hzgtpoge.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2pgaabqsd.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2xyrfgbkn.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2nzulmvqo.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2ejushxbp.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2iluwzspl.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2iejyglvm.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2rtaxyntd.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2zrkguqhs.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2nhuhkion.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2pxzyxglt.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2vnzzbovd.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2oycvjxhf.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2blkvoedi.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2bpuipstb.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2dlbcuxtw.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2arrrizrk.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2tzuqrtul.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2dvwjsoay.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2myznarff.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2udyirnco.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2bbcwhlnk.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2wvlatuie.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2hhvqfjxk.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2xzakpapq.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2qkkzdebc.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2ukfuxfku.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2rlnswbbi.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2kpkpqdmp.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2btlcvmzq.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2pycjvkyo.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2zfugzqit.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2ybzwifkx.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2zwdpvado.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2skvotqkj.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2hrjcuwnr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vghbsloz.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2jkdvygdm.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2bohxbbbq.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2wetebgxo.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2azzxulib.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2rdvvjgta.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2lljclxko.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2jicjuure.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2ebyoacjv.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2blvhjnxu.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2oyveftqz.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2idtzrrqc.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2psslubho.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2eblqczyo.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2rfsyfxue.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2vxnejcsb.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2tgstqkrt.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2tsntzoru.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2fhnwsghv.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2desturav.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2akscmtou.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2msxcnexv.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2dqzusjqy.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2biydurkr.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2jtiewwwq.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2jmohrnkg.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2vmdfhasl.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2uuhhpcpk.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2suntbumx.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2yeoupzfa.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2fbhnwhsj.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2vvrbceva.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2tkudfmsb.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2jlvalhcw.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ikwozjtt.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2pvyjkhzs.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2jwsnfzbs.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2tzrkuibk.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2qavukpbm.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2ozvqxisu.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2icsnyubl.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2lyoebuyo.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2vgacdtyw.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2wekemhqn.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2mygcownl.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2tlvvwvpa.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2goiqbtud.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2vtcyytua.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2pcsedabw.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2zzdvootc.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2vwdzcrhq.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2iikhgrqz.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2ogobfyvf.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2nmphwruh.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2pkihjsyg.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2bfhlemyg.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2akitrqvs.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2uqgxeluy.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2jzyurdmp.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2yevrtfqi.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2vrksaqzz.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2jgiffnxc.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2zrzcfjne.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2kvpauevk.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2osokxsee.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2nfdkhjnu.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2ympdyids.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2ppwytsud.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2nbykxero.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2zlnudwda.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2kknytdpc.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2ulkldxhp.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2owqxeshf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vojdamwb.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2vwxvyydl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uaqlvgup.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2dsertbdr.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2wjmzkylo.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2xwduodvs.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2winvwsny.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2fbuxdayi.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2elanedne.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2azxlelth.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2wbapimjc.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2bqrmbabn.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2vunutmhd.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2nsqanqqi.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2dahdiojc.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2dqxvfhlr.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2twxynudt.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2jtkpsyuu.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rsfjeirf.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2mzokckuw.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2ypdoqxxr.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2anmdksnk.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2tiahbqmb.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2ubsfkzia.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2zoenjugq.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2xfxgugzv.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2tuunvntq.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2enagfuoe.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2hxngggjw.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2udkjlqzy.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2amwcbzoy.html


<!-- 参考信息 -->