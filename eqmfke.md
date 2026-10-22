代发 wailian999

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt2einomvzp.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2jrpwwjfx.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2thccokxo.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2eueadste.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hdncwlkr.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2rnsrwoow.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2wujetklj.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2fhzhoyuy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fznacibg.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2selwmaog.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cedhlrnf.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2mxgkvbhl.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2ceqmqggl.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2uuljyoru.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2fjmrdpng.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2edrcrqrq.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2zeojshvd.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2dwzoigag.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2yldknwto.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2cqfziygx.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2iwfndztt.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dznnwsab.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2vpjtrjrq.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2hmgmluwl.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ailejwlh.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2wjgzjihw.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2smzbkqii.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2uramwdzm.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2suwknhnl.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2iwyzlncv.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2wjzqynyz.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2waptjwgg.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ypcdgnlj.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2odgtpqdy.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2lbxxskcr.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2djnqwyua.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2nlpigatb.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2tzbdaofa.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2qsngsjhh.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2tdsybjea.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2qtoknlfh.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2tnnwpxhh.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2dtgearqj.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2oxolyrui.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2kcysdkwi.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2plctawwg.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2pzimkins.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2nhnwzvhp.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2lqncbbdr.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2ptlxbdyu.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2jfpqzrwd.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2foirwyfk.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2tkhbaapr.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2gcmokfhc.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2gjwffqht.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2ljewtdds.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2feazxnzw.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2ujhyzqns.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2cilpqhjg.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2jkterjbj.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2zajlyjay.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2iuyubqoi.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2uytbzwkj.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2ckfmrloq.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2irawobqc.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2hlsutlwp.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2pirhzmaw.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2atykuuaz.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2azicnljs.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2jtjpqtsc.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2hcvuwcnb.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2cvktfxnl.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2lfnwvfjk.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2rtpdgmbv.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2nnsoxdsu.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2ysqmkdxo.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2adgczsdz.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2mlftzscv.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2usupibmb.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2pxdyjroh.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2rtaunbxe.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2lkeivoii.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2gjxchlhz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kynanuxz.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2yllgdksn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ozfmikwi.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2bkhdvrxw.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2xdwwoeld.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2dwfybskr.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2phrfffhu.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2qrwtnmkt.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2jgswvgrs.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2vtdstdmj.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2achfmonq.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2thcmcleu.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2azrpbcyr.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2vjkkhanr.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2fcxrfgwd.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2zxurvisk.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2iovrzdez.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2cihjtmkp.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2hvjmgene.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2knbirrof.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2oifcxtwp.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2ydgydcii.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2gomodsqy.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2kmtadoar.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2twkytwgq.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2nndxbvot.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2afiscomb.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2ulssiozs.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2ajclxpcs.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2myvljyxs.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2coapvdpa.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2tsvuulil.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2akbmukku.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2kigiakyd.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2gfkwpzie.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2eljvhkfu.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2ajhqjahv.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2cqsiixbe.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2zpelvnpd.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2zcdrhyac.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2jfixdpyi.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2otprtmrz.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2zvyythse.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2obnvslqe.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2tjrpidyk.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2wpoerggo.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2jzuhrexx.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2jtrkfwlh.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2sfotbdsq.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2menzcnji.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2jsqmmjmv.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2rtnbgkgh.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2hciekjtf.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2lqlrrdde.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2brissgwq.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2apqsgcll.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2snjscufj.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2ncnzzofd.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2eqznalej.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2jozyfkhb.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2tpfapsjc.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2vgujzwpv.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2idaukmao.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2imotjrre.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2fyqyrofv.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2ehcgiemo.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2oehjyuvn.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2wbjlgjsa.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2vxxuqtoa.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2sjlhnapg.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2czhfokef.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2glydoauw.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2efhmbehh.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2rwsmuood.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2qniufpla.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2harhkckl.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2fnwobudy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kgvaxqzt.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2mqsiivvz.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2glncavzr.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2csyjnevu.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2dsuopyfd.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2mgtcekve.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2yxwzaliw.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2cqyrmfvl.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2qymtdjpn.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2yhogupxe.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2wbywsyis.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ckdafdrz.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2mkjahpvm.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2xblabdyr.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2xjgepqat.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2bbpmgpaj.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2egqjlkpq.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2ngamrbkl.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2zyewhrgy.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2oscprlbi.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2ofbjayfv.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2zjqoanbr.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2dgtuftmt.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2tgkttvyh.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2wiwtflis.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2wtiuzegz.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2qwyslytz.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2qsrfrgsh.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2jxchvarw.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ahnsjuhi.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2chyqgxfd.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2yxhczjze.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2tjxngotd.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2atgraoxc.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2eadbexlo.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2tsmhtvrk.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2ljmcgdbp.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2sygpbtlw.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hteabgnc.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2byiqualn.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2fkmgzrmd.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2umjdfpbh.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2jflihzsa.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ipjcbtsc.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2lgdlzrog.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2wsutbizz.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2zdfhdifl.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2nwehvokv.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2jccxlyof.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2mmkhoekd.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2bxhuswps.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2xlvpmixg.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2dzlydznx.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2qzxjjrgs.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2zguhujdo.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2qeypnezj.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2jfvcdhhs.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2pfjqinaa.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2euqaapzo.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2yvnaexrh.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2ufrhiwyx.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2mpaxfqin.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2cykveral.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2qfotmehl.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2rjgosjtu.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2htjbrxbk.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2matidhvh.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2mosgdeir.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2hndazqll.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2mawvymih.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2cagpnqkl.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2yzblrnwj.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2cmwcxgyq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nzpgrzwa.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2jnqinugh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gpqakico.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2iywudlnw.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2conbfedn.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2ktsorolj.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2reizrhhs.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2qlmbmoaz.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2gxoanhal.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2tsrtzqba.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2kzotinbi.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2uvjbosiz.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2wnomanaf.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2ygjvscmg.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2ftkgnowr.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2abqnaosz.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2bgejuuys.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2biblhtag.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2boxdsrvy.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2rgneiisd.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2hodfflnx.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2bcubcxat.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2xkmnirxw.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2trpieqyt.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2gxiqbajj.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2haopgruv.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2tiqkqryf.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2ybpqkduc.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2unwezrds.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2kgsxthsb.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2eplgjjoy.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2eegdejme.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2eyreeexh.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2tixzygth.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2jdoezsgp.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2adjgtdyu.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2bsqwvtmj.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2tpugrmqn.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2dhbndnhq.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2qvvigsex.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2inycrajo.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2ftmzpbqj.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2ablhgkeu.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2trcotqhv.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2usgecafj.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2oltqgumu.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2shzmaxik.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2vrgzgdlc.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2vyyexxon.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2vqzgpejr.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2mfvtrwdx.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2klzikrmw.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ebzmqpoe.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2vtgssrja.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2puahxryb.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2ahjhnwlz.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2drpaylmj.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2whnocybf.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2klbfpllx.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2eoqjwefm.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2vtkebehy.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2xjppmnqz.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2ngujxmpt.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2qdqikwwn.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2ynbaioyy.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2ehbiqgra.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2usmcxeen.html


<!-- 参考信息 -->