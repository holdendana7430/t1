代发 wailian999

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt3psvbcamd.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3frlqxwzh.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3qerhzhcg.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3ifkqmjzk.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt3jpbszsxx.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3djmxysaz.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3ohfraxif.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt3gzytwjbm.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3qmvbgvzi.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt3bhmqywoq.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ezbfunfm.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3rcwhmeny.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3adgajlfb.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3kqoidzjv.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3jumathxb.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3engsbwde.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wgkmsfrc.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3edehhbxu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hkmcjbdn.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3kzftbnjz.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3jivzywku.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3uwoveyyx.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3xftfvstj.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3mjmapmpx.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3njbnmein.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3jtvnxltd.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3yopyqgdo.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3vnueponb.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3zwnwxjsi.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3irxjlukc.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3fbzeoqlq.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ojeitxaj.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qoomuyqq.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3bxliwymb.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3lnxrddox.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3uwqfdisw.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3tdrqwctz.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3nbdbgwbt.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3mhkpyawp.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3bpgznpxd.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3nyvsmpkn.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3oqscyfdk.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3fcikrbql.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3oelcxind.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3jecvwais.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3zdxqanbp.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3lsgntxyw.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3bbgqgcag.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3vulxnvuw.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3dadoulfr.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3iwxxwtqh.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3vgyzkngr.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3vpjzdawh.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3aitstbza.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3zoigscwq.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3cjkkdgtf.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3blxxxifq.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3omyxoccs.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3lgmbahtm.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3adwxyfbr.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3kuamvfap.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3xplyxfvm.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3tzmfelro.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3qspfhjbw.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3meswmpue.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3hizqqxmx.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3abdahpkg.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3tciyuwcv.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3mnlfsidd.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3hdzxlldn.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3stjofdji.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3gahvpcxr.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3iiqixcex.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3prmozmbq.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3kfmbkczr.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3eoqcfdtp.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3kjybamhp.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3hrcxjcxi.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3flhpmfft.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3nysxfwen.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3nzeovpgh.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ofwqmgyl.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3uzbgwjak.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3anknnpbz.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3dgkseeku.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3zkcfileg.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3uezxrnzw.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3aytatuhf.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3iapnxdcl.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3sfgozxsa.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3ajzjjqba.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yuustumm.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3cislsniq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3udcdytah.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3qabxhvdw.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3fhvetyht.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3klhawhez.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3gqmhvjfz.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3wfmtbgyl.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3ccqsatfu.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3razrappo.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3odidnesv.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3iunawxuv.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3zedkhcxf.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3hxljcrea.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3eeifawvj.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3krifapgu.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3fshuqwyn.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3oovwsokd.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3yibnracd.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3mphfadyt.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3ezchnbeo.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3jferbeur.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3ymggauww.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3yyfodowb.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3vprzpjaq.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3fnhcgsxh.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3ttfghhib.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3ptkdnkat.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3epstwwfl.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3wnwanhij.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3zohepvfz.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3moxdvblw.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3aztwsvvb.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3jnnwjria.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3jmqlicrl.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3gvzyjwzg.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3ooepeecr.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3riowpbty.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3raqfxhwr.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3irvohruu.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3cgammmjd.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3jjtevsnu.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3eclaasgg.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3pkfzypjf.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3ecjbwnoe.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3iejvnpje.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3oqosafmf.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3bquyewne.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3ddrjxfze.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3ztmhtinl.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3tfdxjase.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3asjajerk.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3qetdpdkp.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3mycgeypb.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3sfqmmndq.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3cbdfmdzq.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3eoxmuuyh.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3bdlfcsqh.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3lnsqldpq.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3kqmwsirj.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3ivwmgovs.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3vhtewrle.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3xviwqntl.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3ihxazqzm.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3vboveaio.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3avdpyepy.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3mklygqyk.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3fecqrjei.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3focgxbuh.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3gbbjvhhc.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3oralfzjc.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3ylsxfuaa.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3gucqqurd.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3ziwnnbws.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3csfdeaay.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dqgceinh.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3atsgmtpp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pmxvukyg.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3icfvgozf.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3axipaodh.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3jnjzdqmh.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3jjpmwhst.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3qbacxvwl.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3cshqaqsn.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3cfigqitr.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3tjzumimn.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3lxrwdcia.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3lznjlogz.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3quhnodkj.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3majiuyvw.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3knmgoygv.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3bhhssrrf.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3wophorlc.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3gqhkrpjd.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3zcklfjuh.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3qkkgptif.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3yyutumxg.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3vjlnvaeh.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3vbscbkjq.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3qdckqmyt.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3muyomhnj.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3nenbmmel.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3zzuiuuns.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3gaoqvmzb.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3ptdpdoif.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3sfchnlud.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3wkldkisi.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3jbnibkgz.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3kfigqqjp.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3ickxcoeu.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3ukbhefqu.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3qcmktmzf.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3grhcifnb.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3guraqdyf.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3jmejjcye.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ixumcpsp.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3tyiosira.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3cyrpsast.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rexugeny.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3eoirokyw.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3mfkwxtpl.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3vagjwnjb.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3cthngrtj.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3sgotevjk.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3efphzpbf.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3vqcihbbn.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3tpaticiu.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3yghnsplv.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3wstjbtwh.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3nvpwvlcu.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3ybafnsdv.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3xetgyijs.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3ufkajtgx.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3bnwpthce.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3khapswci.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3ctvdxesg.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3uxsfmrtt.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3ovejdtdq.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3cvpdfdil.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3nxlokvan.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3pzjwkual.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3vtabnmgt.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3vnfqcida.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3rekbjbez.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3sxbztddi.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3ccwaxspc.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3ckhtkmkp.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3rtlldjvn.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3gwgcoepv.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3luckjydh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3btuoauon.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3ptdsfcnz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uxtabmuy.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3rkcpxasa.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3lwqaqrul.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3lubyxtxp.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3nimlfxei.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3vsvjxvfu.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ldkzpfsk.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3oqifammi.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3kojakujt.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3pxnwyngu.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3bpksahvn.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3kbxtaizg.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3uugnqkvu.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3nxomcsww.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3zptdwqic.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3rxmzzfbu.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3gznjzpld.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3qaqgrvvp.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3yphvwtky.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3ptvxdrjt.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3orooosyr.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3rjactele.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3cnobbfrz.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3lcvutbxl.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3ckfglday.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3nurexkbs.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3nyexviea.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3bsvdiumf.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3mwwlfxoe.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ezqqzdpq.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3wtqrsleq.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3eorxxwhq.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3xhbivlet.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3jldbjnod.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3nqqbhonu.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3xtusberm.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3aknbhgfx.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3rhdimzei.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3pogcdtac.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3ejuupmtr.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3fjaeeaib.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3dnskrlxd.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3qmkauwam.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3gcfqiypv.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3nmhayyct.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3bfvcjdoi.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3vggvrnzu.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3tqcmnomf.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ompbyxgd.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3toqfvnug.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3rgbjrtfq.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3huvcudnz.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3bzntziwv.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3owgzlzos.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3cnmkhrky.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3wgtxivre.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3tpqutafc.html


<!-- 参考信息 -->