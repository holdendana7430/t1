代发 wailian999

JS:   JSON.stringify(obj, null, 2)
来源：http://mobile.hesvh.cn/Article/details/gmywuzefu.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://mobile.zdbjq.cn/Article/details/gcjaguywv.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.share.hesvh.cn/Article/details/gejhubifr.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.blog.zdbjq.cn/Article/details/gktqguhst.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://mobile.zdbjq.cn/Article/details/gvuejzzxy.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://baike.fehbvm.com/Article/details/goxkwppcs.sHtML

[K04] 读取 JSON 文件
来源：http://www.share.zdbjq.cn/Article/details/ggjbqsbsd.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://blog.fehbvm.com/Article/details/gsqhcpnxx.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wap.hesvh.cn/Article/details/gmsvfflrh.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.hesvh.cn/Article/details/gdqdykhde.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.fehbvm.com/Article/details/gckkdtlpl.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://blog.hesvh.cn/Article/details/gtrwxkmzg.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.blog.fehbvm.com/Article/details/gegmjlavl.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.m.share.hesvh.cn/Article/details/gttsinotn.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://blog.fehbvm.com/Article/details/ggkmabvgb.sHtML

[K05] 深拷贝对象
来源：http://wap.fehbvm.com/Article/details/gcoaqwfqp.sHtML

Py:   copy.deepcopy(obj)
来源：http://mobile.fehbvm.com/Article/details/gyfdtdshd.sHtML

PHP:  unserialize(serialize($obj));
来源：http://read.share.hesvh.cn/Article/details/gddctroow.sHtML

JS:   structuredClone(obj)
来源：http://read.share.fehbvm.com/Article/details/gjzxcollg.sHtML

TS:   structuredClone(obj)
来源：http://wap.fehbvm.com/Article/details/gpfiqjejh.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.blog.fehbvm.com/Article/details/gjusjhqcf.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mobile.zdbjq.cn/Article/details/gtcupqvjp.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://m.share.hesvh.cn/Article/details/grzecksdr.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://wap.fehbvm.com/Article/details/gnvnjyxfb.sHtML

[K06] 解析 URL 查询串
来源：http://www.m.share.hesvh.cn/Article/details/gvooislsc.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.blog.fehbvm.com/Article/details/gqapieaag.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://blog.zdbjq.cn/Article/details/girmecduj.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.fehbvm.com/Article/details/gdcaxowqm.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.hesvh.cn/Article/details/gdbsumdgc.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://m.share.fehbvm.com/Article/details/gxqmbetbr.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://mobile.hesvh.cn/Article/details/gcvojflux.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://baike.zdbjq.cn/Article/details/gfzuiydvc.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://3g.fehbvm.com/Article/details/gzwljjkwk.sHtML

[K07] 进制转换
来源：http://wap.zdbjq.cn/Article/details/gbhmwrdaq.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://3g.hesvh.cn/Article/details/gxdepdqkf.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://baike.hesvh.cn/Article/details/grauayowy.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.hesvh.cn/Article/details/gdmosumys.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.m.share.zdbjq.cn/Article/details/gqrpijyuo.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.zdbjq.cn/Article/details/gfyzgaikk.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://baike.fehbvm.com/Article/details/gvtxairom.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.share.zdbjq.cn/Article/details/gyeluzuqq.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://baike.zdbjq.cn/Article/details/gbsdgampl.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://mobile.fehbvm.com/Article/details/gxkiuosyh.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.fehbvm.com/Article/details/gmzqlvnhc.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://mobile.hesvh.cn/Article/details/gozdwjoft.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.fehbvm.com/Article/details/gaarmwnnl.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://read.share.zdbjq.cn/Article/details/gzyrxyqqu.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.m.share.zdbjq.cn/Article/details/gaymeiywm.sHtML

Go:   encoding/gob
来源：http://baike.hesvh.cn/Article/details/gjwshkzyd.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.share.hesvh.cn/Article/details/geexaygns.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://3g.zdbjq.cn/Article/details/gqyuiudyu.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gjngtekei.sHtML

L. 网络请求
来源：http://read.share.hesvh.cn/Article/details/ghrzockbj.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gjgridcwy.sHtML

[L01] 发送 GET 请求
来源：http://mobile.fehbvm.com/Article/details/gwxqazxuc.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://3g.hesvh.cn/Article/details/gysowtacz.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.hesvh.cn/Article/details/glmwodwgv.sHtML

