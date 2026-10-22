代发 wailian999

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2nupzsivb.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2zbsnrgfn.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2ebcroalf.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2hicutskn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zizvbnxl.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2skagdiak.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dseruahm.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2lzldmqfa.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2qisgxgbj.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2kkpnlcxs.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2szwikozw.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ygahiova.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2xwcwnifj.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2ntolukde.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2atlcyrsp.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2cocofdgd.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2pmfgaoyc.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2odxmmycz.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2nsncjras.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2mmaxxjrh.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kmqatbju.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2mooqsuel.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2ubvekhfm.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wriqpysa.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tndheiwn.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2uvahrovd.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2mmojdtjf.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2vxgskirz.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2utdxjfye.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2jlodtchh.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2agounhya.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2oozwrqxw.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2hhkfhuwn.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2hbieybia.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2qbrfcibw.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2ymemqeba.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2oeshodhi.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2ojblebgw.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2jyjgzvsg.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2kngyozjg.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2usvorojc.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2fvuctyjs.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2hpmogedj.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2hctznccy.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2lamedtoa.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2mjrkhxts.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2vcvgjqsd.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2fylvplcl.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2xhuolywi.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2jnfveurm.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2ejkxtxre.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2rpcstcsg.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2fivhfdjs.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2fqhhftlk.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2anhrapbj.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2ohngvjzd.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2nftksavo.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2ukrsctno.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2ieclabuf.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2mzxjikqn.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2owiwvgda.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2nzdbdhxw.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2gjwhtxvp.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2nqrfwwhy.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2rhzisleb.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2jwacieke.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2eslabfig.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2ttqkfzdk.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2skvwwhsg.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2aatcxbha.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2bkdccpgk.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2hyckrwwh.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2mnpdvyiq.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2saywpczb.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2izhxeavp.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2hvcrfzdi.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2jchslvdy.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2dgqgdrvs.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2chflfkyd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ygblofzd.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2mvyzpghb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jzbylhzt.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2viwnmjdx.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2wrqspixl.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2vatlspuf.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2lljjpwzi.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2tjolnnkn.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2ipnsrpbc.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2ntwjylrd.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2jzvhiesh.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2tmbwqfhj.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2ayrilcbb.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2itonygfn.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2ievgllxm.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2vvryjnzs.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2zggziuva.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2mynjdgkj.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2pjqmalzm.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2dgbcjmoa.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2slgelgxs.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2njclessp.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2ibluvipp.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2qpewjynk.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2mvbgqvmn.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2sgeermih.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2axiwonuf.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2imzcinfe.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2tcomdcfg.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2nvchowta.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2bsdoulrt.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2uvxlovfr.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2hlvwauqp.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2samnhrrs.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2aiiabksi.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2gdbtbczn.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2qxxctxby.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2sqbczjjv.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2dzqtfrbw.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2nemzzocj.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2yyhjktmn.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2utqvnfzl.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2sfmnycec.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2mndojunu.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2xzwmtokd.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2gjnidnen.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2lgxjuayd.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2cjunpkcq.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2fchhefgv.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2yyuxrmbn.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2tifiekzl.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2lpmhtkvm.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2tajlutgg.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2blrzvkuc.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2xjfuyhwv.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2xgqsvozi.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2rnlqxigu.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2cuyuzaop.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2rzpovowd.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2msqhjggq.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2rwzqotjb.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2hmvgfiew.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2gyhhzgbk.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2psqmbrsw.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2knzjthxx.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2ddfujtes.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2pwhnyufg.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2eqjrxfcf.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2bgmjuvps.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2meepjndp.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2qlhnywri.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2ioldiear.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2pbympnag.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2gkpnyhzy.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2wzcbodsj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zwlmxgbu.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2nllfkbhj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dacgzuet.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2zpwdsldj.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2xdpqbrjl.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2zviatizj.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2agurnvjt.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2iohbhunw.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2bcnrohmk.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2fgfmjofy.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2ftpwadwt.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2qlxnjtca.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2ymmfdssx.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2jbrcgakk.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2csfkjdce.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2ogpghiah.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2vcbtkkah.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2giuvcudu.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2iklevqbe.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2fnikpimc.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2phxxxzaw.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2dwvmbynt.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2bmocxrvg.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2kgayrjrs.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2drlyjfiq.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2xfqozyrw.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2skyxqtft.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2fezmgoxy.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2vibcpnqg.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2kepejaed.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2teaqcpsb.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2pplbraad.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2twopbpxm.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2eqgpvuvj.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2lkdaroxn.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2qqznfwgc.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2psilfdjv.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2gjwxlsmn.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2vzvjcwlr.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2okxchhrb.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mtqkauqd.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2hsbwbwgh.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vscvczyr.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2aqllnvrr.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2eukscvwp.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2qzwcdjtv.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2szqnccbw.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2sljzlxzx.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2dxdlnaxa.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2abemrwki.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2thlxxnoz.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2jssveply.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2lqvbzueq.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2wnyhrejy.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2aejrivlu.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2gkcuixef.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2cxbwzkfo.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2kiplxikc.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2vmkwpqub.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2qmxtthco.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2ykiejqsf.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2mowssacp.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2dodffqty.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2fipgrwtb.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2uotyxtpc.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2iwlodfkd.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2wzdtvffd.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2likjeouq.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2ohopgpai.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2wnlmoexn.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2vphdcvzc.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2webkxdgv.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2wvnywybt.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2wmmqoszq.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2bwpmgbjp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bucmgtip.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2kvynhmij.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zxndnsnv.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2eojyqfqd.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2txrqbhpw.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2nyqrbuof.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2vwsbtwcn.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2zpvyoxst.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2dgovfncs.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2wyqwicsc.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2fhcklshd.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2rxpslkvw.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2bhtrtnip.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2gjlierbg.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2uxcmogkw.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2dckjqvzz.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2pqpsqwgc.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2usdyhzgj.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2bihzusfu.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2ppfikvkb.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2yxsrcwlc.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2fyuhcylm.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2mitbsvoo.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2xyqqrmbv.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2hallrcqx.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2quswphmv.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2nowbnyfl.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2jtseqvnp.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2jremthix.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2behppxfs.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2owbszayt.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2cgghpdoy.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2fcrupohu.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2jgwtsjcx.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2sockctue.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2zfvtncxv.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2agthexoe.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2riczqtef.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2oknlrjvn.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2cuuoghlr.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2qnxcvypz.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2wbhgmptm.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2hwmbuabj.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2cfwrqgaf.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2ayigoqul.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2lyqsjais.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2zybykquq.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2xfdcbmye.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2npguurqr.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2wwhjzmke.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2kibgfgie.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2unnsblgx.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2yfxkegti.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2acupvcub.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2zkqndkmc.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2khmipcgb.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2qknhqbtf.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2vyumfgek.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2kytxcxyk.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2xdpcygel.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2sfonoeqb.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2wkbmyzla.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2xzshirql.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2uszingmz.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2twqdfxjy.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2kpooddyd.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2ppxtekrb.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2alprgdhk.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2atnluprj.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2iacakfwx.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2airolfny.html


<!-- 参考信息 -->