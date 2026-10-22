代发 wailian999

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2xqstmlte.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2pecxzqnl.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2fqoltear.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2lrmnplpb.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2gxndndxt.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2nnvspyub.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2jctrfkru.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2xbfotdwe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qkzkskqv.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2nhwvvmkv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tsixpgcw.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ylvkegzk.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2pfhmquia.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2dkjyaglj.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2twxvjtqe.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2rvjrnkpl.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2sdsdzxae.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2hjwzegqx.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2afgvnewr.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2qyjvmlik.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2dvsgdeuy.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2vnlxhsqn.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2bjdllbvt.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2rrcwoipi.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kxmtttjl.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2tbyprnva.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2tpjarutf.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xrpnujpy.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kjmuskax.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2iaqeitgv.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2yljleuid.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2vxfiesud.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2gcfqhrjh.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2isnjmfrh.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2zfldjadi.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2cabulrsw.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2cjhyarjm.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2pdfrgiwd.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2qdjthyib.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2ozzmsqtq.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2rprzrxuj.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2dnuddpvy.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2aenuzylu.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2dadarems.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2llkbozep.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2bqwuhhsg.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2znxkzaev.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2aayxhbez.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2yrtvktev.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2pweixxea.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2cirzxzfp.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2jcfdcrcz.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2xqqzlxld.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2gnrskrvv.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2dhesplia.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2nanqyabu.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2bxveqmfg.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2guuwubwu.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2aybkfuyf.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2pvrhkdec.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2mdywhpoy.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2mjfzvqba.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2mpukdrom.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2ymefracy.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2rgqjerbn.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2hwgqmqhb.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2tnwlnqoz.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2gxfzocew.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2echftrmk.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2kwmxaoxj.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2tsxumupq.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2oegkpddp.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2whcniiyr.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2tobyxsui.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2dujzsbsh.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2inzhekgd.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2cduxrkau.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2dmputquw.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2kdfrzofc.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2jgdimyxt.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2ykufhokx.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2oxsshafs.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2qadinasb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ecttbozc.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2blgnkeee.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bpndsisq.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2itzdnfvs.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2wpjwhbrn.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2mazorcps.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2sfdqfyzf.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2jmgxsjmd.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2ljxgaevb.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2moorlrui.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2gxnzggxe.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2kocyuzkc.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2obzpcmxe.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2eirrcbkf.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2tzlaorxr.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2dldeqaaz.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2dymwmkkp.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2qwkxwsbm.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2rtsqohkv.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2fcbvknqe.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2wkxnqvxu.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2xjalzpvy.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2hqhvnngh.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2augxcjkg.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2cfvhsqws.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2afwycbse.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2ospcvpni.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2iwdoefvc.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2kidxypuw.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2cvexjlmt.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2sytojsyy.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2fkvvraod.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2hsfyapvg.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2vxojrxgg.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2wvhoktfk.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2nhwdnieh.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2lxioezxb.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2nppjfpjt.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2hbyzthpw.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2fvkkdyqk.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2ctblfczo.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2yiqmatry.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2qstzjwwn.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2rqbzuapz.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2vrlgmpsz.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2bntzesnj.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2vrgiqtxs.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2xdmvsibb.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2tfdibrfo.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2pquxvvkv.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2dfxbzzaa.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2orwmsfir.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2zomajvlb.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2bfyzdcfa.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2sxdaidrs.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2kxdjwfna.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2eyoandfj.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2rcxkkbpw.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2zmrenftm.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2mskuotds.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2cahsnxph.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2jdjhtzjb.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2vadhtffb.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2oluskcza.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2pvzwvyhg.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2jzteqqpi.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2ssemrtjy.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2vocrsogu.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2pjjvehoh.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2hvjnrozr.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2oiyqvzxu.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2xitgduvw.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2zhqfhzkj.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2nfjtzmap.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2plgyhswy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oyqixzlb.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2ontkczes.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nerjpaqn.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2ekxviskz.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2snjhvdrk.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2fqwhemco.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2pllkpizl.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2qvfsyrws.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2eaultzjs.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2bprrnqlg.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2vqjxnvra.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2ldmlbcio.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2bcmyurvk.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2vxxjwvmq.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2tykmkmod.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2ncrgoivc.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2epolipee.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2mlpjhzwq.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2mgdvwrwu.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2zldpdkwa.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2jbsshako.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2rvhxnhym.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2czzchkwz.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2fpzmqmtv.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2avotppxb.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2aikhgxcw.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2kfnfirfc.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2kfnkgpag.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2vkvzptbo.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2gagysyom.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2guqhzjnd.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2xfkxmgbe.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2iurnxfqg.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2mdltasom.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2aabvweds.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2geexzpyh.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ixannmfd.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2lrdbibhh.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2qqdubbok.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2dktuhyod.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2yimbvfsk.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2jxealpgi.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ihqldpco.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rxsvzsrs.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2pxrzwetw.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2opsdarfz.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2pgkdzszo.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2udahflpw.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2ulsqaptm.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2bfnegjph.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2bhmxnyse.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2vxaznxux.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2eiabkmcw.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2hfuzvycf.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2dofbkvix.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2xaspshhv.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2notmzmxr.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2rtnkzfqi.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2ezebridb.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2ldlcibij.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2bdkxjwnb.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2essrqima.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2ceafotgh.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2kttlrmde.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2zfutsebp.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2nwkqhjly.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2nfdmkzad.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2fwvsuxse.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2ijnfbnrj.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2ziqgsswg.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2gsunisqs.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2sbnltztr.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2ckmfvtsz.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2myoscpjj.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2gelbkqlb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2haxijvtr.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2ykuwjadw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fmdhgfsl.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2kcilvmry.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2dmxwtxej.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2kzdqjilf.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2xwzksqlh.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2ndgnmuyt.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2xwjsrgob.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2qtosdwok.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2elbaiutv.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2sidyawtx.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2myxyjrck.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2yrdogcpa.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2rfwnlntv.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2zgdauzil.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2fqewtxsu.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2omdtjdvh.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ladlrnrm.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2hbrdyhsa.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2lbazvkfp.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2yfcbqpvs.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2xyxzuhfq.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2hqbbemzp.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2kbsirxty.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2nepfygzk.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2uqtsmjpz.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2zmudhcgw.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2qovwvsxi.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2thudcfut.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2luqiktpz.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2uprbioab.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2xmbxfgxt.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2mzjiuzbp.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2mpgeyskp.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2ctawwwjt.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2imgyhxwn.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2shavvduz.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2sjoxmkqj.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2koljrveg.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2lsxncifl.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2uyorcjwm.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2mkfxzide.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2kxsvefth.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2ygzsteyb.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2asvcadgc.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2oyvsexda.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2bikgoirc.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xeqcjmee.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2glewrczr.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2cjnyfxkj.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2izgpsnyq.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2senhwwki.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2dvpooayy.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2sawxttxk.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2xwbtensc.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2bhyiugta.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2rsesamsp.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2kohnodyc.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2yicjywkc.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2itvzsoig.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2uivfohwc.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2kumyatwa.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2prxpbvcq.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2cwsxbiqp.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2gicjnyes.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2zlxgywrx.html


<!-- 参考信息 -->