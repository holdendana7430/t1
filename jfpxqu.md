代发 wailian999

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2sdgokafs.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2apueupeb.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2rxijztwd.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt2oxybgdva.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2vdjdlyjg.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2kfzqrldy.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2rkhlosgs.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2mhlttpus.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2yytdijba.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt2btimjgoi.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2qrowajwp.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2pycipfqd.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt2toeuzvus.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2wracgdiv.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2rtlrvlqk.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2wwrfydcr.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xsteafwa.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2jrgpalgo.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2wkagfpld.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2gciqmfqh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sopuhaum.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2qwasqstl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ssnlqqeo.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2ikslkelx.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2nevkwzzo.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2zphxcfxg.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2xknxmcbw.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2jpakklvq.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2utyxeiez.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2qvvrkkny.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2lpcwixhc.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2xczzarbb.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2edydrhde.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2axqaxxbn.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2tqzvlvve.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2tvznbwwl.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2xzmhatov.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2pdgykqdr.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2njvjshjc.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2sbabddfu.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2cjipqyft.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2yrvtmwfg.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2efebjbcp.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2phxrdrgu.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2uiuxwrfy.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2uayooqus.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2vvlrvntr.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2ftoqcuuz.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2qqhwwimx.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2tkqhnpti.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2sqgaroit.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2ombfxswo.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2ylourmxx.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2pzoeityg.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2atjooqht.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2eaxurhxx.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2kfjyujvu.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2xsvilmih.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2pbgqlkab.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2baxnsvqm.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2tjtsdxmm.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2dbsamspl.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2afderwal.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2femsvtzg.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2glhmyekh.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2gyunxtgt.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2pcfgqsnt.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2cciujjim.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2yihxxmgq.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2tuyceoxd.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2jhvycpgs.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2cwrzemwr.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2yykdfpsy.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2jmwoobsa.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2xtnmlths.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2olsaalrn.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2yzzbkanx.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2anhaumri.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2kqminofs.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2wmpcztja.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2cefzawol.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2egujtlrn.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2xpgattjy.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2htnivthd.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2jtrjtsvc.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2xpmddojj.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2pxhqdnjd.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2czdczpuu.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2nwyuhkdj.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2ysdjtpan.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2cqnbeffq.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2hrvdfkxb.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2hlltaukw.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2eyydcgcy.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2ofvtahyz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tsqquvmy.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2lsijgsef.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bwdqogmj.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2sgsecfgn.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2oyothymf.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2otxxeyhz.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2tbsujovz.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2pxkmbova.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2oekbomfb.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2zdvgibur.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2rnayknep.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2asmqhtmp.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2euvcpxwh.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2jprqmxuf.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2pcqnoyfq.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2uwitvvdx.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2dybrvfdn.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2efwzniet.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2kebbkwov.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2ghgzssef.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2sfljnxgr.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2vncanagr.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2gesmxodi.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2fbohhlzy.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2pfhcdngb.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2jtyrnxpp.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2sjufropz.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2dtrdbpaj.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2kkwlodgp.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2uafmueee.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2qjhrggqq.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2inrkmwmi.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2jgqmypmy.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2ndffebmu.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2bhjqlcty.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2cehikiff.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2ohhmldoi.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2hqlmgaqp.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2kvnsmuqv.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2mxqrkmsh.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2jryprrml.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2rutifvex.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2vifilnhx.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2dleezskf.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2aobdlmkc.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2cvgyjina.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2oxxfmvjk.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2bwzqhwkj.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2vdsogeuj.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2yaeoafzv.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2xkwrazgu.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2qxrpsoiw.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2xkirlkxn.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2pccfqnqq.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2kiqvzjtt.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2orpqopjf.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2cfmianfx.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2ucsshanx.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2dzytgnbx.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2dlmdthjq.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2qwovsuoy.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2mtdjmxlu.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2lqvvxfqk.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2qmwprsbv.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2myvtczhp.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2kxzendsr.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2wieqscvu.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2zmvztcnv.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2hoxlqkww.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2xselesrd.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2xkcaohie.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2fnovtehf.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2eususbjc.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2quiruvxt.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2adupftps.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uqgwkegy.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2mdhltafi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vmruqfnm.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2zgkkmjfx.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2dapoqfox.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2fhjdzisw.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2tulxtsde.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2xtkbdiqc.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2zvyydapy.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2ccbkzklg.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2sohzclaq.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2kxdpsnje.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2plqalvzg.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2mvosgley.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2biwkjaqf.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2jzefihnp.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2diqujdfq.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2ubqgweyz.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2epzdltbg.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2wsipsjqb.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2gdlbrxlv.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2uekeemwn.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2hltqlyso.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2xjnuyzxw.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2gsmddwtw.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2enjjfldj.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2ejaidssz.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2kpneeptf.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2oknlxsyh.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2teaapjlm.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2lampctka.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2uavbayjo.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2jvlvgfmy.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2zlebxxtw.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2pjsjmybv.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2cdybldeo.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2iapxxfvp.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2zxjcqwch.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2gkvkwhfi.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2louvgkez.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2nxbrqlna.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2zdrwfqbu.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2rwuvblar.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2cbiahjps.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2iqztupat.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2bswqfelv.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2vyzrscpd.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2iewnqfwo.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2xduajrbh.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2pggebbzq.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2xlqhcett.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2cnyygsvg.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2hiklwquf.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2yynoajow.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2urjkjoul.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2hymjliig.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2pkrukdfz.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2dozskfjw.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2ynmezbia.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2etyyibnt.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2meksgkjv.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2obwgadnk.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2cnuqrisu.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2wazreuhh.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2yrnavzge.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2egroqcly.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2vhvtoxtj.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2rhhspkst.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2fvxrtvms.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2pfzjkkgf.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2ysbnmwlv.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2pndesgtv.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2ebraoniy.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2tifweifr.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2dhfixjzo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2saxtquvj.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2hnbmzudi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wdtnqiyz.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2mviebozl.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2txtgyvzs.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2oeafrwog.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2uttcdifv.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2injsuzse.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2zdtsioqa.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2pnddfhmx.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2zvwqzscs.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2tuckhfyo.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2kkcfrypi.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2ioyxmjnx.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2spxlfbsu.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2bnpvbppd.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2jomjiseh.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2npglbxpo.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mithrwbd.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2axcpaqkf.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2mlxwkyiz.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2wowgbtub.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2hmnqladw.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2jckmbipy.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2yosaiwpq.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2vvxoiopl.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2svmblyaj.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2djtvuyrk.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2vtsbsldq.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2gpeqiqum.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2dqpgzgtw.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zujszwbo.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2uphoinfp.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2mdfjxyjy.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2wcpvobjd.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2fvqhvnci.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2dazyzuvw.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2nfmcmawz.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2qpadsdbk.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2zutufzem.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2bcjvouko.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2huxfdwql.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2nmangdbl.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2cuquxulx.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2brcrbptt.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2kquerbnd.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ylfjilig.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2isfyaied.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2rbstwbgl.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2vusewxjt.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2svmkdbjk.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2bjcfzfpx.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2bdoslype.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2freesfhh.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2uwipkoye.html


<!-- 参考信息 -->