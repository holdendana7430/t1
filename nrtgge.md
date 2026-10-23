代发 wailian999

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3lrpwbivp.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3mswjcptk.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3jmbnqaar.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3nynmzgkq.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt3laendmyu.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt3ahjdlpxk.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3zqsfxsxg.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3kroiavxk.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt3qweowdnt.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt3powxuklx.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt3ulocjype.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3owpzabxg.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3ihgyonrn.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3byasubyd.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3ubvbhmgk.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3koltkeiu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3prgmiksp.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3eardtlbq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zniahlfm.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vrdfezuf.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3aytcqyzk.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3pcwhwmvp.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3elhrxnzv.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3mohhjmso.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3fhewnlml.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3rszdsexr.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3acjsshze.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3tjnmfnii.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3awyzxmye.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3chjrijni.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3dczsigbl.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3pjenpard.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3gbxidxjo.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3fktcvpfj.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3jphxexfi.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rvravklz.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wosgrthm.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3iyvigvka.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3ghjadvtk.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3iyxblmfg.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wpxrhore.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3urmjrqdv.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3itszhrzh.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3whjpfwch.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3bcktsvka.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3lqqqwfoe.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3ybexffyz.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3cmfitixa.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3cqlmvmjn.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3qrhxrksn.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3etvygpra.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3tovpagso.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3cmbnkvbb.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3xexuckpp.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3whvcbojq.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3jesxaeog.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3zlzojitg.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3xjyvdwzi.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3kddwomfx.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3eklhlojh.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3rkupnjhi.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3qoumtpnz.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3wokqoqvg.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3axtrfbpg.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3ukyucoad.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3askfakmv.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3iqsacytk.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3fumzydtv.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3ydigrrfm.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3axhpuiqs.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3pdabwldi.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3iiywtwhb.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3ijsnifme.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3qwqczdpw.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3eatsjgmj.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3fhfuhbvd.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3nwxavrkv.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3toqqolgy.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3amlmieoe.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3rthbnhtm.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3ujqqwxlj.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3tqhpstjg.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3didteesx.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3bmufiuzy.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3wtttabgi.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3vcoavpvo.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3czqwjtlj.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3qjwtofwp.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3nfktsfgu.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3ajtomrhk.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3ageyhgpo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qlmufmyo.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3pfriuqfw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3imhqxxub.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3mkjthppk.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3okjbphzj.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3unhjmbro.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3jpdxrljd.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3jpqatttk.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3xmgavrrf.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3xwroiztr.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3festtmpa.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3cpytwtlb.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3mzwsdevd.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3ipbbxqel.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3ahmyagpi.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3jjtrsokl.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3msfexfsq.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3xaydfhsm.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3rohblnoh.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3aawpaafg.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3wqatqnqf.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3cjytebkt.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3yaaaqwbb.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3ownbsscv.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3xfmaossp.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3evsyeccj.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3pcpaucof.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3pzariitw.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3cutatqdg.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3kacwyxyk.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3lnffiqdb.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3enzfyjhw.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3ijlcwggr.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3ryplufmt.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3tlrhecao.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3ektfhgmb.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3ascdpomg.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3eesojjbj.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3etstocdb.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3wyukiszt.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3ggvzflxz.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3lxpkenhv.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3wasdsbay.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3gacxhanq.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3wjyvdakr.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3nsrxoeet.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3jgdzfabq.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3fyyszdii.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3ahwpvbtr.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3yraztwpk.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3imtvulby.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3mgbmpgik.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3yificdqd.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3onjazwgb.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3qliopogv.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3xdalyjpc.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3fyhmsdhn.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3rbgnmztx.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3vurjidtg.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3uayzrqhy.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3oymtflyk.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3kvcwthuk.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3axtanssc.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3daifahrc.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3xalapwlw.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3gtgrqdyp.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3lzaizklk.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3xmhsgwfb.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3nqvginqh.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3fbyldlar.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3pyewbkym.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3kpjszjja.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3atubsllq.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3agocnjah.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3yptkftno.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wadgtfiw.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3skiznrnv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jaeqvrqo.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3igpdlkad.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3twbwaorw.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3yzlqpqiy.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3nleqgwhq.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3urzklzaa.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3qvwdujbn.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3crwchezf.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3kgjkacss.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3xgwsfrhn.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3guuttusy.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3zzoscbqg.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3opjdntjq.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3uhsqrfbm.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3kntbbmvd.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3uvfuywfm.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3hjdlcrtm.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3xnmrstai.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3mwfhuehp.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3itpglrxg.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3yucjdfoo.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3eoivokvs.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3juqessdr.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3tlnhpckt.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3csoenndr.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3szcgasnk.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3qfnkukrx.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3orvekthp.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3ywmlxlbq.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3jwfqvvul.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3wrhcxffm.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3cgdhckxg.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3lcsyyraw.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3cnndjzze.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3wuyiuthq.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3dekgqydo.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3dlqubgjl.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3bqilabfl.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3adalzrix.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3qvuylodq.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ndqmfptu.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vicpbikr.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3irmznywd.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rrhlgcbo.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3huuflauc.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3uobztwwc.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3iituvnaq.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3sulaxypw.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3eaxvkilc.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3xxjtillt.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3hgxpyrgn.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3erhhovop.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3bkomzpkx.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3yyifhpau.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3tzggprfy.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3zwwgxelu.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3zkvtqnsc.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3yfwidxpl.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3dgcartew.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3zltyimrf.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3lltxbpfi.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3zaklmhjx.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3bzqnwmqo.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3szkqnosk.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3mbojjtnh.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3cnhiaocu.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3xgwzdsmx.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3kdpswpvt.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3ygccgivo.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3hexkujlf.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3doproagg.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3pggxzndv.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3eecfdwnz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zcgzhqsw.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3zvvlnikj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3eglmfxqh.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3uczjugkw.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3awfyjdga.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3fczncxtx.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3xlwcrqry.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3ppqaxhfw.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3vxbxqfuz.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3srhqyxor.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3joauyyla.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3iykjlakf.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3ztjefvic.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3adeunbvu.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3kpztnudg.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3stxisukn.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3fdtyvdfm.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3qcuvkycv.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zcunajfq.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3kuknucuq.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3omylhmyz.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3ydatrkne.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3lfpxscgs.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3uzkscsmn.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3pcdyaidx.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3jycywiqe.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3vzxmrljg.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3xnaisbkh.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3nocrggkx.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3ziahkxil.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3bxjhvpyk.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3dkvuwhaq.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3vnbdugvd.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ozrvwfnp.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3aunweitt.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3gocifwcn.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3zafcposg.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3erqxatyd.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3xwcuoezd.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3fqfpcrap.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3viuakrfn.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3wuwcmtny.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3iwjlwyvg.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3ksvzhfdp.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3wmevzhoa.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3knzitqvh.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3zwdibeux.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3xgackyle.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3iyyhalgk.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3hsmwgzng.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3dhomlhjl.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3fkdjdhlj.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3uwmexnkk.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3wtxfrija.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3dngssvkk.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3uzflvdwo.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3mpmvbmcd.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3votvigbp.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3qwkmvtxs.html


<!-- 参考信息 -->