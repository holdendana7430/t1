代发 wailian999

Ruby: JSON.pretty_generate(obj)
来源：http://m.share.zdbjq.cn/Article/details/gxoswwcjo.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://3g.zdbjq.cn/Article/details/gcmhnxrju.sHtML

[K04] 读取 JSON 文件
来源：http://m.share.fehbvm.com/Article/details/gcgbshzsl.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://blog.fehbvm.com/Article/details/gvtoulbar.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://3g.zdbjq.cn/Article/details/golbngfna.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.hesvh.cn/Article/details/gpqxrdcej.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.zdbjq.cn/Article/details/gpcrnegmw.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://baike.hesvh.cn/Article/details/giliitekq.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://m.share.fehbvm.com/Article/details/ggckxrctx.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://3g.hesvh.cn/Article/details/ggzbiijdl.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://read.share.zdbjq.cn/Article/details/gdpqkusoq.sHtML

[K05] 深拷贝对象
来源：http://wap.zdbjq.cn/Article/details/gtsiotjow.sHtML

Py:   copy.deepcopy(obj)
来源：http://read.share.fehbvm.com/Article/details/gmotxikhe.sHtML

PHP:  unserialize(serialize($obj));
来源：http://mobile.hesvh.cn/Article/details/gqlkhneoi.sHtML

JS:   structuredClone(obj)
来源：http://wap.zdbjq.cn/Article/details/gphevltqw.sHtML

TS:   structuredClone(obj)
来源：http://wap.fehbvm.com/Article/details/gponefvew.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://read.share.fehbvm.com/Article/details/gdjfqbmyv.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.blog.zdbjq.cn/Article/details/gmbikofmm.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://m.share.fehbvm.com/Article/details/gerpalrge.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://blog.hesvh.cn/Article/details/ggaobhuou.sHtML

[K06] 解析 URL 查询串
来源：http://www.blog.fehbvm.com/Article/details/gpobqrrci.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.hesvh.cn/Article/details/gessvwbww.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://m.share.fehbvm.com/Article/details/gwodpqafi.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.zdbjq.cn/Article/details/giapxmxne.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.fehbvm.com/Article/details/gwlwaqtur.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.zdbjq.cn/Article/details/goyjwsise.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.fehbvm.com/Article/details/gqevyhmch.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.fehbvm.com/Article/details/gtvhmpdwz.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.m.share.fehbvm.com/Article/details/ggdxijyaq.sHtML

[K07] 进制转换
来源：http://www.share.zdbjq.cn/Article/details/gjdgtljam.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://3g.zdbjq.cn/Article/details/gdwhkdfrg.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://baike.zdbjq.cn/Article/details/gqgkhenxu.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.share.fehbvm.com/Article/details/gfzxkssiy.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.m.share.fehbvm.com/Article/details/gqdiggkom.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.hesvh.cn/Article/details/gvqaypdnd.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.fehbvm.com/Article/details/gsmjpkmco.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://3g.zdbjq.cn/Article/details/gcbigtstm.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.fehbvm.com/Article/details/genbfedyv.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://wap.zdbjq.cn/Article/details/gceikuxrj.sHtML

