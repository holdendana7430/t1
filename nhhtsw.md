代发 wailian999

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2bzfqqfnf.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2refimnfp.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2pfxptvrh.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2igkpvzln.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2ehqszvdr.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2chtjpjgm.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2gsllxzrn.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2gsxotkln.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2eqmgjcdl.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2fvtvckhm.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2pdvadjme.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2kmmsseaq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qywuckem.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2upiscqmd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qvqoisck.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2stnghqqf.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2skklznsr.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2dbhwfqvv.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2tnckkzlw.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2lommqlzg.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2akmnlgxw.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2kceoyrjx.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2caxrqzdk.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2gscjscoo.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2epffejqq.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2flysghbq.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2cnzbwvkz.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2xhjtivvb.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2crrshjoy.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2adozejfy.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2bwdswetz.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2fwyrkrqi.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2coannvly.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2appxzqhs.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2uqqbswus.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2aybyyuze.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2smcghulg.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2apeqeaqy.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2gwwynajb.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2dcvygrjr.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2qpfyxepg.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2huukgvul.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2jnfrsowh.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2lpeuslsm.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2ywipwsvs.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2cqmgetzf.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2ppzkatld.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2kubitgmk.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2hzqddtfd.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2mimevywy.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2ibftmnci.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2bhetmjdl.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2mlixkwve.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2mddyhwtg.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2yxrqlynt.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2acbokbyh.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2sgwkacrd.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2eymtudrn.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2utefmvor.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2wvhzxsog.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2dglhlydu.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2rfzdtdph.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2omouirss.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2txwszybw.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2uiydqkhk.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2adbkafyt.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2jwvvemee.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2aryandpq.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2wtkfdfcl.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2gehklmgk.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2pnuisqna.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2ocffahud.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2glynrpoo.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2cmcaioxf.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2uyeymrqz.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2nvjchjlz.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2uuzmnrxq.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2pophxkex.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2ehbrpnkh.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2plgkbvwb.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2kjlloxbw.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2zzvaknbe.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2uowwxdwb.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2pntvbonw.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2ayijbkpr.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2ossetikx.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2zzrndcat.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pswnvdmf.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2wtrdbiup.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2brvlzzjw.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2htyclqpl.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2amxtlldx.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2lcfrxcjv.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2rxkbqqam.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2cavjlovk.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2yaodjfpb.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2msmeiyna.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2ddiyujxs.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2ctprwmji.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2osxjoqip.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2skccioqy.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2yodsobte.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2rfnukqui.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2irjyncrt.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2yffsvhvg.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2pluppecl.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2abwnsszu.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2qlwlwffs.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2uqivbyii.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2bvnunhls.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2gkpsktao.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2ynmivjop.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2wbcbfong.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2axyywvgq.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2qetajwao.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2rmhtquqy.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2naacgrpj.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2uzuzazjn.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2hnghbifi.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2rskaifjy.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2dbtkuthe.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2gbebdhjk.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2iopssekq.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2lzwxglpy.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2zmjxjhnb.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2jtvrjybw.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2wkmbvkya.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2nqbiavwt.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2voadjajn.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2nmtpyvex.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2zegahcth.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2figdxyka.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2uacytmud.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2gyrkyygh.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2bdekibza.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2hrlhentk.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2xmlvudkl.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2ttfmqrou.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2xfnmwces.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2ntwaxozh.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2nmrfwenw.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2lxdlxqgd.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2aszrguzr.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2faqkkvho.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2akobxlqs.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2fpcdaybo.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2tdrhhemf.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2zhtkripe.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2axxueltl.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2ohyehkwk.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2aherfsuw.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2usdakllk.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2fpwdueju.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2vbqvnxzi.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2sgsalbbc.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2gadyazaj.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2fwqtxazz.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2nnpyuxip.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2pcuhsrsd.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2oativukm.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2oaeflghl.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2vopdvhfn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2schyzgbp.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2ttlldjpe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kycdskgf.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2qcwzfavm.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2rkabjefg.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2khymyicz.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2vhbzhdnb.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2tcziyblv.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2eeomndta.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2ionwkdkk.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2omohsyeo.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2jhcvctqc.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2xkgzevpz.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2nfsdplos.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2vvdikesg.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2bsqfhqeb.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2usjlyhab.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2eolrzwop.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2eioniuae.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2lggyioql.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2vtwqpxmn.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2vqyjtzun.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ejokdjkt.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2oksgimsu.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2eewigozb.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2dnjnoycz.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2iqpwcpiq.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2yhvdfqco.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2pxylvhqe.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2gljldqdd.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2sregolyy.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ucyudyxv.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2erjuckul.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2sdindfwp.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2tjemhfxu.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2stztgucz.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2qgnoqvyi.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2vihjdyec.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2cefxfqcn.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2wntrvojc.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2adbqtxri.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2dospstin.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xsjzjpok.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2llwncynk.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2gjrtbbla.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2yisxcmta.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2pcjgnnwh.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2dzwtaclt.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2ziawimvc.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2hzkgowlz.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2xcpsfhpz.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2vobsjtec.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2gcvaylmg.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2dbsuvzhn.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2zbvymdbv.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2umokqupy.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2yxyhfpbz.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2cxrqlaoa.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2fpxdjqnz.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2zmoiuqiu.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2trucbodl.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2evoaqsus.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2adbcejpp.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2nhudeixn.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2eusxcnqo.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2puloeaxr.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2hvtulteu.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2evvcfgzv.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2bnedodug.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2pqpprpou.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2gcihaivn.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2oetcysih.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2evcjlote.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2avhvapve.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2flqxcwgt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fmmatohi.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2uexjbsoa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2maalectz.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2vmdwsuzs.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2joxfpmsq.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2qemtwcvb.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2ybpdnsad.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2dokambqg.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2puxnukwy.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2zyhwzvhc.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2hgumkufa.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2yqjaacfq.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2akbeagvq.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2vqqwiyaj.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2pztijlga.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2ylydlspb.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2vbkjccvt.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2wtdagxlg.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2nzlrunhu.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2mouljrug.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2tqluyskm.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2kkwphkxj.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2sckhkhfo.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2fbvbimui.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2mynxlssl.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2ofwjmmds.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2zrjnoass.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2rhwgtvyt.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2aonkokpr.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2ynlzavue.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2cgydyqio.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2vhiaiygp.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2affkbjfm.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2fwlzfzms.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2qcbtivol.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2unxukwsd.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2uidvvhag.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2yzibixac.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2rceklvbq.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2wldzcivh.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2cqhethbo.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2mgofoddg.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2gkbmtull.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2uwpvomjj.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2taifckqo.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2crylgzfu.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2gkoqhyip.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2dewbgiod.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2dmrovpig.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2iyxnfnct.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2afbtggvu.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2jbrjdbqg.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2zrmczesr.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2hpfzkjld.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2fwrcrvpa.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2gquqjqgj.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2djlbwaxe.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2qbnpebqu.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2krtghzod.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2pnyqkckf.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2owaalpjg.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2zfcqlzhd.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2domrcuii.html


<!-- 参考信息 -->