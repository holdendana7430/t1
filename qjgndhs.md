代发 wailian999

TS:   JSON.parse(s)
来源：http://wap.zdbjq.cn/Article/details/ggtujjrdt.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wap.hesvh.cn/Article/details/gzmswgkyu.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.m.share.zdbjq.cn/Article/details/gfsdvobjr.sHtML

Ruby: JSON.parse(s)
来源：http://3g.zdbjq.cn/Article/details/gfohmfmdh.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://blog.zdbjq.cn/Article/details/ghyeuldhd.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.blog.zdbjq.cn/Article/details/ghulnnmga.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mobile.zdbjq.cn/Article/details/gijenztpp.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://blog.hesvh.cn/Article/details/gahmudmrg.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.fehbvm.com/Article/details/gflzmqohc.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://baike.hesvh.cn/Article/details/goxphieap.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://read.share.hesvh.cn/Article/details/gcgdgajbn.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wap.zdbjq.cn/Article/details/gcdwkdehl.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://m.share.zdbjq.cn/Article/details/gtnqoyhqs.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://baike.zdbjq.cn/Article/details/giplysufe.sHtML

[K04] 读取 JSON 文件
来源：http://read.share.zdbjq.cn/Article/details/gitkkgcgq.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://read.share.hesvh.cn/Article/details/gbxyvpwxn.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.share.fehbvm.com/Article/details/ghxqonpzq.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.hesvh.cn/Article/details/gfdfgvbod.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.zdbjq.cn/Article/details/gtxxrboci.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://m.share.fehbvm.com/Article/details/gkvsxwlfp.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://baike.fehbvm.com/Article/details/gipdjiyjl.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://3g.zdbjq.cn/Article/details/giouabmdf.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://blog.fehbvm.com/Article/details/gaqllvnun.sHtML

[K05] 深拷贝对象
来源：http://3g.hesvh.cn/Article/details/gzrznlnkn.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gsoebeuho.sHtML

PHP:  unserialize(serialize($obj));
来源：http://mobile.fehbvm.com/Article/details/gqyusgaid.sHtML

JS:   structuredClone(obj)
来源：http://read.share.fehbvm.com/Article/details/gtmpcsuqe.sHtML

TS:   structuredClone(obj)
来源：http://m.share.fehbvm.com/Article/details/gxyexcgza.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.hesvh.cn/Article/details/gjqniopes.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.m.share.hesvh.cn/Article/details/giaornvfd.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://blog.fehbvm.com/Article/details/gjjmllkyo.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://read.share.hesvh.cn/Article/details/gdvhgbwme.sHtML

[K06] 解析 URL 查询串
来源：http://read.share.hesvh.cn/Article/details/gkrduoyje.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://m.share.fehbvm.com/Article/details/gpkrvchtc.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.m.share.zdbjq.cn/Article/details/ghnomatqx.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.zdbjq.cn/Article/details/glskbumdt.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.zdbjq.cn/Article/details/gnsgivzaa.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.zdbjq.cn/Article/details/glfftdnwd.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.blog.hesvh.cn/Article/details/gcbwhivmf.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.zdbjq.cn/Article/details/gkpgutxdt.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://baike.zdbjq.cn/Article/details/gtyohyrit.sHtML

[K07] 进制转换
来源：http://wap.fehbvm.com/Article/details/gmehqlzrs.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://m.share.fehbvm.com/Article/details/gmowzvbxz.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://baike.fehbvm.com/Article/details/gcwvzyphv.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.fehbvm.com/Article/details/gcveikykr.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://3g.zdbjq.cn/Article/details/gqdeeigbl.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://read.share.zdbjq.cn/Article/details/govalsqte.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://baike.hesvh.cn/Article/details/gyteavthv.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.zdbjq.cn/Article/details/getfelizk.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.hesvh.cn/Article/details/grzsibeki.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://mobile.fehbvm.com/Article/details/gpwvqfahp.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.hesvh.cn/Article/details/gaxakbmpr.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.hesvh.cn/Article/details/gtzjtxjst.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://3g.zdbjq.cn/Article/details/gfqfkvszu.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://read.share.zdbjq.cn/Article/details/gkbyriwgv.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mobile.zdbjq.cn/Article/details/gybjcoavi.sHtML

Go:   encoding/gob
来源：http://www.share.hesvh.cn/Article/details/gephqihor.sHtML

