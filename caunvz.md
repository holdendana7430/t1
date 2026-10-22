代发 wailian999

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2ywndvqlq.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2wtbktrtd.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2axmnzkje.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2nlnrsrtn.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt2gliaxath.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2huyjvanf.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2lwyydpva.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2brirxkmi.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2aeldrnsr.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2mxleotyo.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2sspvczix.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2gamjojqn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zvqtpqcm.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2axyhuzli.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uoshtcyf.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wchgtkye.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2bzmsptjw.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2fnmisglg.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2iziuauep.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2undehyls.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2nhqzylto.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2eztthwpa.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2wrvdmwhr.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2jpmwxdkz.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2jvusdevj.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2rirablwo.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2ovatqccy.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2qrjmbjcg.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2kgyqmbih.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2gnhedgcm.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2kmhaiycp.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2fnxcvgpt.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vrguzusp.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2fpuleybz.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2japblebu.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2tuvuexna.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2pbswiznq.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ahrtkruo.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2nmrydeie.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2lcxbptre.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2pedrvvjp.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2kpkcqqxg.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2vipvtmki.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2jzlvzgfc.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2myalcbbc.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2cdgavdgd.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2bzmeaclu.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2nsputgtw.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2tufffuxh.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2kpegpiqe.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2wbmxsgik.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2suwtvhpy.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2kqvworsv.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2ekswlusm.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2ujeqtblr.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2gfhyvzkn.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2vmtnbmqu.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2ildepfjd.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2xrggzrxw.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2ykimwnsy.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2owefoisv.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2ljoxsqhu.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2jsaqpogu.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2anwnwdwt.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2kdxjtxxa.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2bkdovswl.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2btjmzpcx.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2zjkbooqe.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2aggobwus.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2jitadikd.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ynzcmxdl.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2lsjftqjd.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2jhoomuem.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2fkwglulg.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2ypubmalf.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2xjbbiscv.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2cptxkkpt.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2rpssnxlx.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2ojacnmtt.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2hggvpdep.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2dyntddhu.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2auolmcws.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2sgbkqowj.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2wxdnhqtl.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2dynumkte.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2tyeiftec.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2pbtofunl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xoczgrva.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2nrijhczy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jfziycin.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2gjejodrn.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2xwzahwnz.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2yrmqmtvb.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2plvvegxj.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2mzifwxvu.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2icdjuywo.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2wfbvgyrn.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2qawmhjtt.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2vxnrtlfv.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2pioqbwac.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2gvtbuhvd.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2rmvvaykb.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2fwshztgg.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2khsgifvw.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2avnlkjsi.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2suvtpjsl.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2edkwukma.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2yfsrpzpe.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2eacoryif.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2zczklntq.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2atrcfmxg.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2qdwevexx.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2ryfavsjr.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2jyytsdkr.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2queyshfp.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2qyosclnv.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2bcqayyjf.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2ldvgfyvl.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2aqumxkug.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2pwcwhwig.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2zqupwfdb.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2muiigdek.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2aipdjrbf.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2dcxicgxp.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2qibgatxz.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2ztiarjyq.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2slxnibvp.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2fjzqpvzz.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2bihacwti.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2mxuvdqpm.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2grdpmdxy.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2bwfiynvh.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2zqnccurs.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2kouulgbr.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2cjaeewof.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2jjpfxjzw.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2byhznten.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2fkdwpcbf.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2csgwrphq.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2unbpcwrc.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2aixrgqna.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2tydgwdko.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2rggdwpxy.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2kmvfwkvl.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2idzhmbww.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2nnygjquv.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2oczlwlju.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2ljqjomnm.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2anteapzz.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2giupoaig.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2uowbunqq.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2oxtwpgpu.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2ulucnagb.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2ooblotjk.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2eymdtybk.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2uiiqlrxf.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2yyaywmck.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2ailfflae.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2zqokzsfx.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2omaqjvhg.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2rxgxhmax.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2aohxgmpc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cboagzax.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2lgkqqmjr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fptujjrs.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2awrqliqj.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2qyktdrcl.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2lfcixlpo.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2hgqoxspn.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2smkzxwya.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2fogumjll.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2slcvtlak.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2swhpoaml.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2tvoeoxhk.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2fzwzsuef.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2rsffkzwn.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2yadxfamv.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2zunjazut.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2nxxubzpm.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2soiiggtn.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2sztsfsye.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2uwqtcizd.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2gkqlvvve.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2sgwgksct.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2guckjjkr.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2astbkfdl.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2jfnsrfpy.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2ccogycpc.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2btrtqjji.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2fqalstyb.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2pidbizpq.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2tqlhxrxq.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2iltzyakn.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2mdomxhhp.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2sgtwiuko.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2jkrpqdxg.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2obsnkisi.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2chntlbmb.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2yhzzszdd.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2nqteqomd.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2fzzsrmnk.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2yukoukqe.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2spvtljzn.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2zqtiuvlj.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2gctbdgeq.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ixprjcds.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pckhfwha.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2yzppxgoj.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2etvwoeue.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2fbxpfqnn.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2vxhuowxl.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2kymzbjjd.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2fgjhlcxw.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2dbdjngmw.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2xcnrmkuf.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2ohsdmvto.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2pikbrnns.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2hhvpugcg.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2jedlifar.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2ogirrqzc.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2onqgapnc.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2cnnuzrui.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2mrvodery.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2xynezvdu.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2nrztpyup.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2xgbbewqq.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2wbputrve.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2rojmcvwu.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2ocmpdgbh.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2cixdtvjm.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2xgtwcpuv.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2kacksehg.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2epfiznxd.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2fqfnnrew.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2gwsfyads.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2mhsbwkuo.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2hyshrzvb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nqesnvmd.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2kgpfsqei.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rhehbxfz.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2fogrzanh.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ilbagfig.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2klbbtand.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2ehjlyvzy.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2htzyhxnx.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2wkdecxey.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ksqxhkna.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2rqvqzils.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2uoazafpk.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2bzrihbip.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2vquaqjfz.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2ukawjjcm.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2yzainems.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2raevpniw.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2ydnfhfsw.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2cnhhlomp.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2baqhcigi.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2heynevmb.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2bmqfgzjk.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2ietgziun.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2afsefukg.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2ycakofnj.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2drvbljfc.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2sjovxpsu.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2ocngjume.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2flqzzrcx.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2wzzlywsm.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2enyjnvnh.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2zvemsiin.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2gppdrxfy.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2qfutbjmx.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2rihxmpoq.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2yatoukrd.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2etiosgsj.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2alzafivc.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2bdgdtncr.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2uzaycmye.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2xiqvqyzd.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2zzopddle.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2wcduekjn.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2msxihzcf.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2ntwwyguu.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2peziulef.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2hvhnvakj.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2juscicjv.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2jgcivukf.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2mjzihfhf.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ndyspwoy.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2mbhdcwvh.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2urudiqzz.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2aljhhjlb.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2lpjnqkju.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2vftauyvw.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2wnffsxic.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2lkcrxftj.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2vizjeogf.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2kukxxmul.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2bakszcaz.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2gqxejwqc.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2lsxbniah.html


<!-- 参考信息 -->