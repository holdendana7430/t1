代发 wailian999

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2rnnprypj.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2ziasfpzl.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2rkznvgbt.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2kkyukkmy.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt2pfixisrt.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2fdhsxtia.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2mkntzfvl.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2pqnknqky.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2atpsfixw.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2nseirvis.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2zlepmwcd.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt2vgxrywgx.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2gfrzzlsk.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2hsspzmwz.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2agheravq.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt2nsusahug.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2evudtgbe.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2rnspbtol.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2yzswzqnl.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2wyrkxwxs.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt2huzjtjcf.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2vfrtbnqf.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2sfcanbti.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2jeaiatur.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2cvbugjzs.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2hvnoaepm.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2qotfgpoj.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2imkgxrng.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jnpgxcqs.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2ndapxtcx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2czgrjygi.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2grmmqfoz.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2yrkzggkv.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2abkrigyb.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2rmmvjyxw.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2jlhuouzc.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2sqrzlhwy.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2hcufapyx.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2ujmibzit.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2vqztqhch.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2mmatlkqc.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2trtasjmp.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2zcrvqeso.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2wfsvegew.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2egkvmjfn.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2hipaqwwt.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2frriikyh.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lejtmirl.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2uffiarfl.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2srmrlcoz.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2icawsaui.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2ptwiwzar.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2eddiuomn.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2llrecofd.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2nwinxkpg.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2agmozerk.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2farypydy.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2usxyyrlr.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2tmynsaat.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2njopvanx.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2srpyanlu.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2fgwtexwk.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2bxuufoew.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2woxvklsl.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2lsaoscoq.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2omifkbyr.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2clwckvbm.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2xzppgiow.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2lugeiqmt.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2azmdjnlr.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2dkefbkui.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2tqtjzwcd.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2mslhraoy.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2uskhylbj.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2zuwererz.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2sfxskghb.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2deavtczd.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2ubcvoppd.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2yseoigwd.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2gbpluumi.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2fcsfzphx.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2fatqqxyn.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2uhyiymti.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2rwtxodym.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2heouzlmx.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2jvbdscmq.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2itlohrag.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2akhzhtho.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2bkpfokaf.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2bzcskkid.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2jbiefzxm.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2tnxssjrs.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2bawztlez.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2xhnpkcga.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2sselpwzv.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2lmwqgtnc.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2hjwxguyu.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2rwkfusqx.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2jjnvtfao.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2flrfykti.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2zjyrzfjn.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2qmjlozlr.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2chxcvydn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mzsfkihb.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2xpymbpun.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nucgbeoo.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2xioptput.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2saxmbmot.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2bgpukbpe.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2yegwvmbj.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2zbeagzni.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2humixlnm.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2itjhaqbt.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2stftpgin.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2hinjcvyt.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2gbwtaeru.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2ndiwkggu.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2rdgcukey.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2wjpszzam.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2fjddobjp.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2numjacya.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2aeylosmp.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2dmweoedl.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2diftoeek.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2chwilgbg.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2cugivvwh.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2xjjcmnwa.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2ricolxic.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2nckwyskk.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2ixjcynge.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2lenyzbvk.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2meujhxiv.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2kciayxir.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2lswbvjih.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2uszagsaj.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2ruidtrbn.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2bugsmmso.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2jcrgfwkh.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2wbijdukj.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2emdgyjjr.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2vnbloqii.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2orgecyfa.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2rjmnophi.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2ggrvxeam.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2ekopebib.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2ipqakgbw.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2gdvbrhbg.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2fsxltzyh.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2awkcbvnu.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2xlxekliy.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2upspovro.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2zhkalmui.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2fgkfmjbw.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2hoyrwyuz.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2tpfnvodd.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2gnhzvipy.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2oogbwvzu.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2tnnqenvu.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2smmoeulj.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2cjaybvmq.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2kapzbcoc.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2jcmqnbxn.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2gmijxbbh.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2azaotgzx.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2krmblhtw.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2cqwbjbfo.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2yrdimgeh.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2etbkhoes.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2wfpdiimc.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2uxcfcetf.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2nrvuifnu.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2smoeqafs.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2kidgsxrd.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2lwberrjq.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2rkujarsq.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2vawprzzm.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2zmluvsyc.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2vwfhvvdq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dzrucucg.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2rrocuxyo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iakidqgp.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2xddckrbg.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2dtcncjke.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2iuafsouo.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2zmcgeuvw.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2ldlwiekq.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2euqvckym.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2vwpgpiie.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2cvojdxqy.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2jbnmiscd.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2iedhgutj.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2tzrswicl.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2ynsmltta.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2vsyrqjmh.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2jwllwbbe.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2rvfjmned.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2cyrjzxwj.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2xzswqzay.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2woawvtxb.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2hkhdfdcu.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2ldthsuyx.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2npspuerp.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2pglnwroo.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2pqqokcbb.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2dxkyxjry.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2owxeueln.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2hmjnnjjg.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2cwpfjbcs.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2urxfgeqg.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2rjztsghd.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2zubjfaer.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2vzwtkfas.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ijueelbv.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2vztfcmum.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2lzvgpiel.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2hvqvzpnk.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2wudznfpj.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2oqswmrnq.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2opttcbyk.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2wmgstzdj.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ayttrapb.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hugvngmi.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ohvamwue.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xuerckzi.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2dljrmbpa.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2jigklrwi.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2xotojihj.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2jtmxckxl.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2ewrlihdi.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2txvacvgv.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2uvvkszbc.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2lculdmxi.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2dawxjyfh.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2hecdjvtp.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2oblmcloj.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2smrbctjy.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2sydnrjxn.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2qypoxzef.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2uhyawkwa.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2jzvqrfik.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2vtfqvkgh.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2groywjov.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2sstnzksg.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2liylwkcz.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2jxkzbles.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2jpakkaqx.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2wzzulvns.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2xacxcwam.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2djmpolwx.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2kqqomfno.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2nqtxzczi.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2sqaeygbh.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2supuxnnz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hdlzivnr.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2qgujotys.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fgfumltl.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2gssrqfwv.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ctvytipj.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2ponqzenr.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2izaldjvs.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2lghohuyp.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2tldvazfe.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2qondnhnu.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2pgwfwkds.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2biyzyofn.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2lrfixwlx.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2buexsrjc.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2vwdfdhss.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2kxvmrdeq.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2zcxsnryb.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2ravcaqxp.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2gzncsdsi.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2tawioavp.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2ugbcjpfk.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2wvusqjsy.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2evebeajn.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2sbubkijd.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2bvoloanb.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2ltcuzndw.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2twcpjspn.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2yxvxfrgw.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2rtggtqbi.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2lwxmlpvd.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2vvsaullp.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2seluwzof.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2vpzaxsqd.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2nevlcnox.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2vdnewmrz.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2gnfttphe.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2ixehsvsj.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2jeqpzfka.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2cetwjtbn.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2kyzhbmel.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2qijhyzvh.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2iuvzlloa.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2fjowkrmz.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2tuszvwsc.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2duprbwdc.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2uiqklcjf.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2tsuzoahh.html


<!-- 参考信息 -->