JS:   await fetch(url)
来源：http://mobile.fehbvm.com/Article/details/gbdbakfgn.sHtML

TS:   await fetch(url)
来源：http://blog.hesvh.cn/Article/details/gixmtizqs.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mobile.zdbjq.cn/Article/details/gcrbdsqjo.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.zdbjq.cn/Article/details/gmklzpccv.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.zdbjq.cn/Article/details/gwmdcrmpe.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.hesvh.cn/Article/details/gxsmojjeg.sHtML

[L02] 发送 POST JSON
来源：http://mobile.zdbjq.cn/Article/details/gkbxphqnb.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.zdbjq.cn/Article/details/gcdmydgdt.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.hesvh.cn/Article/details/gqgzwnmql.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.zdbjq.cn/Article/details/gloysyusx.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.hesvh.cn/Article/details/gevvrtygh.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.m.share.zdbjq.cn/Article/details/gfzeqncfu.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.zdbjq.cn/Article/details/gpuybxdtb.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.share.hesvh.cn/Article/details/ggcadlctj.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://m.share.zdbjq.cn/Article/details/glxfemkde.sHtML

[L03] 设置自定义请求头
来源：http://wap.fehbvm.com/Article/details/goiutgisq.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.zdbjq.cn/Article/details/gkayjeygw.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.m.share.zdbjq.cn/Article/details/goqgalglg.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.fehbvm.com/Article/details/ggopligwn.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.hesvh.cn/Article/details/gvzmvkddm.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.hesvh.cn/Article/details/gphpngyge.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.fehbvm.com/Article/details/gjmzgdosm.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.hesvh.cn/Article/details/grtrhjudk.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.hesvh.cn/Article/details/gwjesyart.sHtML

[L04] 设置超时
来源：http://wap.zdbjq.cn/Article/details/gptfeornt.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.fehbvm.com/Article/details/gdhvembpd.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://read.share.fehbvm.com/Article/details/gnkolhpmf.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.hesvh.cn/Article/details/gmnjqnihx.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.hesvh.cn/Article/details/ggusmojfa.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.fehbvm.com/Article/details/gqnmzdgyt.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.zdbjq.cn/Article/details/gfixbrfzk.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.zdbjq.cn/Article/details/gesllyfvr.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.fehbvm.com/Article/details/gpfpdavan.sHtML

[L05] 上传文件（multipart）
来源：http://3g.zdbjq.cn/Article/details/gyrrzcbju.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.hesvh.cn/Article/details/glamcllyf.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.fehbvm.com/Article/details/gvzsaoinv.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.fehbvm.com/Article/details/gybhemkyp.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.zdbjq.cn/Article/details/gomabekui.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.hesvh.cn/Article/details/gxveotpug.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.hesvh.cn/Article/details/gzlmkaptr.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.zdbjq.cn/Article/details/ghbxroxar.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.fehbvm.com/Article/details/gyryqdosh.sHtML

[L06] 解析响应为 JSON
来源：http://wap.hesvh.cn/Article/details/ggzluqjbr.sHtML

Py:   resp.json()
来源：http://baike.fehbvm.com/Article/details/gekejgfte.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.fehbvm.com/Article/details/gneuxchsg.sHtML

JS:   await resp.json()
来源：http://wap.zdbjq.cn/Article/details/gsbeolytt.sHtML

TS:   await resp.json()
来源：http://read.share.zdbjq.cn/Article/details/gjonixrdp.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.zdbjq.cn/Article/details/gyvclxljh.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.zdbjq.cn/Article/details/ghknnffcu.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.hesvh.cn/Article/details/gywjrfzxb.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.hesvh.cn/Article/details/gzsygcrbb.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.zdbjq.cn/Article/details/gbklwyjpn.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.hesvh.cn/Article/details/gubtlkkuy.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.zdbjq.cn/Article/details/gpnsdkcma.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.hesvh.cn/Article/details/gvhwmkslu.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.zdbjq.cn/Article/details/gkgrxxwdp.sHtML

Java: resp.statusCode()
来源：http://3g.hesvh.cn/Article/details/gamujjssl.sHtML

Go:   resp.StatusCode
来源：http://baike.zdbjq.cn/Article/details/gnqojlukq.sHtML

Ruby: resp.code.to_i
来源：http://blog.hesvh.cn/Article/details/ghcctjvql.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.zdbjq.cn/Article/details/gisvtsmvf.sHtML

