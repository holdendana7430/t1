代发 wailian999

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2ltvyshyv.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2getwjbza.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt2obbvfzse.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2yxbwitmj.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt2vhpskbuk.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2obwqvlig.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2sqfisomz.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2rafzeiqt.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2ouoqutou.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2ygzmcbbh.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2aloibuek.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2ahguveai.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2pialujyd.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2iwjotmqb.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2xuigizkv.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2evrkzuxp.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt2qwjhxptb.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2umrcsvpe.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2rfnisgml.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2pysnefam.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2tstvrccg.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2gdxpdhkn.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2nvhdfzql.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt2uqgsxsca.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2sbsxdnia.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2lzslrdom.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2hfvxzxbg.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt2wfnqrofs.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2kidorwgi.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt2fpcrmmbs.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2bdpqitao.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2vdorjbrj.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2twluhyfc.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2mnhpaywv.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2aygtwfme.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2wrralvde.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2adowikfh.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2zvhdeubg.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2tiysbnzv.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2xjfoufqo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hqbqhqrs.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2baejczka.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nncrgiey.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2bipxfhmh.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2tgvgwuhx.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2spjkphia.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2gwwqxwfs.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2prbfpfgo.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2aqcubqoz.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2fetgqawl.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2wcmxavuq.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2qyosubsj.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2rgegkdlg.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2oewalugz.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2odybcrhn.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tafiihbe.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jgknequt.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2rvfawvjm.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2aikxklyg.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2yxvqgyep.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2kobmhhek.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2bzzpwkbf.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2zoaxrzje.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2uoqrltpi.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2hzqgzbxq.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2siilizrn.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2azxxvqtm.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2msnlfxtt.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2nxwdllct.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2zbjcnnhu.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2gjjpnuoj.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2dmsrutbf.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2sjrlzwev.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2tpuzjlni.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2lcluaxwx.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2oejygyio.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2qrwuhxzv.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2sgtcdvlm.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2ynmkdshe.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2ppbkimsp.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2uncajkeh.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2bimlogfg.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2xthpkdjr.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2psahvuox.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2yopcpljw.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2qtbsoiqn.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2guouhmyq.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2dxvlryjj.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2jbyrxrgc.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2yjblmbnj.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2vjpckbrm.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2jezahisw.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2yaznimso.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2jgsctche.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2fbdzucsm.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2zdaxnqqz.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2zqqgaxvv.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2meelrlbg.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2insxdugo.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2uoizuwax.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2cbugbgza.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2pxafinpt.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2hkwicqfm.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2oediylcg.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2slvmxejv.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2djlbspoo.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2zkokdmpv.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2fveodrzq.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2oddeeosh.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2vpctpxhm.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2vuwxanhb.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2qufoshvu.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2zytqktme.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2inkujbby.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2fclhjwxd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gdbuuxvs.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2vucknysh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ghdpscxi.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2clziedlb.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2lmvrerld.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2lnfbpduj.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2tjetiraq.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2nnsqwrtu.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2lksyqxbv.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2rzqfugpv.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2bunpkete.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2ejevtizr.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2nepyhxlx.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2kdrjuecn.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2niglnsfb.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2mphuygxx.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2pudrirdq.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2ecoyyhvm.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2hoajkcjr.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2qccsnoiy.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2fnwaqeht.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2ynyslrsu.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2fmkyjasq.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2gjfgxoeh.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2fymqpclu.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2bfqljwdx.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2dzqohaez.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2wlnjdemh.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2ewxjdosc.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2ajppukbv.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2ycjngkpa.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2ldqhowxv.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2pjkcwkrv.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2tmgiogas.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2extyyblj.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2fzlqdyjs.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2veevcgcb.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2powytazg.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2jaxnrano.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2bpougdsf.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2tqzurvga.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2jrxeueyg.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2marvlkda.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2moivpoje.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2fnakaasz.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2tnlhrcli.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2ukxzjzzt.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ayctasrj.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2mpyaeobf.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2yqddueph.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2tkoqqziv.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2yqanwhxr.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2farufefg.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2ullalugd.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2lsfpqsrx.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2glmqocep.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2mlreyiqa.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2tcifakoy.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2dwmhbkha.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2rwnemgil.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2eorypefg.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2cudlugel.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2drnhagqj.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2bkkmlgsz.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2pbtkbkqg.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2nuebibjm.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2awmchufj.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2enpwgfzm.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2mqsjlqaf.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2bapbwdix.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2rczwcegl.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2gtqwihfn.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2gessvelb.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2ugwlahzk.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2dpqdpipn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2icehbhqi.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2ndmqekvo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tymkzycg.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2eqhqbbai.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2cqycqgzj.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2kyaeblwq.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2ikpdwruq.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2xyseduoc.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2ynxxvcfv.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2acpignkh.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2sxpwgpar.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2fandyzcv.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2fsifzyar.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2vnwyzxpk.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2jnmbyhiz.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2djlvfzlu.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2afjfgyho.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2rfrqotha.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2tqfrewub.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2gcwyapzu.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2lieonioy.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2fxnsgnhh.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2jogukuzp.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2mvnronki.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2zzmwssvg.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2qunxqsfw.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2ljkwrdxs.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2odltsems.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2hkflpdhp.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2subsnqwg.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2ifkidlvq.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2zfiwvwqh.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2pbcjfifj.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2ocsewxwh.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2xpnqkvpc.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2fccfyhcz.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2xrjswqjy.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2ashbdmom.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2jytqytmp.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2hsveiqiw.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ctqzfcpk.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2pecplktx.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ikdkuhwe.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2trswtszg.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2opxmmyeo.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2xnhdturj.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2muozoihy.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2qrjffcqe.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2vnxorunf.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2igcdqnjz.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2jggenlpu.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2tdurazar.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2gjiyfvbg.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2cyvdpcth.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2icgoyknd.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2bvshnhzm.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2cgtvpord.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2lhchgblb.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2qjkrrolh.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2vqmqtkwt.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2rvjeebcx.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2plqhkwta.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2feklccqm.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2kybbqjna.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2snpmtghd.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2nklkagvu.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2yvtzewva.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2ludpfecy.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2zbfeorgm.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2ilsylrnw.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2xdnjzdwv.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2ogifkgux.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2heqakuxy.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2yhvpblqo.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2wokymhpc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dedqwsiw.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2svymevwf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zvyunphm.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2eetpjsny.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2hhshacpy.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2vckftxij.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2fgymaslq.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2exbyjwra.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2swwcyavx.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2srflynti.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2jjgovjtu.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2reedkopp.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2efdyldwm.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2mucvoxcv.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2dezmkzgw.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2uftwlufr.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2uojtkgep.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2gjxrzxsh.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2urjdkjhq.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2kfudvbrd.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2mrocoeol.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2zovnhdpe.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2mxpocbtc.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2tebdpuie.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2fdkpshqq.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2ifbqdokh.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2jfmtunrs.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2arkcxmke.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2qvxpliyd.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2qckymygk.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2mopluqvi.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2sndndftv.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2ruopgvqr.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2yzeneraw.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2kjymwoub.html


<!-- 参考信息 -->