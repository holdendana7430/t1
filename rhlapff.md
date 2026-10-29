代发 wailian999

TS:   JSON.parse(s)
来源：http://mobile.fehbvm.com/Article/details/gnlakpnez.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://read.share.fehbvm.com/Article/details/gwmxfduyz.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.blog.zdbjq.cn/Article/details/glichgpsx.sHtML

Ruby: JSON.parse(s)
来源：http://www.blog.zdbjq.cn/Article/details/gaovwlktj.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mobile.zdbjq.cn/Article/details/grcvdfrec.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.m.share.zdbjq.cn/Article/details/gbinchatx.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://m.share.hesvh.cn/Article/details/gljzvrnma.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.fehbvm.com/Article/details/grcqxiwlb.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://wap.hesvh.cn/Article/details/glqvlzguq.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://blog.hesvh.cn/Article/details/gcfpmixer.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gazpmxzai.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://3g.zdbjq.cn/Article/details/giebsfmwo.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gdsfdcpcz.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://m.share.fehbvm.com/Article/details/grhcbmzed.sHtML

[K04] 读取 JSON 文件
来源：http://m.share.zdbjq.cn/Article/details/gdedywxkf.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.fehbvm.com/Article/details/gxjkuiktr.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mobile.fehbvm.com/Article/details/gupcekocl.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.fehbvm.com/Article/details/gegvnfjkn.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.hesvh.cn/Article/details/gwdwwhwks.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wap.fehbvm.com/Article/details/giwojytbb.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://baike.hesvh.cn/Article/details/gmbgwkbtc.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://blog.hesvh.cn/Article/details/gdagwtznl.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mobile.fehbvm.com/Article/details/gkbfioryg.sHtML

[K05] 深拷贝对象
来源：http://3g.hesvh.cn/Article/details/gmjbbhaxm.sHtML

Py:   copy.deepcopy(obj)
来源：http://baike.zdbjq.cn/Article/details/guifjdbio.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.zdbjq.cn/Article/details/gkazbcpqn.sHtML

JS:   structuredClone(obj)
来源：http://baike.hesvh.cn/Article/details/ggmkhlkjc.sHtML

TS:   structuredClone(obj)
来源：http://www.share.fehbvm.com/Article/details/glsihpiyy.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.share.zdbjq.cn/Article/details/gkfaodpwo.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mobile.hesvh.cn/Article/details/guxiaqkeu.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.share.hesvh.cn/Article/details/gxtwjfkgn.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://m.share.fehbvm.com/Article/details/gkbghpfpo.sHtML

[K06] 解析 URL 查询串
来源：http://3g.zdbjq.cn/Article/details/gqfvxchyw.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://3g.hesvh.cn/Article/details/gmatjnyjd.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://3g.zdbjq.cn/Article/details/gclxicygy.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.zdbjq.cn/Article/details/gkeichvuc.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.zdbjq.cn/Article/details/ggmhsuuyc.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://blog.fehbvm.com/Article/details/gfgrfvebf.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://mobile.hesvh.cn/Article/details/gqqsatdgt.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wap.zdbjq.cn/Article/details/gcbiftdcq.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.hesvh.cn/Article/details/gtkehnnar.sHtML

[K07] 进制转换
来源：http://www.m.share.fehbvm.com/Article/details/gxyvlnilj.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.hesvh.cn/Article/details/gkgrxwomv.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mobile.zdbjq.cn/Article/details/gfooynzxm.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.zdbjq.cn/Article/details/gbdjzzkyq.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wap.hesvh.cn/Article/details/grfripmii.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.hesvh.cn/Article/details/gtogzculm.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wap.fehbvm.com/Article/details/gphyuqjbp.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://3g.hesvh.cn/Article/details/gglnxcbne.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.share.zdbjq.cn/Article/details/gmdeqlcgy.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://wap.zdbjq.cn/Article/details/gtsemgvdj.sHtML

Py:   pickle.dumps(obj)
来源：http://baike.hesvh.cn/Article/details/ghlaxaiwk.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.share.fehbvm.com/Article/details/gwiogjgqy.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.hesvh.cn/Article/details/gwgkagiqv.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.fehbvm.com/Article/details/gotdushkn.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.m.share.zdbjq.cn/Article/details/gfsrhlcof.sHtML

Go:   encoding/gob
来源：http://www.m.share.hesvh.cn/Article/details/gbkiibusx.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gatvwdzbr.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.hesvh.cn/Article/details/gkxlnehvq.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gkodzchmy.sHtML