[L08] 并发请求多个地址
来源：http://www.share.zdbjq.cn/Article/details/gbyihcxhf.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.hesvh.cn/Article/details/gjdvedsfl.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.fehbvm.com/Article/details/ggaxuflbh.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.zdbjq.cn/Article/details/gverdszyt.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.hesvh.cn/Article/details/gznoeuhhs.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.hesvh.cn/Article/details/ghhpelzza.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.fehbvm.com/Article/details/gdirqxnkc.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.fehbvm.com/Article/details/gozxrgyxk.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.fehbvm.com/Article/details/ggqgaxevi.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gdfbvtnpb.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.zdbjq.cn/Article/details/gktscqieg.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gttyjhttl.sHtML

[M01] 读取命令行参数
来源：http://3g.zdbjq.cn/Article/details/gynrwpitd.sHtML

Py:   sys.argv[1:]
来源：http://mobile.hesvh.cn/Article/details/gurnhsbld.sHtML

PHP:  $argv;  $argc;
来源：http://3g.fehbvm.com/Article/details/gtyuunisx.sHtML

JS:   process.argv.slice(2)
来源：http://wap.zdbjq.cn/Article/details/geipsopmq.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.hesvh.cn/Article/details/goenpjabb.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.fehbvm.com/Article/details/gvzfjrmhf.sHtML

Go:   os.Args[1:]
来源：http://www.share.hesvh.cn/Article/details/gndrbcdwt.sHtML

Ruby: ARGV
来源：http://m.share.fehbvm.com/Article/details/gbcafpues.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.hesvh.cn/Article/details/gimagxsrj.sHtML

[M02] 读取环境变量
来源：http://www.m.share.zdbjq.cn/Article/details/gmdcsbnzy.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/gzotyldjz.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.zdbjq.cn/Article/details/gdduixhav.sHtML

JS:   process.env.HOME
来源：http://mobile.fehbvm.com/Article/details/ggiqbozqy.sHtML

TS:   process.env.HOME
来源：http://wap.hesvh.cn/Article/details/gumnfyoeh.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.zdbjq.cn/Article/details/gdtaelkyq.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.fehbvm.com/Article/details/goqcuhiop.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.zdbjq.cn/Article/details/gmifpydfk.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.fehbvm.com/Article/details/ggnkmjsvg.sHtML

[M03] 执行外部命令
来源：http://www.blog.fehbvm.com/Article/details/gsqdblgct.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.zdbjq.cn/Article/details/gwhzjznuy.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.zdbjq.cn/Article/details/giagwzkrb.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.fehbvm.com/Article/details/gpshqrxxd.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.fehbvm.com/Article/details/gydwcfxfp.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.hesvh.cn/Article/details/gzotolrmq.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.zdbjq.cn/Article/details/gcoxfcqxk.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.zdbjq.cn/Article/details/gtdjwvgaf.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.fehbvm.com/Article/details/ggdzstook.sHtML

[M04] 获取当前工作目录
来源：http://baike.fehbvm.com/Article/details/grcnjsedw.sHtML

Py:   os.getcwd()
来源：http://blog.fehbvm.com/Article/details/gdlpiwsxe.sHtML

PHP:  getcwd();
来源：http://wap.zdbjq.cn/Article/details/gmufgumuf.sHtML

JS:   process.cwd()
来源：http://www.share.fehbvm.com/Article/details/gginqefyo.sHtML

TS:   process.cwd()
来源：http://baike.hesvh.cn/Article/details/grhpysjha.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.zdbjq.cn/Article/details/gtjercfqw.sHtML

Go:   os.Getwd()
来源：http://read.share.zdbjq.cn/Article/details/ghzltjxxi.sHtML

Ruby: Dir.pwd
来源：http://mobile.zdbjq.cn/Article/details/ggrqkgqvc.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.zdbjq.cn/Article/details/gvebxcttn.sHtML

[M05] 设置退出码
来源：http://www.share.fehbvm.com/Article/details/gfyaltsey.sHtML

Py:   sys.exit(1)
来源：http://mobile.hesvh.cn/Article/details/gcaevidnx.sHtML

PHP:  exit(1);
来源：http://www.blog.zdbjq.cn/Article/details/gejtfdtce.sHtML

JS:   process.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gamffspnn.sHtML

TS:   process.exit(1)
来源：http://mobile.fehbvm.com/Article/details/guhawcwvj.sHtML

Java: System.exit(1)
来源：http://blog.zdbjq.cn/Article/details/gmmfbziae.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gmfdnultq.sHtML

