代发 wailian999

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2liivmidw.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2ekjedhvn.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2eosdvuuf.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2htwoncpl.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2fjhqkjzl.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2peonflan.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2rysrauug.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2hbfttwrd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yxzqjjps.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2ymfeofuk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ibhdmnev.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xztklyoq.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2pisvaesn.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2fynubqul.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2cxxejeax.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2qhxzqurl.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2eddfznlj.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2kghwmzot.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2fjuiciap.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2hcdzzenk.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2gvnqyxgf.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2ekmulock.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2hmuraegf.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2uaiopiwd.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2emegmmty.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2zmdsyuwa.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2pihclict.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2maisbdnd.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2qrzybess.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2mksixyvj.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2mpxwmdrm.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2ythnoqxj.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2cyrdsfbb.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qqcjruzx.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2smfommaj.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2ngjdusge.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2mreghjgi.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2plzbtcza.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2pksjhyul.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2jvqaedjf.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2znohluxm.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2clfbdlar.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2gwiofzhk.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2uihubaok.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2smdqnpqv.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2tngzbatp.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2bgrbsgpy.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2eageoqnx.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2jkbyxyih.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2wclgtrrh.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2iioyjukf.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2eybgiusa.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2lqadokkz.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2giniukxr.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2zhdipngp.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2hustjwwc.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2lfjyncju.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2hzkvodba.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2dcylclrz.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2duejpzyj.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2iszruhvg.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2byevvemq.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2bdknmclv.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2pcrqisop.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2ofdoiami.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2wlgttgav.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2buzuddjn.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2cjagjvok.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2jwimkqem.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2fharcdia.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2lcdmerlt.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2vffwugmg.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2umwfjevm.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2jrsddmlp.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2nycaqvsg.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2hoezxhmp.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2kzumaqfz.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2txnszixd.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2eujsluwf.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2hmmqwbaw.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2nzdveasx.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2cwtqcwas.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2mgdqhgso.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zipjjxnq.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2fjawohov.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jqdbxsqz.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2jseaxyzz.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2grvcwqov.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2noyhgrks.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2fthzpvkl.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2twlffsuv.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2dsfszfls.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2zigowegb.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2kqcavgml.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2ipvevwiy.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2cjnruiod.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2rhdtemis.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2buoblwkb.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2teffizrd.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2bsvmbayg.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2wlktefdq.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2xelrupts.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2dfgltrfe.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2qhaejyqm.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2uacmnzsr.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2fsoxwjjp.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2syufodaj.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2thelqbyj.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2pjipigfb.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2uutxrgbm.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2gehccfxc.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2avbzbftb.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2rszskqrs.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2trpgnxwk.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2ivljpxkp.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2dziekqhy.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2hbzftpty.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2xheqjibx.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2madaqzyv.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2kvybvdov.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2lrjvrvjq.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2qmrdilxp.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2ccimhvfv.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2ydluhsnl.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2enysanyu.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2gjicavrn.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2kzspnmcs.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2itesgzgc.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2elxlglan.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2oaylolmg.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2jreujbzp.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2wmdaulyq.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2ndcnylkr.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2yxvtxvyq.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2urzrkflt.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2ktnaoifm.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2ygnpxmln.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2fsbmmasm.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2egghnonb.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2zppxooup.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2jjbkqlkr.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2guizotig.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2wgtjcimp.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2jolbdkop.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2wcrzosps.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2minbrjae.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2twiggfdj.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2owpzzlzb.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2gboolwdz.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2tztuonbx.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2iyhayonp.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2weqlbyvv.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2tlibggww.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2jvarejmn.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2poaozasf.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2ujpozxef.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2qetfrzsu.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2opmzhius.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bneegjza.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2mphvjpux.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xugvrseh.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2letrngep.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2oqapjtgy.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2tdrabrdp.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2glzvjrdn.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2ziucuzit.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2xoyvluyf.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2uufwaoba.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2rszuhqud.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2fvimufsf.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2tnjvxhyk.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2cgdpbrzl.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2aqxqltoh.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2fkabmpzm.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2lkjcrwwm.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2sbccepvr.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2xvtqlnnr.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2trhwakeg.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2tmpkxprk.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2vrkwayew.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2yrfiyrwt.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2qrfdzvev.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2fkwmvhww.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2wqtszorl.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2rifjmswn.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2driawzdr.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2dqobbyeb.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2dohcsetc.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2ookcmbel.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2gmjetgko.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2lofojdjd.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2snnfuqng.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2jypnrkzy.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2svlavypf.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2texlbuic.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2rdjhbuau.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2idyshwax.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2jkxgcydm.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2gxawjspq.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2lfwjvess.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2axlffiog.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ofxfufiu.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ayaegnps.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hvexcsns.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2lmsjwutm.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2qqjacjuw.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2guvigsri.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2gheetulj.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2ykzpjebl.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2rultukgb.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2uhnnhgwh.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2clkhlvda.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2xriwggnz.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2llzzerxv.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2jtruraui.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2xgddoert.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2sygvclof.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2shwqhgvp.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2czpnvjyj.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2chsyvzca.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2jzduizlh.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2jmepwsoo.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2xyzxkkww.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2qtzftpfj.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2erdysaod.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2vehazfic.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2zsyntyhf.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2ffsynyce.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2vuidtlys.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2hzgybqyv.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2xqvqrcxb.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2rjvjhbhs.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2tuxegtax.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zfwuitqd.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2lqncpmpc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qzmybxhj.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2uqtmnxrg.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2exprrhsr.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2mujozqud.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2jyhisrgc.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2hkesuyqm.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2audqkszr.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2gpphdscr.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2gorpkmkv.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2hptzastg.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2zhpoxcdu.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2rqdnvkbq.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2iulgpcvf.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2dcvixplb.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2hjuabjwj.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2hpjxvdvl.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2nuabzxva.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2pjxtqgac.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2vshpivex.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2afxgivez.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2dugtbemm.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2whzoedhj.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2vflahkek.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2bpgrlfxq.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2pekphiva.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2hykuvcdu.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2smpgmtio.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2qhkylwtm.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2cmfovrps.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2zoyodhzk.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2vmoxcnuj.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2bisgvqfq.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2lwqobfpa.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2fgfwlptj.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2fpdyvxny.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2fgkkypyw.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2sjymjzsi.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2ubbptalf.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2dxhrxfgq.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2ytuvoavu.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2drvfrkqf.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2tqajbmye.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2menenrnt.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2mihdatjs.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2vugusrcr.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2ivoizble.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2auuzpypx.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2zewmtcxv.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2trnmuoci.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2vwbhpkjr.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2xtjorsxp.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2qajhzcaa.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2xsljrepi.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2ivgvnmgv.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2otdzfycf.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2jtmxdhvy.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2zrcivmhx.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2anakqbcg.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2bpztbpgw.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2pkxzolmm.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2zunyztct.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2ukwejezx.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2amytqgaa.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2jdljhets.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2vplbmpqy.html


<!-- 参考信息 -->