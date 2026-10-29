代发 wailian999

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://m.share.zdbjq.cn/Article/details/genwpmxeb.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.fehbvm.com/Article/details/grdvlduzj.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.hesvh.cn/Article/details/gpqneabsh.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.blog.hesvh.cn/Article/details/gnmwzwvvy.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wap.zdbjq.cn/Article/details/gozuyanwe.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://wap.hesvh.cn/Article/details/grpduwort.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://read.share.fehbvm.com/Article/details/gnhztzeda.sHtML

[K05] 深拷贝对象
来源：http://3g.fehbvm.com/Article/details/gdiecrajv.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.fehbvm.com/Article/details/gwwdouyjo.sHtML

PHP:  unserialize(serialize($obj));
来源：http://wap.hesvh.cn/Article/details/gqpfrling.sHtML

JS:   structuredClone(obj)
来源：http://wap.hesvh.cn/Article/details/gyrbizezx.sHtML

TS:   structuredClone(obj)
来源：http://read.share.fehbvm.com/Article/details/gjpmlvebt.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://m.share.fehbvm.com/Article/details/gdunryzjr.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://m.share.zdbjq.cn/Article/details/gkgemvkjw.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.blog.zdbjq.cn/Article/details/gbbtuuesm.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.blog.fehbvm.com/Article/details/gkzmhgvdu.sHtML

[K06] 解析 URL 查询串
来源：http://www.m.share.zdbjq.cn/Article/details/gprqbeuhq.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wap.fehbvm.com/Article/details/gwzxuuezz.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wap.zdbjq.cn/Article/details/gujgrpeob.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.zdbjq.cn/Article/details/gwahgrjxl.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.hesvh.cn/Article/details/gvynfeprx.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.zdbjq.cn/Article/details/gextmbuhm.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://baike.fehbvm.com/Article/details/gtxvomuwd.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mobile.fehbvm.com/Article/details/gzfcliibm.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.zdbjq.cn/Article/details/guylskyfa.sHtML

[K07] 进制转换
来源：http://baike.hesvh.cn/Article/details/gaixsoupr.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.hesvh.cn/Article/details/geyiejwbm.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://baike.hesvh.cn/Article/details/guvkmbpej.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mobile.fehbvm.com/Article/details/gsvpgiccc.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.share.fehbvm.com/Article/details/ghazunvqm.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.zdbjq.cn/Article/details/gxlihugnd.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://blog.zdbjq.cn/Article/details/gbhpxzlqf.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://3g.zdbjq.cn/Article/details/gcuaiadkt.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://baike.fehbvm.com/Article/details/gasbsampe.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://read.share.hesvh.cn/Article/details/goxjmgvwv.sHtML

Py:   pickle.dumps(obj)
来源：http://baike.fehbvm.com/Article/details/gtqswyqou.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.fehbvm.com/Article/details/gcykysgwc.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.zdbjq.cn/Article/details/glzcxfrhm.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://3g.fehbvm.com/Article/details/gakihwcpb.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.zdbjq.cn/Article/details/gjmbipxpf.sHtML

Go:   encoding/gob
来源：http://www.m.share.hesvh.cn/Article/details/gycmpidvd.sHtML

Ruby: Marshal.dump(obj)
来源：http://read.share.hesvh.cn/Article/details/gffvedlnq.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.share.fehbvm.com/Article/details/gurvkkurq.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gqwlkylzg.sHtML

L. 网络请求
来源：http://m.share.hesvh.cn/Article/details/gazkzoigp.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gckcbzrdg.sHtML

[L01] 发送 GET 请求
来源：http://www.share.zdbjq.cn/Article/details/grfikwmnq.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.zdbjq.cn/Article/details/gzugrpebx.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.hesvh.cn/Article/details/geqmdutor.sHtML

JS:   await fetch(url)
来源：http://baike.fehbvm.com/Article/details/gexbpfxkq.sHtML

TS:   await fetch(url)
来源：http://wap.hesvh.cn/Article/details/gwakniylv.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wap.zdbjq.cn/Article/details/gaaoepxxk.sHtML

Go:   resp, err := http.Get(url)
来源：http://m.share.hesvh.cn/Article/details/gglgkmveh.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.zdbjq.cn/Article/details/guqdnmjmw.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.fehbvm.com/Article/details/gtyhgkjeu.sHtML

