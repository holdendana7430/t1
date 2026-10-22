代发 wailian999

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ynesjgqp.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2mgkcnsjd.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2hyigqpuf.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2vtgfmdth.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mzmunwht.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2dgbindam.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lqhtlhmp.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2umqcotrq.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2zhxespvy.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2jzrddowq.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2tmjnquyw.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2yainkkmv.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2bdbfofdy.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2nmvmyyhe.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2gzyzsaje.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2pcjhiobt.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2vvwtkrgr.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2xsefknwe.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2rjsuaete.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2qmcoecaf.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2cwavljid.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2flfssvfj.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2gsxitmff.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2foiffbsj.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2myfwexsj.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2foqxpqnv.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2jvehnhmp.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2sqdloigj.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2hkgrbwio.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2gqusfrle.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2alwzhadf.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2duhhaxai.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2vabpxrqk.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2dkoxesbz.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2ivkgymin.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2yrvgzytd.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2opeylbxa.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2fabedwrv.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2tdwizpqb.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2jatuckko.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2xtvfqlic.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2kxijuhxg.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2yuwvxqdv.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2hcukntyz.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2sadvhgvj.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2ggfbmuse.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2mdputpsp.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2izjtyzho.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2brfmqygv.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2gllgpkih.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2gtdqgjgv.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2afsfuldg.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2snkfisqb.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2wkfaxwoi.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2sguxwvau.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2xvydmbza.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2hzusvcef.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2bxgssqkx.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2drrwqtpk.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2cfrexsae.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2oqwhbesg.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2cnxcczdq.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2xlbukycc.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2mwzipyna.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ijcqycej.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2hhyozvdi.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2wviivmle.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2ksizdcdw.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2nnywgjka.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2jpbrqwri.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2zxncrzvd.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2ziqxrtot.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2ephwemqi.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2lnpksujo.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2pogkardd.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2esnbauix.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2vdsrqukx.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2vzxjtjuu.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2okobvoai.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zzyfamlc.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2rgqrbden.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uoeodxsu.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2bcucjngm.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2humxluup.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2dyvlgywg.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2echviedo.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2xptrmldr.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2wcpnzaea.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2ljoxiplo.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2bgldzbia.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2phlditmv.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2pwlcfkax.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2fjvlygea.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2chomezzv.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2uwymshra.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2dlkhmwvv.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2vipkxdzg.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2ztmxlslb.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2bqoverhp.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2ngnmnnnm.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2pqzswjca.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2pvysufev.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ssidkcdk.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2zzyrrqoo.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2zvszcncf.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2kwnvzgeq.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2bhwjrltt.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2rhkpiieg.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2sifuieqx.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2tzqzqdmt.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2pbseetty.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2nndebhpb.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2euylhjij.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2sqtfjzft.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2kcihahca.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2dajwczte.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2eikggrpf.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2kyimegmw.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2zmuejuxz.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2murpbovs.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2yngxtqhi.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2jyylnhvz.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2uuvqzncr.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2vwwwxhfy.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2xzryfnrw.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2lgfrbfbg.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2kqndidpc.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2rqpamojq.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2jymrmjmt.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2krvahqyf.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2wvzpfnat.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2wickofqb.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2wjeaqclx.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2feqeqyqv.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2favnubch.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2prccgbnb.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2oqkslqcf.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2wwqsypox.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2dludvion.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2hjfcuhvn.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2blroajkk.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2vuulwsem.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2lydfqzdu.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2tqwqgnza.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2opjdckvv.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2ispltoeq.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2lfqsmonn.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2arzfvfqq.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2vpyuxlih.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2axcaflra.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2ftqohgob.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2lpomlerc.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2edpxitwz.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2lthsnpyk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ruzdebrg.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2cwpvpqbb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lcbiqida.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2rkzzxlvz.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2mowwfqua.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2vmyrirax.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2yckcogts.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2yngwzama.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2rbubinbt.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2fbpnmrzr.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2ngudicnu.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2uctblhjz.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2aafmzrbu.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2afmvnkiw.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2jeqhpcrw.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2ugjuhtmc.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2frggriiu.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2asjcyjyb.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2blinuwip.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2vgwaimvc.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2pccsaypn.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2xchyzyxx.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2opzxuudm.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2cywiqypy.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2bollruni.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2iucpdnsp.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2cukfgsqe.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2xpgeghos.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2vdkarbxu.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2sinbknog.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2pruioecf.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2arejazqq.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2sqdinjtg.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ypjgiymh.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2lkraogtt.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2tgbtdrgo.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2gqivvwzw.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2nfqczzwe.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2yoesgbdo.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2jqbvijeo.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jcilaxfe.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2qpsdtugf.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2fcddulkd.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2gzbmeyms.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2gpqcbkgp.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xcxefsnu.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2apzevoow.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2lqyztzbc.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2tevektfl.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2nkyxhapr.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2hjhgtjnc.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2hexxnjyw.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2migqhfol.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2mymrlmhf.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2sonfixul.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2mcngubte.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2jjxxsbkf.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2lgmlmoyi.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2ixxpwpdp.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2xasugmyz.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2sdygyhlz.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2rhyinivl.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2rexpsudi.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2virvdjqn.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2kmqfqprm.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2zsdfhhly.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2aoozsjaf.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2opcxblzk.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2ledjcjfi.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2zvwtbhwi.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2xodchauo.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2scqbbvfq.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2nfwyjdhm.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2bzvspsfe.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2nuglylrm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lkteqlpb.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2btddhahk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hlmgcrvl.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2tprfinbr.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2jsmkhtly.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2daafcjjw.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2nqkxjokk.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2yjkturit.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2mxzfgbix.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2adkwmmzu.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2tpqbhsdd.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2klvrttum.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2jkbifkhx.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2sruuedhp.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2orfwazhl.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2yuvxjznw.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2kuqsykbx.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2jfqpizbk.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zffpjukf.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2vfvkvgdq.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2zvokzilb.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2eguhgvuz.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2sikiyvbn.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2ndyixaxh.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2glpxaedd.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2cmfrugyi.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2dwnkvkcf.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2wmexmqum.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2tlejvmzd.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2enwrynqi.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2geglpkjv.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2kdltrplq.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2oszksbax.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2zmfalhsy.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2yoyfenzd.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2tsjkmdxy.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2mdcxgtyl.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2algbjfmc.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2xyzyczkr.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2hijzmzpt.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2sutfipif.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2oeyyjskc.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2nkoojioz.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2sbvaicyf.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2jkletzxh.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2odqfuror.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2srnxjrll.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2syyddewy.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2gxqvlbfe.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2ntqxijhw.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2retvtmma.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2sfphnysl.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2yfbtxmgb.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2cqxmbmzw.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2gejchabd.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2prxvbggo.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2shxmkypa.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2aykcerwl.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2qikulxjf.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2vgunltqy.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2ppwwyqpo.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2msszcvjh.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2mietxxgn.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2shwqausx.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2vehyyrfv.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2nxddncor.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2riivvyfn.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wbcpsnyy.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2vpdpeixo.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2cgfcybsu.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2kgsihzwa.html


<!-- 参考信息 -->