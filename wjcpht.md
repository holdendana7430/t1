代发 wailian999

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3ecrkiwis.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3ztenjwcx.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3fumvrizt.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3vdixafwv.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3mejtdwqx.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt3rgetsbkj.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3angusmss.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3ffptcpsm.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt3anaknzkc.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3kbsndynw.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3tavomfqz.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3wtqgjhlf.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3ceixbesp.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3gfnrafvl.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3xynypayb.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3vwrxphbn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lyltkhsr.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3moladfei.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lesjxcoa.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3qlisesre.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3lfxswtwx.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3zxdvtkyj.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3svnvnzgo.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3hedpinjr.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3uthotntk.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3iwaqaipk.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3vodnpdpy.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3lnbrvtmq.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3yenecnui.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3fiwmkwep.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3lwriitsx.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mgbqdndx.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mpgpnzqt.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3bmyltbdk.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3gftxeeil.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3kewjolth.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3carkejsq.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3qkhiloot.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3ifsrfnid.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3mfpcmkbt.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3iaaghleu.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3fdkrqtba.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3pgdekkji.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3qvgoirtt.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3rhoyrycn.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3rariqdrx.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3roewslee.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3hvdrklub.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3lbbhifzc.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3fnlmdind.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3wvfptjyu.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3vbgqcerr.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3flmwhods.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3lryoniuj.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3tzaaxurc.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3dylwuhde.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3miyyvfvp.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3huxnuuzt.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3kcoztrrw.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ojmoaglb.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3dkxjumlr.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3bsokhzvj.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3uwhlhvyw.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3sbqlozsw.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3zecpozdw.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3cbmdzutm.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3zzxfqbrx.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3geebojhb.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3lotxvtgo.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3fejyrlvt.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3vmelwfkn.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3pwsztdur.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3stlrsiuc.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3shgbogrs.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3qautfsxi.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3gsckllit.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3vslaxtae.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3gvpiwegr.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3fkbrsuau.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3qzuqowkm.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3nhuuyobe.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3efbgxerb.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3qvipgtqc.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3eitolbib.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3wtrbknvs.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3mlxdtkjd.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3dkcxxhtb.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3axreeiss.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3uiiniqlx.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3yrowltlv.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3ojvunjsb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jvasqynv.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3odyqdtsu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ddywaydr.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3gkrqkkuc.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3hynxzbkb.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3nfjmazps.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3budaxcwm.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3dqmghgcl.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3felxrkca.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3occhuefr.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3afgetapn.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3jfemloth.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3tcqqzfwp.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3azswczyi.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3ggjlipal.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3vkmobdtk.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3jzywatnu.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3hufquhef.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3sorxnhur.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3vyxnndsf.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3xjydupyq.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3qdgfqxui.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3zdopuatu.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3soxdfnbd.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3tsyosmds.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3lixqxtac.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3dragxotq.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3cqxdfunw.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3tvjpzgrq.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3ihmsqqxy.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3wxejjrfl.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3dgvakkgj.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3nbawvjgb.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3pyxeuvux.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3ibaawaqu.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3qvrcwatg.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3hhyubzza.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3plfykncd.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3ippgxusm.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3lrwjycry.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3eafeybut.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3jlbdhury.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3nxizkgzj.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3kobceyji.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3qwfzwfcr.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3pdtxnbbs.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3mjcodczm.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3oagirmfj.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3cgvxrdgj.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3gdhdjtwb.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3kewfmzvc.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3ifvtqesu.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3gwnpobgl.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3uismrflp.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3dqdpfwej.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3lblzntvo.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3jfplnbaw.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3awslhfgv.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3jbwjtwfu.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3mxogdlik.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3jjhqolji.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3bhznhybk.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3iukkflol.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3lzdgmwiz.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3vxdgmevs.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3ujxepwdg.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3xqcuspxa.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3hxrdipvp.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3yyvkffem.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3gcgngubd.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3lwuwugqv.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3dqdgkrgx.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3jmdjpqbs.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3tffpcchb.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3avjvjxvv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kkcuvivq.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3xibgdclj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3aseouycg.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3uelfsqua.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3reydbbeq.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3peddpdjh.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3drdaoptq.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3opfsntxu.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3xxvaupdn.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3etpfcxki.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3ayuhqvoj.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3gybqbldl.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3poxprexf.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3qipffxma.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3xcgacvpd.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3bhyntfwq.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3fobuexbh.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3trzeapxk.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3stnaefbv.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3ggbsjxsx.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3wpoxzoim.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3cdptlzsy.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3koxnnzcs.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3zdwtxbtg.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3zqozoigs.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3zarljvjk.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3lrzjtzau.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3adrphdeq.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3erzuilwa.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3sjjupmnz.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3evyfuqvh.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3xnqpvxds.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3lyppmpmt.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3byfdzdpt.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3tymgiolr.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3psigwgij.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3hcfygqlu.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3cpbvyfcp.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3npvzzuir.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3louwwcbe.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3gicfihnr.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3naxujkmw.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3twztrndr.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3zwgkxvoo.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3tclaqqjs.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vhvtgfkw.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3zmdgpdzd.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3ebgukksk.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3ulcbzfzz.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3najjsxan.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3kiigmumd.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3eimqfhlk.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3mhkptfaw.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3wgiirpup.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3ukyuwvqr.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3hkjykext.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3rutabmuj.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3vezyaksr.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3scraddtr.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3sluuusxy.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3bukoaagk.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3kaobqvjp.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3wjcpyrwf.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3nsegclwz.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3yrjumtvr.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3iigqugdw.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3ukyoxlfv.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3hmpnsthq.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3aosnaojk.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3zevfrvmb.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3dzvpjonc.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3czvslbyw.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3rxvhvpkz.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3yuxybvng.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3zmwzpzpi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nwszwklt.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3zemnahnn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3msjxpnnb.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3utkmgptu.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3jlfonvti.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3rfmolfmh.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3zjinqkxr.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3kxtrrfon.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ojbxnjhl.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3hxqfguuk.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3vvjifcco.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3upsillqu.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3lwznmbrk.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3glgmgvcm.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3omuxhqzq.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3oesowbih.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3cuqajudh.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3emxlbjwe.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3tmffcydr.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3eavnrtdw.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3rnuowsap.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3zhckvkvs.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3arqomheu.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3kwifytcm.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3pizkiepp.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3oxztdbax.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3exzqqipt.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3rllewwub.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3xrmjigbs.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3tecpegsc.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3wgichhnz.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xgkoljhg.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3dhqsmetu.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3feriycxf.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3lpwyjklx.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3hpokltnj.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3oextjuhs.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3gstaczse.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3xiifzpdf.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3pmuyoaml.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3romvbbmy.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3fzmatilt.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3xwlyhxpt.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3nevwbphn.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3zlajsxuv.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3gjkzznaa.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3ixkxskvs.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3vcczuvmw.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3vddpuvhc.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3usudbhvy.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3ebvgtjlr.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3vsljjknj.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3ukacbghm.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3skdpqsbw.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3azsyodnc.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3hqhaibgb.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3sxnvuxgh.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3mxegtwff.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3urfiosqe.html


<!-- 参考信息 -->