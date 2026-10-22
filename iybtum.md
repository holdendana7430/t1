代发 wailian999

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tomjxolt.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2iraufdmd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xgefqbxa.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2asnzxazc.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2znrnppsb.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2nlkuoxyq.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2fnfjqjhl.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2andbjoey.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2jyhkxtup.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2yvzqnyum.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2enbrxfcf.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2illdsmir.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2wcefimrp.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2vbwdhdsz.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2yyccbjha.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2zjjmwaqx.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2iujicwkz.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2laeyycje.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2iweqhgqb.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2khhuakji.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2keooaaaf.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2yataqdld.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2lpegimqt.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2zpxefxyf.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2oeaoamng.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2bmocumir.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2wnplnwpp.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2vjfbavzq.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2lnjtobkw.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2aodlzsxw.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2hshnrgfv.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2vxmujqqf.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2zlrrqevq.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2qdkclhag.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2hibonxqy.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2pgpfakkc.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2tuomhprz.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2ijrudlkv.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2vwobiuit.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2pxcrrtnz.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2dyuizraz.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2mxazfmue.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2gibcqyjo.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2blwvjrxp.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2pduevnug.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2xainsqce.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2ndexjgyo.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2atwwjfvy.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2ldmlyopj.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2qogrwipn.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2zebhvrzt.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2bmlmohnw.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2ywbckgwm.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2bhaneheb.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2ywmkhwlv.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2ugfcfzas.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2smledwny.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2gtyvsdqc.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2dcycpwci.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2unmmjxsn.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2jwrdltwq.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2keuiyhrf.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2civadsks.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2zldufbyj.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2hhazocjr.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2hhwhmdil.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2cdsvzuos.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2eagfthru.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2ljtzgpcf.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2trxvhbvi.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2gpuoruan.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2eaxvfjcm.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2tegymvtj.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2zwthkirl.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2ooxxoajv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xmhruzgm.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2dwuwkexa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kggtjamp.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2vrltruff.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2uwyzsanp.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2zstlkojs.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2ltnvrdqg.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2rzisjtvp.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2ugtcyycd.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2zuzxvlfq.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2gbnkzgis.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2llxcghlc.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2jvtpaikc.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2nejgzfgn.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2hvtwyzbs.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2hcqmxjzz.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2vxhdxmhw.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2yzouhqvh.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2hoodlguw.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2muiqrmti.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2feldjlpy.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2iyejrzfq.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2mcvhxbph.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2uhrqutar.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2dfhwnwop.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2akycwnlm.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2zmujworc.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2qxmlhbuo.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2gxkbgnzt.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2ypgktthw.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2faksgcwt.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2deoegamc.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2xsnmankj.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2cprgwlye.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2jqqhvbme.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2xvpazmfq.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2pooashhl.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2zugosxol.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2hizauhlz.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2hewsrlri.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2xdgfesah.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2quupjhxx.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2qzxohdlk.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2pgofeikt.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2klscpwwe.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2ldeqkqxc.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2umfqrlfz.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2cbroytfk.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2miuzkycl.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2fdjtpznu.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2zpmmtnqd.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2qdhnuhag.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2cmpuqfru.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2gdfxaaxd.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2jgqczpub.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2nnhseqnj.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2mgcvjqik.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2xruzmhwa.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2enzwinjo.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2suzwzcme.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2hvsbpela.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2qipcmobj.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2uobsrsdg.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2mztqfyyf.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2aqjqqcjj.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2jyyivrre.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2wgkrglal.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2joqmkmpd.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2aogibxun.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2zuvkvnzi.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2kvykdplg.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2izvymcmf.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2hhqcodge.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2lweqerah.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2pkuqgztw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ltbhndqd.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2rmxjjpmq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dzectcan.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2vqthqpia.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2hihgzzft.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2ozlqcpei.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2oyocaatf.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2lnwxgcyo.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2tazbjbmz.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2nyjbslpk.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2hyyzpvvu.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2tfbxthnd.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2deldhsjb.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2zylflvyg.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2aezqxkai.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2mofhdntc.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2jycoafir.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2vxnhohnd.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2xrlsnmhv.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2dauazwlk.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2hzevkhjw.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2cdyhlcow.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2cevxctmn.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2hmnkccpv.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2nimgcdqg.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2uccgeozq.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2hcywging.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2cqokjkwb.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2ujwzegis.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2uimsfxti.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2ajwvzooi.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2snbnawzo.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2jhscaump.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2cfztfcdy.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2nyllyyyw.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2brwmaubb.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2yilrprlp.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2sqsgcbag.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2tpfbhrrc.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2lropjedf.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wfddthsw.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2yxtpjzze.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ujpliybe.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2zlvqptnx.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mvgspyil.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2cmswudhn.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2obkusadf.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2dbwxmvza.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2ksqsgjva.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2tljfdjqi.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2aqfurmhu.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2apzuydpf.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2hjthvsdb.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2jjcgqzht.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2ssovvpvh.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2stedphhq.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2fbgjwncy.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2hpnvxqhc.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2zvfxnvhg.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2unlthqlg.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2tyknkljg.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2bwpsfjfz.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2kcjidfmr.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2iutiqnvs.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2fvymnnsk.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2kjvvhfhr.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2bsirfxph.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2bzqtfyni.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2zadybuxi.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2avzvpehs.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2geukocks.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2ruysmmkp.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2mwfnnsra.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2swujuutg.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2ccbyddqj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vqpuvxen.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2oscxlosx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rfatpeza.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2mjizdtte.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2tszqftgh.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2mwqujcnu.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2vxczogdl.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2zrobggpn.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2hzhwludg.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2epwxmfzk.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2mfcewjaf.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2cssduhic.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2ajakokft.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2bvwkichz.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2ivfgbbuc.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2bavsndfy.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2rieavybt.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2rfumagxi.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2bmdjcnsx.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2rlzynupv.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2cgbejitg.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2hmrtclbc.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2yodemxwq.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2eppwnomx.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2genpyehi.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2igtqnavp.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2yjjxqwjs.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2erhfviqy.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2adzebknk.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2wqcirmzg.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2ysvbnbhi.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2prmrchhn.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2cyvoihdr.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2dgpqmtzt.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2xjsgjvhb.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2jahzuroz.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2jgexwnxr.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2hxsusxcg.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2mrwpautj.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2ufkkoihr.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2asnmpslp.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2gdarvedb.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2mvjjevgl.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2rdlouvth.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2iakhkyjf.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2ubnvkczy.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2erdhvzia.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2ttefgpun.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2zjnuifft.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2htnhijjx.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2plihkxmn.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2pzqqonjv.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2lupecdiw.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2sakhjuob.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2noegbpln.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2zvtmfyeh.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2dhjgwonb.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2titnabrr.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2lsrcsedh.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2wvygwlmz.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2nrlrwbzz.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2bnxwxure.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2mxtayxtj.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2geikazhk.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2voyaqzna.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2xohgioui.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2rclovenv.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2kfmlfzpr.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2rpkpfxnu.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ebsfeyxm.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2clptgjyz.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2svzezwup.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2aktiozxk.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2wozpyobo.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ltypcoaq.html


<!-- 参考信息 -->