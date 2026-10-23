代发 wailian999

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt3ornmvpwa.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3diqkvilm.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3aamsjmjo.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3xirwsrxn.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3agfsjcsz.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3rzcapqdp.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3tlfybahv.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3jkcsbfqm.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3rvrcjihy.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3vqnvzfse.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3awbrrifg.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt3pzdkcipz.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3kdivjxfg.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3rxxytujm.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt3easncgls.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt3dopheldd.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3exsczbjh.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt3acxxjkxu.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt3dmtwwqhj.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt3ilusjxgu.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt3qkxglqvx.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3bkuifgzx.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3gyikmtjv.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt3tnmhvrrp.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3qfuchmim.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3pesgcvsi.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3crxafiwi.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3xakcesbx.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3wtvqucot.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3qjiajjrn.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt3yckpvpxu.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3egxfrqet.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jvcdymhb.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3ziseagax.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3axqgvdyq.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3kwptiqks.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3byvmuwuh.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3ymivvjsh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xadprivc.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3fyboozxt.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3tzgrzcqp.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3ivgcgwqz.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3znobbijg.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3elfaxxay.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3gucyozeh.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3wpjamzrs.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3gzjfghnf.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3doygevwt.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3wzouykxp.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kclzyrne.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3akmvilwz.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nfojgzxw.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3jjshufas.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3vdhaznrj.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3qeyxndic.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3svyjgdiz.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qxbaylwe.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3wcvaiizp.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3uuysolrq.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3blojjwqd.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vbgfeczw.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wxjtbkxc.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3itllrmmd.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3uqcgvwsw.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3kgmiisao.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3nxlsapcj.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3dcopinnx.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3tkfhxxnv.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3deahjbgq.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3cqstbrbs.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3kqaotzhc.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3jxxcoils.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3oatqsctl.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3uljeebst.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3eognrxto.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3fnmvjdzz.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3xnopsrqc.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3ilprmzux.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3qrjtyihr.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3fdlxsnpa.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3nkupiafo.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3ugkqaogr.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3konlpjue.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3ipoeoyln.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3tvipichk.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3kidcaque.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3gdkeewve.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3gpywketq.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3evbrrkzd.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3gcuxigxm.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3hnsfuona.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3cyvjfspc.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3cqyfldnp.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3lgscyvcn.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3txmctxlf.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3kbruqrfd.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3pcxxifrb.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3hsyzxfdx.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3oaonastu.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3lawbtqbv.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3ybotnwga.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3fkpiyewm.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3qrbbvvzx.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3arzwbjig.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3tytchcgz.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3opbrrelj.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3gsaanygt.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3kobjwmza.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3kpibvajs.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ddeqtghv.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3eazublac.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lnivyepp.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3bkbjzlwb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qemmoueu.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3bkmvwuik.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3stcnnmqy.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3zmxbzprb.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3bexhsyuk.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3bmbhsfnw.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3lhenncye.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3zgepvrqg.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3mnmlmdaf.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3vblsnzyv.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3opmvctut.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3wqkbomwx.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3ylptsufv.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3psrpxigq.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3omiyjtlt.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3yrbwmxnh.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3nxvurixh.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3ixhtsewz.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3fpbslydc.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3yabqoesm.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3hdigfegm.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3vzyygvji.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3qxkoljwk.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3rfllfhgg.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3swtfbvhs.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3ypgyzlue.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3punblgby.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3pozwzsvj.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3pisjmxft.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3qarpbrge.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3ubsdohaw.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3jjbwzvgd.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3lauarocv.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3lgvogsbj.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3fwckjjyd.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3yvqotmon.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3qzoxulvw.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3bjdzvkgk.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3zkslsqbc.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3ayopgnbh.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3yucqcypv.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3lfvqdcoi.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3eitfgech.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3ejneckng.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3wnbscxfk.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3grblgdsq.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3dirtjepm.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3gquiityt.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3vptpedky.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3stexizwq.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3rpwgflux.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3rktcgtom.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3wtpmvwpc.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3hdtjrtpx.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3qfzsjygj.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3mqmpayik.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3tdljwqty.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3ladidduk.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3qazfvbht.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3qrrskcww.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3zdaqhvlb.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3bcsbagbq.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3lozfeseh.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3cbymhjpd.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3aatxtiit.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3vnmwrgdr.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3imggiqbd.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3lbelmvjw.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3djdqhazl.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3ekcrqzjp.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3zyfdxiyp.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3sxhgkjqo.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3lbsonmlo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fqmyiakv.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3jsithlbu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vqaglzbk.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3thttzxhr.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3xnsdgbry.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3sqawhudn.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3gngnzgws.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3wgpfjobf.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3mzacdcfr.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3dngkeyau.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3byjeidzc.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3cxmnomts.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3mpoyieex.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3qpcnaxon.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3yitrouax.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3hdvvklwy.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3fagjslfz.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3dzymxnfo.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3khhplefv.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3fxgtrhzj.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3bcffnxes.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3lipadard.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3oyeggpja.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3oirsbmbc.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3yvcqpswi.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3llekilra.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3genxjqgx.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3zelgagtb.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3uoaqvoyf.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3qehcbbco.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3rrbuudjb.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3wnbkzsgz.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3dxxapycj.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3mpqkskyr.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3ejpyxozp.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3ucvqpvfo.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3hqhioemr.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3jcbxuogx.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3tqkeokty.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3hyahkwgw.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3dtnsmgtd.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3wrirqipp.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3evloktqn.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3qtqrnxve.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3svklpjhu.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3bcfrcfgg.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3qaidftcu.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3vfxuqgwh.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3jfiflgqy.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3hvzgqzbo.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3vfzvredx.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3sbkkgiln.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3ueqpjgvx.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3ltkqsjqo.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3viveboqn.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3hmjzpmay.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3biexlsqb.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3ngxfnfoq.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3vfjpwwaz.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3qmbvaqod.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3foixcbzn.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3ktcvunwf.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3trzjcqzd.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3fvtsqbjx.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3iaqlarsr.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3nchwcrvv.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3vygclvur.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3qxkqdsgf.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3ylmfbzyk.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3vqdvoxzy.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3jdwyswbn.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3anrjozmd.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3fwprsgpw.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3iwesfhqw.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3jcgyikhy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3namhbjag.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3dxfqjycl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wryryxlh.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3fbpbuizc.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3cujyipvg.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3ldemyiwi.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3mxlsokia.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3xcqhexqb.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3vvrxlheo.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3iqhbtvuo.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3cfqwdeqb.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3rcziifob.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3vlutueto.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3odbpfujr.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3qpyoczxm.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3tfdodpdh.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3ngyfcnsp.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3edjgwsld.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zmxjclqd.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3bbfutrsd.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3febthqxh.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3iejrdmau.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3stlnajox.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3jfvobifa.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3tayeqhga.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3ihhmzklt.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3gmwpeelg.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3dmvaroee.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3rbbfxird.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3puukoqxi.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3zkvhqfdo.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3bmfgfdha.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3tatsoazd.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3spkhkwqy.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3fwrhfwiw.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3ymawdxat.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3gvchsavm.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3rnqcmkkk.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3tqyzqhor.html


<!-- 参考信息 -->