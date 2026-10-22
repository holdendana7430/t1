代发 wailian999

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2rwptpydc.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2vavbyghk.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2zgmlskmz.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2mmghuwap.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2fisxldnn.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2qkcsjogw.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2gigmzznv.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2mvimlgco.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2fsexneit.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2anlbsovl.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2kibsscsb.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2zizulewn.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2cdlvdqst.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2xadacbka.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2wyvyqrst.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2qtbttwvn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bleaxpop.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2crtxslwx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fzbkttqm.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2iberlytt.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2dntuwffn.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2ecyjqpos.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2intfewgx.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2uuwfwfyc.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2csnneofk.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2fdqkllhu.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2jnsxhtzv.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2paqhxrxe.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2svcnpmfs.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2ylzdlpbz.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2vuhxbuxf.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2eibcaasd.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mrczhzaw.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2bfuaufpv.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2kcqesrqg.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ysgrbtkj.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jbeqipkk.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2pnafnzic.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2trignssd.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2qkvyezoq.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2zmdjrgnf.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2jtlaaqkz.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2ruqtanob.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2vqjocoau.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2gsbxoknp.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2vcnmugml.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2terdxuvy.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2nykqkpxb.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2zzjpgnpn.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2yhtbbkiu.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2spmdidsd.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2yhnahshz.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2qaguryzx.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2spwtdpcv.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2kevndtbw.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2lwrbtkiy.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2opqddjxz.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2iojkjdlp.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2mjfvuzma.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2mmrmaqaj.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2mwzzsrnh.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2nftzuoeu.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2wryufmqc.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2qbcygiih.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2egqvpcwr.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2ycvljrsx.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2yfisfjlj.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2wqmqzhip.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2stqxjwib.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2podsrxyt.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2enlnyijd.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2kjuimzlm.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2mbamvxib.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2qrzuuhye.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2mlihekeq.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2ignydwxi.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2mifoabmo.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2lwxdaetw.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2zflsjsrd.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2sjcwnjxw.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2fijblcyb.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2uymkkgil.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2mrxghbch.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2uqhlsfoq.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2tnvovmun.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2ldyrziye.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2grmjksrb.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2ayzoxjgz.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2lgwnasvl.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ustvfegt.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2gmkdgczi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2slizswfl.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2jdyeeujl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2eubofpea.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2wbufpqlm.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2ldhtvffb.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2vjmdaktl.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2kdfkifax.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2qbeofeij.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2fprtyyzm.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2viumywdl.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2uiflrzct.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2ktkpxoga.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2kzqufzjg.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2xjrxwagh.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2qlcmyjta.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2qjohnzqq.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2veungnjw.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2foauspwx.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2qudadxqe.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2zahwqpiu.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2holwmhsl.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2clzrfrpb.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2skjiloxd.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2wnzerisw.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2kjqppxgu.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2ssohnegn.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2nojwnutd.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2izausbax.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2uwtnuvjx.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2vjvtsdpu.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2zrkbljyr.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2oktjbrrq.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2uzrkaezs.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2zjozmpfs.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2myvxonau.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2yzfdxiwy.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2qdwyapsy.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2hbwstpes.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2rhbvzsog.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2rqzakjrj.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2qjriqgil.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2penyntlo.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2dvijfzqn.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2nyzwhtzg.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2qgvssxgj.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2qddhefvf.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2qnwfubgx.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2dnqcukee.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2pitbtnon.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2eysfahks.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2ejoexrda.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2wgufcunk.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2evsjfcpm.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2pwjmxokn.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2drpybxgw.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2itffquhs.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2skiljcrp.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2fpgtxrnw.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2cezmivwt.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2jdmgscbs.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2ytomwzci.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2pgsigkxw.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2mozknyhj.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2vrqwgbbd.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2olxpcydz.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2lyqzsjvw.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2ouukltwn.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2qdkdadko.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2xzevmnwd.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2oqbxuaic.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2zpxiaipv.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2sjxbeqyx.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2tsrjyvfw.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2ivbiyqzx.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2feouviud.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tmimqqom.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2pprozlbg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kfedjsdg.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2vrhtomjl.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2yoifjsmx.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2vpyrckar.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2ineiorox.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2kzecglri.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2srhyqelv.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2pwqjrfxb.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2merthbrt.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2agxjaxac.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2tuigcazz.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2oambsgfl.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2nljjloed.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2lfenbzee.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2hceksojr.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2twgmxgei.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2yrombtjn.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2cpxrjnbi.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ilfmzkvj.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2aulrkbvb.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2vtzfzwou.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2plfuhlng.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2egscswzu.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2xbqazlla.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2kgrqjwse.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2qibkacvj.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2gghnpphj.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2nlrmcfto.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2gozzpwrn.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2trytdrdn.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2mtevqzkv.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2pyaagmyf.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2gfdexopp.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2ydiirwmb.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2dqhzawne.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2ohkfqysz.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2fhrejjno.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2qbuiymso.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ogglymrx.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2irzoldtd.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jpvxhkwo.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2tlquhipi.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2rzlhfiph.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rdzxsvla.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2faeuiszl.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2eaddsxby.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2bcqfijld.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2lrjbhlhs.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2oxuowbys.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2wwsqufwf.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2bqzhmhgm.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2olsnxbsj.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2fphnjygg.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2lxenvvmt.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2ncirpent.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2beafgsew.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2suiuvnwv.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2mhzwzbya.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2zmjdafmk.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2dpqpaunw.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2ovjriqsy.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2nuflqgvn.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2fbstgpml.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2hfggwgnd.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2tncoldjw.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2yjrqokvy.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2nuhvwtto.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2pxnmjuwd.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2bxackiyd.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2ywfpliry.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2yfrvvfvg.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2fribuiam.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2wouoriau.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mmszncpr.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2tebekcak.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2elujjiey.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2cxjcvntd.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2uittrztv.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2mhwvhxkd.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2hqvxxopv.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2ncvhgokx.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ofmrxdks.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2dzujxkwu.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2jraqnjnp.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2inlsbxgs.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2mjgwjmny.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2slfzxbsx.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2rnenvxqt.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2pqhzielv.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2xzsszqxn.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2norirlup.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2qtyiwcgk.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2megaqkxs.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2rbiyiykp.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2nuapeqjs.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2utlspqxx.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2vjdahzxy.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2pcbpszyb.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2etuuiarp.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2lonolkij.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2kixtrilv.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2vatcdqqo.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2ibejnyhn.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2goxdvnmc.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2pprsfman.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2jlmyeizg.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2hnvjcaux.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2itnlczcb.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2jonkwter.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2wsopmqqy.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2dlmzsdgb.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2pdcmaydd.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2niomeknl.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2jrltofti.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2fvgvygeg.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2eibmlasd.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2cmezgczp.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2ddkwcsou.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2zzttqauw.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2efpzghjl.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2zvcnrcom.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ipqpzifi.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2obyfbpny.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2xupuasvz.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2jdzvyjot.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2anmxopsl.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2sgrycnky.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2spsdykjl.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2zkusbojn.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2bodezorv.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2bqwixfxu.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2deropgwc.html


<!-- 参考信息 -->