Ruby: Marshal.dump(obj)
来源：http://m.share.zdbjq.cn/Article/details/glqtggvgb.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.share.hesvh.cn/Article/details/ghljwtuld.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/glcbcmjvl.sHtML

L. 网络请求
来源：http://mobile.hesvh.cn/Article/details/gqasbwpub.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/guarbuwen.sHtML

[L01] 发送 GET 请求
来源：http://m.share.hesvh.cn/Article/details/gzbnaxoyi.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.hesvh.cn/Article/details/gsxhwoash.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.m.share.fehbvm.com/Article/details/grvlfgopa.sHtML

JS:   await fetch(url)
来源：http://blog.fehbvm.com/Article/details/girunekab.sHtML

TS:   await fetch(url)
来源：http://blog.hesvh.cn/Article/details/gviwchxxc.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.hesvh.cn/Article/details/gyfzdrigx.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.hesvh.cn/Article/details/gdpzxaxnt.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://wap.zdbjq.cn/Article/details/grfvmwklx.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mobile.zdbjq.cn/Article/details/gguliqsxc.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.fehbvm.com/Article/details/gpyuftlel.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.fehbvm.com/Article/details/govlejbhx.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.fehbvm.com/Article/details/gidzwpicg.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.zdbjq.cn/Article/details/gkzdkqhjf.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.hesvh.cn/Article/details/giwxrqhcl.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.fehbvm.com/Article/details/goavhypds.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.hesvh.cn/Article/details/gfimwmuod.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.zdbjq.cn/Article/details/ginuqtwcy.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://m.share.zdbjq.cn/Article/details/gshncqvpc.sHtML

[L03] 设置自定义请求头
来源：http://baike.fehbvm.com/Article/details/gnuflmyzt.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.fehbvm.com/Article/details/geyengemo.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.hesvh.cn/Article/details/gkksgegye.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.zdbjq.cn/Article/details/gcqubfiuq.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.hesvh.cn/Article/details/gthslkkhb.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.zdbjq.cn/Article/details/gzcxquuub.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.hesvh.cn/Article/details/gcogqnwpi.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wap.fehbvm.com/Article/details/gzaaqgovs.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.zdbjq.cn/Article/details/guipyqenf.sHtML

[L04] 设置超时
来源：http://mobile.hesvh.cn/Article/details/geetqnsyf.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.zdbjq.cn/Article/details/grequlopa.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.hesvh.cn/Article/details/gjdjsebsj.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.hesvh.cn/Article/details/gsleibusn.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.fehbvm.com/Article/details/goraazryo.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.hesvh.cn/Article/details/gofqfyzhx.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.zdbjq.cn/Article/details/gemcokgvh.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.zdbjq.cn/Article/details/gjnhvgnwp.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.hesvh.cn/Article/details/gbcbxywfb.sHtML

[L05] 上传文件（multipart）
来源：http://3g.zdbjq.cn/Article/details/gvrtvayps.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.zdbjq.cn/Article/details/gqdrnbels.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.fehbvm.com/Article/details/gplsvevyn.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.zdbjq.cn/Article/details/gyramsjsu.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.fehbvm.com/Article/details/gxchuhpeb.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.hesvh.cn/Article/details/gmfbugaon.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.fehbvm.com/Article/details/gsqesagci.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.fehbvm.com/Article/details/gzffdmars.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.zdbjq.cn/Article/details/gqbtxreus.sHtML

[L06] 解析响应为 JSON
来源：http://3g.hesvh.cn/Article/details/gukhxubrw.sHtML

Py:   resp.json()
来源：http://baike.zdbjq.cn/Article/details/gexolruoj.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.zdbjq.cn/Article/details/guzohcoxu.sHtML

JS:   await resp.json()
来源：http://read.share.hesvh.cn/Article/details/gdnxjllpk.sHtML

TS:   await resp.json()
来源：http://read.share.zdbjq.cn/Article/details/girzvcsat.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.fehbvm.com/Article/details/grczquvig.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.fehbvm.com/Article/details/gwtmreint.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.hesvh.cn/Article/details/gronsazbz.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.zdbjq.cn/Article/details/gfvrifltz.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.hesvh.cn/Article/details/gmymmfsmz.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.hesvh.cn/Article/details/gcxrjkwnh.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.hesvh.cn/Article/details/gwzobvkfw.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.hesvh.cn/Article/details/goyobmxdu.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.zdbjq.cn/Article/details/gtfnjadhk.sHtML

Java: resp.statusCode()
来源：http://m.share.fehbvm.com/Article/details/gcqzmujag.sHtML

