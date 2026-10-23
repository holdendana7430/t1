代发 wailian999

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3nulkozaw.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3cbmzaqrd.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3gpkcpmou.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt3gmvbddne.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3cxumtvra.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt3tcliphzm.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt3fwxllprm.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3nmyzsjhw.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3dpjbndkr.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3cbvekizo.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3ztrspgla.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3ezntszlv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bvzqogng.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3shaoayji.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3itedvxrl.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qapimwhd.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3xldkqgwm.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3wftekiox.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3gtutobrz.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3xiktmpcq.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3rmlxgzxv.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3satpwkfq.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3lzfykelv.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3belcusis.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3yiodfanz.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3pnqnfbzk.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3eamiauht.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kwgfwbtk.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dhlmmbma.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3bssidrdq.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3zklbaedq.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3mwfivlpg.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3sgjdbcao.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3cplfkvlz.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3rsxzoshb.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3kmaavnxa.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3myndfclb.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3mbamsqpl.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3dlodmbhn.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3qdklxzit.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3jjyfypcm.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3rskfpeli.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3jfhbslff.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3yhhgesvm.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3orpdmxos.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3rfyfwpie.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3xdcgqwed.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3yqjwakyy.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3geqtichs.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3egkvxlwu.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3uktxoesh.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3rrxfoqoz.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3uzfveuhu.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3jbnzuyjc.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3offhlshz.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3rupqmarn.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3pkepwktw.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3qdlirese.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3xlogocgb.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3mcjfvyzt.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3priugdxl.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3datfopoi.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3thvxiith.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3nrwkustn.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3ovwlygtp.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3kbcwpdgn.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3uvrovvyo.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3dyidaedj.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3byskuxpx.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3mdmrhmqx.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3zacylepy.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3yamfwjvq.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3lydwrbuj.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3dpyxcnyn.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3baoaqepf.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3edasiujf.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3sfgsatag.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3eazzwqwo.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3bjvgaztj.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3xyidrqms.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3iglxtpkc.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3lzkexkhc.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3szkxgwzd.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3clkwkjca.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3xfqklabg.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3usnsftrz.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3pdddpahv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3doigmcgk.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3wvwovytv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wtcykdcx.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3jrqckpie.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3jnnmrtql.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3sycnpaaj.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3ykxqtwta.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3iizsncel.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3zlbixzwk.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3rwxozykq.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3bzvwijnw.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3rspncnob.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3hjqucirw.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3xlfpmylu.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3mzsjpmtn.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3zslslsai.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3jqaxxled.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3gsrslykc.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3lqlthicf.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3dhcnzzgy.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3ncgiwewd.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3jcbwohiu.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3qyiormcc.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3rwitvrcg.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3rxzpznfy.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3jnruzotk.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3bgrppkvq.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3khpppdhc.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3pkgfsevi.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3xqaugwhx.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3jdaqqqmu.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3dzlgfzyi.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3mnkndtry.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3ynycvgbu.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3pzivqprd.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3pmmemuqt.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3llcniyio.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3bnawmbwf.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3fmxkklnw.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3vsrbwrsr.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3mthjijai.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3ywhstheo.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3hlmxhkfn.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3tzvcgvjh.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3zyyksqon.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3sjclnckx.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3vxgpvqux.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ddraqpwa.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3cqjbmbso.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3tuuwrbvx.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3fehcftsn.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3qtxqbavg.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3lrktezqz.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3skasygwu.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3buxqanyv.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3rwlnrpry.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3wxepehdf.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3qimoppjv.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3copltzdi.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3femztric.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3uxsdokah.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3hobmiijg.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3mtbiqddr.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3scdtiiuj.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3kdcrhykn.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3dyjxckem.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3vlqxfpkg.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3byperbkx.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3jmlyxbun.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3qqatsuna.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3urumazkx.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3oacweedf.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3iwvwkqex.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3uzuqigmc.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3vbknopfh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ctxwhzoe.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3odedxxca.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3akgowxuk.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3ljadavva.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3dwsgiawa.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3iypbtugy.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3aiuojmzv.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3riauzkdo.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3goavoaxp.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3cdckqhlc.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3rgnsrepv.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3dbqlkigq.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3zuewntfi.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3czalmfem.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3uglttxbc.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3bnzmaqjv.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3iovisjno.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3jdzixaaq.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3empirkut.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3dgcouclx.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3flttdmpz.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3rkkhyguv.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3faxscacf.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3hulfbdhi.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3howysdlf.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3zlogpanu.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3fhtcmupt.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3tuyxtecy.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3whohtfdx.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3fwykhyyb.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3tggfzhct.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3bioqtqgg.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3oihzlfko.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3yhpinlxs.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3pjtllmdz.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3jrfxyinb.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3vcfhmfwc.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3irmjzpnr.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3pwrfjgdu.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3hnyttiuo.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vukmuxcg.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3cvlyqklr.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3dbjxgmsr.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3dcejflpu.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3keiqgker.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ftnfynuq.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3vrzcbiev.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3yjdggrhg.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3gkmguxnj.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3sjfxsglj.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3wwmgubum.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3qrepseox.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3mcqhigmx.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3kkbqjoki.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3rcodbqxk.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3kaeuqnkb.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3bstatrnt.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3khgbnctm.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3qrvssqor.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3rcvdtrry.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3rddekwee.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3hlsalhze.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3evdbactf.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3feiwhfnh.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3vzlacebg.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3dvyklpwh.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3xlukguil.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3kbimyruh.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3fwuxfhxf.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3pvzdgudd.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3enoirbkm.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3abxwlmol.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3zyqaoxdq.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3ctitcpai.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3rvwgcofb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3arkyaunc.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3wtvsmvjm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mbbiijnn.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3ouogprzm.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ugewmpff.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3zbiznume.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3ixorjkdt.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3ugyldtoo.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3vjrsbnjo.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3doiivfjv.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3hsdezlif.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3pwiznxny.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3nojlchat.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3omjgxqxs.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3vpivldca.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3vduebdby.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3moacmcuj.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3chfioxxv.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3seiremhd.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3aahkzaex.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3gjpgvttj.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3btpnqlxk.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3nuxixbia.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3ubyrcobi.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3spuvzvpk.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3vvdvbann.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3uushuwuy.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3pvmcochf.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3qpypxusk.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3ttvijwjy.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3vdmlsgne.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3pypttqvw.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3umhxmyay.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3qbnzojvi.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3leobvfrs.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3qqiaczgd.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3xvsqcdqq.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wqbbairt.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3ucwklhbn.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3sibrbqsf.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3vzrxptep.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3iczcgirz.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3xfargmsu.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3jnewkzcl.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3luqjalfi.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3jckimyug.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3zgdatybw.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3nhiuducv.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3zmxgzcod.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3yfbhqdnb.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3yqkgcewu.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3pdagbcxz.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3sxelxbnu.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3xbqxkyeb.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3xxpcwyyc.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3xgnlwrdv.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3oniuvize.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3ljshojdi.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3acxxftof.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3nszmpwrj.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3ojonshnp.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3rooodwpj.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3hlfizica.html


<!-- 参考信息 -->