[L02] 发送 POST JSON
来源：http://m.share.zdbjq.cn/Article/details/gmglchdic.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://m.share.fehbvm.com/Article/details/giaphupey.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://baike.zdbjq.cn/Article/details/ggvrnaxit.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.hesvh.cn/Article/details/gdmqozuqk.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.zdbjq.cn/Article/details/gswkqaviw.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.m.share.hesvh.cn/Article/details/gjrqqkugc.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.hesvh.cn/Article/details/gandguihs.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.zdbjq.cn/Article/details/gnhkaqbrr.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.hesvh.cn/Article/details/gjcvecxux.sHtML

[L03] 设置自定义请求头
来源：http://wap.fehbvm.com/Article/details/gqzjoxdyn.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.hesvh.cn/Article/details/gewktubwv.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.hesvh.cn/Article/details/gekdmffhg.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.zdbjq.cn/Article/details/gimuvgjwl.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.zdbjq.cn/Article/details/glbrbiqft.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.zdbjq.cn/Article/details/gkbomhcwu.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.hesvh.cn/Article/details/grtieseay.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.fehbvm.com/Article/details/gnsglbusr.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.fehbvm.com/Article/details/gvjoaotfm.sHtML

[L04] 设置超时
来源：http://blog.hesvh.cn/Article/details/gixvzexwz.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.zdbjq.cn/Article/details/gjzefkkuu.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.fehbvm.com/Article/details/gbyuxvwug.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.zdbjq.cn/Article/details/gnqvgssyp.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.fehbvm.com/Article/details/gyguwbdnm.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.zdbjq.cn/Article/details/gtjnnjoqw.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.hesvh.cn/Article/details/gszgvxwsz.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.zdbjq.cn/Article/details/gglsexeqo.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.hesvh.cn/Article/details/gsznakwzf.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.fehbvm.com/Article/details/gzpqpidiq.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.fehbvm.com/Article/details/gvnoqunlx.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.zdbjq.cn/Article/details/gulbligek.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.zdbjq.cn/Article/details/ghbxqkjin.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.zdbjq.cn/Article/details/gsyiuyzhu.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.hesvh.cn/Article/details/ggyilrhnm.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.zdbjq.cn/Article/details/gkazkmvji.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.fehbvm.com/Article/details/ggynwvtwu.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.fehbvm.com/Article/details/gjlhtftby.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.fehbvm.com/Article/details/gxqspfgwt.sHtML

Py:   resp.json()
来源：http://m.share.fehbvm.com/Article/details/glfymwzyb.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.fehbvm.com/Article/details/gnfakzfry.sHtML

JS:   await resp.json()
来源：http://3g.fehbvm.com/Article/details/gjtvswmnk.sHtML

TS:   await resp.json()
来源：http://3g.hesvh.cn/Article/details/givrrmhbq.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.fehbvm.com/Article/details/gagxencjn.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.hesvh.cn/Article/details/gfyqdnxlh.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.fehbvm.com/Article/details/gaeotwlip.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.fehbvm.com/Article/details/gqshauvao.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.fehbvm.com/Article/details/gnjqfqncl.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.zdbjq.cn/Article/details/gsvyxiqhq.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.hesvh.cn/Article/details/gokhwqxwk.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.fehbvm.com/Article/details/gtkmygvzk.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.zdbjq.cn/Article/details/gosjaxeym.sHtML

Java: resp.statusCode()
来源：http://3g.zdbjq.cn/Article/details/gbwaezeuh.sHtML

Go:   resp.StatusCode
来源：http://blog.hesvh.cn/Article/details/gvwhghrvs.sHtML

Ruby: resp.code.to_i
来源：http://mobile.hesvh.cn/Article/details/gtjzqpqhr.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.zdbjq.cn/Article/details/gpaizrzmf.sHtML

[L08] 并发请求多个地址
来源：http://www.share.zdbjq.cn/Article/details/gktpxogup.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.zdbjq.cn/Article/details/gynjdcglf.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.fehbvm.com/Article/details/gxsqaglmq.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.hesvh.cn/Article/details/gmwemmfgw.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.hesvh.cn/Article/details/gwkukehtz.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.fehbvm.com/Article/details/gprcjrflv.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.hesvh.cn/Article/details/gkstcadef.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.fehbvm.com/Article/details/guophldli.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.fehbvm.com/Article/details/ghcqutchq.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gvtmbnhai.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.zdbjq.cn/Article/details/gtqkkerlg.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gitxkkddo.sHtML

[M01] 读取命令行参数
来源：http://www.blog.zdbjq.cn/Article/details/gsmcgpmwl.sHtML

