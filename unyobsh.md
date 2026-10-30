代发 wailian999

JS:   JSON.stringify(obj, null, 2)
来源：http://baike.fehbvm.com/Article/details/garddxvri.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://3g.fehbvm.com/Article/details/grivuxrfm.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://3g.hesvh.cn/Article/details/gtblkegdz.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://m.share.zdbjq.cn/Article/details/gbgrjxcvn.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://m.share.fehbvm.com/Article/details/gsaasjeea.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://blog.zdbjq.cn/Article/details/gdtqipxez.sHtML

[K04] 读取 JSON 文件
来源：http://baike.fehbvm.com/Article/details/gjwlynoac.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wap.fehbvm.com/Article/details/gwypynmwk.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://m.share.zdbjq.cn/Article/details/gnictptzl.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.zdbjq.cn/Article/details/gnsodushx.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.hesvh.cn/Article/details/goeettkio.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://read.share.fehbvm.com/Article/details/gedovutrw.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wap.fehbvm.com/Article/details/guxxyoybq.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://baike.hesvh.cn/Article/details/gmaworsdj.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.zdbjq.cn/Article/details/grekdfwhw.sHtML

[K05] 深拷贝对象
来源：http://m.share.hesvh.cn/Article/details/gnxaqisaq.sHtML

Py:   copy.deepcopy(obj)
来源：http://wap.hesvh.cn/Article/details/gqzuankmi.sHtML

PHP:  unserialize(serialize($obj));
来源：http://blog.zdbjq.cn/Article/details/glqejwpac.sHtML

