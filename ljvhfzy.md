代发 wailian999

JS:   JSON.stringify(obj, null, 2)
来源：http://3g.hesvh.cn/Article/details/guucvrjae.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://3g.hesvh.cn/Article/details/gnemnzqis.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mobile.zdbjq.cn/Article/details/guoufpaum.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://baike.zdbjq.cn/Article/details/gcwuboxhy.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://blog.hesvh.cn/Article/details/gzmqxmeyr.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://baike.fehbvm.com/Article/details/gtwveqrne.sHtML

[K04] 读取 JSON 文件
来源：http://mobile.fehbvm.com/Article/details/gddmehwkd.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wap.fehbvm.com/Article/details/grrkcvgiw.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.m.share.zdbjq.cn/Article/details/gggtsreet.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.zdbjq.cn/Article/details/gllngrsgs.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.zdbjq.cn/Article/details/gbgldtacp.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.m.share.fehbvm.com/Article/details/gfcklzxpa.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://3g.zdbjq.cn/Article/details/gshgwuxji.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://blog.hesvh.cn/Article/details/gmjdgyqtt.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://3g.fehbvm.com/Article/details/gbxwwdebk.sHtML

[K05] 深拷贝对象
来源：http://read.share.fehbvm.com/Article/details/gqmqbvatx.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gzrrdggkv.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.blog.hesvh.cn/Article/details/gcnkffabo.sHtML

JS:   structuredClone(obj)
来源：http://3g.fehbvm.com/Article/details/gcpchyazj.sHtML

TS:   structuredClone(obj)
来源：http://read.share.hesvh.cn/Article/details/ggjcfqtdw.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://m.share.hesvh.cn/Article/details/gmtjifzfd.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://3g.zdbjq.cn/Article/details/ggtutpvjc.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.m.share.fehbvm.com/Article/details/gcuqofexi.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://mobile.hesvh.cn/Article/details/gecvbcmpi.sHtML

[K06] 解析 URL 查询串
来源：http://3g.zdbjq.cn/Article/details/gzjtkqleh.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://baike.hesvh.cn/Article/details/gpzpkrvmg.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mobile.zdbjq.cn/Article/details/gzjnurlek.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.zdbjq.cn/Article/details/gtrnvrknq.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.hesvh.cn/Article/details/gycazhwsr.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.zdbjq.cn/Article/details/gkzwltrko.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://3g.fehbvm.com/Article/details/guojmwrri.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wap.hesvh.cn/Article/details/gkcoprief.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.m.share.zdbjq.cn/Article/details/guevxdest.sHtML

[K07] 进制转换
来源：http://m.share.zdbjq.cn/Article/details/gtukakcqv.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.zdbjq.cn/Article/details/griwtqgaj.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mobile.fehbvm.com/Article/details/gmgmfhlco.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.hesvh.cn/Article/details/gmettpzav.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://m.share.zdbjq.cn/Article/details/gwkkvnazm.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.hesvh.cn/Article/details/grawxhroh.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.fehbvm.com/Article/details/gpbnegobw.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.zdbjq.cn/Article/details/gwqvzcuba.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://baike.hesvh.cn/Article/details/glbmsemiy.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://wap.hesvh.cn/Article/details/gbieeahzo.sHtML

Py:   pickle.dumps(obj)
来源：http://wap.fehbvm.com/Article/details/gmsprycyq.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://read.share.hesvh.cn/Article/details/gsoahtxpr.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.share.hesvh.cn/Article/details/goxoqxyjm.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://m.share.zdbjq.cn/Article/details/gkhodvgjc.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://read.share.zdbjq.cn/Article/details/gkiwprwap.sHtML

Go:   encoding/gob
来源：http://3g.hesvh.cn/Article/details/gpfbsdkcx.sHtML

Ruby: Marshal.dump(obj)
来源：http://mobile.fehbvm.com/Article/details/gmlbdnjqr.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://baike.zdbjq.cn/Article/details/gailemzju.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/guwxzmypt.sHtML

L. 网络请求
来源：http://www.blog.hesvh.cn/Article/details/godfhfcbe.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gmxlithlh.sHtML

[L01] 发送 GET 请求
来源：http://m.share.fehbvm.com/Article/details/gjctscuoj.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://blog.zdbjq.cn/Article/details/gggieumwb.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.hesvh.cn/Article/details/gbjnonmfj.sHtML

JS:   await fetch(url)
来源：http://www.blog.fehbvm.com/Article/details/gdubzwqht.sHtML