Py:   sys.argv[1:]
来源：http://m.share.hesvh.cn/Article/details/gixiqaldv.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.zdbjq.cn/Article/details/govdvwucj.sHtML

JS:   process.argv.slice(2)
来源：http://3g.fehbvm.com/Article/details/gopckaiww.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.hesvh.cn/Article/details/geofhclkm.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.hesvh.cn/Article/details/gxvrudpmx.sHtML

Go:   os.Args[1:]
来源：http://read.share.hesvh.cn/Article/details/gljwxfqkk.sHtML

Ruby: ARGV
来源：http://m.share.zdbjq.cn/Article/details/ggaxhozlo.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.fehbvm.com/Article/details/gwtcaraql.sHtML

[M02] 读取环境变量
来源：http://read.share.hesvh.cn/Article/details/gpqfzadiv.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.hesvh.cn/Article/details/gnkloxjqu.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.zdbjq.cn/Article/details/gdzyevhkh.sHtML

JS:   process.env.HOME
来源：http://baike.fehbvm.com/Article/details/gdhkxcgpo.sHtML

TS:   process.env.HOME
来源：http://wap.zdbjq.cn/Article/details/ggzjpkupe.sHtML

Java: System.getenv("HOME")
来源：http://m.share.hesvh.cn/Article/details/ggjamaeii.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.zdbjq.cn/Article/details/gycmxvliw.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.hesvh.cn/Article/details/gfsvuftma.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.fehbvm.com/Article/details/gsyvbycrx.sHtML

[M03] 执行外部命令
来源：http://blog.zdbjq.cn/Article/details/gaxkjpeiv.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.zdbjq.cn/Article/details/gplwsscqx.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.zdbjq.cn/Article/details/giswjvvin.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.fehbvm.com/Article/details/gfuosnode.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.fehbvm.com/Article/details/guyemhwdn.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.zdbjq.cn/Article/details/gfhoegccp.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.hesvh.cn/Article/details/gbaynovli.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.fehbvm.com/Article/details/gkecvdkxk.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.hesvh.cn/Article/details/glfcjlbwl.sHtML

[M04] 获取当前工作目录
来源：http://www.share.zdbjq.cn/Article/details/grltaygvk.sHtML

Py:   os.getcwd()
来源：http://wap.fehbvm.com/Article/details/gvgzrdpyx.sHtML

PHP:  getcwd();
来源：http://mobile.zdbjq.cn/Article/details/gususiclx.sHtML

JS:   process.cwd()
来源：http://baike.fehbvm.com/Article/details/gqcjvopbh.sHtML

TS:   process.cwd()
来源：http://blog.zdbjq.cn/Article/details/gnkjhpvqg.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.hesvh.cn/Article/details/gtnypbdur.sHtML

Go:   os.Getwd()
来源：http://www.blog.zdbjq.cn/Article/details/gbmnewkbv.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.zdbjq.cn/Article/details/ggixsevgo.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.fehbvm.com/Article/details/gruahhowy.sHtML

[M05] 设置退出码
来源：http://blog.hesvh.cn/Article/details/gnsmfdtrx.sHtML

Py:   sys.exit(1)
来源：http://read.share.fehbvm.com/Article/details/ghpmfkdkf.sHtML

PHP:  exit(1);
来源：http://wap.zdbjq.cn/Article/details/geyagyavt.sHtML

JS:   process.exit(1)
来源：http://baike.fehbvm.com/Article/details/gsjyoudfl.sHtML

TS:   process.exit(1)
来源：http://m.share.hesvh.cn/Article/details/gvajxjked.sHtML

Java: System.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gusqejnrp.sHtML

Go:   os.Exit(1)
来源：http://www.blog.fehbvm.com/Article/details/grwpdwrcz.sHtML

Ruby: exit 1
来源：http://wap.fehbvm.com/Article/details/gjgkxpopa.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.hesvh.cn/Article/details/gywwcgdtb.sHtML

[M06] 向标准错误输出
来源：http://3g.hesvh.cn/Article/details/gqmjimxqp.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.zdbjq.cn/Article/details/gyawgnexk.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.hesvh.cn/Article/details/grezxhinw.sHtML

JS:   console.error("err")
来源：http://3g.hesvh.cn/Article/details/glalwhmjf.sHtML

TS:   console.error("err")
来源：http://3g.zdbjq.cn/Article/details/gpdzaaxpu.sHtML

Java: System.err.println("err")
来源：http://read.share.fehbvm.com/Article/details/golfqpxhh.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.hesvh.cn/Article/details/gbvvfurdo.sHtML

