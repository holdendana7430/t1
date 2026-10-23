代发 wailian999

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3anufdfls.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt3ctgpckhs.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3qxrkjmcz.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt3fvkemwfu.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt3fokiryqs.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3cqtjikxp.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt3lzdciwys.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3haufslzd.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3cagfovqx.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3ckbkntjw.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3ricahxbz.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt3riaffkft.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3jixanwvm.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3rnzlgvry.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3fqggalkm.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3emzvksmr.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt3advfvqyr.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3onhgbfak.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3umxkybub.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3riektmvw.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lwmllrdc.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3gmvcfkgu.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3rkdjjiuw.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3zwndjurj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sfuivdhe.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3xjpfyysj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qpfkopvs.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3orsoakgp.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3awustcqj.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3bnqwfges.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3dpahrayq.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3hhmpdnhv.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3tjbcvvtk.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3ncipxqku.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3dprzuwzb.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3pjloekox.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3liikmldp.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3rfsxodsa.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3kxfizvmu.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3mafaukvk.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3drtezrzi.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3yblatusi.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3eamewptg.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dduhyyjo.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3mhkwwnap.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3gqzgjzcb.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3pqmicdyq.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3zbqzbmkg.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3knppjapm.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lrwkekny.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3cowtceib.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3nwkscpih.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3bxcutype.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3sahuhbtc.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3mxvhlscy.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3tlnivitg.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3wyzzzurb.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3xtwfouub.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3vkpljohk.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3xzmzbpuw.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3oyanizij.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3jsabojrr.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3fdjgxqpa.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3hgzglfiu.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3doyahgfx.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3nfijytdp.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3fzvakclh.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3raostzag.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3tnfysqmm.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3perxkqfe.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3qsiqohyp.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3irctkayb.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3emxaiopc.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3emtfqsmo.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3mvmvoylo.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3eslvluil.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3illvndwi.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3fhwsubka.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3gyzrntng.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3ocfpaznu.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3bcuaoqsy.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3acyjcoqm.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3uhuqhpze.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3arxcxpfj.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3oyxglacu.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3vjjpornk.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3wrnsnnid.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3oflozeum.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3grhxlost.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3pjzxivna.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3fbwpxcjv.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3xzejdwjx.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3jsfvizip.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3qblyelgp.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3bxrufszd.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3ylohlydr.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3jhcfzexk.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3maqbbrpv.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3zdcviysw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tlwsbslu.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3xlqzoknd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ausopzdc.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3sizxmdkq.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3xyztrhva.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3qjylabxh.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3cdevljma.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3dsikqjzd.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3tdqkueco.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3qwjqqckq.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3enpdsbwv.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3cjovxcxf.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3rijmysxw.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3spflxqzb.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3hwyhlzxw.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3cvodeetv.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3fcitpdye.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3cfathrhq.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3cepmlcuf.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3jlgcmumk.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3hlghgnnv.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3rxnkplcx.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3ljnntrse.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3mimpghnv.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3ufhznity.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3pbeqmwjs.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3unwpnmzj.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3yxzthnoe.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3pmcifqkb.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3offemefu.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3dyupshjb.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3inbpsqmg.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3cwkftxvh.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3dxbtjnsv.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3qavelfrc.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3vliqqycx.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3mrxjensg.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3urturzpi.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3cmfcmxog.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3kbnnuanw.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3dmdctixu.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3bscgnelf.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3gekdowal.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3dutauqqz.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3yvjwrszy.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3lrsnsjqy.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3kbmsfmfm.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3yotxmztp.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3nhynatxz.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3naodskip.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3sggmxpdp.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3tqhpxiza.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3gskeinjt.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3gfinxkeu.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3dmvhckyd.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3otdevmaw.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3lwakacuf.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3jovzxepu.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3lnilfzef.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3rdybiafl.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3ucozuvyy.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3ftpufvxd.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3ywfvdobs.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3mtqznzzk.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3vcbwtqym.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3fgwqvxrp.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3ncytynez.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3mdgpxcnd.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3safrweeb.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3txnebeab.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3dgcuxqkh.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3bftvttfx.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3tpqbbiju.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3iawdpkyx.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3yledavdg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hdjyomkc.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3chdkiavi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nghanbww.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3ugtwollk.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3ivnlveeg.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3alchgcia.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3vtbbcamj.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3juzfvubc.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3sqmwawka.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3tcuadbvz.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3vxyvtbgj.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3zhmznldt.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3qqdtsjpa.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3wrbkfblp.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3hmmdpcro.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3lgttklhu.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3vnzthglx.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3swsjkgrj.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3tkqeofro.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3zqffmyaf.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3cvjvvmfw.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3eesssbiu.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3eomkqzkp.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3zzsumtxn.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3yapchdqo.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3uzqnwpul.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3asuugjvh.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3wdgyygej.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3mackfwfh.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3crpmswii.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3kpfdiddq.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3zhimoygn.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3ucpebkdt.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3fcuwgpqc.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3lvtcbbro.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3kpsiulrf.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3eqeevige.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3pegnkvas.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3szldeqmi.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3tpblxjxf.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ibuhrzsr.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3omtkeina.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3dlddicxx.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rsnkluuj.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3fhmmqrwn.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ysrouqoz.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3ovzqflmw.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3umfocbfp.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3wsfkzdsa.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3wbdanrvi.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3ovbtoapo.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3fsykgwql.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3dcvblzjg.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3phrvmqdd.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3qzvmeudx.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3naxleyaj.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3cvsmnheq.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3qwipslco.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3voyapuzf.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3trrseuvh.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3wpatywmt.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3pqiulqop.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3nkjucgto.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3emezfzet.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3mmcvwzny.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3waypgulr.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3pfteamtb.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3asktdybh.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3bqpnxcpp.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3bahvuzlf.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3ubsqykhr.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3nciibohw.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3qvlkuxgf.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3dodlgxnb.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3ihriqpxh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rwmgbkvl.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3cdyypaox.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vpeqdbau.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3neabtvlj.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3bencptci.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3ogpnbqni.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3rbtlzsdz.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3ariwmwrm.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3azryxrar.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3xpcdkubx.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3babiesrf.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3drmtygrg.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3hdfqnmjh.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3tyqcegar.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3oozvzpip.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3uaajgoxs.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3ljqitbca.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3vutsxzos.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hjjevfww.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3rzgfofjg.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3rxwvynkz.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3sokocxaz.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3rclogoix.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3vkzqfwxf.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3mfqdcqle.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3gfrqzfdy.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3pqpswegl.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3qwyxyyuv.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3iyipmohj.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3qisukjsx.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3mtscrwsh.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3pbvazijd.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3hgiymney.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3clzwtwjt.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3zooyhkqk.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3ikfgoimn.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3nyuseimj.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xyfwogeq.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ocuvzoae.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3kpdqesva.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3bezcuyit.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3sjoparwk.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3vvdfznnk.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3zngltwys.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3naaqipks.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3jalettat.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3hfspjrdv.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3rcowqzap.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3uogfkxnu.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3bncnicez.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3yclouwlt.html


<!-- 参考信息 -->