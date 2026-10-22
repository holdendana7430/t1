代发 wailian999

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2gxdpfblg.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2zykwtdmm.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2upfuizqa.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2cozdjzys.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2yrwmbggw.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2icqtkkdm.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2njktnfzx.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2kpqvcvji.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2utchvkzn.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2pmasivzn.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2idaxabyx.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2mahonkjc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xlbixauq.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2kwpeoysp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2irklzbkx.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2skkilyct.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2oeoborau.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2hjeigrwz.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2dbiatxxt.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2jatljfdf.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2ighepwrx.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2lkonqeet.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2rprspxsq.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2lpvfbaft.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2gwekkfvm.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hdgjvifg.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2yplhgglc.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2aecmbtso.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2uniplsmh.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2pvfsqkse.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2nxhfuhjt.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2smfpuerj.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lcjqnots.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2fqjngrqm.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2tzqkuzil.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2bdfuyqlb.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2rgaarown.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2cvozchqs.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2emkvttir.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2cgjkqxms.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2jjjcsesf.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2kvxdujdi.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2cynsffom.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2zafnusoc.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2lpmolmrq.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2ddsrgosd.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2afgeyblt.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2btoynesa.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2kqmgtpxa.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2zyxjqmhq.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2lkbxkvma.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2xmorrhab.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ibhbqpzp.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2fcanlpeb.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2qpuxoxcq.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2divuhzqc.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2pytymidi.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2pmuklltl.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2tjodtrwh.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2ablaleqk.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2oqnmxmjt.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2pmzxqdzf.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2jyyzqhis.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2pydhrwni.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2gvvrnqul.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2zjenlyqp.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2ytjdxxfq.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2kzvgiljt.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2wxspsmzc.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2ekzszbne.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2sdaxncfo.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2vrhgtdoo.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2jylbxkpk.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2aqnzxdou.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2autefugs.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2cydccser.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2ybopaqmt.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2tnbrjmkb.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2dczkxfzn.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2hyqfnxom.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2uhcjqvwt.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2muqcjcpk.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2wrkagnge.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2orvwkiru.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2whzdznvl.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2altfidmk.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2okcwoymc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xgbndqfd.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2zpafdvel.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hradcezs.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2ylqywrcs.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2upncfpnu.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2kenkefkj.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2hqhvmlbh.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2ulkzanco.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2jsotcidx.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2pdxnombz.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2emiqgvrx.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2cpaxaogj.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2tmovbowf.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2gsqdckbu.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2vjtdheqs.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2ervsiqzn.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2reoefklr.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2ystcepdd.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2dhhdloyu.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2tnrwjtxn.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2lxucsqqa.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2zwhapgbk.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2tapkoqeq.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2pnnirtxm.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2ftkrszmu.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2ltbxzrie.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2hetmfsst.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2yhmprbvy.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2wyyhcmri.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2kvbgtall.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2avcjdkgx.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2xohxdxuk.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2knoqimpb.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2kviuzdbz.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2wiwpvard.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2tyxcqyoh.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2jurxeuzo.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2mimijbfw.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2wsvzjdyo.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2kqrewhpg.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2ogruolyc.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2psqmhcgn.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2jgvhnkjk.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2plwxexsx.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2nlnfrxsy.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2pumcmnlt.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2qoxbvmgy.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2rusjcaul.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2upuptbrf.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2mrveeywh.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2qakrhwvh.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2ynsrpwaj.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2lgwtehfu.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2zxdhrran.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2eehsdtlk.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2hexekeoi.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2oaomtzii.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2hamkxnpx.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2yoigoqoh.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2ltwhkflb.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2wkuhmtam.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2haoliiuz.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2qzbohnap.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2gnhzxqyz.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2heoezafu.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2kbmbcdxc.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2pegksios.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2gxnuthfp.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2lkvwwuaw.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2cpleesgm.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2nihugdqs.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2yiwmjspl.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2puvujzxl.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2qqkdosnd.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2mxsocjai.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lxpvfslk.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2cwbxknnv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2prudzxli.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2gufkzbol.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2mvtkwoec.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2qzejkecv.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2mexblwpf.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2ylgczjrq.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2szbcadrb.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2tiyyjacc.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2tagwofih.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2fnfthrni.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2gcwfccaz.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2uwsezipw.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2bqpmycdl.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2uvcpkxut.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2hpwtqwlz.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2jpdzabfl.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2lfahmqjz.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2bsrzfcaw.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ntbisbuz.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2izzaocdn.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2hxbotjgb.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2tsdconyy.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2bekdigqv.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2vnqifciy.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2xbgwbpaw.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2nktrsyhz.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2ncsgfiky.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2nznstmmd.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2aslcedda.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2lwaraihd.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2fkiqxoiw.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ryfrtvkz.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2fsjwicwe.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2cbjhatyc.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2cqsnkzgb.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2iluteqgc.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2evohwucz.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2jvrndjjr.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2pjokdqcq.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2gkarmlsu.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ywdzhfav.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2miljfhbt.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2bfetuptj.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ptuvmdkl.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2lfsagvir.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2przfrfuj.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2rlltwqvq.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2ptmviywg.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2eplizxsq.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2xcoatgxi.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2ixnbzxfm.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2veunvwke.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2xqpsetvv.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2tndhemfz.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2hgwxcgja.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2mwmqjrks.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2nqmdhlbd.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2cvbeapcq.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2wbqhczsg.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2vfrxpmew.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2kbwmveqj.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2uxngdvad.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2phcvsavf.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2rpumksct.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2jngcworv.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2wrxfldoz.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2tcqxxumb.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2kswjuaks.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2ycoymnqq.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2umvogsep.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2wiliuqlj.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2xlctvahj.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2drbcvhga.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ckhguekd.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2dvyouqns.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sniycnpj.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2pcbuohhu.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2zcbjtten.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2suiobeuk.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2tcomsajf.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2hbiffpwz.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2qgqcliuz.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2zjavsgue.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2qczmpwhh.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2dqysaryt.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2tbyfgxtt.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2bzwjfpuw.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2xcfnwfkh.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2enezjaso.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2hjmhzdqb.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2oicaibqq.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ewbbtkji.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2yigbeczd.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2nznywlry.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2vibabdix.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2gtzlnxfz.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2dyceegsb.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2ymoeepdf.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2toosswra.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2dhhptnar.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2fiuhyatk.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2odgufavq.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2cjpltcip.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2ephtnble.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2pectatky.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2pruvnwhx.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2smgjgphf.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2lmtxtzxp.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2ihvwqkbs.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2pqkuhjmd.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2dxtctkjc.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2zjppyfpd.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2hlalmjwp.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2bzxsnfth.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2gjebecln.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2ovglsauc.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2exllfdkp.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2crzuslsf.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2jyqcpvff.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2klhttjjf.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2djmotrpr.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2fmcpbnxm.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2xdnbvzvw.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ksuzyzie.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2flxetqsv.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2evbrfzlk.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2txbbxktn.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2mwtfetig.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2wdvvapvc.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2ekpprjmr.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2kwbmrwzu.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2ciupkibv.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2eemsglwd.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2otctgzbp.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2ytyxqrhw.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2cvkiciux.html


<!-- 参考信息 -->