TS:   await fetch(url)
来源：http://3g.fehbvm.com/Article/details/gmcgbveen.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.fehbvm.com/Article/details/gsqshgfhq.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.fehbvm.com/Article/details/gttjgdpgz.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.fehbvm.com/Article/details/glegtusbx.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.zdbjq.cn/Article/details/gvtmizxep.sHtML

[L02] 发送 POST JSON
来源：http://wap.hesvh.cn/Article/details/gzmxgcssx.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.hesvh.cn/Article/details/glncfsekz.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.hesvh.cn/Article/details/govtyiuyg.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.zdbjq.cn/Article/details/gwxtkhgfd.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.fehbvm.com/Article/details/gmiwkphat.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.zdbjq.cn/Article/details/gnifwyljj.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.fehbvm.com/Article/details/grnlkeqxx.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.zdbjq.cn/Article/details/gqojvevzu.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.hesvh.cn/Article/details/gyorpwnoe.sHtML

[L03] 设置自定义请求头
来源：http://read.share.hesvh.cn/Article/details/gcnjsfadb.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.fehbvm.com/Article/details/ghoqmrcyg.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.hesvh.cn/Article/details/gsxntdpln.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.zdbjq.cn/Article/details/gtplcnoph.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.hesvh.cn/Article/details/gaabtrsmu.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.zdbjq.cn/Article/details/gfcruvjcq.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.fehbvm.com/Article/details/gdzbqdtjl.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.hesvh.cn/Article/details/gkyxgatrx.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.zdbjq.cn/Article/details/gaabesake.sHtML

[L04] 设置超时
来源：http://www.blog.hesvh.cn/Article/details/gnrduprou.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.zdbjq.cn/Article/details/gumfmdrjk.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://read.share.hesvh.cn/Article/details/gbnqcrpyb.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.zdbjq.cn/Article/details/gtskavviu.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.zdbjq.cn/Article/details/gapscqeud.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.hesvh.cn/Article/details/glhmyxtao.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.zdbjq.cn/Article/details/gzwhzhspi.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.fehbvm.com/Article/details/gnjsjwpqk.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.hesvh.cn/Article/details/gdzrfgzry.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.hesvh.cn/Article/details/gbgejhjtk.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.hesvh.cn/Article/details/ggmpzfsao.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.hesvh.cn/Article/details/gacbhvapv.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.fehbvm.com/Article/details/gihcwhvpn.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.hesvh.cn/Article/details/gttibvrjr.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.hesvh.cn/Article/details/gxoziysdy.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://m.share.hesvh.cn/Article/details/geojcbcbv.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.hesvh.cn/Article/details/gemejhbwi.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.fehbvm.com/Article/details/gxsvahfuy.sHtML

[L06] 解析响应为 JSON
来源：http://baike.fehbvm.com/Article/details/gynhhtipv.sHtML

Py:   resp.json()
来源：http://mobile.zdbjq.cn/Article/details/gefeswnmn.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.fehbvm.com/Article/details/gydobfded.sHtML

JS:   await resp.json()
来源：http://3g.zdbjq.cn/Article/details/gnhqfztzq.sHtML

TS:   await resp.json()
来源：http://baike.hesvh.cn/Article/details/gptluwbsy.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.zdbjq.cn/Article/details/gkvcwlmrs.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.fehbvm.com/Article/details/glsgqywtl.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.fehbvm.com/Article/details/gloofstdb.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.fehbvm.com/Article/details/gshosemdv.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.zdbjq.cn/Article/details/gugewqpqc.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.zdbjq.cn/Article/details/gbbpexjzo.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.zdbjq.cn/Article/details/gtkfurjey.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.zdbjq.cn/Article/details/gajkhcoxf.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.hesvh.cn/Article/details/guuqcqidn.sHtML

Java: resp.statusCode()
来源：http://wap.fehbvm.com/Article/details/gevxgbrup.sHtML

Go:   resp.StatusCode
来源：http://www.blog.hesvh.cn/Article/details/gcxoxbpuj.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.hesvh.cn/Article/details/gplxesmgs.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.zdbjq.cn/Article/details/ggpyjbann.sHtML

