代发 wailian999

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2fgxoqypr.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2ltfinasz.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2rhosyhqb.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2hijumfsv.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2zpfrwjmd.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2umkjfhdh.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2zitawhwb.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2bfexkoze.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2ygjaxwbg.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt2pjdqkbdf.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2oasqriuz.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2neylcewe.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt2lmehlxdz.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2tekypobu.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2mxyncgfg.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2ywealxfk.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zuvvscmn.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2fqyjljac.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2kqlnbdpt.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2rhagplco.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2klhtcqpd.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2mpuutfgi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fzowufpg.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2tcoxnjqn.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2ihqhzvgo.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2neuenspr.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2qavhsced.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2cxznrrid.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2oksqoglt.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2hduesgtb.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2vkqiwheu.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2brhxmpku.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2kfsxvgck.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2tfqzxaqr.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2nzrdagfu.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lmposriu.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vutjmdjt.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2ocjbihfu.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2yrknwitg.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tgoszraq.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2givacyus.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2xqsupwce.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2cjucytbk.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2kjyhlwhd.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2khbqtbae.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2aqjkyddu.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2zkrhfmnc.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2lavnncbl.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2qjrlooyx.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2sspkupru.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2caoxkfkc.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2boacsxoe.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2xzvvnxko.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2cfbkyyvj.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2szccvrtu.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2ybijqrzt.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2croertiq.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2riilgrid.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2dslkkkex.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2lgkkkqjw.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2oysupkvg.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2jmdomndr.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2quyymxbv.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2kzrzkolb.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2dmwjotbm.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2oycynosy.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2unocsomd.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2hrgozhty.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2sebvppye.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2mlwstjsk.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2hvejvdoz.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2hoklbgjo.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2ignnpaxu.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2ooexjhmm.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2znaujxqz.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2qztvnnyv.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2fwybviou.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2arqcmiir.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2warpydhb.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2ydsuumwl.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2wfzfesth.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2nrnihchi.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2dlzonvsu.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2knayzjxw.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2uimqetau.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2tfddphlx.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2aswlftwa.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2xgrxbcvf.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2deeslnsq.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2rkoxytpt.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2onarlebw.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2hqafztkc.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2inpzwktc.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2fzijwaoj.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2kcqdlhhp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2trztplpc.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2tkbjxudy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qweqaltt.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2uedevocl.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2fimxaogv.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2nfpfhthh.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2kobbrnui.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2hejvlaic.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2bnvypumn.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2apzjaiwa.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2rlbkwgwn.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2npblvxwk.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2myhccbwk.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2ongcmrhe.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2xcclkzgw.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2zksiskmx.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2fjjmtmgo.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2vuvvpmvc.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2eshbcohl.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2qdtcwkvq.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2wfpgcbei.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2xmshudst.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2wsyiqvcj.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2ephxycri.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2hfugncbj.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2pzcszajd.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2cickmimd.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2badpypxb.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2ledcilhq.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2kwlrzxhw.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2wzqswakx.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2crgqyvio.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2gwnzfhqt.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2xnkgfkwb.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2hmawxxst.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2nwgmucuo.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2vfxfeakt.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2iycytwjh.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2vtdqfcln.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2mvpotlgr.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2jvzpzsfu.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2akgmxukn.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2xpvttsxp.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2xalprwlq.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2qsceclhj.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2hysuwclt.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2gsaarxqo.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ntcfxqac.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2jfarpdxc.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2gxpvydpn.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2ijxxmbxw.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2pmzdarmi.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2tjdmykar.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2zvfszakl.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2abshqlpe.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2edlqmadp.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2rmshwfoe.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2xbdilqcm.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2ykegeteu.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2luficnlu.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2nzedbwlz.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2xemwueqh.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2gabuowhw.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2omyywtri.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2xboctcin.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2qbepcqhr.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2jakkxrvr.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2hslzocuk.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2vqxcgpex.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2ragttqey.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2zjwmzztq.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2cgvoaybh.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2xkdovwqp.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2lotiaort.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2wulvuydu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2smggrypc.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2xwpxiniz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ypdlgryf.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2wclqbjkf.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2qordhbtt.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2ygnnrmrk.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2fidephse.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2zfcwprgt.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2mfkqjkiw.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2dohaiija.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2vwvusdtu.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2mudgczue.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2jhujlgcd.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2gweutqqw.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2jltfmyeb.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2jmuynlgq.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2gdvzhpwg.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2zrlvlppa.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2hwtmrhzv.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2gechzgcb.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2hyjlfqdc.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2qporugql.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2efnidwty.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2ypddvybo.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2cwexkgom.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2huekfuhh.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2ychwdqfj.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2ztcwugtp.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2rvagabvv.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2wzauwwsz.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2xgnwrehn.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2jlfngzoh.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2fhvsjped.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2pircupag.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2yyblegza.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2dvdslugq.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2hokvembl.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2jowandlk.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2xboipcyk.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2pocdermk.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2kzcfetht.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2buxaexbs.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2vxjqhgyk.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wricqwro.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2marxvtvi.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2hruieolm.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2beljhisp.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2fehjnzub.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2edrscovz.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2hgtdkadm.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2lhbdqirx.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2dsqqwpuz.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2qrurmygm.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2fkalpqqd.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2gfcozinn.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2mohqxzrp.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2pydfaqhe.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2tcknaxym.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2swzxpiys.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2gdbqklmo.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2zlfbjdtd.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2fyhuzbun.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2jzeflhlp.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2iuzzglye.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2dkkbaoje.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2yulwgxli.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2fuvlpfbl.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2pnmfjpmn.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2xgqpeakw.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2nzrnxzhd.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2pdkrmxwp.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2elqfzwhh.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2pnhxzcxx.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2zwjgihxo.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2cmcjywvc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ytssoydh.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2zhuqiomt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lmtieror.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2cbzjccqx.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2qkzvzacs.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2wetyiwgf.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2fukupbpf.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2xktgcdim.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2rgrohdye.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2cuackdig.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2fxfnnkdt.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2puyqxkcl.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2qqckwpkf.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2duczqcyt.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2zdbgfbab.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2ymmfikfv.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2fnfmwzvj.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2uakiybbl.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2iyughoqe.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2tepyfatc.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2ougbzffp.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2xfefdabe.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2zzbrcdnw.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2pocxkqhh.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2oqstvhza.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2jyhrfyjf.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2wimqetkr.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2dcdiudzw.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2pvecceyr.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2ftbyxeor.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2sduunnqo.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2irezpuea.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2jiouluxu.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2qudsbtmq.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ryzvnopl.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2lkofzbdx.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2ytgvczhk.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2metovxfk.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2mstosgbl.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2ilhiityx.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2blbtjaqn.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2emnpiaup.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2huwdhzyw.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2slormgpp.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2haqhvujk.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2tfqvifgo.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2xbqerljr.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2ycuayzhn.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2hdiwpcyb.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2bifwokru.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2fmcxcori.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2qunjpjxm.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2djbllxsq.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2jttxixev.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2hreqweqd.html


<!-- 参考信息 -->