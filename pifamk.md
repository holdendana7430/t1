代发 wailian999

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2kglczmla.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2mprmhqcd.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2lwcwxcme.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2eobxdvkq.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2ovbmbwyg.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2bvwavpln.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2xowuoccv.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2mhiunvgn.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2honugxyi.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2yrkucbre.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2fuzivzun.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2uqvflexh.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2biwcxcku.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2engafsnw.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2unmdhvqs.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2cvlscdwb.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt2ecsmqels.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2ykjjnvhh.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2kdylfwgx.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2pdqutvzs.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2ifavoouy.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2wtyvpkpo.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2npioibmm.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt2rviefjoo.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2hxyvwliz.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2mbnffila.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2krprefgf.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt2wyqnnaqz.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2fyfkiepq.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2yicwjydr.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2qqyrxqkv.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2qawcdmhu.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt2mgmzktez.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2racffonl.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ixludeam.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2jowmrdeh.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2swkwbzeo.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2rsocobdc.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2lnkfirze.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2tumuqfey.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2grpyofgk.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2ibevfcmn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ypguhmnk.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2aonwnllx.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2filkoyrb.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2iinmlshs.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2rloybnrt.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2jzjbtdji.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2npknfobj.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2qlamxilq.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2vtiugnnz.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2bnfluocm.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2kyyoojoz.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2faahrqck.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2kgajnyie.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2guunhlgv.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2immgkofb.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2fkqnkkxr.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2yxzssbzm.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2ehvqxioe.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2naprhlck.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2vbkmlotx.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2udppjsnk.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2elzawkfj.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xrnvcjah.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2yegsmswk.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2hvhgonjt.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2idllacwb.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2toeisdna.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2bqmlhixu.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2udbqofjn.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2nshnmiau.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2chsqonnt.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2zhpqgpao.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2qnuwdaug.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2xzgvqjdc.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2igxrtwwc.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2povetbzf.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2jsjpliqq.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2nfvvixcn.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2slobmjva.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2tpobafkn.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2srhkquwp.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2utgkllkt.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2sgeihsvq.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2phjmehkr.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2physnbba.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2tmegycuf.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2vudzeiwv.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2ajhuypyq.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2xvsnzxcq.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2xrgihxkq.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2nsrmgojn.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2nfhedcrf.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2afxjcuci.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2fpjewauv.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2hgohmije.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2vkhlpkhj.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2dkbqrsey.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2sqyoqloq.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2yfhfilur.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2uvkitiou.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2iivizhho.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2zkkapino.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2lyxhtwcl.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2uzpfrlsi.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2iuuhlhbf.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2ervlcrna.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2tdexcxql.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2pwhlzcyt.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2zlmganca.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2fokpcwdj.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2loiolhkr.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ezlzvbfl.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2iybdmroj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wqemwghb.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2zeqbtlwe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kqucpldi.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2llylmecn.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2ireiqpef.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2smvzzxuk.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2lqmoiwzi.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2bkeciuvo.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2lxljdlro.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2qirifxbq.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2kvkmrnqn.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2wcqhvoqh.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2ayyqmnfb.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2ysfdezxe.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2wgoytkvr.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2onpznlhr.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2rwcqjslf.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2pmswcabg.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2tcablagy.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2bagdbewl.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2tqufhmhi.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2ksyojpiz.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2yyrufdhc.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2fpfhmuea.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2cpzshhrw.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2jbanlexl.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2uucbuhtf.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2skhiemlu.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2rfgcqstm.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2xsszjxnf.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2ytmixfzc.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2wlcthxtg.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2lwzjiymz.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2hlxrcssx.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2qzkovczu.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2xfjfgtji.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2rhvylogs.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2kvaqvdnr.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2gnkcsphn.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2bakpeexp.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2dirhxdwq.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2cplwagrp.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2koowdttl.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2qvzclmjt.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2mpvnntuq.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2wrafufqs.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2kzjojxzz.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2qanwpmim.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2txizlsjm.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2wqfvlmjr.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2nivoqpkf.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2halinwhg.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2vhovsokw.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2qkctdspc.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2nzwjiorg.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2idvghcum.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2oykjeywh.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2oysdtelv.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2sbxsatwg.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2keysgajj.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2lykuties.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2cvvoqfey.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2phgwkbgl.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2nsjceuzs.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2crgscewv.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2ggqfmxfd.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2rnusilbu.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2jlxmgizs.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2bidmnkjx.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2gmfnilte.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2zcegggls.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2vgdyqzxu.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2mygucouv.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2ehsewtri.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2sxtnpqpu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2emlivfdq.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2uzmqalhx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lnwlelxy.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2lzinwqop.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2enwwrdtm.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2mfswxeiv.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2rfkzsaac.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2euapbdvj.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2feucukuz.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2fihqjefu.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2mlmnhpzh.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2xqiktihw.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2xtuirkyn.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2hpvuzfyr.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2pclfrbdr.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2xipssvdw.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2wxslsxuv.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ycqolqjv.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2amfhsmmg.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2crbuoveo.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2vohmfzgz.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2ccfmyqpn.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2scljixsf.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2obmmuryi.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2slrhxoet.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2swcrfmck.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2vqougwfo.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2drrboqhl.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2mxbdwwpd.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2pbgbswfh.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2pttyxniu.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2exxvlyxi.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2qyycxzse.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ishphnyd.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2xkunwari.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2dqtrebnm.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ilakdgkn.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2rudpruct.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2wchyykbn.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2bxotcyds.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2nmifljfs.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2qjuymnra.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2hoagnbhy.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2cufetrlq.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ccjurcmq.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2lmcknoew.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2cdevkdps.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2yhkncola.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2lpxxsyuo.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2wngsxhac.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2pdixyrog.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2yzsawbgz.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2pctvozfm.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2iwefzkrl.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2nzgswjos.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2kcscofhz.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2resfemee.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2plxzcord.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2lbqvitxh.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2nljxbqlf.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2rpcyzoet.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2fhojlrhd.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2ugnmjsyv.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2gtettrxr.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2szaiaetq.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2zlvcsrqt.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2ggidbjnp.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2ifqmerzz.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2kwcohned.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2nujzwpzv.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2yholavys.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2kztfkakn.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2soiuktow.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2stlucogt.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2ywaclfeh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cgpwioqr.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2kydmrhax.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2orvxjgnd.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2jbfkvqns.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2dwmdqvus.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2lwrxfghl.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2qpdjtbet.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2oadsrqux.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ujdzqvde.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2yzugeqyd.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2vivozbgx.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ohdmhylt.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2oscsvxpg.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2sgbfglih.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2pusqtirm.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2ifskywwp.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2llfcjjud.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2kdywgvdr.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wgbnqwya.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2hkoaxhsr.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2hqwtrlui.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2fhsfkcmt.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2egfspapn.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2sfhaushu.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2qbwdjfnq.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2dwrzbvmm.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2cowdbmgv.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2umdiifxo.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2vqmemyzm.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2lhqxxinv.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2hpuvhkho.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2pmqatvdr.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2qqlijlrj.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2yrcpgfbq.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2icpnovkj.html


<!-- 参考信息 -->