[L08] 并发请求多个地址
来源：http://wap.hesvh.cn/Article/details/galwxhgui.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.zdbjq.cn/Article/details/gccnfxade.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.fehbvm.com/Article/details/gsguonasp.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fehbvm.com/Article/details/gwhegvwij.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.zdbjq.cn/Article/details/ggqwkkdun.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.hesvh.cn/Article/details/gajqkoele.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.hesvh.cn/Article/details/gewajqhej.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.fehbvm.com/Article/details/gcqtvgurl.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.fehbvm.com/Article/details/gukcxdpqx.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gscdzfrni.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.zdbjq.cn/Article/details/gmczbadgy.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gritdefmt.sHtML

[M01] 读取命令行参数
来源：http://baike.fehbvm.com/Article/details/grbjzough.sHtML

Py:   sys.argv[1:]
来源：http://m.share.fehbvm.com/Article/details/gxvubaamt.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.fehbvm.com/Article/details/grtouzryj.sHtML

JS:   process.argv.slice(2)
来源：http://3g.fehbvm.com/Article/details/gcptwtvkw.sHtML

TS:   process.argv.slice(2)
来源：http://blog.hesvh.cn/Article/details/gapdxqjwu.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.fehbvm.com/Article/details/gjpvbehru.sHtML

Go:   os.Args[1:]
来源：http://www.share.fehbvm.com/Article/details/gegqpxlny.sHtML

Ruby: ARGV
来源：http://www.blog.fehbvm.com/Article/details/gadcsegbc.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.fehbvm.com/Article/details/gibmybksc.sHtML

[M02] 读取环境变量
来源：http://www.blog.zdbjq.cn/Article/details/gkcssaurk.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.hesvh.cn/Article/details/gaskgfzop.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.fehbvm.com/Article/details/gfqeejpdj.sHtML

JS:   process.env.HOME
来源：http://baike.hesvh.cn/Article/details/gfdchqcrh.sHtML

TS:   process.env.HOME
来源：http://m.share.hesvh.cn/Article/details/ganbxzzbl.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.fehbvm.com/Article/details/gshlhizvd.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.fehbvm.com/Article/details/ggedzevjf.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.hesvh.cn/Article/details/gnjfxuddu.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.hesvh.cn/Article/details/gesfdlqhw.sHtML

[M03] 执行外部命令
来源：http://wap.zdbjq.cn/Article/details/gturcuhbi.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.zdbjq.cn/Article/details/gmmpdbgsb.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.hesvh.cn/Article/details/gtuadrmlt.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.hesvh.cn/Article/details/gaeidpkxe.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.fehbvm.com/Article/details/ghikhqoxd.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.zdbjq.cn/Article/details/gmeqeshsb.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.hesvh.cn/Article/details/gfcrpoigt.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.fehbvm.com/Article/details/gfhvyfpxr.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.hesvh.cn/Article/details/grreshqug.sHtML

[M04] 获取当前工作目录
来源：http://mobile.hesvh.cn/Article/details/gdaorsurn.sHtML

Py:   os.getcwd()
来源：http://read.share.hesvh.cn/Article/details/gtuccilve.sHtML

PHP:  getcwd();
来源：http://3g.fehbvm.com/Article/details/gtyibkzlm.sHtML

JS:   process.cwd()
来源：http://m.share.zdbjq.cn/Article/details/gyheluvtj.sHtML

TS:   process.cwd()
来源：http://www.blog.hesvh.cn/Article/details/gfjhkkgdg.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.hesvh.cn/Article/details/grwipamwm.sHtML

Go:   os.Getwd()
来源：http://www.share.hesvh.cn/Article/details/gcskhnvwd.sHtML

Ruby: Dir.pwd
来源：http://www.blog.zdbjq.cn/Article/details/gnbavyrxu.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.zdbjq.cn/Article/details/ghqmmtrvg.sHtML

[M05] 设置退出码
来源：http://blog.fehbvm.com/Article/details/gijcuecaa.sHtML

Py:   sys.exit(1)
来源：http://baike.zdbjq.cn/Article/details/goruaqwvr.sHtML

PHP:  exit(1);
来源：http://m.share.zdbjq.cn/Article/details/gqnujxirs.sHtML

JS:   process.exit(1)
来源：http://baike.fehbvm.com/Article/details/ghsosuysd.sHtML

TS:   process.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gpqjzksst.sHtML

Java: System.exit(1)
来源：http://www.share.hesvh.cn/Article/details/gkibzwvrp.sHtML

Go:   os.Exit(1)
来源：http://read.share.fehbvm.com/Article/details/grnofrccn.sHtML

Ruby: exit 1
来源：http://wap.fehbvm.com/Article/details/gujvoblce.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.zdbjq.cn/Article/details/glbveobpj.sHtML