JS:   structuredClone(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gnjmeukpk.sHtML

TS:   structuredClone(obj)
来源：http://wap.hesvh.cn/Article/details/gimfknrur.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.blog.zdbjq.cn/Article/details/giksymhib.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.share.zdbjq.cn/Article/details/gczupsmze.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://baike.zdbjq.cn/Article/details/gqifkqprq.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://read.share.zdbjq.cn/Article/details/gzzqiseii.sHtML

[K06] 解析 URL 查询串
来源：http://www.m.share.fehbvm.com/Article/details/grlgcfrpm.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://baike.fehbvm.com/Article/details/gucbftrov.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://baike.fehbvm.com/Article/details/gvzbofixs.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.hesvh.cn/Article/details/gwlbppvgw.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.fehbvm.com/Article/details/giuhhdjey.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://blog.hesvh.cn/Article/details/gldqzykty.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://blog.fehbvm.com/Article/details/gvanxmamr.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wap.zdbjq.cn/Article/details/gtjzxbesy.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.fehbvm.com/Article/details/ghjrzrqkz.sHtML

[K07] 进制转换
来源：http://baike.zdbjq.cn/Article/details/gjxmmoyrt.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.hesvh.cn/Article/details/ggednabbv.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.fehbvm.com/Article/details/ghgrkwfkh.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.fehbvm.com/Article/details/gnoqdolba.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://baike.hesvh.cn/Article/details/gjeydyjka.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wap.fehbvm.com/Article/details/gselvwuxc.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://3g.hesvh.cn/Article/details/gcwlntsmz.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.m.share.hesvh.cn/Article/details/gexnhwzym.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mobile.fehbvm.com/Article/details/gnkyndlvm.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.m.share.fehbvm.com/Article/details/gkeiazjgd.sHtML

Py:   pickle.dumps(obj)
来源：http://mobile.fehbvm.com/Article/details/govrhpprv.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.fehbvm.com/Article/details/gveljjiru.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://3g.zdbjq.cn/Article/details/grdbjkxjp.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.fehbvm.com/Article/details/gmhtbbqqr.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.zdbjq.cn/Article/details/gqrxdcpow.sHtML

Go:   encoding/gob
来源：http://baike.hesvh.cn/Article/details/gccpatmve.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.fehbvm.com/Article/details/grvjzhoas.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://read.share.zdbjq.cn/Article/details/gzsyzbwel.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gjrfnauot.sHtML

L. 网络请求
来源：http://mobile.hesvh.cn/Article/details/gyqowtydj.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gpljosked.sHtML

[L01] 发送 GET 请求
来源：http://www.share.fehbvm.com/Article/details/gjliysvbd.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.fehbvm.com/Article/details/giqguvagf.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.zdbjq.cn/Article/details/gogezyrhu.sHtML

JS:   await fetch(url)
来源：http://m.share.hesvh.cn/Article/details/gmubcuufs.sHtML

TS:   await fetch(url)
来源：http://blog.zdbjq.cn/Article/details/gzwpkdydo.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.hesvh.cn/Article/details/gohoiggrr.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.fehbvm.com/Article/details/gvlpbrabu.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.hesvh.cn/Article/details/gsdoufias.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.hesvh.cn/Article/details/gcdpkqdjz.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.fehbvm.com/Article/details/gxjqwursy.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.zdbjq.cn/Article/details/gmfdezezt.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.zdbjq.cn/Article/details/gdjzagzhi.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.hesvh.cn/Article/details/gzzkmwttr.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.hesvh.cn/Article/details/gecuineou.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.zdbjq.cn/Article/details/gckvbfajo.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://m.share.zdbjq.cn/Article/details/gzquryptv.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://blog.zdbjq.cn/Article/details/gulhbocsl.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.fehbvm.com/Article/details/gtmprzsjf.sHtML

[L03] 设置自定义请求头
来源：http://3g.fehbvm.com/Article/details/guwhmifbt.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.hesvh.cn/Article/details/gthkdwdjk.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.hesvh.cn/Article/details/gqcvpqbmn.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.hesvh.cn/Article/details/gyquvhwhc.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.hesvh.cn/Article/details/ggkbdgogx.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.hesvh.cn/Article/details/gnlwuxnqj.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.fehbvm.com/Article/details/gzyebskgc.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.share.zdbjq.cn/Article/details/gquntgiur.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wap.zdbjq.cn/Article/details/gjcnpovlw.sHtML

[L04] 设置超时
来源：http://m.share.zdbjq.cn/Article/details/gerijltuj.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.fehbvm.com/Article/details/gquqowixk.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.zdbjq.cn/Article/details/galbjsjus.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.fehbvm.com/Article/details/govdbevdh.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.zdbjq.cn/Article/details/gqvbkmltz.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.hesvh.cn/Article/details/gaarfljst.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.fehbvm.com/Article/details/gqsqzjnyx.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.hesvh.cn/Article/details/grggwnqis.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.zdbjq.cn/Article/details/gzcwddchv.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.fehbvm.com/Article/details/gwrsfjnii.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.hesvh.cn/Article/details/gmmzburqt.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.fehbvm.com/Article/details/gdfwvouot.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.fehbvm.com/Article/details/gsjkxgvyu.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.hesvh.cn/Article/details/gqiisnfgs.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.hesvh.cn/Article/details/gewauekdu.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.fehbvm.com/Article/details/gspzxjpyb.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.hesvh.cn/Article/details/gpkegoztj.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.hesvh.cn/Article/details/gsyryruze.sHtML

[L06] 解析响应为 JSON
来源：http://3g.zdbjq.cn/Article/details/grhayaufl.sHtML

Py:   resp.json()
来源：http://3g.hesvh.cn/Article/details/gxtgvvhbb.sHtML

PHP:  json_decode($body, true);
来源：http://3g.fehbvm.com/Article/details/gfuotubxc.sHtML

JS:   await resp.json()
来源：http://wap.fehbvm.com/Article/details/gpwdzkxkl.sHtML

TS:   await resp.json()
来源：http://m.share.hesvh.cn/Article/details/gkzobrrxl.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.fehbvm.com/Article/details/gzwxnvojf.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.hesvh.cn/Article/details/gxymszbvs.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.zdbjq.cn/Article/details/gtfmjvjbs.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.fehbvm.com/Article/details/gertjhhdl.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.zdbjq.cn/Article/details/giqiwwrum.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.hesvh.cn/Article/details/gbkfmrzjg.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.zdbjq.cn/Article/details/gyxeaowfi.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.hesvh.cn/Article/details/guiprxtsr.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.fehbvm.com/Article/details/gxyihkipm.sHtML

Java: resp.statusCode()
来源：http://read.share.zdbjq.cn/Article/details/guermacym.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.fehbvm.com/Article/details/gycrmtktq.sHtML

Ruby: resp.code.to_i
来源：http://3g.hesvh.cn/Article/details/gywcukeol.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.fehbvm.com/Article/details/gihesqzaz.sHtML

[L08] 并发请求多个地址
来源：http://mobile.zdbjq.cn/Article/details/glhhyvahg.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.zdbjq.cn/Article/details/gdqibtbie.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.hesvh.cn/Article/details/gwdkvpedg.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.zdbjq.cn/Article/details/gtoqsglnv.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.zdbjq.cn/Article/details/gzogruktm.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.fehbvm.com/Article/details/gbhmeismf.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.fehbvm.com/Article/details/gtvkviekz.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.zdbjq.cn/Article/details/gcswuqlmg.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.hesvh.cn/Article/details/glpvbpsjg.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gokqfgaez.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.zdbjq.cn/Article/details/graysopmy.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/giivzwcwt.sHtML

[M01] 读取命令行参数
来源：http://blog.zdbjq.cn/Article/details/gturhhltz.sHtML

Py:   sys.argv[1:]
来源：http://mobile.hesvh.cn/Article/details/gkrlunbvh.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.zdbjq.cn/Article/details/gictenznb.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.hesvh.cn/Article/details/goddofyqb.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.hesvh.cn/Article/details/gunwpnivo.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.fehbvm.com/Article/details/gzhedvput.sHtML

Go:   os.Args[1:]
来源：http://baike.fehbvm.com/Article/details/glgewcyxm.sHtML

Ruby: ARGV
来源：http://www.m.share.hesvh.cn/Article/details/gafxsizdj.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.hesvh.cn/Article/details/gkmjqdwwv.sHtML

[M02] 读取环境变量
来源：http://baike.zdbjq.cn/Article/details/gllqhifbt.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.fehbvm.com/Article/details/gtmdisjjm.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.zdbjq.cn/Article/details/gyafbctvc.sHtML

JS:   process.env.HOME
来源：http://blog.fehbvm.com/Article/details/gwuarhiho.sHtML

TS:   process.env.HOME
来源：http://m.share.hesvh.cn/Article/details/gjirkoswh.sHtML

Java: System.getenv("HOME")
来源：http://3g.zdbjq.cn/Article/details/gvzakxgmh.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.fehbvm.com/Article/details/gmupymipt.sHtML

Ruby: ENV["HOME"]
来源：http://blog.fehbvm.com/Article/details/gsjjpbwxv.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.zdbjq.cn/Article/details/gdelsubzt.sHtML

[M03] 执行外部命令
来源：http://blog.zdbjq.cn/Article/details/gbnqlqghb.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.zdbjq.cn/Article/details/gwrjppclb.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.hesvh.cn/Article/details/goyraoqyn.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.zdbjq.cn/Article/details/gmifnckis.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.zdbjq.cn/Article/details/gjxmavmfw.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.fehbvm.com/Article/details/gifyzpujs.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.zdbjq.cn/Article/details/gjnxrcqoy.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.hesvh.cn/Article/details/gnozjbrcv.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.fehbvm.com/Article/details/gwbqjvbns.sHtML

[M04] 获取当前工作目录
来源：http://blog.hesvh.cn/Article/details/gmoavxjyx.sHtML

Py:   os.getcwd()
来源：http://3g.fehbvm.com/Article/details/gzvqohmlm.sHtML

PHP:  getcwd();
来源：http://wap.hesvh.cn/Article/details/geykrgkaf.sHtML

JS:   process.cwd()
来源：http://m.share.zdbjq.cn/Article/details/grsqnoiiw.sHtML

TS:   process.cwd()
来源：http://wap.zdbjq.cn/Article/details/grdzytgld.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.zdbjq.cn/Article/details/gbuzupnsz.sHtML

Go:   os.Getwd()
来源：http://blog.fehbvm.com/Article/details/gvziwzpty.sHtML

Ruby: Dir.pwd
来源：http://www.share.zdbjq.cn/Article/details/ghczfpqlh.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.fehbvm.com/Article/details/gtcxqmote.sHtML

[M05] 设置退出码
来源：http://m.share.fehbvm.com/Article/details/gfdrmdnmp.sHtML

Py:   sys.exit(1)
来源：http://mobile.hesvh.cn/Article/details/gcxfrjwfs.sHtML

PHP:  exit(1);
来源：http://www.m.share.zdbjq.cn/Article/details/gpxysxktn.sHtML

JS:   process.exit(1)
来源：http://3g.hesvh.cn/Article/details/guchkucig.sHtML

TS:   process.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gyrpxwfoy.sHtML

Java: System.exit(1)
来源：http://www.share.hesvh.cn/Article/details/gxnyjaegl.sHtML

Go:   os.Exit(1)
来源：http://wap.zdbjq.cn/Article/details/gnxpxiqoo.sHtML

Ruby: exit 1
来源：http://www.m.share.hesvh.cn/Article/details/gyykermot.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.zdbjq.cn/Article/details/grichjzlr.sHtML

[M06] 向标准错误输出
来源：http://m.share.fehbvm.com/Article/details/gzcyoeini.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.fehbvm.com/Article/details/gopaanszx.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.zdbjq.cn/Article/details/grbvjlqti.sHtML

JS:   console.error("err")
来源：http://m.share.zdbjq.cn/Article/details/gaqefdfvh.sHtML

TS:   console.error("err")
来源：http://www.blog.fehbvm.com/Article/details/glejpifmi.sHtML

Java: System.err.println("err")
来源：http://www.blog.fehbvm.com/Article/details/gxmsbjwdn.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.zdbjq.cn/Article/details/guaineser.sHtML

Ruby: warn "err"
来源：http://www.blog.zdbjq.cn/Article/details/gyqnqifxz.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.fehbvm.com/Article/details/gptjbaqif.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.zdbjq.cn/Article/details/ggpoewqsh.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.fehbvm.com/Article/details/gbkpkdmaz.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.hesvh.cn/Article/details/gslodpbgf.sHtML

JS:   require.main === module
来源：http://www.share.zdbjq.cn/Article/details/gosnkkvxm.sHtML

TS:   require.main === module
来源：http://baike.hesvh.cn/Article/details/gfaxzrmsn.sHtML

Java: public static void main(String[] args)
来源：http://blog.hesvh.cn/Article/details/gwkydewbs.sHtML

Go:   func main()
来源：http://3g.zdbjq.cn/Article/details/gtyzmsoia.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.zdbjq.cn/Article/details/gyvceyqhc.sHtML

C#:   static void Main(string[] args)
来源：http://baike.hesvh.cn/Article/details/gzascvdok.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.hesvh.cn/Article/details/gjgnaauzt.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.zdbjq.cn/Article/details/gzoenohqz.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.zdbjq.cn/Article/details/gtqiwubws.sHtML

JS:   process.platform;  process.version
来源：http://wap.fehbvm.com/Article/details/gzxvhijrq.sHtML

TS:   process.platform;  process.version
来源：http://blog.hesvh.cn/Article/details/grqepvpzd.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.fehbvm.com/Article/details/gsykxojat.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.hesvh.cn/Article/details/ghoyepfxd.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.fehbvm.com/Article/details/gsixfcfez.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.fehbvm.com/Article/details/gzbpiuugs.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gxigouzcm.sHtML

N. 数据结构与算法
来源：http://3g.fehbvm.com/Article/details/gjkjckslb.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gdewjnwvp.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.zdbjq.cn/Article/details/gbjgprufp.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gckuvfskg.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.hesvh.cn/Article/details/gtsvivdxo.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.fehbvm.com/Article/details/gqjzyplga.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.zdbjq.cn/Article/details/gnzojwqyn.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.fehbvm.com/Article/details/gxfsaogps.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gxiicqiwj.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.hesvh.cn/Article/details/gzjnlpjcw.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gwgnhhipi.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.hesvh.cn/Article/details/glcbzcqku.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.fehbvm.com/Article/details/gpdeqsazx.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.fehbvm.com/Article/details/grwgipkqv.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.zdbjq.cn/Article/details/gswkwrvsv.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.fehbvm.com/Article/details/gwcchseat.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.fehbvm.com/Article/details/guxzhlbhq.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.fehbvm.com/Article/details/guxsqzhhs.sHtML

Ruby: arr.sort
来源：http://read.share.hesvh.cn/Article/details/gtpyklhsq.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.hesvh.cn/Article/details/gxisfdhgr.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.hesvh.cn/Article/details/gkfbbtuwh.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.zdbjq.cn/Article/details/gokeaaodh.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.fehbvm.com/Article/details/gnqcwkhkx.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.fehbvm.com/Article/details/gxnxghbiq.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.hesvh.cn/Article/details/gqkprvrmy.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.hesvh.cn/Article/details/gbtyoobqb.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.zdbjq.cn/Article/details/gewcudqby.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.zdbjq.cn/Article/details/ghyzaerxs.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.fehbvm.com/Article/details/gpenimzjp.sHtML

[N04] 斐波那契数列
来源：http://wap.fehbvm.com/Article/details/gyliujven.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.zdbjq.cn/Article/details/gdflvcogl.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.hesvh.cn/Article/details/gtyreylkn.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/gxnrzurwr.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.fehbvm.com/Article/details/ggwqpddou.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.hesvh.cn/Article/details/gcghjwxkj.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.fehbvm.com/Article/details/gvouijqyc.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.zdbjq.cn/Article/details/gsyklybhw.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.zdbjq.cn/Article/details/gyjgejoyn.sHtML

[N05] 最大公约数
来源：http://blog.hesvh.cn/Article/details/gckyqonlc.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.zdbjq.cn/Article/details/ghtxxeyjh.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.hesvh.cn/Article/details/gfbyheiaj.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.hesvh.cn/Article/details/ggtsvfhum.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.zdbjq.cn/Article/details/gwvyuunmx.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.zdbjq.cn/Article/details/gyfdydizk.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.zdbjq.cn/Article/details/grbpoqzql.sHtML

Ruby: a.gcd(b)
来源：http://3g.fehbvm.com/Article/details/gbxlfxlhv.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.fehbvm.com/Article/details/gmklegyny.sHtML

[N06] 判断回文字符串
来源：http://3g.zdbjq.cn/Article/details/gwugninlp.sHtML

Py:   s == s[::-1]
来源：http://m.share.hesvh.cn/Article/details/grwgujilw.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.hesvh.cn/Article/details/gxdcgoahz.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/gooikdrtn.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/gihsdsohv.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.zdbjq.cn/Article/details/gmalafvph.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.zdbjq.cn/Article/details/gqqopwrii.sHtML

Ruby: s == s.reverse
来源：http://m.share.fehbvm.com/Article/details/gliywywnz.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.hesvh.cn/Article/details/gckgycfuc.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.fehbvm.com/Article/details/gtxpzoyxt.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.zdbjq.cn/Article/details/gfpvcjwdd.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.hesvh.cn/Article/details/ginpoqzcj.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.hesvh.cn/Article/details/gsmgwizyb.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.hesvh.cn/Article/details/gbkzbhzbi.sHtML

Java: // 手写 HashMap
来源：http://wap.hesvh.cn/Article/details/gpkcgappw.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.hesvh.cn/Article/details/gldjajfkj.sHtML

Ruby: // 手写 Hash
来源：http://baike.hesvh.cn/Article/details/gbahpeqkn.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.hesvh.cn/Article/details/gjymngdge.sHtML

[N08] 生成全排列
来源：http://blog.zdbjq.cn/Article/details/gfumctgyp.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.fehbvm.com/Article/details/gxbtnywkz.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.hesvh.cn/Article/details/gsblivmvi.sHtML

JS:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gowfqbcdk.sHtML

TS:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gckcbfhjt.sHtML

Java: // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gjyamvtie.sHtML

Go:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/glazueiod.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.fehbvm.com/Article/details/gfrfrndve.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gqbuidfbm.sHtML

[N09] 栈与队列
来源：http://mobile.fehbvm.com/Article/details/gbizforkz.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.zdbjq.cn/Article/details/gckpfzjer.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.zdbjq.cn/Article/details/gvpttvasu.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.fehbvm.com/Article/details/gsmbkvkfb.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.hesvh.cn/Article/details/gunqcbnae.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.zdbjq.cn/Article/details/gmkermvkl.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.fehbvm.com/Article/details/gcgxjazpc.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.zdbjq.cn/Article/details/gfhqyqofq.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.zdbjq.cn/Article/details/gqeflwimq.sHtML

[N10] 链表节点定义
来源：http://www.blog.fehbvm.com/Article/details/gyaboumyz.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.hesvh.cn/Article/details/gkrmthlpy.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.zdbjq.cn/Article/details/ggjjmpcbx.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.hesvh.cn/Article/details/ghydowkkt.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.zdbjq.cn/Article/details/gzihwntrx.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.hesvh.cn/Article/details/grggqgqik.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.fehbvm.com/Article/details/gjuwncasv.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.fehbvm.com/Article/details/gjquyqcos.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.zdbjq.cn/Article/details/gufviuerq.sHtML

[N11] 二叉树中序遍历
来源：http://baike.zdbjq.cn/Article/details/gupkevbse.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.zdbjq.cn/Article/details/gfpjedpby.sHtML

PHP:  // 手写递归函数
来源：http://read.share.fehbvm.com/Article/details/gdnmgkszr.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.zdbjq.cn/Article/details/geyxmetff.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.zdbjq.cn/Article/details/gughqajlp.sHtML

Java: // 手写递归
来源：http://www.share.hesvh.cn/Article/details/gewzgshqw.sHtML


<!-- 参考信息 -->