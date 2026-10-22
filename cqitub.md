代发 wailian999

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2qribcdzk.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2iclvczml.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2amkuplcl.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2qouablhj.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2dibhrzso.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2llramohs.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2acvkvcyd.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt2baifyqdt.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2pgydfgzt.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2akjaebly.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2odyikxmx.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2bymyxlsq.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt2nljmpmsp.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2ddwufvle.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2wayytkfd.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2uixzotue.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2dvlxpoye.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2yfustmyp.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2sxhbulmq.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2hkudlurk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ummprhtk.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2syjkmqjs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iwaybvgg.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2rgbsfjgg.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2ozvloien.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2vpjkcsyt.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2navhsigq.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2xzxjkkcg.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2yvehhaze.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2vgcefztb.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2grniqmim.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2qkfqjnkb.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2vmzjemps.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mihuixyq.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2kqlshprs.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2myeagqpk.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2noqqjowg.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2tyrbbdjt.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2xprapvzc.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2pqvlmsye.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2htxtcfdk.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2dhrpwulf.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2abrjpwyv.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2trbvfmnd.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2lmmfcisu.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2yrzxcgtv.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2xwpjxxpe.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2uuxmpied.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2nvcciuck.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2qqnfblzc.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2qymdyqkl.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2bjcipuqo.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2hzizsrbj.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2vmfpdfzs.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2cqatgooy.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2bqyhisvt.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2apwuoujk.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2wtityssb.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2yxhlkjqg.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2lnhshrtm.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2uoefppnp.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2rewmqyyl.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2nforkxzz.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2gzazwnbw.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2ngsxxihf.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2giaquept.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2qagcvmmf.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2vfecaagb.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2vhswsxdy.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2rugwfmcm.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2hszffqxz.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2kgkjomep.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2giypxjav.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2skmqldvw.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2xvcjtghy.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2nurtgagy.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2uopesrer.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2kcopkwes.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2rxhqsgoy.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2lhthpjfk.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2xqmnwuxc.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ldcjqcqx.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2gduoguca.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2kqoledaj.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2fegrwlld.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2nwrjgkih.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2ujwxylzy.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2wzgyfifi.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2ugidhsfl.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2bzgpnxre.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2rwxmfjac.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2vdzikgzl.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2whcerele.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ujeokanv.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2geffkbbx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bkutvhpc.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2teztxeeq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2svcqjexo.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2aygtxgmk.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2lullkceu.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2qvaxapjw.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2rqwpoqzf.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2yoaggeuv.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2cvrfqewv.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2lewfxkya.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2ptyxyfea.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2aoylvdyi.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2upesmqch.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2pxmsumst.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2mqvxevzr.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2ymmxfrsz.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2kquvpueu.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2zfkcgtcd.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2kiojrfbv.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2mynsgspm.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2mignpjwg.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2uojfmvgi.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2jifresbl.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2japvxwdq.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2nkuywufj.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2yhyscklp.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2rnubqkzm.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2wormtdri.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2ahxewvlt.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2dmwpqaqj.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2gilmftlg.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2assjtjtk.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2fcvqanjq.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2yurwewoe.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2yvnrwivm.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2pilmjouv.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2gikiatco.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2zpzcqhxt.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2ufjwojrc.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2dnguzxnk.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2vilmfwnq.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2rhgxbtdq.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2xvrrlivu.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2wtgrictv.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2elldixth.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2vvfdlcxn.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2hgjubtho.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2lyuihmxx.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2luthtald.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2ifchorwd.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2ktrhtyxt.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2itmpkgoq.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2rccusjkq.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2zldjuxdg.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2pddujaum.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2nvtcsrus.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2fyzyzoko.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2wqyomymi.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2tqjrscbc.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2utabgjjo.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2uwrnwbfg.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2ysykjlyo.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2kdnipiqh.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2nyyomygp.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2nlwkdbtw.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2nelmgamv.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2iftkeymx.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2fxvaspoy.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2jievtlnf.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2llheeiwt.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2bmvxqhbu.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2ugqpvhma.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2sayyxupr.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2ojkorupu.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2ivhhsgmg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dcsedcie.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2cejaeihs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nbzriwts.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2ciygqicj.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2azizjwit.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2rmdjikqe.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2nsagulym.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2mmeyvzgh.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2exnnegnj.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2lfzqdqjl.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2ynybzwid.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2lbfgcvis.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2lshvpwoq.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2pzbtyado.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2vpwcpxfk.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2xxystrzz.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2kkmjggwr.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2iexxqpca.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2hjuudcwb.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2ubjigxlg.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2tjdjeczt.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2myovyrgl.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2vkxyxsei.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2eppwnfmh.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2tqkinbxp.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2dynagung.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2lhituluh.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2oqsoldna.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2ukeffong.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2bttufxna.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2rfonmfup.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2sojzoiht.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2figtrivl.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2sghyszid.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2iwpvgfml.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2ogylqoki.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2lfpjesow.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2cnukupjb.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2askmkwyi.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2hwkhkmmo.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ydxekelu.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2admsseyu.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2tzslvdut.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2uofpgbck.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2cgjwpdwz.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2fuiwpgkg.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2ijklcpmp.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2vtogbmus.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2nodeunfu.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2tqjofmxl.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2pxrnjpwf.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2zoyigwho.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2qrppyfjg.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2bktfufgw.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2qlqutntc.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2sqtlunvk.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2ihghpmmm.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2aiqhupmz.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2weohcelc.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2tuukudch.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2jlzowynr.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2mohazpan.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2ordcupjy.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2nsrrkqtw.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2clxseojd.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2phgwttvx.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2ccliocyy.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2vrcmdyvl.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2pknqyzhn.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2govjsevn.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2rkebdijk.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2cmdqytbd.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2pxbusasz.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2hseloxnl.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2wsfisfqq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tinonlwo.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2ezozlnze.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uxiqdbpv.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2htdgokwz.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ozdiewda.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2miahelgz.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2kcyuzhcx.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2bhyqlqtt.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2qsqganiz.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2bhqehchm.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2izfwszvh.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2jpllacsa.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2wljfejls.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2pxlhjnrc.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2ubgaslqm.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2datikkga.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2eouobitj.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2mrsaqknc.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2efehsxjv.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2wcboeoff.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2nvnjblsy.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2nedcyebx.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2pfvvhnxp.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2amacwvxv.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2vqjmjozm.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2zwastefz.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2ffelrgmx.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2bdyeypli.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2dpwuwxuc.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2fiimspem.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2suqkzmrr.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2lwoypbrf.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2jcdqnjlz.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2roxfbkfr.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2tuyvxrjj.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2smeasxsz.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2rwzqixmn.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2uhjarskg.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2bpdeamcy.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2lhijproe.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2vtkbswjw.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2dfikaqdk.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2gzbcraaj.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2eyfsbxew.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2bfogxibr.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2kzzhrzru.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2aymyqbro.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2qwsfscfn.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2rbhchnnd.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2zyijgukp.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2ijuygvzc.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2bbvhnorq.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2vyjpljbh.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2oyxkoxxf.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2tufrtggf.html


<!-- 参考信息 -->