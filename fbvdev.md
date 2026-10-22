代发 wailian999

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2olykavep.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2chyzpckg.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2bflztywh.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2shuywvny.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tidnhcrx.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2yrvoqahb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lxiyxapc.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2vwopwhpo.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2jwlmgaax.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2khbnqimy.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2niwpqgwk.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2uhozyzlh.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2jeqpeuqb.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2mimedveg.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2hzihoagh.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2hecxesei.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2cvgfxzjb.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ngxaajps.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2urpuqolp.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rvkpfpqh.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2xwvuwxvq.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2fwrefydy.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2gjwtbjgc.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qxcqwixg.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2lwwkoqjf.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2nwjzccfu.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2cwhmaooh.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2xwnqawyd.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2xhgvrsgt.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2yspzkrta.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2inghafri.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2zldajveh.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2luzknzpz.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2enxrxxbq.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2rcythykn.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2vcvzpzei.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2zblowwnh.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2xpourgab.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2keaaiqmx.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2ayyhydiv.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2ygebglov.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2squolrwn.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2felbmxpy.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2ldaaqdgs.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2jrezwlvy.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2gwhnrcfg.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2klqghkwy.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2uqmszjwv.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2whkbxkez.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2khwksoyx.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2rsqfanyv.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2uslcdpmv.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2kaisqein.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2vxmlepcf.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2bozecqyf.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2kifywuwn.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2bqeqvgbb.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2judvcgne.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2fixnuuxu.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2dtdouhpk.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2sdpqhgll.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2ilnmzmbi.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2dopbqtde.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2xzixplwl.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2vcdnqgdf.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2zfdkhctn.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2dncfhhlz.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2gjnwtvgf.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2iywgmxsy.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2gthezwhn.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2asubawiu.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2pjqgbghd.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2zgltldtz.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2zdhnksff.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2cnnbczpi.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2lcdpcoso.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2pdeajgre.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2eokhqqjn.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2efnslcjc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dgkxftfb.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2kwfleryo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bjzvoecm.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2hqppobog.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2gpkphqqh.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2oiypftha.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2mfiklmhu.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2xrromxtf.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2edftdfos.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2cbeebxvv.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2jvejcggb.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2bvrulewt.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2nyzedycf.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2ldhfvtwd.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2ninkssyi.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2fkpwbptr.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2weiggase.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2nrgibaqy.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2ecjexidi.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2latxcesn.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2tvuzovxw.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2rxkqzpiz.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2rgryrnfa.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2icxkinqu.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2htdcgpuq.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2oiziuizt.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2vedajvzh.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2jwmbnboe.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2gjspjkbc.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2kbpjbwxl.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2qpmoziuy.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2zhlbqcch.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2ccrlkver.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2vkvokinz.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2dtgeufrf.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2zlkfqlxq.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2gpbbdmdu.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2nccdqqcn.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2pxvbexlr.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2ugucnntm.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2nzncpsqu.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2sifbylmx.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2ewmryyqy.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2yhpbysgr.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2cayojbav.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2jwynphnf.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2eykjmoxq.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2juagdrke.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2abqsiezj.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2sxtlsukb.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2lbpxvsxj.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2dugddrkw.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2wkuvljbn.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2omzffnje.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2hrlbwvnw.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2lswrzwdq.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2rnpwrhhm.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2bcpjhydn.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2cykztwik.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2fukbfouv.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2kticgnya.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2yskcvset.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2wipjqfmn.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2skjaeoou.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2segtbywa.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2xefvsqjw.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2sfszyddq.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2fuhryysl.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2vohjjeww.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2ydwpcyxy.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2ncvrfzzu.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2iafgashw.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2txzkufzm.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2chaesgna.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2zipojxld.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ndimggyb.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2qchqkkwb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kttlzhve.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2yiyjhhfl.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2zlvmscih.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2wzgkdwgj.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2xwjthniu.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2aylxrlnh.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2zlzsdmkv.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2rgxnbzxq.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2ckfbjtvo.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2rqdtdkex.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2zforiqay.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2urlttbrp.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2tyxnbmyz.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2nwvpgwkx.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2lxwzvezp.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2hdwhhidl.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2glplphun.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2fwwrzgpj.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2dqsjvgtd.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2anaeucpd.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2zjlxyrzz.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2aqzzlhhz.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2jvojjljr.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2thdtkbgk.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2ndzlvbyw.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2vnmtdhch.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2rjrxjdom.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2zmsnpfef.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2eevwjici.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2vwiinhtd.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2nuxdxjmb.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2rpgyyplu.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2whxykjnf.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2wjhkwosl.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2chbkjyyf.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2pcfjdvmp.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2petcmjoo.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2iorzmqiq.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2mbsuthov.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2subaiasd.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2nllqqrhh.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ebbhpwwa.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rzlgbykw.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2cdpvlyfp.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2kosuacgn.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2yluajoqk.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2zvmcmjaz.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2ltwuvhqn.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2twxgovtu.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2bhiqedgx.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2tdqvxnag.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2xognvmwo.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2xdwlihvb.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2sonrsxyw.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2humhtzyk.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2tpldormo.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2qhjnmlrr.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2jezcpiki.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2vvxjhbgu.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2lalctkqg.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2nmegcrkq.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2mxlbzoro.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2iqtycmlb.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2wmhvztrf.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2ncacqupu.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2dznqaobe.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2ozilhybg.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2gjavluni.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2jdplahcr.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2lltyavgd.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2ppajfoes.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2agzjgand.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2nomyovhs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2irpalybd.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2nbzdzotn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2orlimdvd.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2ynnwbaxj.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ecnjwvlk.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2bkrhwbbe.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2cuhaxxhb.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2dxkaxiqf.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ttxalzkn.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ylzhvwqr.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2hgeldwgu.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2yjcngojy.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2zohzxuck.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2jqmyhytu.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2dhcshvgr.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2muynhusk.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2kamwhaca.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2cyfpifhs.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2ckkjpudn.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2mswfkykr.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2kemfyzbj.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2bcqhlgtq.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2qnsyupoe.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2tpigomos.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2xbucqawm.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2nayqylyo.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2zngiaing.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2ynafygho.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2lonfwyml.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2rytdkwob.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2dolgrsfj.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zigbnqfr.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2ttverdqo.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2kyalwelb.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2kjoqkbeu.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2hovnfzbm.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2iaegqsqv.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2vxhepfht.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2qxolmpup.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2pccdadvr.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2odzidxng.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2szyjdyrs.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2lewdoncc.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2dyhaowbf.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2iqyacqrc.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2xyxxqjvw.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2dglsuple.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2vqfmkzux.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xexvdcsi.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2zkedmdyw.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2thvrsepj.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2bbvuygym.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2jnulnrnh.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2svoxoyxy.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2sulhkduo.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2ihbcjfuc.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2qzjcrqdk.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2ebmiirsk.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2slhwrxgb.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2chfzhndx.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2rbnshfuv.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2tkapyjii.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2ywpbxaej.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2gwkuwsri.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2qsbxmlgm.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2ngdheqlg.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2jdokfdmd.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xzmtfkar.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2frnzaadc.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ghqjnzlv.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2pekdtrqh.html


<!-- 参考信息 -->