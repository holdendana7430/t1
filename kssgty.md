代发 wailian999

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3botnpnap.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt3pmvylopo.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt3sfvbznex.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt3dkihdxwx.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt3rjpzolks.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt3fdtjazlj.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3tpdhnwtp.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3jdxdefly.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt3aajwblqy.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3nkwxcrpj.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3rywkeafo.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt3qhyhhawx.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3vkgxpiwg.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt3oimfdtaq.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3uaiwaxlq.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt3oewqiamb.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt3ombupgfj.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3bydxnkal.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt3jjkpfbkh.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3hogigrma.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3tkvctlxj.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3bjozbwgk.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3zmbgdnch.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3kbhoopcu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gdslxzbp.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3vvxfpjpa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bzxummlq.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3hmgtjkmy.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3lurennpv.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3rdspmjxo.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3oqfpkibo.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3nbdeqhri.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3segpmwts.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3rheyuadf.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3hzvhmejs.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3ygnuptdd.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3jhyxevsp.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xgtgpatx.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3ywctnrne.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3bzpemxyi.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3pcwveklz.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3wxlfdqbe.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3qvibftdo.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3hfhjxjbb.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3inxarvds.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3lnzbarmn.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3gklhqndd.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3azrdswxc.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3nnoputdc.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3sdshrtsm.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3fyhjcclq.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3pndaoabg.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3ocuqxbkn.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3jityaont.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3iyepzmtu.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3phtnzzmq.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3ordszkor.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3llforblh.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3dihcgnym.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3wftzoclb.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3gqcyaiig.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3yssufsex.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3ekoljifa.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3yxwrmphe.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3ducuavcn.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3knoeucwe.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3wdtsdocq.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3flsretpz.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3pxihbmfm.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3vaxukbzq.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3hafhqwbx.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3rezihddt.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3jclieimq.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3agyhwblu.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3kgzuhuqn.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3ckquoehd.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3rwyoqgse.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3hupzbjak.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3ybvzxmom.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3fkdjcalx.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3eazelpkv.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3mkdnzwol.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3fsetteao.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3ooflihtv.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3pauspnvx.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3bjfqctfk.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3isrtctih.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3qpkijlyw.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3vsdqpaxb.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3gyklodjr.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3zqqwysem.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3udqmrbug.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3bpdierym.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3zomjcxxi.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3bjfoqvkq.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3fyoirrug.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3hkegpvkf.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3sqwrifso.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3zmiowzpz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3agkbnmfl.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3obzaocyb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sgvrzmad.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3jkhbygrm.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3kdmutpby.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3hrmyfpva.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3toigjyle.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3xfntfgbm.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3awjofckq.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3lmiwucto.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3drozktew.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3oqcvilix.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3claoadur.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3utxabcrj.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3egbagbcc.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3ppnoevcc.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3pkvgpiew.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3etbrnncf.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3yznqyirg.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3cspwtpxs.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3tmjwykre.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3ymcjerol.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3sdyfejmi.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3bdbaqdhg.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3xxwevzxn.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3shhbhzkt.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3yqhcktmu.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3smbdhgzg.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3joqbloyx.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3nqfvwdei.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3zsysnhkh.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3ynkneyaz.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3ijtxmluq.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3ozvdwmyt.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3mvaflljs.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3viwuuwaf.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3qderivfl.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3vodxqpqp.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3ntiybfjp.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3figvddfb.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3hbnkxbmr.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3rjxcbysz.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3dsthkkvq.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3phnubuym.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3gliwhdar.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3ouhskuod.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3libcjlgm.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3obzkgnsu.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3bjjbcsso.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3mherlygw.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3ehsfirrq.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3rjumilop.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3opwhwrgc.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3ckjqbdun.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3hihqaoni.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3zpamyjav.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3qlzmwwhv.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3fmbzkllr.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3yzxvveuf.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3ambdxlso.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3wqbxycjz.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3njxqwbvp.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3vijahqha.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3fkufjfil.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3kchyiulw.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3pairwiuf.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3dumhaovt.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3ehfdcmfa.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3ukyxhruq.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3brssnnjm.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3yxwgyocf.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3msxzyfda.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3wzuhmwmp.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3lhqnpfxm.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3tuyoocup.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mvkzsegw.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3rmkpfieu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rvlrdvep.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3dccupgdf.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3anccoolz.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3odcuejlj.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3tujtskep.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3wmumysvj.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3viehbovc.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3yjjmmgry.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3rkkmhkgt.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3ytxpeotk.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3vyyirqed.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3wiakxvow.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3bphgornp.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3ptnruswe.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3dlfkdany.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3fhycwear.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3cbvfajud.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3sgfkrulp.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3qgtsimdi.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3tlgypbly.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3fojxiwcj.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3iuabmyff.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3zvyjfruc.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3wcaiocok.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3lpywucxt.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3xxhumpqi.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3lqtjvomk.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3gxmdiaup.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3ebjzxadd.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3iybgcmco.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3opbdvfkf.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3kvzgkggr.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3yylakicr.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3rasvaxak.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3yoeyuliv.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3drtyqxuz.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3rctvxomf.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3gsitepbh.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3qigoxrlq.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3deehzgbu.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3jeuyqcyt.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xwoiyknz.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ghtyjizp.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3sfaavken.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3yfzrxojz.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3afhzpuqu.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3njubktyg.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3fvjunoej.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3qjdafuhb.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3qsizujto.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3wgaukese.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3gdmwqeqf.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3hopefkrz.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3opdqaoho.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3ljffqozn.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3mrstablv.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3iuupshpw.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3zfogemgq.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3gyudqqta.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3yvsdymsm.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3yxeetjtm.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3iqlkizyc.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3zfsibzda.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3mmumibwi.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3aeuycnbn.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3jlrngsrd.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3ffkjjnps.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3hxypmcnl.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3vrvwslwz.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3aqtvidov.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3gxznhqkk.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3cpodzgxc.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3ibvmfhkn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vvmuqgji.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3obefqesn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vghuuyhw.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3qiueuhaf.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3zrmastcc.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3qucjfodh.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3jiwzesrj.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3fdarsjas.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3jttpjnke.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3qsuymvhc.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3xuanqafp.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3zjjoovat.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3xljstuqx.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3uhnxclvq.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3cffbjuau.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3lxhuwkpj.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3daskyzxj.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3wcyeptfc.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3uraevfnk.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3snqclpvu.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3bibazidm.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3adgfobhi.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3shsnsstb.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3aymoqxhq.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3trfnqtvm.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3bjalooyo.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3qpydqvcv.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3dxltmgvj.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3bhlkzbgc.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3rkdomkcc.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3cvhmhjhk.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3sdvmgvly.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3rxsuglaa.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3bqishful.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3uiaupkqi.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3pnfgutmv.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3sihnzdsv.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3tewzlega.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3nhzzbogq.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3pmywlytr.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3gxfdgzql.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3kjahrpmo.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3ixktuozl.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3vxbeskil.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3znruezuf.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3bulasmyj.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3gflpuahu.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3mksnnqio.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vufmpdxg.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3ptwzygzj.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3yicmuzoj.html


<!-- 参考信息 -->