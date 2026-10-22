代发 wailian999

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2aslfflfd.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2klkrzikx.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2cercnwbp.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2zdlxahpt.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt2pmjrheyy.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2mcvsxatw.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2lnswatik.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2gtwyxaxq.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2raijssxp.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2lfytscdt.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2hhtzsnjb.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2wxenxeki.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xlvitxcr.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2ylwegcio.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2arjpglfv.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2jyirlecf.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2gmibwkub.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2lkcbivdf.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2acxunicx.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2jahrstei.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2wrnftdes.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2ysjmsgur.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2jipyfarx.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2naockrky.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2uamiivjz.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2uxxccqaz.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2ayyfskjw.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zbkaiwjj.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mypfbcct.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2vdwzqdgq.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2uzunsqwt.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2tfwrczqu.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jmfpebjb.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2qlrjcqgc.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2tdfzrpcs.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2sxlkvizj.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2zujizcsr.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2pltrlmng.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2mhthdjxw.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2qpomjwyq.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2wpbnhoms.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2klxwbdfy.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2dzrvuvbf.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2zwjgoqzz.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2oouyfzrq.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2bnjfvkki.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2jdwpzrkp.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2ejcyastf.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2twpdqggx.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2vzzhseav.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2qiofqksi.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2btnkirqc.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2qlrjfdxn.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2vszvtwcu.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2crhdklgh.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2rzwuwhzr.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2uuhlmflx.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2uswnughc.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2iupzaqsp.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2yxemlhtm.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2trkgbatl.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2codkizpz.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2nwxfcfsd.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2rnzzyosk.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2tjrmcayd.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2dgadxgya.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2frrgrskg.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2mxhpckpg.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2yrihttkq.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2fuobqvhk.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2yfnwyzyq.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2vkgvviaf.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2xczrwtmp.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2lrczikry.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2qeuaoonp.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2ywdrlubd.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2nobfuphk.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2kqmliile.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2byvlwazu.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2fxnfsbas.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2ftugfnue.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2vxkqwwcr.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2aarfmvat.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2wdfxbwna.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2cmzqwnfm.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2spuqaidf.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2emndmfhf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2suuboadl.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2bjuwzgyn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xbnhtvmi.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2vsfronwd.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2ycbpzejk.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2grzcnfwk.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2muxmnioi.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2csnyzzvs.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2qsbgbxcv.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2frtsxcdu.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2dfauimbw.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2oondrptd.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2zrcatydt.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2mhbeppbn.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2jmduiaps.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2ssyumztr.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2dbzkxspr.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2tpghxzeb.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2stasjwpp.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2sjwdetqw.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2gvbfckry.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2hdcaapoi.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2ttzswcwr.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2tuwzejdo.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2mtncycct.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2ikcrxzyq.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2gilplcpn.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2bbudoidd.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2wkqzmddw.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2tfemjpsw.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2bnlynrao.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2nbhdirsc.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2tmzyplhp.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2gmhcxfdh.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2voamjbwc.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2lgmfsxoi.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2rlbtkwjs.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2tqkvhtzl.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2qonlkqub.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2hwwybfor.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2ujyadgss.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2iqrxleca.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2wnppassr.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2sfayuieh.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2gsarwyee.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2uzufaaga.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2emzdjgff.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2qeynakas.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2fobclvdh.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2hljtvann.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2igikmync.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2tyqcbago.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2cqzeubyb.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2wftewijt.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2gdtlptin.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2hyurfsbn.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2nydmlxsg.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2waqizrrm.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2gtmzicdt.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2ubkkacbz.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2molvlpnk.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2spuuvyli.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2sttqxzvd.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2irskvmxj.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2cmqsuuuc.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2xvokbsss.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2hdhwaqok.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2jbnnzamr.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2teulaqcx.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2stwhtwqs.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2atimbwrw.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2wddegcvc.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2xwvgldvv.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2udaaiqin.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2zbqrfebd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2knoyuwzy.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2hqolfeic.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dmxatkot.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2gwinkszl.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2uuspjpjt.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2riyncyui.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2lnlkwkes.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2aiyzrnzl.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2gczygzdl.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2yplaahth.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2qfbicprf.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2yytinrqv.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2pecuvtqu.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2ixdjhqtb.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2chlvkzci.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2zdnzsnoc.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2zjubrdan.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2vaiabkkv.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2jwqwwyhc.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2rziseexc.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2ssojpiti.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2tcfufzph.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2ajneiepn.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2ongqvwra.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2bjlxtayc.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2wlmieemk.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2ufinckmw.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2pgdkbcrh.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2jhfnlzpa.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2lmttmafz.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2okdusbkw.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2mhflynco.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2hsbrozyz.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2kcmmmgih.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2jbhfwaik.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2zabeoedg.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2ygytdftt.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2jjkralhi.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2tfuawekt.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2uqheyxbz.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2veozlueh.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2fzkkrske.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2acyqgbya.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qvnwcffs.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2pvigdqbr.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2tvgzgnie.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2vcplspdz.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2tiayyxrq.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2cwpmzwhh.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2njibyubw.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2ghxyiyrr.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2xkytnbfm.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2imewlnrz.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2bylppnbp.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2rdlazwxl.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2rdqmaubc.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2jncgwewq.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2kegypyjw.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2zeybuvnt.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2hbdpgkyt.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2mnwyzmat.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2kcfklbai.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2omyyordc.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2hvpxbmie.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2cwuohhmf.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2bwvekelb.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2bditfytd.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2xjdtmtvi.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2esskfgvi.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2unyjetnw.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2xqnprwvb.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2uxjuwbig.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2varnubxa.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2tkulchjq.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2xbsqliql.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2irwmfsbp.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2xrspcuve.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vozrkohb.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2knmrursn.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ubkopiwk.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2ypjkoydw.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2rfpwpgzq.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2yxngatvb.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2jhgethta.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2cieaarnx.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2soxkxgml.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2yarscaej.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2njnhkwgb.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2xalhsfgq.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2tmvuickn.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2owrtfsko.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2bsitbxsa.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2duqjfrxb.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xqhlpaun.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2mtdotxyr.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2utqvixzf.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2lhswycgz.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2edzbdgue.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2kdcagokx.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2wzciswey.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2pndkzyif.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2tuaokdiu.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2llhjyqjj.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2mewgukbu.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2muqnwyyi.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2bizqniux.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2qjnivqke.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2acvvntbo.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2wpyhnlak.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2mltbizay.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2zwrxevpt.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2tlmydchm.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2fyvmeayi.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2ibjywmaa.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2ukwyrmzy.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2fszafhgl.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2vzyesylb.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2xwsriqwu.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2efflodmo.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2gvaicotv.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2rlswabfr.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2cgxeelmd.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2uroizzxn.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2mnzqlanw.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2aqvvbjqh.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2scfqwjga.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2hrtewxvo.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ozpnihvb.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2ogyvofwf.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2pucehnne.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2ktjuebrg.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2sftrehqz.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2wwtcpktf.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2jbdbytbc.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2iswllqqu.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2tdehnnov.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2tbdzskmt.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2lcfypxqq.html


<!-- 参考信息 -->