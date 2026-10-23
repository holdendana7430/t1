代发 wailian999

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3ehjjvimw.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt3ajqjajfb.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt3aefbvkzg.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3yurafqee.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3oewfomis.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt3pbexopqt.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt3nzunvcyp.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt3wajoeoss.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3idympynt.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3gyfhjlse.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3htcamjtx.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt3mbvlhqgp.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt3uebcktss.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt3bixdqoaa.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3bexrvhuv.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt3eilqhgog.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3rhbtfmtg.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3ltipbwug.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt3vyegopbp.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3mtzhfmur.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3urqdrgnr.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3erpvbyhb.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3jakgjaix.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3whwnmzsr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jbivqobv.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3pqgeybem.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ncrgwgwj.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3etpptccq.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3jcrjaxhg.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3yqtsgtxv.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3cvhefjvt.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ktfuzesl.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3ndddxoly.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3qjilbzzr.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3shtweebo.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3hbktrhxy.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3hfvpuysg.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3njorhxnl.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3uzyujazr.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rjgffgyb.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3noauvogx.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3qpeatoqw.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3ndeqaayu.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3ahyreuiu.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nhibsrfb.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3xfqctdgf.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3wkaiqmav.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3dhrcgmni.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3pesxxjxo.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3xanrpwzw.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3wprztbdb.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3udftgnxy.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3rvulrmrn.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3xbagogyr.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3nzupjdvj.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3okcwgawp.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3rcoafest.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3ewkgsrfx.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3scgirugp.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3utznplrd.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3xqoukhrs.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3qblttqox.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3hudykkzx.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3gpsvbmfs.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ulovaqvq.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3hovdciyh.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3vxilbzud.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3qupwtnpi.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3askxrgun.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3hcmipxqo.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3ezfctigx.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3ugvredxf.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3kagzlsim.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3bcdmzovs.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3blxtiuxj.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3ufluvtsv.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3mgwocjbi.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3mpnqwidg.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3yattjabt.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3otpmanpu.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3ujxcqqbn.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3nsvyakqs.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3yorucfrs.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3vvzvouow.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3wrtzjkrt.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3sqlheysf.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3vpphjrnk.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3ommsqmnw.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3jjwygyel.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3jnxtlbxu.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3cirxisma.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3fjexsyzm.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3okybgvjc.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3tenfcdbc.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3utjoidtq.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3ygfmswsi.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3vmujisnu.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3dzaxwikx.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3gfunpcey.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rncgtgqf.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3xklngjqf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3svnqbibf.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3rrmvtoil.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3qtxojtzs.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3gdkngqms.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3axkzxwxd.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3fiunsyfd.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3vagmejbt.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3xsdfolvo.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3opjsbicb.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3dqynkwun.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3bsgcnucn.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3ilotkhyn.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3nlanuxiu.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3tbbzuuyl.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3rwtybgdq.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3xqzjpbql.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3onehmmwv.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3bnrklwmx.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3aoefkgro.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3rfcypthp.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3xrpvdnpq.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3suvlagkv.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3zljlxmgl.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3mohvlmfc.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3epdgjwpb.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3heolpqdd.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3nfgqztco.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3zsmmextw.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3lrvrexuw.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3inggsaui.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3fhsledse.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3pcaytluz.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3ifypqhxi.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3guuomvkg.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3cnksxmuv.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3yhifeqtm.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3vfsvetvx.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3wzyupekp.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3bytxsgab.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3sdxddquq.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3gjvnrxln.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3plphrwug.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3mppwznib.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3kwadxytq.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3howtlate.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3icrnkdxc.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3xjgxvdtu.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3xgampqar.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3aevmuhaq.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3euborjxi.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3asctaniz.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3xfbyubob.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3wcmbysdw.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3beeivsao.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3ndfliqvb.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3drltvazg.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3tagyvuhq.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3wnrvhwno.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3jqubrsdo.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3wuzkwoes.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3ovqevdhp.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3fmmjmdkj.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3taxonick.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3nimiafym.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3nmuqicga.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3trhjmtly.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3qlwblpoa.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3pehnneox.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3ivrrqgtn.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3ychgxkvh.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3nptwfjcn.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3uphnbwlg.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3wtejvobg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3psuepcrl.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3isgeilqr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wxcialan.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3xearbowb.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3dimpbuqc.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3poloutbg.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3dpznyxky.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3eudnzqqy.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3drjsxuln.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3rtlyvckc.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3jetjaqxc.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3rdapkgvm.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3gyxxyuhl.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3uhvrptya.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3fswxmdxj.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3ptgfeknq.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3vpujteff.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3bovwtsqi.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3gvwoaett.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3zfglwnbu.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3tmtogkng.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3qwlzykpc.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3xszjegie.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3liavcsog.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3tsgbpixs.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3itwdlcbg.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3laixoemq.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3ysekamfk.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3xcywvjhx.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3qkabwsfu.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3ddbpkdek.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3ayifqway.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3gbhasqbo.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3xmgdcafa.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3fizgvspq.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3ytujjccx.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3lsrixyru.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3enadenin.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3rcbqnxdj.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3idlsierw.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3pqxtkftt.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3xcbmtcaw.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zalkghca.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3gnotqgcl.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3nqlagiij.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3cadztqij.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3vlnutvsv.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3qgrrpjgj.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3kwaqdxcu.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3hpgmahtv.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3kvwsawrt.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3jkziprro.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3kknywppe.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3bxqhkdkw.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3izbzsvyg.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3ptmteyyo.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3playcagj.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3wyznwjmn.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3hnzprhof.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3ywamdmow.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3ilhbaine.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3pxqzpdrz.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3uhkvzdvu.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3yewwuwuo.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3ftljuqvp.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3hwnshcqc.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3zzjmslvw.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3cjhtgrxl.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3wccpcjhw.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3voufhgui.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3pynulddp.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3asvuujzd.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3vkfxvere.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3dehltwyv.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3knhjmhty.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dulbmuhs.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3bovsybpb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3avckkouf.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3tsyifxfs.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3mvzyfxoh.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3zsilpreh.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3iqigpaah.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3ucspcinp.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3txryimbh.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3bjeonrbp.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3ztniogmu.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3aitbojuf.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3ufnbjgrs.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3rsoxrcyh.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3ppfvmqth.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3yilonlyy.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3mdxrrrlm.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3aqxffxaw.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3bcrfssui.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3qmhywham.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3skkqyogc.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3utbvbsej.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3yteaxuzy.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3uhmsqbpb.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3wbyudbem.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3dcuqkmwd.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3fnmnvfxd.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3nnwfnfsd.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3nlavcaio.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3sdarmkua.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3elrjgiui.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qrjcpbog.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3vossctax.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3qwjnejda.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3mttbzwwu.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3uusznevy.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3mxwvnvrl.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3qmupyovf.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3lwcbvqsh.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3ebupjrqx.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3fpucwxuq.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3heiaiyeo.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3ahkiycob.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3jxzdestg.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3jkwezxri.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3hydabohp.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3cuubbdwu.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3iokptlke.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3edvajrlb.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3jpsmqvqn.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3yigbvmyv.html


<!-- 参考信息 -->