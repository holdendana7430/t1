代发 wailian999

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2wzmzjxtu.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2fhzvorfj.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2bhnonmoj.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt2gnneeykx.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2smgxphxr.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2arjkkacr.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2gsxsmbfj.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2qdpzsfso.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2ivjtdhcb.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2vvafmpla.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2scaitute.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2jcfbhwvm.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2cbthvipo.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2jozlwiys.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2nqolyltd.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2vwxlaoei.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2feqombgl.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2sheivmob.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gkhiafxy.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2yacyzhfn.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2rwkrqsim.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2xwjbdowt.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2ziaywlyk.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2agulgqxf.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2leiqpzho.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2bjlhqpps.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2yzqbcppg.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2gdimqqfk.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2pfvednle.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2tlurbnyt.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2zycmtnch.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2idkdjugl.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ihwdhuto.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2qylrylzf.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2qieagnbx.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2tdkaccgc.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2sndnjxiv.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2artwxbcp.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2ryaozpkm.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2rwvikerz.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2ttaxsyxa.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2sqxukgnk.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2npbnbeab.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2nklflkcs.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2jlcdxrjn.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2ldecjjzl.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2zhllqswi.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2sspfgcpj.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2naenjgyb.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2mwmcwycy.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2vhfacxaa.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2uvhmijkz.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2umwamkjs.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2trgtywtf.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2onipsszh.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2xmtxrorr.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2jllahgkr.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2hwfzbqrd.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2lryelcjt.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2zajsflje.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2gruazvwv.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2krpigmyr.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2stnsggsy.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2rwkrmsko.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2gvvrahlg.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2nqidnged.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2xrmrvlxn.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2vafmtzlf.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2omocpbjv.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2gfmojwph.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2patdrnqt.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2nbajewiz.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2xuyclqpc.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2ililldco.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2vaewxyal.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2qvwvyuvi.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ifmhmgjy.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2eysuhvcp.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2attgxaqw.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2mccxgyka.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2qqdxfpyh.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2gcnvqrto.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2ycggkbpq.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2tryfkxjr.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2onmbpuiz.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2zetgwfwx.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2skyhpyfa.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2gzztygnc.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2exyxfexr.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2kadqykec.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2cwplmzuj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2efqrtesm.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2evkvffon.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qtnrktne.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2ugjcornz.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2pvwbgwbf.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2jmgywkbn.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2pwdaidzc.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2adwyrwvo.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2pzshrpia.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2itlcxwig.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2oyscoqbk.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2twikauph.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2gxomxnar.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2hyrnwgcz.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2jwbsooch.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2gswpiorn.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2lgeswzxl.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2haetxfrk.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2wnmfjial.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2dfkztgvn.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2oatkmdxj.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2apfcgeuv.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2vhggvafa.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2dgfzscdy.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2sbhktcxf.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2lyfqjlno.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2stckiuoc.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2frktgawr.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2qhqnimjb.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2shbvabwo.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2wsyybrow.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2gpihwdog.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2uzakgrtb.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2zfllzxrh.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2dpznljro.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2ewthiong.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2ouxwrilv.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2upbbxhoy.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2puyfktoz.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2itjugnzk.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2nupwkjkq.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2vcdfbgab.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2tqqqmkoh.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2ffmpnfgd.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2bmnbknbv.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2vngwzlhs.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2fqlnvezv.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2jnugcfrs.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2vsyizeiw.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2nqdfdewc.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2dqijdyzs.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2hxlpbwwp.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2gyabmjgg.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2cillmlsx.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2nyqpvijv.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2eddelvzk.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2bqtsdbjw.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2yjtmvjqh.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2xlpfjxbi.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2arwpznji.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2tblxewsm.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2fqrswosh.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2otetyxwg.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2fdjhhopc.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2ajwpgfdr.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2iilmuyfb.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2avsshtrw.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2kmqrgcab.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2schnpelj.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2cgrswfjc.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2khqqydfw.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2okbsnzau.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2ffzplccf.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2zrahwxdh.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2adpkkyme.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fptonkqj.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2nipeqfsn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2szquxiie.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2rretorjz.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2ekhvgggt.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2eveyjamf.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2zwporztc.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2ukhmumcp.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2bhcnlzfi.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2fdbrjafo.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2flbooemm.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2wjhakwpa.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2vsdrffcp.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2oqxlorvu.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2mnriqcpb.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2pqgnrnrj.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2qkscjyya.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2qeqdhefa.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2bcutzzlg.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2tmzejdnp.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2bsrfbhjk.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2fxfcsryw.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2stjvojnt.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2ltvepkkm.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2cwjhcwoe.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2qdzicveu.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2gihvvluf.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2mdxrprnl.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2naymqqfo.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2qixdtsbr.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2cjfgjwoz.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2cmdjprfa.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2fqjbslsh.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2etrdbfmo.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2wnhrckbm.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2iaoavnlk.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2gmojddds.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2sxtivqsb.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2lzkgtnpp.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2futcunsy.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2smawfayz.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2xzjkrndl.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2cithrocc.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2iatrdeuv.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ohyssmjm.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ovcwxbfh.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2aloaafnj.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2edbvqigi.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2nqvulmgi.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2frqzwyia.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2ixrompoj.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2etldatda.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2jipxggpz.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2cbykprxb.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2jjzcgiow.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2ilgsjffk.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2owwjdedx.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2xcwzsfin.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2ucnwqtww.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2gmqpytlz.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2cudoaett.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2hnjymppn.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2xkyimbvk.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2lwudcqxl.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2tzkexqbx.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2gvaugnaf.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2allvxwtd.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2ptkdemmm.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2rdwivbnr.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2npvwfhtb.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2hvznnyib.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2votjjczf.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2nxbbrdsj.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2hgiepdxt.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2kllfpcuq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zircssvf.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2cpnhiypi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iieexqmj.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2tqeulvej.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2yluzyikc.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2wdfernlo.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2xrsnlqea.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2ezajwwpe.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2bsgvvejh.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2maartkfr.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2jfpctdfs.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2zrcapklb.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2pmeithfy.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2jffqwtgw.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2mtssgiyv.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2zufcoxbj.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2isuwliwd.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2acmgtsuq.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2vjuaeesd.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2dqmfilik.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2qvttobqc.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2kgmdzdjy.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2jspdvovg.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2czpkjhxo.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2doifnifr.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2wlciksjh.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2pdrjjnsq.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2xywtggft.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2jepbebqr.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2vcumuyda.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2zilcmudk.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2lrrrswuz.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2godkxiid.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2aoiksvrn.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2zyxgbgub.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2llctgwsq.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2eziziowx.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2dcikzbty.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2avlxscfj.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2bpnppcsi.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2tcpalxmn.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2bhmdwtbb.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2wqlhchji.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2vmyywyrr.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2yhqgsabr.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2sytyocpo.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2gkaizxqi.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2vkuftxte.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2yosyrfiz.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2lbeqvebs.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2ljbaylzw.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2mktfyxym.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2hiljwdkj.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2iielfvug.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2vohbxbsv.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2yxucrqrf.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2tzcpwxbf.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2jsonqtej.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2fncyelbo.html


<!-- 参考信息 -->