L. 网络请求
来源：http://3g.zdbjq.cn/Article/details/gzvojwybs.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gyzklsiah.sHtML

[L01] 发送 GET 请求
来源：http://blog.fehbvm.com/Article/details/gpmekrqwo.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://blog.zdbjq.cn/Article/details/gndairnhl.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.m.share.hesvh.cn/Article/details/gssmfjgyl.sHtML

JS:   await fetch(url)
来源：http://read.share.fehbvm.com/Article/details/gibtwhbfr.sHtML

TS:   await fetch(url)
来源：http://baike.hesvh.cn/Article/details/gizjmmvpl.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.hesvh.cn/Article/details/gmvnymhts.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.fehbvm.com/Article/details/gvrykvure.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.fehbvm.com/Article/details/gfwbkhaac.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.blog.fehbvm.com/Article/details/ghneneyhz.sHtML

[L02] 发送 POST JSON
来源：http://baike.fehbvm.com/Article/details/gfubhijkb.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.blog.hesvh.cn/Article/details/gxpnytpiy.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://m.share.zdbjq.cn/Article/details/gotcitagt.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.zdbjq.cn/Article/details/gthqwjppv.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.hesvh.cn/Article/details/goouahmfw.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://read.share.fehbvm.com/Article/details/gumqddocg.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.zdbjq.cn/Article/details/gsbvozled.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.hesvh.cn/Article/details/guqesxwlw.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.hesvh.cn/Article/details/gonekoocl.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.zdbjq.cn/Article/details/gwulnorhs.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wap.hesvh.cn/Article/details/gzggsinwp.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.zdbjq.cn/Article/details/gpvfxakaa.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.fehbvm.com/Article/details/grkekhusv.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.hesvh.cn/Article/details/gfirdpugj.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.hesvh.cn/Article/details/gavzbtspa.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.hesvh.cn/Article/details/gxxlypvcr.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.zdbjq.cn/Article/details/gdmkwlngy.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.m.share.zdbjq.cn/Article/details/gdeqaswzb.sHtML

[L04] 设置超时
来源：http://www.share.hesvh.cn/Article/details/gktwpnrqn.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.fehbvm.com/Article/details/grbxesovg.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.zdbjq.cn/Article/details/gsllhykwk.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.zdbjq.cn/Article/details/gxdelsifu.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.fehbvm.com/Article/details/gibgeqcre.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.hesvh.cn/Article/details/gvlshhvdb.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.zdbjq.cn/Article/details/gmdlpjchx.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.zdbjq.cn/Article/details/gzhblbqkv.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.zdbjq.cn/Article/details/gmfiwukdu.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.hesvh.cn/Article/details/gaimaxanx.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.hesvh.cn/Article/details/gdsqwmlig.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.zdbjq.cn/Article/details/gtkbrdhue.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.hesvh.cn/Article/details/geurksdxf.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.hesvh.cn/Article/details/gxxuzphvz.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.hesvh.cn/Article/details/glfhseewc.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.fehbvm.com/Article/details/gfawntmob.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.zdbjq.cn/Article/details/gojacmggk.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.zdbjq.cn/Article/details/gpyfsdxfo.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.fehbvm.com/Article/details/gviiwktee.sHtML

Py:   resp.json()
来源：http://wap.fehbvm.com/Article/details/gwqwmudkl.sHtML

PHP:  json_decode($body, true);
来源：http://blog.hesvh.cn/Article/details/gghaokrnk.sHtML

JS:   await resp.json()
来源：http://mobile.zdbjq.cn/Article/details/gdecngtka.sHtML

TS:   await resp.json()
来源：http://www.blog.zdbjq.cn/Article/details/gqleyvyrk.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.fehbvm.com/Article/details/gfvurgtwm.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.fehbvm.com/Article/details/gljstuvbc.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.hesvh.cn/Article/details/gplwjdtit.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.fehbvm.com/Article/details/gdluclmtx.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.zdbjq.cn/Article/details/gdnzbhyhd.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.hesvh.cn/Article/details/gcltnwpzc.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.fehbvm.com/Article/details/gurbcltsz.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.zdbjq.cn/Article/details/gmuflzyat.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.hesvh.cn/Article/details/gcciirjdc.sHtML

Java: resp.statusCode()
来源：http://www.m.share.fehbvm.com/Article/details/gwantogax.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.fehbvm.com/Article/details/gpirqbxni.sHtML

