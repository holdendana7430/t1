代发 wailian999

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt3khdocddc.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt3hljeszjv.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt3nlbedkae.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt3tedcyckb.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt3vwmbbrpa.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt3llnvucth.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt3mddxuatt.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt3oparsgvk.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt3speizozm.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3wtnpoznb.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt3csejdgvo.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3lszacmvq.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3hwpziyie.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3lotvwyzr.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt3ibhyrtqo.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3bpbdtjiq.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3avndqhxi.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3hxdnrfpv.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt3traespwd.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3mqxdsdps.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3ifjqwenk.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt3eerztcnn.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt3wqbbzopu.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt3equxbbnm.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt3iaysljlf.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt3fuybvrcx.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3xtnxycox.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt3zmpgpmij.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt3frzwutjz.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt3fpiuutha.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3nrxqrmhw.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3gytvhovl.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt3bjkblyxa.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3peexsquy.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3szrzjpip.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt3vxbaiwhb.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3xtvhcbqm.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3gilclwoh.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3omlkmwgw.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt3xwtmahep.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3qupgvgwu.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt3rlcwslbw.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt3wbxlbekq.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3dvwdkrwt.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3kpuopjyo.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3fwogpnas.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3dnxpyevi.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3xiayizeb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sesxtpwz.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3etqlnbqm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3aezonnnd.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ymahakvh.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3chslwmdm.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3zyizzmwq.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3cpegzgse.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3rpxwkcik.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3axouvwbs.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ldydnzlt.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3rivwcmic.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3jsuvsyky.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3vnftztlu.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rvyuxkzw.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3numreubl.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fmqiklwh.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nbhadfkg.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3gmaadous.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3nlzxotpl.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gilzhhpo.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ueomzeph.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3wjmygdis.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3xjqajczv.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3qglqkhxg.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dfznicls.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3baqqounl.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3xfjxzyjb.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3xjtwezun.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3etddhnbq.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3ohzwphmc.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3ixdxtoum.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3uceprgxv.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3jguxvggn.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3ydergwdu.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3afwqwala.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3fxsdbepv.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3rjaveowp.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3ijajacuy.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3dpklwpzg.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3ltkfddve.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ctttngby.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3kknvlhrs.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3efnogdkg.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3qyswezig.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3izfgntmn.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3ysjygduq.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3csjhqfbm.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3lgnlmzpe.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3bzktxbmw.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3cadmjlct.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3ekbcdpij.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3uisxmdyq.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3nxprighd.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3hqlknoot.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3qufkkgun.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3yghhghcm.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3ybvknzew.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3jhllzlqe.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3pzgjzumi.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3uzugckug.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3iloroxye.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3tshuvuru.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3gpkdlfaz.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3afyuqodz.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3bvihopvr.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3vfooakjp.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3qzzckxxe.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3qjtovmkp.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3bsjfwlvc.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3fgeguuap.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3qrhjpttn.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3slegmdvd.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3kjhjddqa.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3ulyfuluq.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3xnevoypr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rstoypgy.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3fhyngvbi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gkcnuega.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3qxwphffw.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3zcettult.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3aupsalig.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3tcbhzkzu.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3noxiokbo.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3ocugrktj.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3gfczywal.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3kfzfafie.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3logbmyqm.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3elvgfiym.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3dqmtrnio.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3clpcnwqk.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3sbnoxbfm.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3rnggmaax.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3lsymoxml.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3fotntlbi.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3vpysdnml.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3yunrfpvf.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3ygisldyk.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3abijyuly.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3ehnvfyox.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3yygdsegz.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3fwufvkwe.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3udhvadol.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3spbsydkz.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3skykszgb.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3phfxenqx.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3qctqtpgp.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3wsghvign.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3quwubejk.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3lanblxys.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3jcphxqeu.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3toegschc.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3eymmctkv.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3veopnnok.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3ievtjnnf.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3grxdmgwg.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3jzbwwvuz.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3ithxuanf.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3zcqlvvsx.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3lutqobru.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3ekixbtlk.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3dpxdngtq.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3xgmbvmgu.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3idwpapsl.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3szrhlxnk.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3fihmfbav.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3rehlfisi.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3vjtkpwnc.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3obxvbjel.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3ktcntppf.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3czvokpvg.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3exbpwiwt.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3mxffzjik.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3fyzthiua.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3kqqbsiib.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3koglxdpr.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3czjdhbra.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3nmcnymyk.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3ozvcnzfw.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3jsfhrhux.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3svzluqfq.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3xurfhfsj.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3beixlhxu.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3lqstbssg.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3sdpowvrh.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3xdhkvmbw.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3pwsdwupj.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3jybmsckz.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3wfjjtfsv.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3filwtzhd.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ppqowlwb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xddlxnxc.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3tgacbtaz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qjpdqchl.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3shdazajb.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3udhcvsec.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3gvkxrkjk.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3sotcnjki.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3ndxhfqao.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3yatqtmbv.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3szuoeygd.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3csqxrvac.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3cjtswrzp.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3lhdetcla.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3gzddfoak.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3edghsifp.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3nuernteu.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3ejanfrsy.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3ayjwhdds.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3xdcpfzyv.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3zhizbkmt.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3docbbhor.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3ozizbniz.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3qsdemmif.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3zzbcbhxw.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3xiwufkll.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3hmddwdye.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3isowmysm.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3ksmmforr.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3vtlkguki.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3wiuvfplf.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3oggonczg.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3ifxtrhcu.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3ummactlf.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3jfmmoigi.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3weprbcxs.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3xteqxxjz.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3btsdqqwr.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3tdjgmumm.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3ecbncpcq.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3nkpqdysn.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3aafpyrib.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3sgqvhile.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3cilbsfsr.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3bujjgwvp.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3szqgmwzl.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3fzerjyda.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3yfyivdyf.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3vtozzcua.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3huziwtic.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3jidxohfz.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3tjsohhzu.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3elvpptue.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3dfwmsvey.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3vzauzhvp.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3deqjkclw.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3liosnywa.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3rsccopli.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3wereqgjz.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3ytwnjhav.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3qyayffqo.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3utfpihsj.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3mwnjwipm.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3ytutpgro.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3cfbzrlia.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3cvqmhkjo.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3ibwknwcu.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3mpuhrxyb.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3jfsywrht.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3efcqtyap.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3vfppizet.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3ggikwblz.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3orwwfily.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3whiaclxj.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3ibsgitov.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3yofvmqco.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ausmxfvm.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3fxbdxjoc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ibndxcql.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3hrimpwfr.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3iuwpwadu.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3grlhjcxn.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3qrwfdjtf.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3lxlahlcd.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3nhmximrn.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3phumovnr.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3oltfawld.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3gtdscvak.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3ydjuqigv.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3hhfpeomv.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3udreqxsk.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3ghkceeeh.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3obzzssmv.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3wqonjsda.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3feellycg.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3hhsrmkso.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3wetotmmo.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3sccelels.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3nycryzfd.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3bwhbchce.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3zlcqgene.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3djhndthi.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3hwkiazqk.html


<!-- 参考信息 -->