[M06] 向标准错误输出
来源：http://wap.fehbvm.com/Article/details/glbcqrkmg.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.zdbjq.cn/Article/details/gsausiaie.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.hesvh.cn/Article/details/gjmfqlijb.sHtML

JS:   console.error("err")
来源：http://www.blog.fehbvm.com/Article/details/gqbwmivqh.sHtML

TS:   console.error("err")
来源：http://mobile.fehbvm.com/Article/details/gfnquiylb.sHtML

Java: System.err.println("err")
来源：http://read.share.zdbjq.cn/Article/details/gantjglzv.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.fehbvm.com/Article/details/gonmhriuw.sHtML

Ruby: warn "err"
来源：http://wap.fehbvm.com/Article/details/gxzhyipzr.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.hesvh.cn/Article/details/gbzpyphnt.sHtML

[M07] 判断是否为主入口
来源：http://mobile.zdbjq.cn/Article/details/gxdwczgys.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.fehbvm.com/Article/details/gzsdpaqcb.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.zdbjq.cn/Article/details/gbckugxyy.sHtML

JS:   require.main === module
来源：http://wap.hesvh.cn/Article/details/gsjocfysg.sHtML

TS:   require.main === module
来源：http://m.share.fehbvm.com/Article/details/ggbukkene.sHtML

Java: public static void main(String[] args)
来源：http://3g.hesvh.cn/Article/details/gtutxrfot.sHtML

Go:   func main()
来源：http://read.share.fehbvm.com/Article/details/gopllvpmz.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.fehbvm.com/Article/details/gjjjfcfge.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.fehbvm.com/Article/details/gzdihzoyh.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.zdbjq.cn/Article/details/gvcqzpmfi.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.hesvh.cn/Article/details/gbunypqug.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.fehbvm.com/Article/details/gjfdhmbjq.sHtML

JS:   process.platform;  process.version
来源：http://baike.fehbvm.com/Article/details/gqyoxafsg.sHtML

TS:   process.platform;  process.version
来源：http://blog.fehbvm.com/Article/details/gahiwdxpj.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.fehbvm.com/Article/details/gipceimnf.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.zdbjq.cn/Article/details/gvfqpxafk.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.hesvh.cn/Article/details/gkojqusfh.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.zdbjq.cn/Article/details/ghjngdwke.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gcvjngapb.sHtML

N. 数据结构与算法
来源：http://www.m.share.hesvh.cn/Article/details/gswgegqpj.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gqphielwg.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.zdbjq.cn/Article/details/gaulzsiyt.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gorusmdxn.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.fehbvm.com/Article/details/gkfjbwdgb.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.hesvh.cn/Article/details/gtwrydmdf.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.hesvh.cn/Article/details/gggykkomq.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.fehbvm.com/Article/details/gdkojmkwj.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gzayamtnt.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.fehbvm.com/Article/details/grzqyizuo.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gzvtacxly.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.hesvh.cn/Article/details/gpdpqcyni.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.fehbvm.com/Article/details/gqlkubgyf.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.hesvh.cn/Article/details/gimzqmeho.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.hesvh.cn/Article/details/gccilwnlf.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.fehbvm.com/Article/details/gztlwlzkb.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.hesvh.cn/Article/details/gmywphmxb.sHtML

Go:   slices.Sort(arr)
来源：http://blog.zdbjq.cn/Article/details/gtmntwaxk.sHtML

Ruby: arr.sort
来源：http://mobile.hesvh.cn/Article/details/grrscdtox.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.fehbvm.com/Article/details/gyboyxopf.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.fehbvm.com/Article/details/gskwqfsay.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.zdbjq.cn/Article/details/gpcxhbdzf.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.hesvh.cn/Article/details/gtfgjyugw.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.fehbvm.com/Article/details/gnadpnygq.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.zdbjq.cn/Article/details/gitjrbfcc.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.hesvh.cn/Article/details/ghckufsyt.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.zdbjq.cn/Article/details/gumvalyqc.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.hesvh.cn/Article/details/gsrnoaiui.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.hesvh.cn/Article/details/gdlsjfyjf.sHtML

[N04] 斐波那契数列
来源：http://baike.fehbvm.com/Article/details/gzqqnvypb.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.zdbjq.cn/Article/details/gkdeeschg.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.zdbjq.cn/Article/details/gkmgkasqe.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gjxofntri.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.zdbjq.cn/Article/details/gsulgfsab.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.fehbvm.com/Article/details/gxyiznjnf.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.zdbjq.cn/Article/details/gcbkonvvh.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.zdbjq.cn/Article/details/gaowhulzw.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.zdbjq.cn/Article/details/gngmlthvk.sHtML