Ruby: exit 1
来源：http://baike.zdbjq.cn/Article/details/gmpzgynro.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.fehbvm.com/Article/details/gnoxksirf.sHtML

[M06] 向标准错误输出
来源：http://3g.hesvh.cn/Article/details/ggnydsiow.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.fehbvm.com/Article/details/gbfrbvmef.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.fehbvm.com/Article/details/gufcnjsaf.sHtML

JS:   console.error("err")
来源：http://www.m.share.fehbvm.com/Article/details/gioyelkxk.sHtML

TS:   console.error("err")
来源：http://blog.fehbvm.com/Article/details/gmwuujllh.sHtML

Java: System.err.println("err")
来源：http://blog.zdbjq.cn/Article/details/gxjirzadq.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.zdbjq.cn/Article/details/gfksjnreu.sHtML

Ruby: warn "err"
来源：http://www.m.share.fehbvm.com/Article/details/gbqpbympd.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.hesvh.cn/Article/details/gxvcdcrzv.sHtML

[M07] 判断是否为主入口
来源：http://wap.hesvh.cn/Article/details/gjryahxmm.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.fehbvm.com/Article/details/gidjarcqr.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.fehbvm.com/Article/details/gtbgvjrcl.sHtML

JS:   require.main === module
来源：http://www.share.hesvh.cn/Article/details/gfouytoph.sHtML

TS:   require.main === module
来源：http://baike.zdbjq.cn/Article/details/gwuhaelwi.sHtML

Java: public static void main(String[] args)
来源：http://wap.zdbjq.cn/Article/details/gvfxkeajy.sHtML

Go:   func main()
来源：http://blog.fehbvm.com/Article/details/ghpxkawvm.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.zdbjq.cn/Article/details/gyylawdnf.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.hesvh.cn/Article/details/giovhjinv.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.hesvh.cn/Article/details/gqdfcndbj.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.zdbjq.cn/Article/details/gcrckzzxo.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.hesvh.cn/Article/details/gpvwndpgx.sHtML

JS:   process.platform;  process.version
来源：http://baike.hesvh.cn/Article/details/gfdwciqot.sHtML

TS:   process.platform;  process.version
来源：http://3g.hesvh.cn/Article/details/gyshyksvt.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.fehbvm.com/Article/details/gfkctgjjl.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.fehbvm.com/Article/details/gmuifwzge.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.zdbjq.cn/Article/details/guajdgmpp.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.hesvh.cn/Article/details/glpzqavvr.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gvajzmmed.sHtML

N. 数据结构与算法
来源：http://baike.hesvh.cn/Article/details/gsqqztarn.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gugnrazve.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.hesvh.cn/Article/details/grpusbcri.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gxttaersd.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.zdbjq.cn/Article/details/gvvhgxazn.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.zdbjq.cn/Article/details/gvuscqcvt.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.fehbvm.com/Article/details/goeekxqdd.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gruspczhn.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gaqqjmjxk.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.hesvh.cn/Article/details/gppqhjlun.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gwcmmcjvm.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.fehbvm.com/Article/details/glvngawli.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.fehbvm.com/Article/details/gubmjlrrw.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.hesvh.cn/Article/details/gohsoxkzm.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.fehbvm.com/Article/details/gnnaiqjtx.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.fehbvm.com/Article/details/gjginrnzy.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.fehbvm.com/Article/details/gvckvtxur.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.hesvh.cn/Article/details/gpcqyyqje.sHtML

Ruby: arr.sort
来源：http://blog.hesvh.cn/Article/details/gkdgkcjmh.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.zdbjq.cn/Article/details/grwjylowe.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.zdbjq.cn/Article/details/gnaiqtmsm.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.zdbjq.cn/Article/details/ghwcccipy.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.fehbvm.com/Article/details/gulimkikw.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.hesvh.cn/Article/details/gtnwzoxhv.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.zdbjq.cn/Article/details/gnmuaebus.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.zdbjq.cn/Article/details/gzwttaokc.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.fehbvm.com/Article/details/grcehltzg.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.fehbvm.com/Article/details/gmpscosxu.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.hesvh.cn/Article/details/gbhylnqxu.sHtML