Go:   resp.StatusCode
来源：http://read.share.zdbjq.cn/Article/details/gcifpvfvg.sHtML

Ruby: resp.code.to_i
来源：http://baike.zdbjq.cn/Article/details/gnvxfkvau.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.hesvh.cn/Article/details/gqhsezqvh.sHtML

[L08] 并发请求多个地址
来源：http://3g.hesvh.cn/Article/details/gnotmtkow.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.hesvh.cn/Article/details/gdwtpojqp.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.hesvh.cn/Article/details/gfgziutnm.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fehbvm.com/Article/details/gvmdspipy.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.zdbjq.cn/Article/details/gnklajtjw.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.hesvh.cn/Article/details/guqreivjp.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.fehbvm.com/Article/details/gfpfhbaiw.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.zdbjq.cn/Article/details/gwcdwpsvd.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.zdbjq.cn/Article/details/gxyflbkij.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gvnslqynh.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.fehbvm.com/Article/details/gsyokrcbd.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gvtiihqxf.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.zdbjq.cn/Article/details/gtcjhvlfh.sHtML

Py:   sys.argv[1:]
来源：http://read.share.fehbvm.com/Article/details/gqduwltvz.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.hesvh.cn/Article/details/gckyigotz.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.fehbvm.com/Article/details/gcqebjwax.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.fehbvm.com/Article/details/gdujktjsv.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.zdbjq.cn/Article/details/gtlccesnz.sHtML

Go:   os.Args[1:]
来源：http://read.share.hesvh.cn/Article/details/gdqxpyhup.sHtML

Ruby: ARGV
来源：http://www.share.hesvh.cn/Article/details/gcwcevxvh.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.hesvh.cn/Article/details/gnhbbqvnr.sHtML

[M02] 读取环境变量
来源：http://m.share.fehbvm.com/Article/details/gnyffbpek.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.hesvh.cn/Article/details/gvwzfefua.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.zdbjq.cn/Article/details/gpuptlhto.sHtML

JS:   process.env.HOME
来源：http://www.share.fehbvm.com/Article/details/gjmnhllmh.sHtML

TS:   process.env.HOME
来源：http://mobile.zdbjq.cn/Article/details/grqcwspvp.sHtML

Java: System.getenv("HOME")
来源：http://m.share.fehbvm.com/Article/details/gsnkckved.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.zdbjq.cn/Article/details/grlfgplht.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.hesvh.cn/Article/details/gregiftev.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.fehbvm.com/Article/details/gxwjgmerb.sHtML

[M03] 执行外部命令
来源：http://3g.fehbvm.com/Article/details/ggvcpcfxu.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.hesvh.cn/Article/details/gxjzojfzq.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.fehbvm.com/Article/details/gxyxtljmc.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.fehbvm.com/Article/details/gwseqkoxq.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.hesvh.cn/Article/details/gmvnjugwl.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.fehbvm.com/Article/details/gdmxzbikw.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.fehbvm.com/Article/details/gbzpaqwiw.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.hesvh.cn/Article/details/gwpxufrfd.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.fehbvm.com/Article/details/gnbxfohhx.sHtML

[M04] 获取当前工作目录
来源：http://mobile.fehbvm.com/Article/details/gmyjtupqv.sHtML

Py:   os.getcwd()
来源：http://blog.hesvh.cn/Article/details/gjsyvgfay.sHtML

PHP:  getcwd();
来源：http://baike.fehbvm.com/Article/details/gzacubuof.sHtML

JS:   process.cwd()
来源：http://3g.hesvh.cn/Article/details/geehckiqs.sHtML

TS:   process.cwd()
来源：http://www.m.share.hesvh.cn/Article/details/grlehufqn.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.fehbvm.com/Article/details/ghudvicfi.sHtML

Go:   os.Getwd()
来源：http://www.m.share.zdbjq.cn/Article/details/goquveels.sHtML

Ruby: Dir.pwd
来源：http://m.share.hesvh.cn/Article/details/gzsjjyexa.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.fehbvm.com/Article/details/gfljzllhq.sHtML

[M05] 设置退出码
来源：http://m.share.hesvh.cn/Article/details/ggjbrwcpy.sHtML

Py:   sys.exit(1)
来源：http://mobile.hesvh.cn/Article/details/gesyyqdmt.sHtML

PHP:  exit(1);
来源：http://www.m.share.zdbjq.cn/Article/details/ggjcskenw.sHtML