Ruby: resp.code.to_i
来源：http://baike.hesvh.cn/Article/details/gstuqsptx.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.zdbjq.cn/Article/details/gmldprwke.sHtML

[L08] 并发请求多个地址
来源：http://mobile.zdbjq.cn/Article/details/ggnpvgxsr.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.hesvh.cn/Article/details/gzkirxkvu.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.zdbjq.cn/Article/details/gjngmejtz.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.zdbjq.cn/Article/details/gvyvzzliu.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.zdbjq.cn/Article/details/gfzdikxmk.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.zdbjq.cn/Article/details/gqdrfowwn.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.fehbvm.com/Article/details/gzfazayek.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.fehbvm.com/Article/details/gfgeqzlsp.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.zdbjq.cn/Article/details/gpflqeoel.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gbyukjsqx.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.fehbvm.com/Article/details/gvzdshwpn.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gjtkvnoxy.sHtML

[M01] 读取命令行参数
来源：http://wap.fehbvm.com/Article/details/gllcnhnct.sHtML

Py:   sys.argv[1:]
来源：http://m.share.fehbvm.com/Article/details/gkwuydhbw.sHtML

PHP:  $argv;  $argc;
来源：http://blog.zdbjq.cn/Article/details/gaexefenx.sHtML

JS:   process.argv.slice(2)
来源：http://blog.hesvh.cn/Article/details/gnejofgko.sHtML

TS:   process.argv.slice(2)
来源：http://wap.zdbjq.cn/Article/details/gojodiiaw.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.fehbvm.com/Article/details/geecguekl.sHtML

Go:   os.Args[1:]
来源：http://blog.fehbvm.com/Article/details/gmqzakpxp.sHtML

Ruby: ARGV
来源：http://wap.fehbvm.com/Article/details/grjgjhpdk.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.zdbjq.cn/Article/details/gnnouobfg.sHtML

[M02] 读取环境变量
来源：http://m.share.fehbvm.com/Article/details/gpidtnyjn.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.hesvh.cn/Article/details/gmlwvfdks.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.fehbvm.com/Article/details/gfnurlfcn.sHtML

JS:   process.env.HOME
来源：http://baike.zdbjq.cn/Article/details/gxuveucas.sHtML

TS:   process.env.HOME
来源：http://read.share.hesvh.cn/Article/details/ggbqgzshe.sHtML

Java: System.getenv("HOME")
来源：http://wap.zdbjq.cn/Article/details/gpdhhmioi.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/gxqfnjumg.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.hesvh.cn/Article/details/ggwwaoyoj.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.hesvh.cn/Article/details/gzxztairj.sHtML

[M03] 执行外部命令
来源：http://www.m.share.zdbjq.cn/Article/details/gvkogbomi.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.zdbjq.cn/Article/details/gqronylry.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.zdbjq.cn/Article/details/guwgljlkz.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.fehbvm.com/Article/details/gyicphikh.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.hesvh.cn/Article/details/gbagazodc.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.fehbvm.com/Article/details/ghforqxpw.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.fehbvm.com/Article/details/gfyawldfq.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.zdbjq.cn/Article/details/gdngzckpg.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.hesvh.cn/Article/details/gydvpkdwz.sHtML

[M04] 获取当前工作目录
来源：http://3g.fehbvm.com/Article/details/gdvzsbqax.sHtML

Py:   os.getcwd()
来源：http://read.share.hesvh.cn/Article/details/gemkmsdpu.sHtML

PHP:  getcwd();
来源：http://www.share.fehbvm.com/Article/details/gpqxckfkv.sHtML

JS:   process.cwd()
来源：http://mobile.hesvh.cn/Article/details/gzciwcrlo.sHtML

TS:   process.cwd()
来源：http://wap.zdbjq.cn/Article/details/gjttkxrpl.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.zdbjq.cn/Article/details/gkhnfbama.sHtML

Go:   os.Getwd()
来源：http://blog.hesvh.cn/Article/details/guwakelfe.sHtML

Ruby: Dir.pwd
来源：http://wap.hesvh.cn/Article/details/gweuwcdso.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.hesvh.cn/Article/details/gibogdpxv.sHtML

[M05] 设置退出码
来源：http://3g.hesvh.cn/Article/details/gqabdirgi.sHtML

Py:   sys.exit(1)
来源：http://wap.zdbjq.cn/Article/details/gdlryvfys.sHtML

PHP:  exit(1);
来源：http://www.share.hesvh.cn/Article/details/gqsmfxbkp.sHtML

