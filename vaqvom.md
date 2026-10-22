代发 wailian999

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2pnmcpwop.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2uzgeiuww.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2iiqrrcdk.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2jfduoubn.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2astxfbrk.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2dqutlgjg.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2zdqoialx.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2mkbfefqc.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2nhqeuwtl.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2uoiccijg.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2thexglrj.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wzvysaql.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2xqiyrvfl.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2hhmdnmnw.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2vfhbgvie.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fmyyulff.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2cryjkqbe.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2sckyvecb.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2mdqelnmt.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2sojqdemh.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2bmdzsmvx.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2dvnzjnoj.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2kcksaelq.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2ucmydbyn.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2yhpknkwv.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2bmevjqwy.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2zywunybb.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2pyyjkqit.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2innqappd.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2adjdumyj.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2sdmmsfsl.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2fqritrea.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2jlbyrebi.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2fdyoixan.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2vwwbijqi.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2cjwgbjhx.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2deoooqmh.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2tiarkyco.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2dlarizqx.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2omtvwcfb.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2edeucsxd.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2vfuzcchw.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2wsfltryg.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2iyrxajfh.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2xsrurscm.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2uodljuxy.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2ltreqpcf.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2xaudvlcs.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2tsrihhbo.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2fwdyfarq.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2scnefsyl.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2ocphtywe.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2hwwnbggh.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2uvzwlbat.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2jepmyxjr.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2wjnsdggd.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2amnieudr.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2grtjtvjt.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2krnxxmqh.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2uneembqr.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2huurupwe.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2dizmoopx.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2pwffaqme.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2krlvayvl.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2eryxjwlq.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2qwevqcen.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2wyvhahct.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2fbiwinmu.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2pgdaetek.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2uszwwqvj.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2hksxbnqm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gsglaqci.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2pzgxwsyq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jqfqmiwt.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2ndvkjlbf.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2ghviivjt.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2lfzrvuqd.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2vecergps.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2dmrojctf.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2mrffehci.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2dxiujyaf.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2hwqtsdcs.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2tkqxifsi.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2kmuwmeub.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2towimhgt.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2lwjsmqvk.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2uoszlnqv.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2pwfezoxg.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2losbswsj.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2lnqfkxtj.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2czfruapg.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2kndkdxnv.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2cwwsbsjl.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2lizzlqqk.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2bgtevtql.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2ndrpwkgy.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2ikrnexya.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2zbxliemk.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2ernbjssw.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2prkwzypp.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2whpfzupj.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2roninvdu.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2uiccqvjz.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2llbzrpqs.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2jvtcgvnl.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2hzbnmbbk.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2ykrwiklh.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2kmslqvsx.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2kvuczsvi.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2nijknbqa.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2kfzfprpq.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2ldttubeg.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2gaarxjhp.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2wwsmkqbx.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2axxgctkd.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2jrugjhta.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2iiyynasa.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2dznxkley.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2eymopvrp.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2endfnbdz.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2xwwczzha.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2llbjxaqm.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2hklmvzbz.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2tracxhpw.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2kducztbp.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2uupgexyu.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2zjwgpsrc.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2ccaatxhk.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2syjylylp.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2gsexahrx.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2jtubryuy.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2tpfrpnfd.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2hcckumzy.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2ztfcqidp.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2gkbluoii.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2jthxzhju.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2dzhcjnvf.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2kqtxhjbb.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2uzdtjesu.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2fbrjdcit.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2tnhyfpcf.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2bdingzmw.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2ndjaruiz.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2mouloqev.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2zmdkufnk.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2nfgsqkvl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qdnliyoz.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2ojumziux.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dpqpoabu.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2yycndscj.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2wzywhumf.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2mgcigkop.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2sirhxrrb.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2xvsmdhly.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2swygajoo.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2atqzuryf.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2cyctynys.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2igsuzuck.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2cpwwvtuj.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2checnjmj.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2sbapgats.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2ocowikwq.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2qzsqgoih.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2jqxtceuz.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2bdwaiwxb.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2waugtazp.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2bdxcoaag.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2wovarfit.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ikzkwqfb.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2gpsmunfr.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2omnxcace.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2vkdaopvi.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2zrzzivcx.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2yhzapkpi.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2dadfcano.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2utwksyhg.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2btbilpba.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2njqlxxkc.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2cdxzwrku.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2yqtuvkda.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2iankmycx.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2odonyapg.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2spxjuzpl.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2tczntfxw.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2lttxdver.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2ndnminkb.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zfrvvfob.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2jbfizhhx.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2qukpbteh.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pumrzyim.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ggbgccbj.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2mefrxniy.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2utdoosnd.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2isxjnskp.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2qjsiyrta.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2jutwqdrm.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2kvfxkhcm.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2bpvjkmes.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2bvnjbtmb.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2ewuwzpty.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2olpooeib.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2dpdkijxl.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2inbimkqj.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2kvjobjzn.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2fjrfdlik.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2ltlwiffr.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2qjumqbuv.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2cvrrcbad.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2ftjaedto.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2xdcdrxze.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2pfcfacbg.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2euonfvkp.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2fxxoheah.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2nqobynto.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2ztmnjwvb.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2jhdytekw.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2hcoszngx.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2zlxiktmf.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2wmpgbdvv.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2acxauzmt.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2rpgmkdod.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2flhbxdrf.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2grumiukg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2raujscls.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2zhthkykw.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2biuxrbgu.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2umfyardx.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2brhmxcxl.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2ifwigcqp.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2pleyyohp.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ysqubboh.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2elwdoqwd.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2xftoyudb.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2papyzebh.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2ejqpnhyc.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2suogbznu.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2vgdcfodt.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2dsnpxxdm.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2hykqocgc.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2mqpvudmo.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2yqjzemzr.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2nqmkprva.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2nkplwuai.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2ejtxgvhd.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2jhihmize.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2nxsxpbkm.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2rzlesqst.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2fosvqakr.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2cmffvjda.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2kjfegnbb.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2ouaxtwas.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2ecbmrrmr.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2pfikrexg.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2bmadhukf.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2mafdiwwt.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2dqyovrsx.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2lwvnscam.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2tkrysvco.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jqqtgwin.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2fbfvhebt.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2vrwigrgv.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2exqclkgv.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2cjpbtjys.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2geqjtlbv.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2utbmrvsj.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2rzvifion.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2rrjdrqyp.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2iaycmscl.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2egkgugyt.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2mldrnlne.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2blhkpgwv.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2jhfuayna.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2hqlrthwl.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2optbqsfx.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2upihhlzr.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2ioqwnnxa.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2xmoqgakj.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2plnsfabd.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2mytuxoot.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2tegffwlo.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2zdvvgagf.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2vsjbhoiw.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2gmrveqnx.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2spsolhxh.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2qymcakko.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2vfmzzkzz.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2kstsdcgv.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2fedcljfc.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2ramhejwc.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2fsrvibdy.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2twnrxxfv.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2lmxzpblp.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ziklrfjl.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2xzehnmsj.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2lishxvnk.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2hossgcfu.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2dgiulndj.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2fcxighjt.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2syuekipi.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2kndmirqa.html


<!-- 参考信息 -->