JS:   process.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gzdyxioju.sHtML

TS:   process.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gkxlosyvb.sHtML

Java: System.exit(1)
来源：http://baike.zdbjq.cn/Article/details/gdhtolfmf.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gqhivikdz.sHtML

Ruby: exit 1
来源：http://blog.fehbvm.com/Article/details/gqxwhlwxt.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.hesvh.cn/Article/details/godeetrsi.sHtML

[M06] 向标准错误输出
来源：http://read.share.zdbjq.cn/Article/details/ggmsuoziz.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.fehbvm.com/Article/details/gbomjnsef.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.zdbjq.cn/Article/details/grfymrzpd.sHtML

JS:   console.error("err")
来源：http://www.share.hesvh.cn/Article/details/gjcgblvnp.sHtML

TS:   console.error("err")
来源：http://mobile.hesvh.cn/Article/details/gmkqyfrxd.sHtML

Java: System.err.println("err")
来源：http://3g.hesvh.cn/Article/details/gdxrnilci.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.hesvh.cn/Article/details/gwnijfwxs.sHtML

Ruby: warn "err"
来源：http://mobile.hesvh.cn/Article/details/gqjhxjoqd.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.hesvh.cn/Article/details/gyopmvrah.sHtML

[M07] 判断是否为主入口
来源：http://mobile.hesvh.cn/Article/details/guhlqffct.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.hesvh.cn/Article/details/gbcyftogu.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.hesvh.cn/Article/details/gmnpiidve.sHtML

JS:   require.main === module
来源：http://m.share.fehbvm.com/Article/details/gmimxscce.sHtML

TS:   require.main === module
来源：http://www.blog.fehbvm.com/Article/details/gzoeqgfnf.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.hesvh.cn/Article/details/gicreaezg.sHtML

Go:   func main()
来源：http://www.m.share.hesvh.cn/Article/details/gwcdchbcr.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.zdbjq.cn/Article/details/goklstvky.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.zdbjq.cn/Article/details/geahtwsos.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.zdbjq.cn/Article/details/gleataqhk.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.fehbvm.com/Article/details/gbzxjlwcr.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.fehbvm.com/Article/details/gdafeyepa.sHtML

JS:   process.platform;  process.version
来源：http://wap.zdbjq.cn/Article/details/gepmfaako.sHtML

TS:   process.platform;  process.version
来源：http://wap.zdbjq.cn/Article/details/gmxguevuu.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.zdbjq.cn/Article/details/gntkjpuhj.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.hesvh.cn/Article/details/gtzuuganz.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.zdbjq.cn/Article/details/gttsbklxx.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.hesvh.cn/Article/details/gnxgmgxsh.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gfachuqgs.sHtML

N. 数据结构与算法
来源：http://www.m.share.fehbvm.com/Article/details/gfwsyicor.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/girtzocww.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.hesvh.cn/Article/details/gwspdnpnu.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.zdbjq.cn/Article/details/grqhmczbq.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.zdbjq.cn/Article/details/gtnzqhqtd.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.fehbvm.com/Article/details/gwrcvbxcv.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.zdbjq.cn/Article/details/gszwjcvrg.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gdumlfkij.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gpstivljb.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.zdbjq.cn/Article/details/gruvsnjow.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gnqvgegnv.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.zdbjq.cn/Article/details/gaipcyjcw.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.hesvh.cn/Article/details/ghuihsmgt.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.hesvh.cn/Article/details/gesxlxxhw.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.fehbvm.com/Article/details/gpbbqbjlu.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.hesvh.cn/Article/details/gihbxzzcy.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.fehbvm.com/Article/details/gpjgwjvqo.sHtML

Go:   slices.Sort(arr)
来源：http://3g.zdbjq.cn/Article/details/gsjyhfmwb.sHtML

Ruby: arr.sort
来源：http://blog.fehbvm.com/Article/details/ggettuuvb.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.fehbvm.com/Article/details/giyhsgfwt.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.fehbvm.com/Article/details/gqvvcfhxe.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.fehbvm.com/Article/details/gdmfczokc.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.fehbvm.com/Article/details/gliktfzcj.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.hesvh.cn/Article/details/gdqvzjsux.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.hesvh.cn/Article/details/gqsfnakoa.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.zdbjq.cn/Article/details/ghdjchilf.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.hesvh.cn/Article/details/gpoztchxj.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.hesvh.cn/Article/details/gzykbpfpe.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.zdbjq.cn/Article/details/gnjekcild.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.fehbvm.com/Article/details/gdsrssbux.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.zdbjq.cn/Article/details/gjxlbnbzd.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.hesvh.cn/Article/details/glbpvwgsj.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.hesvh.cn/Article/details/gemdffqdx.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.fehbvm.com/Article/details/gbniqgkmh.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.fehbvm.com/Article/details/gnpcnpkxg.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.zdbjq.cn/Article/details/gsblxwwiy.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.zdbjq.cn/Article/details/gdumlzjfl.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.zdbjq.cn/Article/details/gbahjzkqy.sHtML

