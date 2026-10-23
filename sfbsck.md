代发 wailian999

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3zxyppviw.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3xpxyxuqq.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3xtqyeybd.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ugpahkds.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ntleaolr.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3rdqvxkmz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hahxxhlg.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3bwcrzfzc.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3uszuvadj.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3mmljjidb.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3rkumoini.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3xjfejexp.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3ynyfnnss.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3pqdrrfhe.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3mffjnnte.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3qynmaszp.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3pxkgakfu.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3llfzcelz.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3zotigtrb.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3thciiuso.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3zcmlzkhf.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3gvdjzlmg.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3mpclwyrl.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3dadznhxe.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ajzsdccz.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3axgvicxg.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3srmjezvq.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3rxrsvaew.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3wglofijh.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3cuxdssvz.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3xxdaskfk.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3zcdsuuhh.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3jfhjjrsl.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3ltolrihl.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3vigeequr.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3xrrmyqhu.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3abffiuxx.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3ihppkvod.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3acxvhdaq.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3hoinhkyc.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3xwnriuem.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3xxjdvhln.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3gfjvxocu.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3weejqqdk.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3kvuqmnzm.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3zqcgppvm.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3ijbsqwoc.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3kvtlugyc.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3vvwvokkn.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3jnifeign.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3tcyzcwyn.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3owivdxqw.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3egayhkca.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3yfkhjdyu.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3baqabrnl.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3jbdlzomf.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3cjjhsesp.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3lvagygui.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3yzfwwtbm.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3ayqiudmq.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3cjtwmlio.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3pccvgftd.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3oqyzttbz.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3qntmevvw.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3gpuffhgf.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3vpbqdcsm.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3ullpgsjk.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3fakkwxky.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3yflgvgcf.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ppurxcjz.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3badijumm.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3gvnzimss.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3jxvtbnxe.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3ctwprojb.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3splstnrk.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3hhidwvuv.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3qdgbojvd.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3eqbbsrrb.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3lfgaannn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pokofwhx.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3niztdhic.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ijbfazvg.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3qlvblnho.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3jvphfqbq.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3hrbgskao.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3kgtogtaj.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3phmhlfzt.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3vybkscgh.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3odeohdwb.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3ohpxexrg.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3owtfiazb.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3pkvyhojd.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3pvunpjnm.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3rtmyyetp.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3cbvrivug.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3zdwjhlhz.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3udntsfli.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3mkuhdckq.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3yzvikxxi.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3zuujblju.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3wuojxtiv.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3qxyaozip.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3eyfshpsn.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3aggdpexu.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3liwboofm.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3cwtcvbys.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3zqxcbgql.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3hhvgiidp.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3ditbdoyu.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3lvstptmh.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3hpdilamg.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3wznwdqxw.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3vbnkzwyi.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3parhnczc.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3dnosvdxg.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3lxgljugc.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3zoyfljxu.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3edscoxun.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3ydcrdipa.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3oznvoirx.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3otuxzufr.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3pppbzogn.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3cifdpomq.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3oobykebj.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3ybcyiihy.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3poyxcane.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ovirvizg.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3tlfnduti.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3himcewca.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3vnjahfwq.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3poxnnwym.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3oxlgcomo.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3dvmxmqcn.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3akfyvqus.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3kdaccakc.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3ihshnbrf.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3olahqozi.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3urdzsckm.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3asneotok.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3amtqywpu.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3pwyvmloa.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3mjulogik.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3lspzxjgu.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3qadpvhnc.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3juguqwch.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3wkxaxpil.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3uudfvlla.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3grrbzsac.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3ogxovjqb.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3eqdixivh.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3bvtqjwyc.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3rqiznubt.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3riwirjej.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3otcwpaab.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jbbjsglt.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3wctfnosq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jiynwozm.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3whtwwnhd.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3ndaewjua.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3fwgryfaj.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3gaipyyrg.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3jankggbs.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3igfcxsix.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3cprxwuum.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3ihlkghvx.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3jxhqgpkc.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3rsoxpcvq.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3eewcpczd.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3glieyvit.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3vjpffmej.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3zpmbmvcn.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3npbkrqxm.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3abxclpws.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3dymmqrws.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3smkfnnrs.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3upudbnht.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3kyglhgzb.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3ywpngnon.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3izvdvgfp.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3jmkuuyrh.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3wvmbdeca.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3isnitzrv.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3rzdxeemh.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3dhuhiecn.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3czaucrhw.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3hzaqcqhc.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3ewnopryl.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3ovkxdygj.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3pxgqeuaa.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3hhfaiifu.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3dcgqqqhr.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3lavjtqrd.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3cukghxzc.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3rznlgugx.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3nxjrhbzm.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3djytugmr.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3tijijbrx.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3pvecsnbu.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xgteypqn.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3sqcxtmnc.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3ixtiuqwf.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3jayjwrip.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3yyfhfvkg.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3wxvbgawu.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3chonyzaq.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3vwbmssam.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3pswjztlh.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ftqfdehj.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3uaaakwae.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3zmtwrjso.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3rxegordu.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3horemknh.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3iizuhfkt.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3lgjlasfe.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3egihvjib.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3hdmwbkxu.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3qkynzddh.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3euozwnaw.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3vrsxbnyh.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3fmqvohel.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3wkmjawae.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3ckzopxak.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3xzohrhdy.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3dobzgzho.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3jkgolppc.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3cyswmzyq.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3piwywqbu.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3dnwcwwno.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3mwcvfdaz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fqijjxku.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3molirzai.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vlyqhnns.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3nlcubufo.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3auuymadv.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3cixyxvex.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3dxygcbwo.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3ntbdgtst.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3zuuzmerq.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3utwaqtht.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3uqvxzyrv.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3sztxmujp.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3wtjewokh.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3kvaiqpeg.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3bfzrbwdm.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3rezxskfo.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3nxlbfaju.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3haefduzb.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ewuisjzr.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3jyhvweyi.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3fxbitebd.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3qribqbxq.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3klqptriq.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3ixgopjfp.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3ebejizpy.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3kynuandd.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3qwlqkdxd.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3izyygoau.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3wsuzvdct.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3ylbrbyvo.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3bdlyneml.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3omczwhsf.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3eknpupcb.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3lrairoki.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3llawxduh.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3xyefagtf.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3rdcbqelh.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ltiyuogj.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3iqbswvoj.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3bldmdzbt.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3tvwmjjjx.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3akzfflrh.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3wggrijmk.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3dnzbzffv.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3komwbxsb.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3vsbiyxul.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3qjqghlvw.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3bwqnxwxe.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3fusevrcf.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3lipqtdke.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3evfiowxw.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3awevykdo.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3wzvvkwfv.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3aylksdlp.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3sxwaowrf.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3byefolah.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3vsyypqpu.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3tzkmcglb.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3nekzhyoc.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3offgizvr.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3yjkdxpyt.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3joahvobl.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3ztlvrykx.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3xhgzyecl.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3sajvhpfh.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3acrxjtyc.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3puvigmlg.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3unlpcgsk.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3mwgyyvsq.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ioyrqzyv.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3brflpfez.html


<!-- 参考信息 -->