JS:   process.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gpajzuakz.sHtML

TS:   process.exit(1)
来源：http://read.share.hesvh.cn/Article/details/gkjvrfmul.sHtML

Java: System.exit(1)
来源：http://mobile.hesvh.cn/Article/details/gxrnzwldq.sHtML

Go:   os.Exit(1)
来源：http://baike.fehbvm.com/Article/details/gwbqqnaqk.sHtML

Ruby: exit 1
来源：http://www.m.share.zdbjq.cn/Article/details/gasmeqjqj.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.fehbvm.com/Article/details/gdqzwubij.sHtML

[M06] 向标准错误输出
来源：http://3g.hesvh.cn/Article/details/gnsevaxbv.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.zdbjq.cn/Article/details/gaiczqdcw.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.zdbjq.cn/Article/details/gtblfzrao.sHtML

JS:   console.error("err")
来源：http://baike.zdbjq.cn/Article/details/gwwljnecc.sHtML

TS:   console.error("err")
来源：http://www.share.zdbjq.cn/Article/details/guitpuqaj.sHtML

Java: System.err.println("err")
来源：http://blog.fehbvm.com/Article/details/gvoiqyiwh.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.zdbjq.cn/Article/details/geqtwexgs.sHtML

Ruby: warn "err"
来源：http://baike.fehbvm.com/Article/details/gfbtqngjw.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.hesvh.cn/Article/details/gpuevkvlu.sHtML

[M07] 判断是否为主入口
来源：http://www.share.zdbjq.cn/Article/details/gncgbsoqf.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.fehbvm.com/Article/details/geikqvaew.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.fehbvm.com/Article/details/gedtvlqgs.sHtML

JS:   require.main === module
来源：http://read.share.hesvh.cn/Article/details/gtnweuany.sHtML

TS:   require.main === module
来源：http://blog.fehbvm.com/Article/details/gucguebax.sHtML

Java: public static void main(String[] args)
来源：http://m.share.fehbvm.com/Article/details/gpnxsurwx.sHtML

Go:   func main()
来源：http://blog.hesvh.cn/Article/details/gdgehadml.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.zdbjq.cn/Article/details/gxvrprvyp.sHtML

C#:   static void Main(string[] args)
来源：http://wap.hesvh.cn/Article/details/gkuhgnhjq.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.zdbjq.cn/Article/details/ghnuhgixy.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.zdbjq.cn/Article/details/gwggaffgf.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.fehbvm.com/Article/details/glmcyeeba.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.hesvh.cn/Article/details/gezvyrdug.sHtML

TS:   process.platform;  process.version
来源：http://baike.hesvh.cn/Article/details/geaeymdvz.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.hesvh.cn/Article/details/gcphacdvr.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.fehbvm.com/Article/details/gcoxhjvar.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.zdbjq.cn/Article/details/ggakhloyd.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.zdbjq.cn/Article/details/gjltqlcjw.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gfypvqygs.sHtML

N. 数据结构与算法
来源：http://baike.zdbjq.cn/Article/details/gpztysfty.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gciomfiei.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.zdbjq.cn/Article/details/ggslpsxoz.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.fehbvm.com/Article/details/gyzzajlug.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.fehbvm.com/Article/details/gsanthhsy.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.zdbjq.cn/Article/details/gnezhnltk.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.hesvh.cn/Article/details/gnxbsjjah.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gotseghjb.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.fehbvm.com/Article/details/grdatnvdk.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.fehbvm.com/Article/details/gewmkomoz.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.fehbvm.com/Article/details/gumdqkqyu.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.hesvh.cn/Article/details/gzrcumere.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.fehbvm.com/Article/details/gfwzcmusw.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.zdbjq.cn/Article/details/gdrjxitmy.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.zdbjq.cn/Article/details/gphxabeod.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.zdbjq.cn/Article/details/gdzglwmjj.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.hesvh.cn/Article/details/gqckjwhxv.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.fehbvm.com/Article/details/gkfefkypq.sHtML

Ruby: arr.sort
来源：http://baike.hesvh.cn/Article/details/gxwszimfn.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.hesvh.cn/Article/details/ggqhajfja.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.fehbvm.com/Article/details/gwvoalqxu.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.hesvh.cn/Article/details/gcatoejjw.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.hesvh.cn/Article/details/ggcrptrjt.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.hesvh.cn/Article/details/gpqjkmsdh.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.hesvh.cn/Article/details/girjmyetx.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.hesvh.cn/Article/details/gcrleotuq.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.hesvh.cn/Article/details/gpaomctlf.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.fehbvm.com/Article/details/gtwiwucnu.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.fehbvm.com/Article/details/gmuadxkha.sHtML