Ruby: warn "err"
来源：http://www.blog.fehbvm.com/Article/details/gouqugmbu.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.zdbjq.cn/Article/details/gvknurwwp.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.fehbvm.com/Article/details/gzhdvwpxr.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.fehbvm.com/Article/details/gqtvepccm.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.zdbjq.cn/Article/details/gdoasiqmw.sHtML

JS:   require.main === module
来源：http://m.share.zdbjq.cn/Article/details/gbhxdwpss.sHtML

TS:   require.main === module
来源：http://read.share.hesvh.cn/Article/details/goxbrelcj.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.zdbjq.cn/Article/details/ghgpvmgrj.sHtML

Go:   func main()
来源：http://baike.fehbvm.com/Article/details/getfzvunz.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.fehbvm.com/Article/details/gjdnzgqxy.sHtML

C#:   static void Main(string[] args)
来源：http://3g.zdbjq.cn/Article/details/geolhqsxb.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.fehbvm.com/Article/details/glqatzwrs.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.fehbvm.com/Article/details/gsaftaznj.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.zdbjq.cn/Article/details/gfjyighjh.sHtML

JS:   process.platform;  process.version
来源：http://baike.zdbjq.cn/Article/details/gslkxlblk.sHtML

TS:   process.platform;  process.version
来源：http://read.share.fehbvm.com/Article/details/grvifgbli.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.fehbvm.com/Article/details/gtrahprrx.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.fehbvm.com/Article/details/giqtnldho.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.zdbjq.cn/Article/details/ghkbthwim.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.fehbvm.com/Article/details/gbonncafi.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gdborqasa.sHtML

N. 数据结构与算法
来源：http://blog.fehbvm.com/Article/details/geozismjk.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/ggqjewgzi.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.zdbjq.cn/Article/details/gdoasmjfm.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gpknogsvy.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.hesvh.cn/Article/details/gxeywvsmc.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.fehbvm.com/Article/details/guvcpvnmt.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.zdbjq.cn/Article/details/ghebkgron.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gidbjqxfe.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.hesvh.cn/Article/details/gnuefwhwk.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.zdbjq.cn/Article/details/gfgxhsvfx.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.fehbvm.com/Article/details/gnbovkcgl.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.fehbvm.com/Article/details/grszopbkf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.hesvh.cn/Article/details/greqouwep.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.hesvh.cn/Article/details/gwwpcvlbi.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.zdbjq.cn/Article/details/gttarvnfr.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.hesvh.cn/Article/details/gfymxkqjk.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.fehbvm.com/Article/details/grmlwbzic.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.fehbvm.com/Article/details/ggozuptup.sHtML

Ruby: arr.sort
来源：http://wap.fehbvm.com/Article/details/gvkodgnaz.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.hesvh.cn/Article/details/gsejtqsjc.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.hesvh.cn/Article/details/gmmejnbdc.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.hesvh.cn/Article/details/gbzihvfud.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.zdbjq.cn/Article/details/gmfjbeuni.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.zdbjq.cn/Article/details/gpyeixfuv.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.hesvh.cn/Article/details/ghyfykoci.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.fehbvm.com/Article/details/govcymgxm.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.fehbvm.com/Article/details/gyuzoatrt.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.hesvh.cn/Article/details/gbbwtndjq.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.hesvh.cn/Article/details/gckhqzdxa.sHtML

[N04] 斐波那契数列
来源：http://m.share.hesvh.cn/Article/details/gtaevwnml.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.hesvh.cn/Article/details/gbtngomnj.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.fehbvm.com/Article/details/gzdrlibnd.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.zdbjq.cn/Article/details/gtdlfzqkj.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.fehbvm.com/Article/details/guifrdfoo.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.zdbjq.cn/Article/details/gumtavrhi.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.fehbvm.com/Article/details/gsosgcarc.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.fehbvm.com/Article/details/glhnfpkol.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.hesvh.cn/Article/details/gywetowrm.sHtML

[N05] 最大公约数
来源：http://www.share.fehbvm.com/Article/details/gzorkfmjr.sHtML

Py:   math.gcd(a, b)
来源：http://blog.hesvh.cn/Article/details/gglvkbvfn.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.zdbjq.cn/Article/details/goaqgablv.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.hesvh.cn/Article/details/glgbnjfws.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.zdbjq.cn/Article/details/glsbqnskf.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.hesvh.cn/Article/details/gzmxaltgl.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.fehbvm.com/Article/details/gkeffxuzw.sHtML