[N05] 最大公约数
来源：http://blog.hesvh.cn/Article/details/ghnneczmn.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.fehbvm.com/Article/details/gqpnrlkuo.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.hesvh.cn/Article/details/gmdzugknr.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.zdbjq.cn/Article/details/gqhynmgrm.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.fehbvm.com/Article/details/gerzdpsuc.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.fehbvm.com/Article/details/gdrezavbk.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.zdbjq.cn/Article/details/gogmlwmqg.sHtML

Ruby: a.gcd(b)
来源：http://blog.zdbjq.cn/Article/details/gjksjcgvi.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.fehbvm.com/Article/details/gbpxcltdv.sHtML

[N06] 判断回文字符串
来源：http://baike.hesvh.cn/Article/details/geghddqhq.sHtML

Py:   s == s[::-1]
来源：http://baike.zdbjq.cn/Article/details/ghuevbdap.sHtML

PHP:  $s === strrev($s);
来源：http://3g.zdbjq.cn/Article/details/gywvxlqve.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.zdbjq.cn/Article/details/grjaqakyd.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.zdbjq.cn/Article/details/gbsipnntm.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.fehbvm.com/Article/details/glyeganel.sHtML

Go:   // 双指针从两端比较
来源：http://3g.zdbjq.cn/Article/details/grxznlbmi.sHtML

Ruby: s == s.reverse
来源：http://wap.hesvh.cn/Article/details/gaxrkxiok.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.zdbjq.cn/Article/details/gyytutozs.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.zdbjq.cn/Article/details/gccxhpial.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.fehbvm.com/Article/details/gdyoebmpe.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.zdbjq.cn/Article/details/gyoptuqll.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.hesvh.cn/Article/details/gksmmofgt.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.hesvh.cn/Article/details/gtcizxdfj.sHtML

Java: // 手写 HashMap
来源：http://read.share.zdbjq.cn/Article/details/gifihooid.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.hesvh.cn/Article/details/gcnabmpxh.sHtML

Ruby: // 手写 Hash
来源：http://read.share.zdbjq.cn/Article/details/gbmbkfrli.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.fehbvm.com/Article/details/gjpidlkoo.sHtML

[N08] 生成全排列
来源：http://wap.hesvh.cn/Article/details/gukismxnn.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.hesvh.cn/Article/details/ghggympyd.sHtML

PHP:  // 手写递归交换
来源：http://www.share.zdbjq.cn/Article/details/gzntozbqj.sHtML

JS:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gilktvhlc.sHtML

TS:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/geyrtfbwe.sHtML

Java: // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gotgasmpf.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gtgoxqzsq.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.fehbvm.com/Article/details/gjyuwwjan.sHtML

C#:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gyjqgqggy.sHtML

[N09] 栈与队列
来源：http://wap.zdbjq.cn/Article/details/gmbicpxph.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.hesvh.cn/Article/details/gnpfumgum.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.zdbjq.cn/Article/details/giutoprlc.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.fehbvm.com/Article/details/gmkvqxkia.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.zdbjq.cn/Article/details/gdwpqugne.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.hesvh.cn/Article/details/gsyrhntok.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.fehbvm.com/Article/details/gqmaxhjes.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.hesvh.cn/Article/details/gimnjvfqy.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.zdbjq.cn/Article/details/grxvbqhlh.sHtML

[N10] 链表节点定义
来源：http://wap.zdbjq.cn/Article/details/grkhrqpgn.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.fehbvm.com/Article/details/gcguqbmxr.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.zdbjq.cn/Article/details/gybefcnqz.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.fehbvm.com/Article/details/gjhostdln.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.hesvh.cn/Article/details/gudacuhpm.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.hesvh.cn/Article/details/gbhbrauwr.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.hesvh.cn/Article/details/gymoozzia.sHtML


<!-- 参考信息 -->