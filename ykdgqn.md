代发 wailian999

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2qjuwisdw.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2poqraoyw.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2ccnmwtqe.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2dmkuqjdj.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2okcazukp.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2hlbmulqb.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ewsemfmm.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2rpxqzrjq.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vfmneqcn.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2hzljwpey.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2ofhlteym.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2rgacsrbx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bbdddnsa.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2vwzsdemh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2upjwxzbs.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2uoxzdqam.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2zmmlefsx.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2kwjdsjcl.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2whoroilw.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2myudilox.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2rnmjyaef.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2lowiqpjj.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2umwfgvpj.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2hmvcsojq.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2lonrogsa.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2iewlykks.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2qexgkypt.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2yzliklqu.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qlsbjrwq.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2iendsgmr.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2ftpezuyt.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2cnvtaisn.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2rxzqzbvc.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2xnkygtyb.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2sxbzfglu.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2bbxtmics.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2llfmtrcw.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2kgecuojc.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2zqzhcaft.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2kcrnfwwg.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2ewhkombh.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2xkttmsjt.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2ivqbwiws.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2rnczeouh.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2qkdqcmhr.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2uoxgtgvu.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2hlgziexy.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2invvquzu.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2wpxmyshe.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2vrfqryrx.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2igxunzri.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2fuqmybem.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2fssjoxgg.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2vnpgfyvb.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2feelgggr.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2cpkytxfa.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2cncimejb.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2ygbxtcqn.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2kqfrxnwx.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2fgqobrlc.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2lqwccxhf.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2zwonuoey.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2dgsobzby.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2hyctivfe.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2ngtrvqdv.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2mkqabzef.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2yvyydxxu.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2zebxnhzy.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2rzfsedrn.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2kopgyssp.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2oajigqgn.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2tankxtre.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2jmlicpuc.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ttogslvw.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2myoosuyv.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2glbexkxz.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2pjnwtolc.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2zsbgeasf.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2dmylgtia.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ucrazmrq.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2orqqtxlb.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2lbjwuyab.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2rhmqfkrk.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2zxefyzvf.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2noyayfzn.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2oqtntwbo.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2zkcpexou.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wrxpqvxa.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2gbxhlgbs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2syfmoaww.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2rndkmxlz.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2hgarwyhg.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2mweqyovs.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2ynxdrknk.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2vzeksdzp.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2bopfzprq.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2ohklgcsr.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2nykibncj.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2igsfcssq.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2bhebeyqj.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2tyafhcxz.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2azdlnnlh.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2gjzzmynw.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2lvssczgg.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2irmfrjyb.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2uqvrlhie.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2fpmzueky.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2moeypvwx.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2iksyurcq.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2rizqxhzw.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2sfkvaodq.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2crcfwids.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2ikksrtkg.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2psokpkat.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2ufhsglwc.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2cayefuem.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2rpvpnmaf.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2jaeeswbs.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2ivxnitcm.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2zeyfpocz.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2xznnnqaq.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2hysujncu.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2kfhwnvhf.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2hnirqxwj.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2blqdzlez.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2aaxjysdc.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2vnohizsl.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2urvvfxmx.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2pmhkzhhu.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2lxcccgih.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2hsvzavay.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2qyvlfezx.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2lkklfyjy.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2iogbsclx.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2uhfgunww.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2aakoetpx.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2udntngcj.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2terngixn.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2rkjnfsjx.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2mtgdwrgs.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2ihhbuuft.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2cjpzquhe.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2qdrhoaep.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2dmvertnh.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2erujxiyz.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2gegvxthc.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2arfaekdq.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2guzurxjv.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2olzkyxzd.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2ynplqgwh.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2ogtqfaxx.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2nrzwjdlf.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2ifqxaxms.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2xnqkqubp.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2pdfbuwau.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2rkrayupc.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2dtodzehg.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2ftzqamlo.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2cvujgkem.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2jacaqadj.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2gevurhvu.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2wywxgndu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xtjtdgmo.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2cnekfiaz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pszhjpag.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2suhwtywl.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2nnobiola.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2khlvvydu.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2ysutqzqs.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2wygwrpfj.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2vbjturds.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2fguqtcsp.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2nwypednn.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2snlkpftd.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2ibpxtvqu.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ssxggfrb.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2lnrbneda.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2zyoqyhnh.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2ztlbmlvj.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2nwvukxxz.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2mhmupxzl.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2fkzwcmfh.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2hnsodqvf.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2pspabobp.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2uoimzuli.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2cljzifyo.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2pdwsttpe.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2yjglzkge.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2vmuvtgci.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2jftmlujg.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2beanztfr.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2uxlpejsj.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2leuauray.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2hozlgtbs.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2uqsjlhai.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2dkfwjruj.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2fxbqcggk.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2edaqbvpn.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ehdjdrsg.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2wxbptarw.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2inhlahra.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2pqsbjatg.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2lgmoywwd.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2rdpnjswl.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zadoyqgp.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2mpukekqv.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ebnggaln.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2bnumroba.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2gegtgyhq.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2fvynyzly.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2ozpbbdsm.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2yyqfrwaf.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2xyjqllks.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2fftpscov.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2opycddik.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2aoudjanz.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2qnzgzyhz.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2wsrretyh.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2efufsaba.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2vrrtuowx.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2qlluvhas.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2zdbzobml.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2glfvtfha.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2gntwyidu.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2sbsgepqh.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2tczzqjqt.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2gylfrmsh.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2cncjspuv.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2qpdzwhxu.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2ouhaopbq.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2gfhdhklm.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2afdwvtjk.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2bgmniuop.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2ofdvqtcv.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2ujimzifj.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2qmvkkypz.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2jwhrendm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kclsirhf.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2hgfwajzd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2somzyccg.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2mmmxaaky.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2pmvaqumd.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2iojjauzm.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2mawvvbjt.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2agpxyzxi.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2kblcsiqe.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2znkrfavw.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2fertmiqq.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2pmlpwevq.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2cbvmumto.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2zefvehrw.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2oimsvdcv.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2tjvjxdmo.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2nsaabpve.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2jqcozngl.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2pywghlyc.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2ovdraspq.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2fdsmyggg.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2grwrmoys.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2pzrhpxsj.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2pbtlbjth.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2ftvagxhe.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2npbfvlqv.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2jymtxwpe.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2moenjuwm.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2mvgpmfox.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2bggsayxu.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2bycjkzhd.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ocfweqdi.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2rfeymstb.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2ynpvhwbg.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2pfnkbkgh.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2loqwyvvb.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2vcpapcsc.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2jqzzyleo.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2gdgqixje.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2qstzoqrh.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2wdimmfjg.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2qsmsfgfx.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2argfhfvj.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2qprghxfx.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2pqbrcofq.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2vwwejdoy.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2jiiougnx.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2pwqggvxj.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2smgkfbva.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2rraspzph.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2uptzhlyq.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2hvfxfvmw.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2qouiarpz.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2jctcdgtl.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2ngjmbwrh.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2odgovrtz.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2xpaexnfa.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2hznfjpga.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2negjrwmo.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2jxewlvqe.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2hnunmpiv.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2obrfwpak.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2fivqenmc.html


<!-- 参考信息 -->