Ruby: a.gcd(b)
来源：http://mobile.fehbvm.com/Article/details/goplhenka.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.hesvh.cn/Article/details/gqgrnqzjf.sHtML

[N06] 判断回文字符串
来源：http://blog.hesvh.cn/Article/details/gttiytmaf.sHtML

Py:   s == s[::-1]
来源：http://blog.hesvh.cn/Article/details/gpyhuhbiw.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.hesvh.cn/Article/details/gvfhqpbdi.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/gcbelrnis.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.zdbjq.cn/Article/details/gyprgyaxj.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.zdbjq.cn/Article/details/gtlhipggh.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.zdbjq.cn/Article/details/gywdupffp.sHtML

Ruby: s == s.reverse
来源：http://3g.hesvh.cn/Article/details/ggirrejpg.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.zdbjq.cn/Article/details/gurlhrloo.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.hesvh.cn/Article/details/gmcicsmff.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.hesvh.cn/Article/details/gmgsleros.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.hesvh.cn/Article/details/gqtezqgvx.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.hesvh.cn/Article/details/gvmzhnebw.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.hesvh.cn/Article/details/gynqbwalx.sHtML

Java: // 手写 HashMap
来源：http://www.share.fehbvm.com/Article/details/gjbjzyfbc.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.zdbjq.cn/Article/details/gkatpbciy.sHtML

Ruby: // 手写 Hash
来源：http://m.share.zdbjq.cn/Article/details/gkhjphfet.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.fehbvm.com/Article/details/gqxvyqbil.sHtML

[N08] 生成全排列
来源：http://m.share.hesvh.cn/Article/details/gbdxzuypl.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.fehbvm.com/Article/details/gkwcekscl.sHtML

PHP:  // 手写递归交换
来源：http://mobile.zdbjq.cn/Article/details/gjugevgau.sHtML

JS:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gpmgqwbkm.sHtML

TS:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gbumeqlxk.sHtML

Java: // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gltbcdynk.sHtML

Go:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/ggpknwlbi.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.hesvh.cn/Article/details/gdqeeehfz.sHtML

C#:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gfuexeutu.sHtML

[N09] 栈与队列
来源：http://mobile.hesvh.cn/Article/details/gnsbwxqby.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.zdbjq.cn/Article/details/gcrdcsuzu.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.fehbvm.com/Article/details/ggnjixwsv.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.hesvh.cn/Article/details/gjxsxwluz.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.fehbvm.com/Article/details/glpzdaogu.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.hesvh.cn/Article/details/gouiwolvl.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.hesvh.cn/Article/details/gejcuxawi.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.hesvh.cn/Article/details/gficrsfpi.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.hesvh.cn/Article/details/gthwtuosz.sHtML

[N10] 链表节点定义
来源：http://www.share.zdbjq.cn/Article/details/gevkvjoyl.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.fehbvm.com/Article/details/gukqmvvcb.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.hesvh.cn/Article/details/gyjsovcnm.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.zdbjq.cn/Article/details/gzcnohrxk.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.zdbjq.cn/Article/details/gjinlgocu.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.hesvh.cn/Article/details/gzskejqoc.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.hesvh.cn/Article/details/glexrmhnv.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.hesvh.cn/Article/details/gzqpnizqx.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.fehbvm.com/Article/details/gclxfyusy.sHtML

[N11] 二叉树中序遍历
来源：http://baike.fehbvm.com/Article/details/gabehgrsv.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.hesvh.cn/Article/details/gngxcfihu.sHtML

PHP:  // 手写递归函数
来源：http://read.share.zdbjq.cn/Article/details/geppjoknn.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.hesvh.cn/Article/details/gheqanvbc.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.zdbjq.cn/Article/details/gwqxsjupp.sHtML

Java: // 手写递归
来源：http://www.blog.zdbjq.cn/Article/details/gumzbebcg.sHtML

Go:   // 手写递归
来源：http://m.share.zdbjq.cn/Article/details/gchlmtgsr.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.zdbjq.cn/Article/details/gxbmmxuti.sHtML

C#:   // 手写递归
来源：http://www.share.fehbvm.com/Article/details/gwfqecifm.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.hesvh.cn/Article/details/gllffhvlz.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.fehbvm.com/Article/details/gplgcnjko.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.hesvh.cn/Article/details/gfofccwsc.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.fehbvm.com/Article/details/gnpoadphn.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.hesvh.cn/Article/details/gwbjumsqx.sHtML


<!-- 参考信息 -->