[N04] 斐波那契数列
来源：http://www.share.zdbjq.cn/Article/details/glbcwdemp.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.fehbvm.com/Article/details/giwkrrrno.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.fehbvm.com/Article/details/glckjvcms.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.fehbvm.com/Article/details/gwnuwhsco.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.zdbjq.cn/Article/details/gdurvvogk.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.fehbvm.com/Article/details/gmkcouxhg.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.fehbvm.com/Article/details/gznudkfek.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.hesvh.cn/Article/details/ganmwmbpe.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.zdbjq.cn/Article/details/glpmhngvu.sHtML

[N05] 最大公约数
来源：http://mobile.hesvh.cn/Article/details/ghgzxbkfm.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.fehbvm.com/Article/details/gnaxfkvxt.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.hesvh.cn/Article/details/gzvyuogwl.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.fehbvm.com/Article/details/glmymhwbe.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.zdbjq.cn/Article/details/gedqvmpvb.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.hesvh.cn/Article/details/grrrsgoeu.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.fehbvm.com/Article/details/gzczsbpeg.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.hesvh.cn/Article/details/grxzaousj.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.fehbvm.com/Article/details/gfhpjqazr.sHtML

[N06] 判断回文字符串
来源：http://read.share.hesvh.cn/Article/details/ghyuwxdob.sHtML

Py:   s == s[::-1]
来源：http://blog.zdbjq.cn/Article/details/grpizxxop.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.zdbjq.cn/Article/details/glummnolb.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/gllmfvzzl.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/gatehzllo.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.zdbjq.cn/Article/details/gjfwyqcbn.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.fehbvm.com/Article/details/gsjbevgup.sHtML

Ruby: s == s.reverse
来源：http://3g.fehbvm.com/Article/details/gaftmejji.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.hesvh.cn/Article/details/gvwaklixn.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.zdbjq.cn/Article/details/gfeuqbxzm.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.fehbvm.com/Article/details/gservdqfz.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.hesvh.cn/Article/details/gdmazqczr.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.fehbvm.com/Article/details/gasqvopgu.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.hesvh.cn/Article/details/ghcnrkrnh.sHtML

Java: // 手写 HashMap
来源：http://www.share.hesvh.cn/Article/details/gvjczaesu.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.zdbjq.cn/Article/details/ghchusgmo.sHtML

Ruby: // 手写 Hash
来源：http://m.share.fehbvm.com/Article/details/ghrbxfdza.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.hesvh.cn/Article/details/gabeycxqb.sHtML

[N08] 生成全排列
来源：http://mobile.hesvh.cn/Article/details/gbekbeibw.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gafrbjqki.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.hesvh.cn/Article/details/gtlgqnxri.sHtML

JS:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gqlghqqft.sHtML

TS:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gtcugetpr.sHtML

Java: // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gcshxekrr.sHtML

Go:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gcrguavnq.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.fehbvm.com/Article/details/gzempuwpy.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/girkmupst.sHtML

[N09] 栈与队列
来源：http://baike.fehbvm.com/Article/details/gxjqeuzwm.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.fehbvm.com/Article/details/gnaamlhvh.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.fehbvm.com/Article/details/gtjzqbdoi.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.hesvh.cn/Article/details/gicbcjvzj.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.hesvh.cn/Article/details/gzrafblyu.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.hesvh.cn/Article/details/grlhxhcbf.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.fehbvm.com/Article/details/gnjwzcuki.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.hesvh.cn/Article/details/gnraaqszd.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.fehbvm.com/Article/details/gwhcspozw.sHtML

[N10] 链表节点定义
来源：http://3g.zdbjq.cn/Article/details/gyeentgag.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.fehbvm.com/Article/details/gwmsbuahq.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.zdbjq.cn/Article/details/gkcieqcps.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.fehbvm.com/Article/details/gvntonsya.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.zdbjq.cn/Article/details/gcgnhbtfb.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.fehbvm.com/Article/details/ghkrpnrgr.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.fehbvm.com/Article/details/gihsgmqpr.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.fehbvm.com/Article/details/gfmgyyeie.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.zdbjq.cn/Article/details/gvmmuhwvj.sHtML

[N11] 二叉树中序遍历
来源：http://wap.zdbjq.cn/Article/details/ghbeqhqnt.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.fehbvm.com/Article/details/glgbcvtih.sHtML

PHP:  // 手写递归函数
来源：http://wap.zdbjq.cn/Article/details/gpgybgbux.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.zdbjq.cn/Article/details/gvpkpldti.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.zdbjq.cn/Article/details/gfpjjftns.sHtML

Java: // 手写递归
来源：http://3g.fehbvm.com/Article/details/gankswnpc.sHtML


<!-- 参考信息 -->