[N04] 斐波那契数列
来源：http://baike.fehbvm.com/Article/details/gmntvdtmr.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.hesvh.cn/Article/details/geurhmaqg.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.fehbvm.com/Article/details/gnccjegzs.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.zdbjq.cn/Article/details/gxvlwjoso.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.hesvh.cn/Article/details/gshgizyxs.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.hesvh.cn/Article/details/ggxotdupz.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.zdbjq.cn/Article/details/gwaytbbem.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.hesvh.cn/Article/details/gospmjzjl.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.hesvh.cn/Article/details/gwfbodyoi.sHtML

[N05] 最大公约数
来源：http://mobile.zdbjq.cn/Article/details/gfjejfnus.sHtML

Py:   math.gcd(a, b)
来源：http://wap.fehbvm.com/Article/details/gzcxddhbn.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.hesvh.cn/Article/details/gzsajgani.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.fehbvm.com/Article/details/ghkuhvyzo.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.zdbjq.cn/Article/details/ginmlubnj.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.hesvh.cn/Article/details/gyyerpogg.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.zdbjq.cn/Article/details/gxmxsjzep.sHtML

Ruby: a.gcd(b)
来源：http://www.share.hesvh.cn/Article/details/gjwwrvzjg.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.hesvh.cn/Article/details/guhxcojhk.sHtML

[N06] 判断回文字符串
来源：http://3g.fehbvm.com/Article/details/gpniglqiz.sHtML

Py:   s == s[::-1]
来源：http://baike.hesvh.cn/Article/details/gmemjjwic.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.hesvh.cn/Article/details/gfmdfmftp.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.zdbjq.cn/Article/details/gdhmzevro.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/gsvxuexop.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.zdbjq.cn/Article/details/gywzvvnmb.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.hesvh.cn/Article/details/gdgjidelb.sHtML

Ruby: s == s.reverse
来源：http://mobile.fehbvm.com/Article/details/ghcwumrwg.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.hesvh.cn/Article/details/gzhdmxvfa.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.hesvh.cn/Article/details/gpvcrlvez.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.fehbvm.com/Article/details/guqwhyxst.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.hesvh.cn/Article/details/gfjbvlqjd.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.fehbvm.com/Article/details/gmssvnngh.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.zdbjq.cn/Article/details/gbmtptzts.sHtML

Java: // 手写 HashMap
来源：http://read.share.fehbvm.com/Article/details/gojqtbbdj.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.zdbjq.cn/Article/details/gnkdqsfec.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.fehbvm.com/Article/details/gdgqriszv.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.fehbvm.com/Article/details/goagqpfwn.sHtML

[N08] 生成全排列
来源：http://www.blog.fehbvm.com/Article/details/godfqwwqn.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.zdbjq.cn/Article/details/givzusjjh.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.zdbjq.cn/Article/details/gspklufir.sHtML

JS:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gkxcbmfsi.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gecmwjvzz.sHtML

Java: // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/grlcgcjae.sHtML

Go:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gksrnmgcm.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.hesvh.cn/Article/details/giqqsffct.sHtML

C#:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/godznxrfw.sHtML

[N09] 栈与队列
来源：http://read.share.hesvh.cn/Article/details/gudfwtppl.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.zdbjq.cn/Article/details/gfshnnrag.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.hesvh.cn/Article/details/gdwtnnbbs.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.hesvh.cn/Article/details/gqrmxjijh.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.hesvh.cn/Article/details/gmclcxgeb.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.zdbjq.cn/Article/details/gbksmyldp.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.zdbjq.cn/Article/details/gtnfakleo.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.hesvh.cn/Article/details/gfvhpmfrn.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.hesvh.cn/Article/details/gpbiyonpg.sHtML

[N10] 链表节点定义
来源：http://www.share.zdbjq.cn/Article/details/gjqeokpbp.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.zdbjq.cn/Article/details/gkpxvngkg.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.zdbjq.cn/Article/details/gdmrbyixz.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.hesvh.cn/Article/details/gmnixwxwt.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.fehbvm.com/Article/details/gvvozrgvl.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.zdbjq.cn/Article/details/gqsinnhjf.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.zdbjq.cn/Article/details/gzjlgtfgj.sHtML


<!-- 参考信息 -->