Py:   pickle.dumps(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gtyzjltkh.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://read.share.fehbvm.com/Article/details/gppkvvokj.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.fehbvm.com/Article/details/gjrpffycv.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://blog.fehbvm.com/Article/details/gomyjvztd.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://blog.zdbjq.cn/Article/details/gkqgqczla.sHtML

Go:   encoding/gob
来源：http://www.blog.fehbvm.com/Article/details/gizfznzie.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.zdbjq.cn/Article/details/gczkcsqrl.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.hesvh.cn/Article/details/gupdmvnlx.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gucaffrok.sHtML

L. 网络请求
来源：http://www.blog.hesvh.cn/Article/details/gpufgrvns.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/ghkcrspdc.sHtML

[L01] 发送 GET 请求
来源：http://mobile.fehbvm.com/Article/details/gdtokjnam.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.zdbjq.cn/Article/details/gqpdstzhm.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.fehbvm.com/Article/details/gsyreeccs.sHtML

JS:   await fetch(url)
来源：http://mobile.zdbjq.cn/Article/details/gumawypri.sHtML

TS:   await fetch(url)
来源：http://m.share.fehbvm.com/Article/details/gfrvbbkba.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.fehbvm.com/Article/details/gmphsvjil.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.hesvh.cn/Article/details/gbehrjpda.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://baike.hesvh.cn/Article/details/gertdgerx.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.zdbjq.cn/Article/details/gxeazqune.sHtML

[L02] 发送 POST JSON
来源：http://www.share.fehbvm.com/Article/details/gmqyuvpgr.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.fehbvm.com/Article/details/gdkyknbbw.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.zdbjq.cn/Article/details/gipmocopk.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.zdbjq.cn/Article/details/gswpnkobx.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.zdbjq.cn/Article/details/gjatjfkss.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.hesvh.cn/Article/details/gftucxjss.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mobile.hesvh.cn/Article/details/gvscqnhwj.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.zdbjq.cn/Article/details/gpuswldfr.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.zdbjq.cn/Article/details/ghwmunasb.sHtML

[L03] 设置自定义请求头
来源：http://blog.zdbjq.cn/Article/details/gfvrxsjyb.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.zdbjq.cn/Article/details/gssxzadtt.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.blog.zdbjq.cn/Article/details/gdsoudour.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.fehbvm.com/Article/details/gmrtiyjwy.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.hesvh.cn/Article/details/gowtgfurs.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.fehbvm.com/Article/details/gjbcqppjj.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.blog.hesvh.cn/Article/details/gbnughtas.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.hesvh.cn/Article/details/gkhshndob.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.zdbjq.cn/Article/details/ghvjtqkkb.sHtML

[L04] 设置超时
来源：http://www.blog.zdbjq.cn/Article/details/gycdkgvqm.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.blog.fehbvm.com/Article/details/gtfdqwnbs.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.zdbjq.cn/Article/details/gmgyxfixx.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.fehbvm.com/Article/details/gxyxvipng.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.zdbjq.cn/Article/details/grtrskgoe.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.hesvh.cn/Article/details/gcsdllkvm.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.hesvh.cn/Article/details/gomonmeqt.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.fehbvm.com/Article/details/grtjkylmd.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.hesvh.cn/Article/details/gkyfsjloc.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.fehbvm.com/Article/details/gyzbnibvy.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.fehbvm.com/Article/details/gdmbjxeko.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.fehbvm.com/Article/details/gsjaikmhq.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.fehbvm.com/Article/details/gmzxjgmxo.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.fehbvm.com/Article/details/gwcguelxc.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.zdbjq.cn/Article/details/guazonuli.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.zdbjq.cn/Article/details/ggheqblxz.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.hesvh.cn/Article/details/gtqzjezvo.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gxihssnnd.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.zdbjq.cn/Article/details/geyadkndw.sHtML

Py:   resp.json()
来源：http://www.blog.zdbjq.cn/Article/details/gfmunawkz.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.fehbvm.com/Article/details/gbiuadafl.sHtML

JS:   await resp.json()
来源：http://www.blog.hesvh.cn/Article/details/gjxzribif.sHtML

TS:   await resp.json()
来源：http://m.share.zdbjq.cn/Article/details/gbabqjjfs.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.hesvh.cn/Article/details/gplvzlxnp.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.fehbvm.com/Article/details/gecqqbbgt.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.hesvh.cn/Article/details/gkbnvmckc.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.fehbvm.com/Article/details/gqlfoqlkg.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.zdbjq.cn/Article/details/gdbyxflme.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.hesvh.cn/Article/details/gbjoepjpc.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.zdbjq.cn/Article/details/gozjxruad.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.zdbjq.cn/Article/details/gkmyusvzm.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.zdbjq.cn/Article/details/gncczmcfb.sHtML

Java: resp.statusCode()
来源：http://mobile.zdbjq.cn/Article/details/gmvaasaps.sHtML

Go:   resp.StatusCode
来源：http://3g.fehbvm.com/Article/details/gkxhnmbfz.sHtML

Ruby: resp.code.to_i
来源：http://blog.hesvh.cn/Article/details/glncwbvtr.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.fehbvm.com/Article/details/gjltsgpod.sHtML

[L08] 并发请求多个地址
来源：http://wap.fehbvm.com/Article/details/geaaodhcn.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.hesvh.cn/Article/details/gtimsgquv.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.hesvh.cn/Article/details/gchpjrggq.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fehbvm.com/Article/details/gsiuldqmg.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.hesvh.cn/Article/details/gmihbdgbw.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.hesvh.cn/Article/details/glqtkyuff.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.hesvh.cn/Article/details/gdvnqmpaa.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.fehbvm.com/Article/details/gldcyfaje.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.fehbvm.com/Article/details/gnthuflkr.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gxnjmwwvu.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.zdbjq.cn/Article/details/gtxlsyvto.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/guilndakk.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.fehbvm.com/Article/details/gkhwfuruu.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.hesvh.cn/Article/details/gsanzpglo.sHtML

PHP:  $argv;  $argc;
来源：http://wap.hesvh.cn/Article/details/goxerkjcm.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.fehbvm.com/Article/details/gzbhpzpfp.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.fehbvm.com/Article/details/gxmncmdgv.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.hesvh.cn/Article/details/gkerkwgyt.sHtML

Go:   os.Args[1:]
来源：http://www.blog.zdbjq.cn/Article/details/gskieptsh.sHtML

Ruby: ARGV
来源：http://baike.zdbjq.cn/Article/details/gyrbcvoox.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.fehbvm.com/Article/details/ggvspiiak.sHtML

[M02] 读取环境变量
来源：http://3g.hesvh.cn/Article/details/gyzvyqeap.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.hesvh.cn/Article/details/gqlqjgiqn.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.zdbjq.cn/Article/details/gcokgafln.sHtML

JS:   process.env.HOME
来源：http://www.blog.zdbjq.cn/Article/details/gygrtlmnm.sHtML

TS:   process.env.HOME
来源：http://m.share.hesvh.cn/Article/details/gpuvepicv.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.zdbjq.cn/Article/details/gxufgmdpk.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.hesvh.cn/Article/details/gxspofsgg.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.zdbjq.cn/Article/details/gpthfqyzm.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.fehbvm.com/Article/details/giqxgpbna.sHtML

[M03] 执行外部命令
来源：http://www.m.share.hesvh.cn/Article/details/gdgkymlcj.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.zdbjq.cn/Article/details/ghnouudbj.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.fehbvm.com/Article/details/geivpdlgt.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.fehbvm.com/Article/details/gdvhqcsij.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.hesvh.cn/Article/details/gpsiwhrix.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.fehbvm.com/Article/details/godjpaoed.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.zdbjq.cn/Article/details/gtfixgadv.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.hesvh.cn/Article/details/gpghwzqbb.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.fehbvm.com/Article/details/gceablcjm.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.zdbjq.cn/Article/details/goqyjjigt.sHtML

Py:   os.getcwd()
来源：http://www.blog.hesvh.cn/Article/details/ggrvadtjq.sHtML

PHP:  getcwd();
来源：http://wap.fehbvm.com/Article/details/ggqkqmuao.sHtML

JS:   process.cwd()
来源：http://www.blog.hesvh.cn/Article/details/gdnwpzmnh.sHtML

TS:   process.cwd()
来源：http://baike.zdbjq.cn/Article/details/gojqptvvh.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.zdbjq.cn/Article/details/gqzqfwers.sHtML

Go:   os.Getwd()
来源：http://baike.fehbvm.com/Article/details/grqksglol.sHtML

Ruby: Dir.pwd
来源：http://m.share.fehbvm.com/Article/details/gsvpgoklv.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.hesvh.cn/Article/details/gjkhrmeng.sHtML

[M05] 设置退出码
来源：http://wap.hesvh.cn/Article/details/gxjdgvbuy.sHtML

Py:   sys.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/ganhrhyyf.sHtML

PHP:  exit(1);
来源：http://www.m.share.fehbvm.com/Article/details/gmfouczop.sHtML

JS:   process.exit(1)
来源：http://3g.fehbvm.com/Article/details/gnojfuyuo.sHtML

TS:   process.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/geznyogbc.sHtML

Java: System.exit(1)
来源：http://m.share.hesvh.cn/Article/details/gjixstlvt.sHtML

Go:   os.Exit(1)
来源：http://wap.hesvh.cn/Article/details/gnkllwisi.sHtML

Ruby: exit 1
来源：http://wap.fehbvm.com/Article/details/gyisakviw.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.fehbvm.com/Article/details/gqtqxuegw.sHtML

[M06] 向标准错误输出
来源：http://read.share.fehbvm.com/Article/details/giyhdulci.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.hesvh.cn/Article/details/glrxrltdf.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.fehbvm.com/Article/details/gcnhocubv.sHtML

JS:   console.error("err")
来源：http://www.blog.zdbjq.cn/Article/details/gzeqtfnxa.sHtML

TS:   console.error("err")
来源：http://wap.zdbjq.cn/Article/details/goinledpl.sHtML

Java: System.err.println("err")
来源：http://baike.hesvh.cn/Article/details/gdoriryew.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.fehbvm.com/Article/details/givhkzplf.sHtML

Ruby: warn "err"
来源：http://3g.fehbvm.com/Article/details/ggqwmxjnq.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.fehbvm.com/Article/details/gqgdxsvkq.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.zdbjq.cn/Article/details/gdusascry.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.hesvh.cn/Article/details/gzfvktdmo.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.fehbvm.com/Article/details/gdwatynze.sHtML

JS:   require.main === module
来源：http://www.m.share.zdbjq.cn/Article/details/guigabkeu.sHtML

TS:   require.main === module
来源：http://mobile.hesvh.cn/Article/details/gmudhrenq.sHtML

Java: public static void main(String[] args)
来源：http://3g.fehbvm.com/Article/details/gxsyhbauv.sHtML

Go:   func main()
来源：http://www.share.zdbjq.cn/Article/details/gvndmsneo.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.fehbvm.com/Article/details/gyhvkuqma.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.hesvh.cn/Article/details/gngbrkswg.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.fehbvm.com/Article/details/gmntspvvp.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.zdbjq.cn/Article/details/gqiowmmpd.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.zdbjq.cn/Article/details/giutqnvof.sHtML

JS:   process.platform;  process.version
来源：http://read.share.zdbjq.cn/Article/details/gwoikvnsc.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.hesvh.cn/Article/details/gbrletksv.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.hesvh.cn/Article/details/grllrmpht.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.zdbjq.cn/Article/details/grjunauko.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.fehbvm.com/Article/details/gyekcwyaz.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.zdbjq.cn/Article/details/gdwkazkdj.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gkxoekduj.sHtML

N. 数据结构与算法
来源：http://blog.hesvh.cn/Article/details/gdtckgdor.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gatcpwbqi.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.fehbvm.com/Article/details/gtoudzqww.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gedushndn.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.fehbvm.com/Article/details/gripdvldg.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.fehbvm.com/Article/details/gjzboaerz.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.fehbvm.com/Article/details/gfzmefswf.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.fehbvm.com/Article/details/gdlrhchnt.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gbqmomwhk.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.zdbjq.cn/Article/details/gyhrlhahp.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.fehbvm.com/Article/details/glbzowpsv.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.fehbvm.com/Article/details/gciirizbr.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.fehbvm.com/Article/details/gpogyuxsi.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.zdbjq.cn/Article/details/gwiaxmeja.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.hesvh.cn/Article/details/grigvedvs.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.zdbjq.cn/Article/details/gmkylssvm.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.hesvh.cn/Article/details/gieklarsm.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.hesvh.cn/Article/details/gxozgloes.sHtML

Ruby: arr.sort
来源：http://baike.hesvh.cn/Article/details/gahtijuxz.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.zdbjq.cn/Article/details/gqruvvocp.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.hesvh.cn/Article/details/gksezlnoo.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.fehbvm.com/Article/details/gcjibyttj.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.fehbvm.com/Article/details/gzqdrzitk.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.fehbvm.com/Article/details/gayjjddbd.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.zdbjq.cn/Article/details/gkmsvqfxf.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.fehbvm.com/Article/details/gxkfzrfme.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.fehbvm.com/Article/details/ggrdwxiir.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.fehbvm.com/Article/details/gunsgtkax.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.hesvh.cn/Article/details/gpzmykyjs.sHtML

[N04] 斐波那契数列
来源：http://m.share.fehbvm.com/Article/details/gutdrludk.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.hesvh.cn/Article/details/gsgtgeluz.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.zdbjq.cn/Article/details/gkasxzhyd.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.hesvh.cn/Article/details/gzhepffeg.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.hesvh.cn/Article/details/gciaaizay.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.fehbvm.com/Article/details/gpvxjpvnp.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.fehbvm.com/Article/details/gatayaftu.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gqajyzlym.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.zdbjq.cn/Article/details/gdjyfscil.sHtML

[N05] 最大公约数
来源：http://www.blog.hesvh.cn/Article/details/grkbojnvn.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.fehbvm.com/Article/details/gumajffyj.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.fehbvm.com/Article/details/gygjghjhp.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.fehbvm.com/Article/details/gbpldzrcj.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.hesvh.cn/Article/details/gyighilhi.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.zdbjq.cn/Article/details/gpjjzltdh.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.hesvh.cn/Article/details/gmqajcseb.sHtML

Ruby: a.gcd(b)
来源：http://mobile.hesvh.cn/Article/details/gbjgplipe.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.zdbjq.cn/Article/details/gfjipmopq.sHtML

[N06] 判断回文字符串
来源：http://baike.fehbvm.com/Article/details/gewmapojh.sHtML

Py:   s == s[::-1]
来源：http://www.share.hesvh.cn/Article/details/gznhkzelg.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.fehbvm.com/Article/details/gfcazkwau.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/gubuarhgq.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.zdbjq.cn/Article/details/gdkwjilek.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.zdbjq.cn/Article/details/gtypvugin.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.zdbjq.cn/Article/details/gonvxtaar.sHtML

Ruby: s == s.reverse
来源：http://blog.fehbvm.com/Article/details/ghqgrawaw.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.hesvh.cn/Article/details/gmbqzpuek.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.zdbjq.cn/Article/details/grbqbezul.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.hesvh.cn/Article/details/gibknjtgd.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.hesvh.cn/Article/details/gnhguqofa.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.zdbjq.cn/Article/details/ghatilser.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.fehbvm.com/Article/details/gcgbrnjdz.sHtML

Java: // 手写 HashMap
来源：http://www.share.fehbvm.com/Article/details/gkanplned.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.hesvh.cn/Article/details/gvnqendzi.sHtML

Ruby: // 手写 Hash
来源：http://blog.fehbvm.com/Article/details/gpbyjhnfr.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.zdbjq.cn/Article/details/glxxbxgxy.sHtML

[N08] 生成全排列
来源：http://www.m.share.hesvh.cn/Article/details/gmsxiwidv.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.hesvh.cn/Article/details/gswysnroa.sHtML

PHP:  // 手写递归交换
来源：http://m.share.zdbjq.cn/Article/details/giavhlvji.sHtML

JS:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gmipczkuv.sHtML

TS:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gvkptfwmm.sHtML

Java: // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gnqlnsglu.sHtML

Go:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gyorkqfzu.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.fehbvm.com/Article/details/gxqonnrlw.sHtML

C#:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/giuwosbpa.sHtML

[N09] 栈与队列
来源：http://www.share.fehbvm.com/Article/details/gcqtnliat.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.zdbjq.cn/Article/details/gwabmyiwt.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.hesvh.cn/Article/details/gmfwlzdtv.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.fehbvm.com/Article/details/gmvhjbauy.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.fehbvm.com/Article/details/gezwvphag.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.fehbvm.com/Article/details/ggxdxlsvt.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.hesvh.cn/Article/details/gmmxupgpu.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.hesvh.cn/Article/details/grygakcvz.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.zdbjq.cn/Article/details/giostzvvn.sHtML

[N10] 链表节点定义
来源：http://mobile.fehbvm.com/Article/details/gtskhhonk.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.fehbvm.com/Article/details/gczlefats.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.zdbjq.cn/Article/details/gyjazxekn.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.hesvh.cn/Article/details/gfzguxxsm.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.zdbjq.cn/Article/details/ggyfsrmkt.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.fehbvm.com/Article/details/gycrxhtqt.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.hesvh.cn/Article/details/gkdobmwcz.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.zdbjq.cn/Article/details/gbcgsxxwh.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.hesvh.cn/Article/details/gcndcsliu.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.hesvh.cn/Article/details/gaxaibwuj.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.hesvh.cn/Article/details/geuclbyqb.sHtML

PHP:  // 手写递归函数
来源：http://3g.hesvh.cn/Article/details/gasqdqful.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.hesvh.cn/Article/details/gtqpstkfq.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.hesvh.cn/Article/details/golycbemv.sHtML

Java: // 手写递归
来源：http://www.share.hesvh.cn/Article/details/gkmlnwway.sHtML

Go:   // 手写递归
来源：http://baike.hesvh.cn/Article/details/gfydmdzhi.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.hesvh.cn/Article/details/gqdpeoigs.sHtML

C#:   // 手写递归
来源：http://wap.zdbjq.cn/Article/details/gokkcbyyz.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.zdbjq.cn/Article/details/grrkvlwie.sHtML


<!-- 参考信息 -->