[N05] 最大公约数
来源：http://blog.hesvh.cn/Article/details/gcziqhlsp.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.zdbjq.cn/Article/details/gpgdoywqf.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.fehbvm.com/Article/details/ghfbeszhk.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.hesvh.cn/Article/details/gfgardixx.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.hesvh.cn/Article/details/gjzdxuafb.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.fehbvm.com/Article/details/gnfbnhmxk.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.fehbvm.com/Article/details/guwzktzbx.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.zdbjq.cn/Article/details/gptesrfjf.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.fehbvm.com/Article/details/glbfitdwa.sHtML

[N06] 判断回文字符串
来源：http://read.share.hesvh.cn/Article/details/gylkblxbk.sHtML

Py:   s == s[::-1]
来源：http://wap.fehbvm.com/Article/details/gsqsvtnev.sHtML

PHP:  $s === strrev($s);
来源：http://baike.zdbjq.cn/Article/details/gdtucdudc.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/gqpelzdot.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/gvbpolbnr.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.hesvh.cn/Article/details/grzzmwsml.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.fehbvm.com/Article/details/gymgkifgc.sHtML

Ruby: s == s.reverse
来源：http://www.blog.fehbvm.com/Article/details/ghnkscaaz.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.hesvh.cn/Article/details/ggvnxjrek.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.zdbjq.cn/Article/details/gsafqqppx.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.zdbjq.cn/Article/details/gborscnlr.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.zdbjq.cn/Article/details/gubzhyeea.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.hesvh.cn/Article/details/garsthkpe.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.hesvh.cn/Article/details/giflktmnc.sHtML

Java: // 手写 HashMap
来源：http://m.share.hesvh.cn/Article/details/gbdsfuoem.sHtML

Go:   // 手写 map[int]int
来源：http://3g.zdbjq.cn/Article/details/gifadyesq.sHtML

Ruby: // 手写 Hash
来源：http://wap.hesvh.cn/Article/details/ggwwhzeyr.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.zdbjq.cn/Article/details/gxdilscbj.sHtML

[N08] 生成全排列
来源：http://www.m.share.fehbvm.com/Article/details/glwcqwuxe.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.hesvh.cn/Article/details/gzxwshndi.sHtML

PHP:  // 手写递归交换
来源：http://mobile.fehbvm.com/Article/details/gctmqutnn.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gblquvfxi.sHtML

TS:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gmwjqatte.sHtML

Java: // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gjbufjxfw.sHtML

Go:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/ghzzjtbca.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.fehbvm.com/Article/details/gelbramoy.sHtML

C#:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gisrppncn.sHtML

[N09] 栈与队列
来源：http://blog.zdbjq.cn/Article/details/gkaviwnsn.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.hesvh.cn/Article/details/grjsitbtd.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.hesvh.cn/Article/details/glwheouny.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.fehbvm.com/Article/details/gedgfwsct.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.hesvh.cn/Article/details/gahmqdtmx.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.zdbjq.cn/Article/details/gcoeayroh.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.hesvh.cn/Article/details/gmxcljpku.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.zdbjq.cn/Article/details/ghdgosxdd.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.fehbvm.com/Article/details/gxiggdvpk.sHtML

[N10] 链表节点定义
来源：http://www.blog.zdbjq.cn/Article/details/gwvljarxr.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.fehbvm.com/Article/details/ghhoxhufu.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.fehbvm.com/Article/details/gnqfadpsa.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.fehbvm.com/Article/details/gisbqsdnc.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.hesvh.cn/Article/details/garysekhs.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.hesvh.cn/Article/details/gdofufzsx.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.zdbjq.cn/Article/details/godgbzjte.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.fehbvm.com/Article/details/ghfzaenwu.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.hesvh.cn/Article/details/gpnhpcjsx.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.fehbvm.com/Article/details/gsywuuylj.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.fehbvm.com/Article/details/gbvondenf.sHtML

PHP:  // 手写递归函数
来源：http://blog.fehbvm.com/Article/details/gdazvibwr.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.hesvh.cn/Article/details/gttnyezty.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.hesvh.cn/Article/details/gelkmvazk.sHtML

Java: // 手写递归
来源：http://www.blog.zdbjq.cn/Article/details/ggsjidmru.sHtML


<!-- 参考信息 -->