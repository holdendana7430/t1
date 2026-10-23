代发 wailian999

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3fdyqkvhm.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3xrhpigbd.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3tmsimqez.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3iccawdmn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xjrdjdsl.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3apvfiunu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qxqzazmo.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3qjzvggxj.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3eissmdwp.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3ingklpaw.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3yiwxqkff.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3jaerfunf.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3aszivzlu.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3bmvmxttu.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3sjziksib.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3wgfwwcei.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3iroizyab.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3oonrwyzu.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3avlojajh.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3doaquabo.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3cehrjcnw.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3ljwjyqmj.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3uqzqhbuq.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3bdtvpenu.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3eqyetima.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3ckbmzifo.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3lwrxhalz.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3wrownnfh.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3hwysyykl.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3bspbvcyf.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3imotrdqv.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3rtpdewsl.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3wotqmpob.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3npeedzon.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3tnykkmmv.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3iknzrqpd.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3sksqaxhg.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3njdgqlis.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3umuxbtai.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3oqqwsxdl.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3qsjjbebm.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3cuyfqfbh.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3qtahqxal.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3ynxnlkor.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ikplqbds.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3mtdzxiwo.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3glecaajs.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3rdppdoby.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3hylsueki.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3gcfnqixl.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3vcuchhxv.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3bezdlzqa.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3hgbnqvor.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3rzmbovhx.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3umlpjfaq.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3bdjduhgy.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3runtdqfn.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3mstjgaud.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3vhpjdjjd.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3xtipflyn.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3wgjumowg.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3noronucs.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ychxybxy.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3pmugrqrf.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3oouvuqge.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3skinafbp.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3wxfziwkw.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3udtdqurp.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3vutcqffm.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3vcliztax.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3hzqfojjf.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3hjvpxipy.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3xzkbowsi.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3gsfxeqim.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3iapmexmz.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3lizgxary.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3vwramzwq.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3gioyewbx.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3xqrdbcys.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cltbjltk.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3lxqmswpi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3frrruzyp.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3whyqzcus.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3slgivyhi.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3dpkdxytq.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3bxczhlkb.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3diegczge.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3oinhfbpt.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3qseiehcq.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3xulaomup.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3dhysfnts.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3oxvooxjj.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3mkhfknkg.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3yjckjqul.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3tamwjxyo.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3gcxqwohh.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3zddezcjv.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3jvmltseb.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3yccpfzhn.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3qxfgfvbr.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3tehobbhp.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3gazyjugn.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3fjdumdlc.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3zzewlzkk.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3fymppotn.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3ivzxldog.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3orknbxfa.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3cxrbfenr.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3wwnbzedh.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3ssxquwhn.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3lkidsidj.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3kjvqhbzw.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3eoxqfpnv.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3hamjeghw.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3trwniyaj.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3abtpoolp.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3qxjuqapj.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3kclmvvlr.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3vwddzeef.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3jtvxnern.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3uruddesi.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3wtycogtw.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3mggqbkkt.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3fgpquyiz.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3lhjxrotm.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3twbymfpt.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3updjulxp.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3xhrmkbhn.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3xeceqiai.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3lzrkkecb.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3tupkpbyx.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3hkxlhwyl.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3simjxpeg.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3jnatzgup.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3ydqruqkx.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3vusnnszn.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3wmefdmum.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3gvvljrrs.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3azhrfhjn.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3qythwhuo.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3owachuve.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3jdwxfzcq.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3mzfsybvq.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3wvryldvg.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3sufputui.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3igynqqkx.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3tjdbguiy.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3spwcwtwz.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3ehxlmjcq.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ejvzxcpj.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3kqwelbsj.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3pgofjrei.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3eaxvlzot.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3gcehopwu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3owghlalw.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3ugtwllif.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ynwjbzkb.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3dpepelup.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3fgfelrsf.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3sjtykfzd.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3tieyqklv.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3tkiqjmvc.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3bmoypvui.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3cnyciilm.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3zwpeujfi.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3nqsnofmv.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3mfhysjah.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3wljbmjoa.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3gaodygxh.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3wigbmrlq.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3hlomhqsu.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3tpryphgp.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3apcdzfgw.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3wsxxojlu.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3vxtbpizs.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3cptmjrfe.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3okojhizg.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3tiljfcmb.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3wkumeysm.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3logjfnpb.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3qahnguhw.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3qdpfhaeh.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3rvaisdng.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3bkopstqr.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3bbckjdvn.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3cfizytkf.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3djqgzskx.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3yavlamcr.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3zwdvkxrt.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3mremfkia.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3tqmbuybp.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3vpvkfebz.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3bbqehxlp.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3qqnhopzq.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3dusyusgx.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3qjpuxhek.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rwsjvoxu.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3tyadjvvl.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3fvkxszfl.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3qrkoktaz.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3metqnmnr.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3dpguplcf.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3uydgxhic.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3iovfrfmc.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3lwounpew.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3oxgdyxpc.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3hxjlkxzx.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ydeocnia.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3uxlzjnpg.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3cheshzpa.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3fxgtpxcb.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3rnyhinuc.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3bolimzej.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3ybbjfovn.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3ohebyviq.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3ieylqeke.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3sbgkzhmy.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3jilpwhth.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3srtchceq.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3jxablmcg.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3yedzdgjq.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3hxczsdur.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3vyuyauae.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3vciqitjd.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3iiycfbus.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3uxjopalt.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3ghyssmvj.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3cabsyzyb.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3acwdhakv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jsfexkzm.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3lnlopsue.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hwdfqckp.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3rdrymqfv.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3zcnewzzt.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3tdogytiw.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3arzjgrqh.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3zocprtcj.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3cpjgzmxz.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3dfbqnjxp.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3zgbgcbdj.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3yijvhabu.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3kjlqcjzj.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3erpmhnbx.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3mcalousy.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3ysplceho.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3gheugqpr.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3iuvyefxx.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3zpetdakk.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3ewtkmtjs.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3cangtewu.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3qrmumyca.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3qluiccuk.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3bztfqwwi.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3mplrcbxs.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3rkacvzea.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3cvbylcnz.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3nexvyghg.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3wgecktwi.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3qqfkyzzh.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3ookscbza.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3jluapwuu.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3iydzkint.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3uxnyjpbh.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3trkcawtg.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3qdnbmjsf.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3juuozibv.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rdsrmsdl.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3tpataugt.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3ludykxer.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3slbdrnqf.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3zaeewpkg.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3habepagb.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3ggqhando.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3edooflig.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3iypbjnrh.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3exraqnra.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3jreieivx.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zvvwunnh.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3ltopbkui.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3vjxcmqtn.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ecpexmdw.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3kjdowvpk.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3csmaqxhz.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3ppgyrhlg.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3hhkvjrqd.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3dfkrakbj.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3ltiecjfs.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3hqprpazr.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3kazjhinr.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3wsaifwye.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3wvybbppz.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3xermbbvc.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3strhjtyq.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3lqnjerye.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3ypytoaaj.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3yuayfsgy.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3sbdapxnd.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3nzaivlgi.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3fnemvaqn.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3navcewvy.html


<!-- 参考信息 -->