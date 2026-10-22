代发 wailian999

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jolgsvqp.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2zbffqazc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hvaixicr.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2pkpbvjpi.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2eyhuubdf.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2yjuptues.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2kgnvlffn.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2nrjcubqp.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2bmazliac.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2nranwjpw.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2pjiofvkc.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2mgzfhbvp.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2sivndndl.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mnkjxzqz.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2botpcbws.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2obppvgjp.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2hyymyfmw.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2acawpzvr.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2naojkmmn.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qkwooxyl.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2mqrxinot.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2txhwtptk.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2yvyvzrfd.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2wblyluas.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wxbibrwn.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2ccxewzbb.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2uvxxaqft.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2vqpsbbpp.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2cdsegvoy.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2bjctjboy.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2cbcqemcw.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2udxyqktk.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2vhdfizcv.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2aotsacvl.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2agqwmmxk.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2dhmchmbp.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2ispmtuwh.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2yolkaikk.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2usuvknbi.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2mpedelvm.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2baokmpjj.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2lszjzobq.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2jqjtvgsj.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2buxbaxii.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2ilqzmamz.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2xicgycia.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2jmovwdoi.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2ysfajeew.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2jlgyurrm.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2idjttjrv.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2pecnjrvx.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2hwyepcfm.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2gpszsdae.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2wvfwbjae.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2uectdftq.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2aqpstcsl.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2vqtltget.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2datenjrl.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2mzmudlby.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2mqjamhkb.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2mxajovfo.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2spxtzlwd.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2lfpfvwon.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2abecdojd.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2zvhblscc.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2sfginhaq.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2pujzatbv.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2zkspraqq.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2scgcdyld.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2pbuiikbd.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2harbixfw.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2azjoqsmm.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2jfmytblk.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2rgjbhggd.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2orfzjsto.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hmjcctiq.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2mvfxivzz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2azormcbh.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2kmpuymwj.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2bspaqdpo.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2xitzocyy.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2ifgqgaxh.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2qcurbtcc.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2fmbwzpcz.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2mdnsdafu.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2ojyvmjzs.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2jbtmsfhv.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2mbnlrhmn.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2hiwvfhrl.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2rokboupx.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2rfmlsjmr.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2zqlbgkzr.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2wigltvbc.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2zdqyuqwm.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2mopmvxob.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2xkhbzpop.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2fsecmwro.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2ppusfeih.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2xvzhleqp.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2znlxcjri.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2xowdmwrl.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2pfkxqndi.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2phgahfsy.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2zyihkwrb.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2iklaibfr.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2ccuuxcgq.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2gbuslwxi.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2ubwjkisu.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2fhhtckzg.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2ujojsmcz.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2xodbshkq.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2repecixw.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2hnjorcfx.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2uxjdfbsc.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2bgyauxkz.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2clcdvxcn.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2atzsukkw.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2rttjiwsp.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2roeeeegt.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2digyxpqc.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2ezbzlvun.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2kvgypetc.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2jsiuqnpc.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2jndqkcre.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2oczxrbxj.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2xgmbyaqd.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2deomkfib.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2lrfsdmnp.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2jhznxwzp.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2rbbzaoij.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2oseqbckx.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2hghzexgd.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2hvbkpvvy.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2chxxtchp.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2pwwzegwk.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2xxzztexk.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2mckzzmwo.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2rmhrqtcn.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2vzzfjfqx.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2jhromeiu.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2ayggkkkz.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2viftnfti.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2jnymaesq.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2ujpurzxz.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2jlflbgfd.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2mcuyfttw.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2mpxieaqu.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2xxkxsnkp.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2jkblkqvm.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2gxtcanrc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rbcftyxh.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2kmkgksyh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gcpddmmw.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2argvlkft.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2wedwhovp.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2fxswqziz.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2drdiwsvr.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2dvcdeify.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2jvotmvsa.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2ipvkajzv.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2zshodxjn.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2yxhjhkyt.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2bjtugenf.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2jzrsauxu.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2iuulorun.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2otduzgsv.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2ymzazzjy.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2dncugxuq.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2plwmcaav.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2ogeywxtd.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2kpembzkk.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2czqmbbxy.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2eazcceyr.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2jvqfvlkt.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ktaftvgx.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2yolyvluw.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2qaljcfjw.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2rxrnwqgp.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2ltptlsck.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2eyrxzilo.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2nqhqehda.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2wkyvvqeo.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2ssrklxsy.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2lkkxovrz.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2iebrnhib.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2ngsemwat.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2dewqebby.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2zuwruhns.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2zvyucqfv.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2nzadomcm.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vztrhcpk.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2swsqiqvn.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2uekewtpc.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2wllfhmvm.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2apkwovjt.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rhmubiwm.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2atvthhhz.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2bswxwhfm.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2cenkailt.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2tfvkcmem.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2hsbbsepg.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2quksjxty.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2jmrdstae.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2vicnznnc.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2lgfeitwd.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2ofimjkgs.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2ywmiqrvf.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2srmwdigz.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2tgixtzrh.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2bepfkuce.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2mvhmctyx.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2mzgyfemv.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2ceeomesp.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2gznzjsyp.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2omkdndfu.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2zepngabj.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2jxlsexvx.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2uxkevhgt.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2fclklnkv.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2zhjheeym.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2rjuurqwe.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2plaqaeha.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2lzedmtav.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2ugltcxwh.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2dwludpuq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kljfdioq.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2bjpprzjt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hviezlsp.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2cmutuxrz.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2czrhkexf.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2lffwxphs.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2fliqzgic.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2psbalhbk.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2fhbxognv.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2veatvflw.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2mbuzdsbe.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2zndejjeh.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2amflargg.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2vjpzzpzk.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2slphqsbn.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2zkswvwym.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2svcjbitq.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2wbrrspwn.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2horizgji.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2xrbpsubm.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2rschpltw.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2ypeeptdw.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2qmolepez.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2mqkkhcbg.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2zjninqxc.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2txegqorn.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2iybmyqtu.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2uztrqxwy.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2ytgerepi.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2tianroba.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2rbgzbvtd.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wzjfxgiv.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2lepwiugb.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2rgzrlfgd.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2ygkozyei.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2qqbresej.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2osagccpw.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2wrxqqfpc.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2uycyvgkt.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2nvwopvmz.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2fgamnnup.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2qvctmtle.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2rjbshyxw.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2cjbchxzw.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2mrffxulb.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2wjsptizd.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2ayiujksp.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2gtjrxkxm.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2iqppxjvd.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2idwxemkw.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2oetpggfo.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2azlzdslt.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2lsutbnak.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2dvqutluq.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2rgzsfupn.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2iqmqtdij.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2yqoybqek.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2afhhssee.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2fnznslqt.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2nzoibuha.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2xyxjndlw.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2zyzfkntc.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2anwenrpj.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2ffoxsoof.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2igedpqdi.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2rmujrigo.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2onacfdnq.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2alswqmer.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2lbufmezd.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2mfrfyppu.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2gwrpeivz.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2vpizidii.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2mvwmuvff.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2dzorseld.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ytppurrz.html


<!-- 参考信息 -->