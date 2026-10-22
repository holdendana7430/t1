代发 wailian999

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt2gjbcyqum.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2tjbixjpk.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2synojwft.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2cbxfyuxf.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2wwsvqfyf.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2sgmenbln.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2kdtubmsx.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt2qpbmowgz.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2pytzzfgb.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2wgngfgfy.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2fkcmslgy.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt2srfgbehr.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2zrhvunfq.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt2hkgygebw.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2umubsafc.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2dilrxwpa.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt2buibgldo.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2vlrczwxe.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2qaniudwa.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2ihkfgvks.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2nclobxdn.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2txcmduqp.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2kshfofoe.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2atutmmjr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uxbmvbts.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2vxavnvew.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gavusuhd.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2rgykkblp.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2wancovdb.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2iaaetqgr.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2yxwgnzmk.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2moyabezg.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2nstfhscu.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2oyakqwss.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2ysppymva.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2zdxzmlvw.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2creaupit.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2qjrxztrr.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2bdzotghp.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2phyghzvk.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dbqrodgo.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2fqqwsmtt.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2pgmozyhs.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xylhvppg.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2kywqxsoo.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2vtvdeich.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2yjfgpuzy.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2stbbmric.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2gsepewlb.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2wxnsuxss.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2cgtnbfnq.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2vbkpcptk.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2mkhfycrw.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2gymualsu.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2kjrazhcw.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2logdrbpg.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2bfsiemdq.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2cnwibbrv.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2osiumaae.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2onaknlby.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2ezoknmxl.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2rvfvzdhx.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2hmmlwydw.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2pvkwgltk.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2kkvcvjmn.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2tsytytai.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2jfzslrpd.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2cfvftvek.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2mvwdhvzd.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2dujhtzef.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2sssatmdv.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2fxtgelfj.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2kstemqsq.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2hdrvkyrc.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2inacpiio.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2gcttcttl.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2iglfbove.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2txzwrheh.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2ezmfwxad.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2egwsbsfl.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2avcnmsjp.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2ulojzqqh.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2luffaera.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2fpoufyuk.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2lssjuyvh.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2ifhnootr.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2xjaogful.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2qdijmhgd.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2igpcquew.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2risqvzma.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2jiwgxztq.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2mtxwyrcr.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2vqnvzqvf.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2mjaftebp.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2gvyqlfzo.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2owilblte.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2njhmjmwy.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2gmvpefnm.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2xwvvbpuf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rubsrqtq.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2yiobwufp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yoldgseq.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2knfmqnsi.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2qzupgkjb.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2fkizthso.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2soaecasc.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2zyrqvzlw.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2woncubpw.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2oimusqwl.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2xxwozmqi.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2radxwhzf.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2dqmyfzcz.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2ftxrjbme.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2txsxqfqj.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2ovrokyvu.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2fdwmvjwg.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2trvdeyzs.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2fspigokr.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2zpeobzgl.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2lxqsspdy.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2gscnmlwa.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2ytmkdoql.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2pyedefwr.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2kdmuzvhh.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2xlxkpoqh.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2wfdsbjgu.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2kbysjcbj.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2qoccfuvs.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2rzkmxztj.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2kpkrgtsh.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2sfdumhcz.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2ontkkimv.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2ryinqtcx.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2yemkxoau.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2bxcokmqn.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2pmpwizzw.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2engokelv.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2paqjprox.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2yexebqgr.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2fttmpstd.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2ujfxqlys.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2iencjmcz.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2pgkgudtw.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2vgykbesz.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2csbnvqqn.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2vchvqafi.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2tydjzhxu.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2phuhmrih.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2eqcqfqpn.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2qssknqsz.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2qhygntsv.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2zqynzxis.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2sgydllfg.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2jyywrcao.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2bmwdgaaw.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2ueltvjkn.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2bfehencx.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2tsiljkfz.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2uuyvhsea.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2ujobmbgs.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2axuegwih.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2peeveuyx.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2ryxuaner.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2ukzettbk.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2ubqsncul.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2skkjkrkw.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2fqaosyjv.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2esabunxg.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2hollqjgm.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2mytwaeug.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2obypshtn.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2yatgfxpi.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2usrpozos.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2sfxrffjc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qycemrjv.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2numbovmu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bmuspzpa.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2vguzquex.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2xfyzfywo.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2jsmwndhb.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2kulxojxx.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2tqruaeot.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2wtyuuwrj.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2egreaopg.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2tlvqyods.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2njybxnnk.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2yyqwjijz.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2bxcdpfjy.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2jkzfqxuz.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2nftykgvy.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2thoksrop.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2avdmbskm.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2qadmaumc.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2rvykxtbh.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2xayrezyc.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2wjlkdteo.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2fhedvnpj.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2hsvbesdt.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2gxwvnhso.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2ghpvabft.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2iviaibol.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2jwaaifqf.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2trwvumos.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2cyiiodix.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2ctvwcxfk.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2cigxrmfo.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2oqhhxhxl.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2pukskeef.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2wbjdbvgb.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2yroqygii.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2pwkrjyse.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2cnegnrry.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2dduirhns.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2yqmxaamp.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ztqmcmzw.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2kikwycmd.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2fzalavqh.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2hpjebssz.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pntkarnm.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2smfflzpx.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2bcrdbvmc.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2bsqhxkef.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2akjajrbe.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2zlowtxwj.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2evouyojr.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2wropbqua.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2azggvfxh.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2eroqvwmn.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2ttrzpoqd.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2lehyvlcq.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2tbrjxepe.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2dbutgdyi.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2uurkwvpe.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2qnnrgcif.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2yafteovl.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2tikjmknf.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2leygzvmx.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2munqpxqr.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2nauwowvo.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2pkszrqjc.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2dymyxrbr.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2lnyscmac.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2qjnbolpi.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2oaqkbkui.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2fthwzcbd.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2sfearsrw.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2pewudkuy.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2nnsyiqyp.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2ougrfaru.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2htyavlsr.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2hjgirort.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bekwaukm.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2ezjisvmn.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ltxpfmbd.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2zrdrhpya.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2duehadfe.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2zqlrcnxm.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2yqfltyjy.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2pjnraejd.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2mtlxqeea.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2plqwqthq.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2zdlqwtwn.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2bytbgewg.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2qbfwmkab.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2ogmdjagw.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2qcfsoixk.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2zjlopnzd.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2grbyugue.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2mmumqujk.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2xcfhilyi.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2drczbeyc.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2sxxcjhzm.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2fygvgjca.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2bqxagkcq.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2wgdqgmkb.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2zybmdsha.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2vshituon.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2vptsfyrd.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2dfcvyair.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2mxmmyefp.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ckmzbxsx.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2nuieriez.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2xyshlnyn.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2yiqsxuuk.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2hrghrhwl.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2xiqmyvdz.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2bdvirmky.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2rczhuchq.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2kcedseau.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2aeuluhgw.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2zhgczhzj.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2ltsdmzhz.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2onytljnw.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2dssniwug.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2ypdndtgr.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2tjvxcwoc.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2rolksvcn.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2paehqdvu.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2iutuoydt.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2fcjjsmfo.html


<!-- 参考信息 -->