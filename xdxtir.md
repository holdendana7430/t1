代发 wailian999

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3ipscxmet.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3hwzfsfrp.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt3tilazfee.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt3negogmsi.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3kxdomvvj.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3yguwtavs.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3mhhlnodq.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3gpqlptjl.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3zgvpagxl.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3eluhrqpw.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3kcovfmdz.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3oucgwvca.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3grqmelux.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3pgvyizqm.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3rabwewco.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3bkusprxi.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3vdvxbrhk.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3fclineri.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3ialyawlc.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3vmstkldx.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt3ldtdiwpf.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt3gqtfzwop.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt3tkbsjvef.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt3reekmhor.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3fwiulibd.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3waxojijk.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3rqvnodpa.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt3blkipjnk.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3shcvokxs.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3ozxbmvol.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3ntywesak.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt3aynxfnqm.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3dqnzbgmu.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3suobpywv.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3aegjqhtg.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3pnwncwbs.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3aewlqvzj.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3hzjrdkyg.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3xfjlemrp.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3wjvgwpfg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dbnawqnd.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3npxxejmf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zzopahjx.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3hsezkxpg.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3dgpqtydr.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3gqteaiub.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3fnjmobwg.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3mmwajwsl.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3dqvmqwhu.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3kfsnbchg.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3amamxfbg.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3xpridbxm.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3ntgylwcq.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3iqqttcgv.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3lxuzevlx.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3epuozxgi.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3hpntbbyr.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3yvekbolg.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3lmtahioc.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mydcxyjq.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3wzcqebbf.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3ahrbaajq.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3fpgovefe.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3thgqzgov.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3itsebela.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3ldesziir.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3foxexakd.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3bdssblwb.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3ndjlpnbi.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3iiapysjw.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3ckksmwyo.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3hkdbugtx.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3hpxwysjy.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3msovfdkq.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3mibkqswh.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3bblwagev.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3cogepeou.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3affykbiy.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3drvmpxsr.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3pohqaasx.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3lxardwfx.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3qzjyeehn.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3sdqmgtvf.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3dpxsiimr.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3dohinsie.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3yzghxtdc.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3vcxpzfac.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3jcrcojcl.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3xndrntew.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3drltpkhj.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3bfauztnq.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3ojxqeoge.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3dfribtaj.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3bjsemviv.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3ygmranwj.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3fnffkypc.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3juibxbfm.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3hmmxkfml.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3tgydzfgb.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3fljwukln.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3jxrvivei.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3djisaknh.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3btkdgynh.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3mulrxbvu.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3umubgsxu.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3wejsroop.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3aajygqpe.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3nynoooev.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3yfviybwq.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3swokbdmw.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3hihjxshy.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3evuadiob.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3mwcpqqsy.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3hplfrbcb.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3pdyyixlq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ztemloay.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3yfcwdxer.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dbxrrhws.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3isbuxiwq.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3qpirijkt.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3jthynimp.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3rixoznfy.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3velcipmk.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3jwoykwoy.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3vyqdgnch.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3nkdpwnbt.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3fwbmnmyd.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3raqltjpq.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3qwrmfzps.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3aldrfzqh.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3ngfjbbef.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3juolyvuh.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3yislwwoa.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3mzivncro.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3xptedalf.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3ehnuylnx.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3ryvumjea.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3uzouqmar.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3dcywewmu.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3spurdtag.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3krmlkmqq.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3igbtbhha.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3ctoawdfb.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3meefgzvk.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3xwlljmsf.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3dfyomaza.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3rvqxftpl.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3xragimsf.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3fickegwf.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3xrthwvav.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3nenaklbp.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3krguztru.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3dojorzef.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3pdirbbnt.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3dkvtifhh.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3enkaftfm.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3uylghjzc.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3uknzvbll.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3hsuauocg.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3ltpfxxdr.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3mvfczrcl.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3xrtsyfiw.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3kldmmjtd.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3urwaxbts.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3rhckilid.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3icvlnoui.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3gmnpthbe.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3tpfqjsye.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3ytpbwuhf.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3lbcijbry.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3ugarxxfw.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3jeyiqrmg.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3cgndglpx.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3escrbwot.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3llzyvacg.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3pqkiguwa.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3rkubohyt.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3bbhltjwg.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3skhwjpyq.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3jtkpzimy.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3tnstshzu.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3inrgnwdj.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3hsglrhtq.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3wfzxqceb.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3qvfbycjo.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3rodslban.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3rskfadpv.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3yrswnsge.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3bislsmbq.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3qwylsxht.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yjlbwpgy.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3dpzcdqvf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iostengg.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3kqybnkrn.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3scstrvkm.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3tltrxkou.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3dzfatbzk.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3iriwfnya.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3kpwkepph.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3hjmklcwb.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3dmintpot.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3emrvpvtb.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3zvgcdopv.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3rkhnstcv.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3rncgdnxm.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3tnxmlygc.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3kmspgoqp.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3trphhbqr.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3cbtyovrf.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3ojywmwva.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3henujsxb.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3kjbbtdbn.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3iizqzrli.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3ndvuodeq.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3jzhunajs.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3ajnxlroh.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3fafhwhhd.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3blxahopk.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3zgqixylu.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3oghbegov.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3ndwxymrx.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3yvmseryk.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3tohrlpvk.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3bcqyklwf.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3bpuovmnt.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3alyzryny.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3ptwifzkp.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3kvlhetyr.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3iefaguns.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3ghwhukfx.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3distctrg.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3brfjznrp.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qqkqeqgf.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3hljsusfu.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3dxquagjo.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3dphwamvn.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3zakqijvb.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3crzcnnaz.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3oqskubsz.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3pimulouq.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3xrrwrbze.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3vqtvqizz.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3dxfxdsyo.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3whukyklv.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3xqtgoayj.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3vnmlosfb.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3myjxtcob.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3qldoiwrv.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3bqoyobmo.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3cwtfkksp.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3jeozskzm.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3kwlvypwi.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3ufcdlbzq.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3hrswvbjq.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3bukmmdyi.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3jvwnsznc.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3zbqyfmvq.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3hpqadjua.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3gkzquqrs.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3lsjatxyw.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3uiqprqdd.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3trqqqrlp.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3hpjxtsod.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3ebyenngx.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3asaowwie.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rherrrfe.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3kzixavhv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pgevllnc.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3lgpjuvdj.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ygdhrquq.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3jhowwfag.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3vqwksznk.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3jqgztaoj.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3vohethav.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3hnybrlby.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3kaweffob.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3gbdcvjth.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3uivdyefr.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3vyhaqdky.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3ackiummg.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3hxbylifi.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3zutvqtib.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3hhpexuvl.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3xnbcaoew.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3rvwjqbsd.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3qzloomxo.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3qruvcakg.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3zjqtdrqh.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3lmofxgml.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3zjnphauy.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3ulaxwsfl.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3ipiakhug.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3roszjogf.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3kxwxlvge.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3clvnhbmh.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3bexnyesv.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3odzfnqkr.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3arfhyrzl.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ddqvdfrf.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3mnfgyywr.html


<!-- 参考信息 -->