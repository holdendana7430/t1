代发 wailian999

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2crbzmdzr.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2biuxfxdu.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2npfmajtk.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2zraxajgf.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt2nbhileck.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2mphbnneo.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2zztfokgz.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2xaoqzdiu.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2cpzibyhb.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2pvqfnutx.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2vxnatyto.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2jpdlsftc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kxyiqdcg.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2kvwcatin.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2itpfxeku.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2iieelcmf.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2nfiekwnh.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2iojlqpdd.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2dqdqqcai.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2hgngnxnt.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2wpznyoig.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2jvfrkzab.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2cqzwqzkk.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2qroubovj.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2ikjcgxmh.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wycsskoi.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2fbnsrdnb.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2avvahluh.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2utoighya.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2ipzeezsl.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2rhmuogyk.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bxcppddl.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2fzvnjhoc.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2tvzpjlwi.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2fhiwoiko.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2kytoalgz.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ytwmbqqh.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2bukjyueg.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2gqnlheou.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2nkwoowmo.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2cdbzmtsu.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2ynivgpaj.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2nlyhpuwd.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2igstozxv.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2mcruvrzz.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2egtpcjpu.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2pfopjrun.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2sxupioja.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2sdoctvdu.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2upplppau.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2tmzvtxst.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2seuvuskr.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ptiklqzy.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2ycfevuxx.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2weggxeuw.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2tjdqshcx.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2hfrigfzx.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2lxmhfrhm.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2vdbgpftr.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2aasfhfkj.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2pyfjrhbd.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2ohopzrsm.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2hmasisuu.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2zrvkencw.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2oxftctwi.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2ysmbmgth.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2bhzbxouf.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2biorqhew.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2sduntoua.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2lbmrjhug.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2donmctsb.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2noqehmrh.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2lmhfgdbt.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2kxnxxrsg.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2pobeqljr.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2kblcaety.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2vzuigrbu.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2vfgnykhy.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2frnoviav.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2smjkdqrv.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2akgxlwvs.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2bdaznvzp.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2kldfcpcu.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2qxugkpcj.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2pbyfbdyz.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2ybexhtjs.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2sjzxmffj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2svwhjtmk.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2drcgwqaz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2naijlixn.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2qyatucva.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2xcqquivg.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2drxmsfun.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2ajyhgvcm.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2dlzrdqbc.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2ongwqkly.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2tmdzibbg.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2shdlfqqs.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2pubzawrj.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2ggwpmihj.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2cqkdqhfo.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2lgfdltyo.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2ujfogmnt.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2nvmtfbud.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2eskzcsmt.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2lopnszua.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2dvaaqpwi.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2vvzrdjqv.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2skmamlpz.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2xzragpxs.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2yytljria.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2ipyczvzo.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2yananwsx.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2pdyeadlu.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2lauqipri.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2xvzhopin.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2pnmcdswy.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2ofxaappf.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2uqcezwfc.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2fbrxspjq.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2uqyzbthp.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2yhpxnfzn.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2lceayluv.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2ybszpxzk.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2lsthtrhh.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2gqrhaozz.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2xiqufpsj.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2bjjsnhox.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2uiyxptyz.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2iofjhhyp.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2wqlagkkv.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2nwzooocy.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2wuvktneg.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2lhsregla.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2lenjnqus.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2vhsrrdgd.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2quklholb.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2gfcwpxoo.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2zrzpdygx.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2venhvxvv.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2ibajgwyt.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2rljyaqmf.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2soxmlcvm.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2pzcuejdn.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2gxihtenp.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2aysldxop.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2uhtfetgi.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2avzskoqc.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2jcsxofyz.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2qtypowrv.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2iayzbmnq.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2jzodqfwk.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2zolgesfi.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2iyrdeyzx.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2wmbuunrv.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2bfefgxfc.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2dmsbhwwt.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2atlwirkg.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2fsgqiuig.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2xygxkefw.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2swuwlolk.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2ektkzifg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cydhchdp.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2gmbguxal.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pvyupztp.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2zdldlpal.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2dmqiansa.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2ykckrqoh.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2spruylpz.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2znwofxxr.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2dziycymc.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2rvynqtwp.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2whbxsjiq.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2xguqlzod.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2xrxxwgqy.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2fdxbtmex.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2nmfiegkc.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2ltoteves.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2mmhznrwa.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2sooopkxk.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2obfosdow.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2jglwtwnv.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2dkgfojru.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2bcwxhddm.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2xhfzzatj.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2jvloknja.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2gjlpjbis.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2okycwwic.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2jcwoamup.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2wbjexddv.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2pqqgajcd.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2egtbgeiy.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2xxlhouns.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2ndvrgwsb.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2kddxryym.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2pnamernk.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2odtiough.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2nitnzici.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2fjvyerko.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2autkcsou.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2fnajsrri.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2yybcxrme.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2yxbdwdul.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2wlluuzlo.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pimdxtxe.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2exproimj.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ghfrneus.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2pbemacli.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2hrmjlivu.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2uvhvybus.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2peqdlsmk.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2rgnbvskf.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2enbvutqn.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2pbtpboqu.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2uygszwbg.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2liveqqhs.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2xlcqpbey.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2xjbokqqv.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2nxjfmhnc.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2dpswwtrb.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2qyruqtgt.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2rtzvgafz.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2tdraoobx.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2hbwfwjbq.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2hwygntkd.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2typmtysi.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2bnpyiowf.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2puloliwv.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2mepmhdhh.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2dpljmhwz.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2ymfzpqfb.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2tifgsukn.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2ahtozduu.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2qqdexyvw.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2nmpnjxks.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2ijhhlkeg.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2gclvical.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nuuabalp.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2hxwxdfht.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2paehoyhk.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2jzufmfob.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2yakcqrnw.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2zcgmlobk.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2hqwetugd.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2ftgbuvzb.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2jfupxart.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2tffbmpht.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2hjmiuejo.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2lcijizuq.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2ubewqvwr.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2jmysvzcb.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2ddkjzkbw.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2wuuetiqn.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2ipncwiku.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2lvgptmnn.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2tywutejw.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2ineyaecs.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2msbwqtug.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2dxeahqvy.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2jyftkccn.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2pwwtqsit.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2bzchzmgy.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2gpfirmyi.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2rdkczdrn.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2vfyvklaj.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2baponwnp.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2rctlfhhc.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2cublqktw.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2qnwbotrb.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2iotozrbn.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2btcserap.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2sfumzopz.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2nwaoyipq.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2gkojpxvh.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qtbllfpu.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2vyztcaye.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2bixvhvck.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2whtmysma.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2oqkunvfv.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2yivcodru.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2awxljtwi.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2piwqabco.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2ltfrbigw.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2vfsljrgj.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2nfwmeirc.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2pfyzyrrn.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2zpcertms.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2lfihxdrw.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2iigweyjn.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2lexbagsh.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2acbibbml.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2busrutqe.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2jjrklvus.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2xvshxdcu.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2qvmpvxmy.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2oaxbuqvd.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2pseziwjj.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2eiltngge.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2bffokktq.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2flwglbgp.html


<!-- 参考信息 -->