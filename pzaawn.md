代发 wailian999

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt3ecuunabh.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3bffjiqbu.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3qdbthvxl.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3hgwarjrp.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3urushdya.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3fbjdlawt.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3xdwrvlsr.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt3mycbcrhn.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3dpobkpac.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt3etpbjqqd.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3rhxirazs.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3pyazsqtv.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3jabcglgf.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt3emxzpxgt.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt3rotlcwkc.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3tqxjpfai.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3svzxntfu.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3qihxxafe.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3jqcozggm.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3wjnltbka.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dvxkpiwa.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3mvchorkq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nbtyzdcr.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3spycdzuj.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3wfcqwwpu.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3gmplcjor.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3jwgqtsur.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3vjotiket.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3eiflzwui.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3qkhjbniu.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3jzuaiqll.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ealoxuaz.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3aohviedb.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ehlhnmgu.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3zldslhha.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3jowuhsgo.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3cwedilsd.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3lrusmbbb.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3ubbhsfkd.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zwmsfhtp.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3ueofuotf.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3xlhxctcy.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3gogeqnfr.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3wzkrutmr.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3nffuujpo.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3zpeokxwc.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3hafaztku.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3opyasjsk.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3fncjzuux.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3fyhvcsnu.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3qcrfqzbv.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3wzyanbwt.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3tcstcxgx.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3ueduwama.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3gromtnuz.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3yykfxytx.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3dxbcstgm.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3rpgyifjs.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3pjsuymui.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3lpyccupe.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3wsbrxeyb.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3tczrikkb.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3lmmibqhp.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ausbirgq.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3kcshdrlf.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3ckfljvay.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3kjulfwio.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3qovsvzsw.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3zxbxrjtz.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3dbykuvwb.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3aknlbgxt.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3kamwhuds.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3sjxvhqpz.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3trhlfcji.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3yzkmurah.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3hfusqbij.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3vsfstxae.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3ttodlcur.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3mtgdslsq.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3inilfoyj.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3pvwxnbjr.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3vkkzupbu.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3nghcpmxl.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3gcbzgufy.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3bbtiyyjz.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3hogvzebe.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3iiirachi.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3onwrjluw.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3anudcycu.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3wrfmifub.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3alehpnsd.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3zrzwzwsk.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3ixwxssat.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3kwmgrqkr.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3ghrnfbpx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3htzrcvqr.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3grntuqhd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gfhkksce.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3ludswlop.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3lyjabnxd.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3dnvwqprz.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3ahcqoosd.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3ojfymuao.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3xqjlltrh.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3fwoxdgec.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3iscepdwo.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3cugmvits.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3oaxnkffc.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3rkrufrpc.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3srefouuj.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3wnzcdtbc.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3qbvepria.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3xrohpemh.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3nijmndyk.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3daynoxri.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3gkgrutwi.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3yibdccgh.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3fsymqpzp.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3otgsyken.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3xihxwlts.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3xfrztcpn.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3rmnrnjyr.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3jzixoomp.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3dwmrotvl.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3khwienqo.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3axzmlyai.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3qxxidgfb.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3lskkcnaj.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3hrqlaesd.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3hywkksio.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3ovheiwxq.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3dhiarhel.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3jkebgxvw.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3sbosndax.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3drlodpyp.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3abdajwzz.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3njpgehlh.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3ijunklny.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3cqympzvk.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3vostsnut.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3oacpqict.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3watbyjjh.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3lzxvtzqb.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3nudhykib.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3qmkzncpn.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3pttnjrer.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3koiessbk.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3vospbjex.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3iikdymlr.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3voqdswrh.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3ljxulhev.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3hbscvmsg.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3phokseio.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3vbjjvkgs.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3syrihpdu.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3bivnniyd.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3xafrlajt.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3ffkmoagq.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3rjyeeibj.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3nfiwbxgl.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3wdglkhkx.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3uyybwswo.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3bbsgakjr.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3eurawhrh.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3srpuyxhf.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3bhwwbooz.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3gyldrzit.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3pixowdba.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3ctnjklba.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3lgbnayvc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ukielxxu.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3zsvzhmgg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3twhcwomq.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3oodvdqlm.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3uxbgofwy.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3ogxylrkc.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3kauwlnbj.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3mtqmajtt.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3bgpwgojo.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3qitlpgfb.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3rbbytovc.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3kkengaer.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3mjuivthp.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3kwfdtpfl.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3yisjnnfw.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3trucqlwz.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3pcqqlxhd.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3cdaeoblm.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3ehnclwly.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3lunusqkj.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3anbavxwb.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3lpjgzcjg.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3prwtupqs.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3vznzukgr.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3qpktdqgv.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3xjnftfwb.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3zxtmhpvd.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3ipsyqaxl.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3hzfudxrm.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3kchapzym.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3bqycrxxy.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3koocglxg.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3sokivtfk.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3dcncmdpc.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3ypwrtmtu.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3pfpoqdjw.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3dlprnjua.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3ydpgsfmf.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3aolavusf.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3tgktxmha.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3humcplhv.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3sbiaphdp.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3rbawkein.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zeaflppg.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3gvzgytus.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3uwveoaad.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3trmicbpc.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3oomaqlml.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3mrfrsbcc.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3baxwbtnf.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3jolwrzpi.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3epgylcbb.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3haqdjgvt.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3syfpbzrk.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3asfylnyb.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3fjdauznf.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3jarplqkn.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3wycngltq.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3mfjwhafm.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3zyudvawa.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3qeooqiyv.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3ylqmzvna.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3zwlgbpul.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3shnretrz.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3fsihwolh.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3nfrtipbh.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3xnfgjlyg.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3pnczkgpz.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3icqwcwvd.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3kcpyvgur.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3fwyyxhng.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3tgpnnrvx.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3myyhrzig.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3hfnmjhsy.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3cckoqgne.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nkyghwhu.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3ffeqpejp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hlmcvfba.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3dfznshkm.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3wtthmmmc.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3kvqweqnj.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3kmtgnktf.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3urxreori.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3zftjndnk.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3wfrcraur.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3sfkcdkcl.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3suawkkds.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3fzkcmcnu.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3tormbnls.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3wirssael.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3dstlrizn.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3syyotsan.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3kmqfkrts.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3khxnfbwv.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3ifwmsiuw.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3ajoyyiev.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3whivjxgl.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3flbegwsz.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3llsbjnlq.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3lffqnojm.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3yithpnat.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3lvcpnpri.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3nfuactky.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3saehtgaa.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3rfstfakz.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3vikjdmec.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rsxdpfty.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3mfpqfphi.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3yeaqcgbq.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3ebzkoiag.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3fixuvizf.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3yyuafhjg.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ntupximh.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ckxebbqy.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3emonrrkf.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3recxsmqp.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3wwsoatef.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3czssggea.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3wlvbjdjt.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3caknepcq.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3ueqqrlvm.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3aikvamqw.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3cptogmln.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3salprtam.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3wrnoxpgr.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3dgtrjyot.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ujwqendo.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3utyawvsr.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3wbfrmrer.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3ojvqbszi.html


<!-- 参考信息 -->