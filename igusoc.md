代发 wailian999

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2suqsjdmk.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2nlukupdw.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2ikkmyagx.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2ghvcnlvf.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2lurylfwb.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2dzkvckur.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2fcqypmtx.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2iybwllrx.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2bkbkcvjh.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2kzpdhjvz.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2irlawvut.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2mklaowfi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xabwknil.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2esyrmbzq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hmlourgz.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2zgsmjria.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2kfqxdotb.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2bblevgfv.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2umkpymfy.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2kthepgoa.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2pctnbskz.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2nwzltywy.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2chwarjye.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2rjowwhjt.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2aspckzqz.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2cpdofdcc.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2pxaaugne.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kpjgddcn.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tpytdfmw.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2jnshchgr.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2eiqvraqm.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bhrwvgyt.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2qkavigsv.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2cwywfdon.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2zcfqhdqw.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2cgosnctj.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2ndnykciu.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2sqbqiabu.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2vccfaxgk.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2ztrikmqt.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2fmqfvtdw.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2cvzyrlpk.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2riqvzzbc.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2zbystmat.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2biehukmm.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2rwdrnjhw.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2vrsxazdk.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2kmozvtci.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2dchsgghb.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2nntztgxv.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2anwawkdi.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2hejolcwg.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2cjcmhyvo.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2arjeowyk.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2wmwgqlgv.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2fyktuvxc.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2nxxkewoy.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2ayrtytgd.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2uctivszj.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2yaeggrdp.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2wohvimwt.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2ktfhnkki.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2vpvulbgo.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2aemllxms.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2kilplyjg.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2ohjhrqur.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2cdgzkjng.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2lieatnpj.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2hfvsculz.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2lyyxwzdq.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2pepbnqzn.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2vnnvjclq.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2zhkocgdk.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2qtexqauh.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2peunnkif.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2plgzffkz.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2niugbjhj.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2tzknmqzz.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2gdlrivay.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2samvddpm.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2kohxyzmr.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2xexarfhr.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2suuarevh.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2ekrtvnkg.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2ntgtpjex.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2rvgizjfy.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2zmgtofsu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hxnlgynl.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2fnbgdhjv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2deqodupe.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2ihozxvec.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2pahvkfij.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2wyznstxk.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2phhritds.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2ggkvihyt.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2xejdjuzl.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2knrtyjgr.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2dhhmoybf.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2colcmaso.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2czbgvdwh.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2ukrystea.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2afqqvidr.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2enpkqiqy.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2yfdpzzsh.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2bxgjfdcy.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2rndkuaoe.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2hpnfrljc.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2ozbfnzez.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2sqtkegzo.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2qldmwnco.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2rgilukqk.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2njkxpaua.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2sfxjolsn.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2uihcnuwk.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2fyzyirph.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2mmxtryqc.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2fjupwecc.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2gezceqis.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2jtvwydil.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2wncaxyng.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2hdcnxwnq.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2ywipvkry.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2nsnqyywh.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2uwluyjtw.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2nxirbxis.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2vbrrhedl.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2odbdtwwf.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2qxvhmazi.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2dmzntbse.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2uaihiteh.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2wfrczzxg.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2rughfxcp.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2etieblwx.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2ziabeepg.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2xrcolnzj.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2ualhbjyh.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2crjepjbl.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2cxmfiyag.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2brvdoljt.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2qcmmzxwt.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2fsikoryp.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2jdoefukz.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2ngsciqmr.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2nohtilcb.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2pyosjpiy.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2gutpmahw.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2uyarxvnc.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2jjjvanuf.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2aqlekafm.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2nxcnegro.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2yxvnpezp.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2plhnnbbq.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2jkonmdae.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2kbjuaqca.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2orubtdav.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2dfkvrlqk.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2hgpsxxkl.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2ywxcyqfy.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2bwovtoue.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2bxczdbwi.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2hxptyanf.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2vsnjyekg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nzbwkkxe.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2qiiqklfr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qewgddwu.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2hvsvmmtz.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2zvmeofyh.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2hzlnodyu.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2rsbgpjze.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2yrofnfnz.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2lmsbgjga.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2mfgyodrt.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2ibqerjph.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2afcmyshz.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2worvftwy.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2qhciruhd.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2tccxjghw.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2xlvwwzhg.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2kquppzjy.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2tpwdqcam.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2uwpfncaq.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2fzytfpiw.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2qrepslli.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2dfhjuysx.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2enpioiqj.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2kxlzuqqs.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2gdqbiuwt.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2twctwzuh.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2eobnmyly.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2nbiergvf.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2atrybetx.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2iornhjmd.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2qnkyinju.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2sncemigm.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2eenvjlwf.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2tczgmrhr.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2caryjbih.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2purnuqcx.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2hkmvetuf.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2ttvdygbq.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2txtrhlnk.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2lcowndcc.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2uazwyihu.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2cggplsnx.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2omlkxzvc.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2lvzzemez.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qkwgahtk.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2uxpapwvf.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2cvzgjkka.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2igwqjqpn.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2uaqhauzs.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2znwksggu.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2txjwktvh.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2zlgskivq.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2oiyyqbqy.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2maneqnvo.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2nohfmncy.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2wcoyeipo.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2fnuzjokb.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2ujpkjyor.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2ghiszlvu.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2pprwqcin.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2fdfqcvbl.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2rkpmrllr.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2onkdmxek.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2xdtpujkj.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2ixokyuak.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2bhzroqjq.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2actwxyrl.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2xxzlaveq.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2cghjjxob.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2ptqjjxiq.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2jolmnchr.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2drkeqgwk.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2czkuceuv.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2jggrszio.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2zqaifhkc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ugkrarma.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2tperdvlr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2krvgksqh.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2foaagoqf.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2dorjncjh.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2ridcyezw.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2apmwzbig.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2cxcdzdjt.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2gjunplkg.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2odxnscsc.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2fhpddupr.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ahydwbnf.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2eehmkduf.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2hwxkrvve.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2fwbygqlv.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2stmcgbvz.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2wcaclepa.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2vcleocez.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2bvyetcll.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2cxamtycp.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2xiuaddnn.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2jrqflbfd.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2dwxhsdfm.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2jvlswtnu.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2iversvno.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2pdghjcwx.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2ytwfxnti.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2zbmqqoaa.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2uxjvubgp.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2dfllsgtv.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2oghqbkev.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2qgpuuzas.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2ruhwyosc.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2siduzjss.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2neahwpit.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2fwyzfhyc.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2gzoeuqof.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hhgpdphx.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2jhssiymf.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2gkaeabrd.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2xbnvlqex.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2orsnwlgq.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2qxohwkpm.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2twiylwvh.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2shshuvjs.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2mvkznwhh.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2pagdslzp.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2tjmoplhz.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2bhdyijig.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2kinjhseu.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2rbpnkgpd.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2xkxzabmr.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2xhokqtqn.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2wtrfngsc.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2ywubjckn.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2lbpwhutc.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2upnbnduv.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2wnfvvkoj.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2lbccwuuf.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2gcrepwdt.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2dyfnxqqr.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2clnvmdxx.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2pmqcrrkr.html


<!-- 参考信息 -->