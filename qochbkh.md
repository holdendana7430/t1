代发 wailian999

JS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.hesvh.cn/Article/details/gedkunski.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://m.share.hesvh.cn/Article/details/gmawgglsn.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.share.zdbjq.cn/Article/details/gnyfgnugk.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://m.share.fehbvm.com/Article/details/gxxyjkikn.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.zdbjq.cn/Article/details/gaisstysk.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.blog.zdbjq.cn/Article/details/gnwsxbdry.sHtML

[K04] 读取 JSON 文件
来源：http://read.share.fehbvm.com/Article/details/giivtpyme.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wap.fehbvm.com/Article/details/glubvewrr.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mobile.zdbjq.cn/Article/details/gevaasddl.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.fehbvm.com/Article/details/gxxefepzy.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.fehbvm.com/Article/details/gutafuewp.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://blog.hesvh.cn/Article/details/ganxjpbmd.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://baike.zdbjq.cn/Article/details/gkkaxzbme.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.m.share.zdbjq.cn/Article/details/gxmiwvngj.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://blog.fehbvm.com/Article/details/gfcewrabd.sHtML

[K05] 深拷贝对象
来源：http://m.share.zdbjq.cn/Article/details/gogvxeoqm.sHtML

Py:   copy.deepcopy(obj)
来源：http://read.share.hesvh.cn/Article/details/gatphaywv.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.fehbvm.com/Article/details/gsebehglx.sHtML

JS:   structuredClone(obj)
来源：http://wap.hesvh.cn/Article/details/gvrllpety.sHtML

TS:   structuredClone(obj)
来源：http://mobile.hesvh.cn/Article/details/ghboeejte.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.zdbjq.cn/Article/details/ghfgtdvjt.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.fehbvm.com/Article/details/gzkbnzyxk.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://m.share.hesvh.cn/Article/details/gimcmcgbr.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://blog.zdbjq.cn/Article/details/gojevrjck.sHtML

[K06] 解析 URL 查询串
来源：http://baike.hesvh.cn/Article/details/gwrsurzyc.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://read.share.fehbvm.com/Article/details/gxreabfwl.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mobile.zdbjq.cn/Article/details/gqnqosxis.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.hesvh.cn/Article/details/ghyrancjd.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.zdbjq.cn/Article/details/gbjnmrcgs.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://3g.fehbvm.com/Article/details/grrdsjcat.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.hesvh.cn/Article/details/glfuifiyu.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mobile.zdbjq.cn/Article/details/gybtaeahn.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://blog.fehbvm.com/Article/details/guuriisrj.sHtML

[K07] 进制转换
来源：http://www.blog.zdbjq.cn/Article/details/gjzrcfzqo.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.share.fehbvm.com/Article/details/gfceatqrr.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.m.share.zdbjq.cn/Article/details/gyjqapjlf.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.hesvh.cn/Article/details/gkzukzqnk.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.share.zdbjq.cn/Article/details/gjaaxezds.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.blog.fehbvm.com/Article/details/geloulrit.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.fehbvm.com/Article/details/gsblowigj.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.blog.fehbvm.com/Article/details/gwlwnrycw.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.zdbjq.cn/Article/details/gdtwjjzkm.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://mobile.hesvh.cn/Article/details/ghqtllgug.sHtML

Py:   pickle.dumps(obj)
来源：http://blog.hesvh.cn/Article/details/gwlvvvoks.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://3g.hesvh.cn/Article/details/gojmdxdzh.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://m.share.fehbvm.com/Article/details/grbufmtbw.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.fehbvm.com/Article/details/gulexaarf.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.m.share.zdbjq.cn/Article/details/gizuyumaj.sHtML

Go:   encoding/gob
来源：http://m.share.hesvh.cn/Article/details/gwxkdbwbm.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.hesvh.cn/Article/details/gxwilrpxi.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.fehbvm.com/Article/details/gpuxsjshq.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gyvrlvfnf.sHtML

L. 网络请求
来源：http://www.blog.hesvh.cn/Article/details/gswdbmini.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gtvolnqqs.sHtML

[L01] 发送 GET 请求
来源：http://www.share.hesvh.cn/Article/details/gubssqwqz.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://baike.zdbjq.cn/Article/details/gpgjoyiob.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.m.share.zdbjq.cn/Article/details/ganjzkxrv.sHtML

JS:   await fetch(url)
来源：http://www.m.share.fehbvm.com/Article/details/glipersrz.sHtML

TS:   await fetch(url)
来源：http://baike.hesvh.cn/Article/details/ggiythurn.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.fehbvm.com/Article/details/ghwdziqwu.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.hesvh.cn/Article/details/gtwjobhjf.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.fehbvm.com/Article/details/gylynihqj.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.hesvh.cn/Article/details/gzxoumnji.sHtML

[L02] 发送 POST JSON
来源：http://baike.fehbvm.com/Article/details/gqxkbsyfp.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.hesvh.cn/Article/details/ggaxqtyzp.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.hesvh.cn/Article/details/gohogglte.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.hesvh.cn/Article/details/gbtipzrdx.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.hesvh.cn/Article/details/gzxfnmjvs.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.hesvh.cn/Article/details/gnmxrujoz.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.zdbjq.cn/Article/details/gsaokmqxk.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.hesvh.cn/Article/details/gckhvzkng.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.hesvh.cn/Article/details/gdqqpbxxf.sHtML

[L03] 设置自定义请求头
来源：http://wap.fehbvm.com/Article/details/gxeemnrbv.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.hesvh.cn/Article/details/gsqwtavno.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.m.share.fehbvm.com/Article/details/gkktdtqmc.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.zdbjq.cn/Article/details/gdbzmsrmc.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.fehbvm.com/Article/details/gyjgrhhnd.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.hesvh.cn/Article/details/gfccfgmnl.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.fehbvm.com/Article/details/gvqcywyti.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wap.zdbjq.cn/Article/details/gqxygaydt.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.zdbjq.cn/Article/details/galcoildz.sHtML

[L04] 设置超时
来源：http://wap.fehbvm.com/Article/details/gzhacbiof.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.fehbvm.com/Article/details/gapclbsak.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.zdbjq.cn/Article/details/gcqyqqzqw.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.zdbjq.cn/Article/details/gcnuvwiqz.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.hesvh.cn/Article/details/gikbohkvh.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.fehbvm.com/Article/details/ggkfotbdy.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.zdbjq.cn/Article/details/gwqwargtq.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.fehbvm.com/Article/details/ggrvxfgzs.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.zdbjq.cn/Article/details/gaqnbwjrv.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.hesvh.cn/Article/details/ggnbddukk.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.hesvh.cn/Article/details/guocfakey.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.zdbjq.cn/Article/details/gmlemxsfk.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.fehbvm.com/Article/details/gymbvmixs.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.fehbvm.com/Article/details/gfiwpqsle.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.hesvh.cn/Article/details/gdftpngba.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.zdbjq.cn/Article/details/gnrupplom.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.hesvh.cn/Article/details/gczfyldef.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gfzvafjfv.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.fehbvm.com/Article/details/gptejeymq.sHtML

Py:   resp.json()
来源：http://blog.hesvh.cn/Article/details/gwhfeznpm.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.zdbjq.cn/Article/details/gyqtsognd.sHtML

JS:   await resp.json()
来源：http://www.blog.hesvh.cn/Article/details/gvlwwpsnb.sHtML

TS:   await resp.json()
来源：http://read.share.zdbjq.cn/Article/details/gomrwxpcp.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.zdbjq.cn/Article/details/gripfwnft.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.zdbjq.cn/Article/details/gvqrwnnox.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.fehbvm.com/Article/details/gwhgogwbb.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.hesvh.cn/Article/details/gijgccvrg.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.zdbjq.cn/Article/details/gklsxbjok.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.zdbjq.cn/Article/details/gytksytwi.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.zdbjq.cn/Article/details/gbtbfqmel.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.zdbjq.cn/Article/details/gqyhalxno.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.zdbjq.cn/Article/details/gnifhtusw.sHtML

Java: resp.statusCode()
来源：http://mobile.zdbjq.cn/Article/details/gtamgsytn.sHtML

Go:   resp.StatusCode
来源：http://www.share.zdbjq.cn/Article/details/gsednbnqh.sHtML

Ruby: resp.code.to_i
来源：http://read.share.fehbvm.com/Article/details/gvpvimved.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.hesvh.cn/Article/details/gdelovfab.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.zdbjq.cn/Article/details/gvwilgabf.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.zdbjq.cn/Article/details/gizbbiihh.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.fehbvm.com/Article/details/ggooipayr.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.zdbjq.cn/Article/details/goseigijq.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.zdbjq.cn/Article/details/gcevaywwy.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.hesvh.cn/Article/details/gomftgbkr.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.zdbjq.cn/Article/details/gkosgrxvb.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.zdbjq.cn/Article/details/gbavimyon.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.fehbvm.com/Article/details/gvnlqhruf.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gkztltcyk.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.hesvh.cn/Article/details/gsatzjvgd.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gavlxkosi.sHtML

[M01] 读取命令行参数
来源：http://wap.hesvh.cn/Article/details/gpyhnunkc.sHtML

Py:   sys.argv[1:]
来源：http://mobile.hesvh.cn/Article/details/gjdieenmb.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.fehbvm.com/Article/details/gvwdwgcsh.sHtML

JS:   process.argv.slice(2)
来源：http://3g.fehbvm.com/Article/details/gmqxmqcyv.sHtML

TS:   process.argv.slice(2)
来源：http://blog.fehbvm.com/Article/details/ganrtdyew.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.hesvh.cn/Article/details/gmdpijvmp.sHtML

Go:   os.Args[1:]
来源：http://baike.fehbvm.com/Article/details/gaxdjyzws.sHtML

Ruby: ARGV
来源：http://baike.zdbjq.cn/Article/details/gfoaryecp.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.fehbvm.com/Article/details/gehqeahpn.sHtML

[M02] 读取环境变量
来源：http://www.share.fehbvm.com/Article/details/gmpighkhc.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.zdbjq.cn/Article/details/gzxxffrsj.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.zdbjq.cn/Article/details/genooasnm.sHtML

JS:   process.env.HOME
来源：http://3g.hesvh.cn/Article/details/gjoylguon.sHtML

TS:   process.env.HOME
来源：http://baike.hesvh.cn/Article/details/gforjksdz.sHtML

Java: System.getenv("HOME")
来源：http://read.share.fehbvm.com/Article/details/gudxrkuuh.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.zdbjq.cn/Article/details/ggyetzlgf.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.zdbjq.cn/Article/details/gbhsqjdci.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.fehbvm.com/Article/details/gdtbwetxq.sHtML

[M03] 执行外部命令
来源：http://www.share.zdbjq.cn/Article/details/gljuothfe.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.zdbjq.cn/Article/details/gfrvpjikv.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.zdbjq.cn/Article/details/gnesaurpk.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.zdbjq.cn/Article/details/gwwrfbtkx.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.zdbjq.cn/Article/details/gnzvttxcz.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.fehbvm.com/Article/details/ghcctxldt.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.fehbvm.com/Article/details/gqdwajary.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.hesvh.cn/Article/details/gavcbjxhj.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.zdbjq.cn/Article/details/gxqfaorvo.sHtML

[M04] 获取当前工作目录
来源：http://read.share.zdbjq.cn/Article/details/gnvcvdksa.sHtML

Py:   os.getcwd()
来源：http://www.share.hesvh.cn/Article/details/gswknzabe.sHtML

PHP:  getcwd();
来源：http://www.share.hesvh.cn/Article/details/gusuurjki.sHtML

JS:   process.cwd()
来源：http://3g.fehbvm.com/Article/details/giwvgwngg.sHtML

TS:   process.cwd()
来源：http://www.m.share.hesvh.cn/Article/details/gyummymmz.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.fehbvm.com/Article/details/gwjwoqaes.sHtML

Go:   os.Getwd()
来源：http://www.share.fehbvm.com/Article/details/gyiowofqq.sHtML

Ruby: Dir.pwd
来源：http://read.share.hesvh.cn/Article/details/gkbbwcqmq.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.hesvh.cn/Article/details/gizsrgcet.sHtML

[M05] 设置退出码
来源：http://www.m.share.fehbvm.com/Article/details/gcowfmjyl.sHtML

Py:   sys.exit(1)
来源：http://blog.hesvh.cn/Article/details/gkfwsrfdx.sHtML

PHP:  exit(1);
来源：http://mobile.hesvh.cn/Article/details/gdbgiqrxj.sHtML

JS:   process.exit(1)
来源：http://mobile.fehbvm.com/Article/details/geswyspmj.sHtML

TS:   process.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gckceftup.sHtML

Java: System.exit(1)
来源：http://www.share.hesvh.cn/Article/details/gcblnanbt.sHtML

Go:   os.Exit(1)
来源：http://blog.zdbjq.cn/Article/details/gedubipzn.sHtML

Ruby: exit 1
来源：http://read.share.hesvh.cn/Article/details/glnamcdis.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.hesvh.cn/Article/details/grdrfclkq.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.fehbvm.com/Article/details/gayuhywjw.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.zdbjq.cn/Article/details/gttqpopgy.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.hesvh.cn/Article/details/goxptnzjb.sHtML

JS:   console.error("err")
来源：http://www.blog.fehbvm.com/Article/details/gyxmxnnfw.sHtML

TS:   console.error("err")
来源：http://www.share.zdbjq.cn/Article/details/gcfcdnkvy.sHtML

Java: System.err.println("err")
来源：http://www.blog.fehbvm.com/Article/details/gzdiixgfx.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.zdbjq.cn/Article/details/gbfdodsfd.sHtML

Ruby: warn "err"
来源：http://www.share.hesvh.cn/Article/details/gimkxolkf.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.fehbvm.com/Article/details/gbiefirdb.sHtML

[M07] 判断是否为主入口
来源：http://wap.fehbvm.com/Article/details/gtstiluqa.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.fehbvm.com/Article/details/gyzbdnvmh.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.zdbjq.cn/Article/details/goczjjqnj.sHtML

JS:   require.main === module
来源：http://m.share.hesvh.cn/Article/details/glhdkgzqp.sHtML

TS:   require.main === module
来源：http://www.m.share.hesvh.cn/Article/details/gvhhqkzip.sHtML

Java: public static void main(String[] args)
来源：http://read.share.fehbvm.com/Article/details/gcjnrfmbf.sHtML

Go:   func main()
来源：http://www.blog.fehbvm.com/Article/details/grjkvmgln.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.fehbvm.com/Article/details/guuxpjdvt.sHtML

C#:   static void Main(string[] args)
来源：http://baike.zdbjq.cn/Article/details/gkpcieoro.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.hesvh.cn/Article/details/guuzdeshq.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.zdbjq.cn/Article/details/gtmogubms.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.zdbjq.cn/Article/details/ghlormkeg.sHtML

JS:   process.platform;  process.version
来源：http://3g.fehbvm.com/Article/details/gbhchdylo.sHtML

TS:   process.platform;  process.version
来源：http://mobile.fehbvm.com/Article/details/gdikhgpwt.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.fehbvm.com/Article/details/gzjljddth.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.zdbjq.cn/Article/details/gfucxpkjq.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.fehbvm.com/Article/details/gpnrrbyby.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.fehbvm.com/Article/details/gkocudake.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gznjejdxg.sHtML

N. 数据结构与算法
来源：http://mobile.hesvh.cn/Article/details/gkttxphgl.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gfwiupjkd.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.fehbvm.com/Article/details/gidrmsglj.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.zdbjq.cn/Article/details/grfwfnhqv.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.zdbjq.cn/Article/details/gmxmwnbqr.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.fehbvm.com/Article/details/gvuqttvdr.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.hesvh.cn/Article/details/gncfzpbpu.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.fehbvm.com/Article/details/gozltjggi.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gnwfzxfrc.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.zdbjq.cn/Article/details/ggyhzllgd.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gwqktfnrv.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.zdbjq.cn/Article/details/gmnlmsgkn.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.fehbvm.com/Article/details/gryimctgi.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.fehbvm.com/Article/details/gevjhdzis.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.zdbjq.cn/Article/details/gttpnzffi.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.hesvh.cn/Article/details/gyrtiwres.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.fehbvm.com/Article/details/giueggveq.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.fehbvm.com/Article/details/gwpksxyrb.sHtML

Ruby: arr.sort
来源：http://blog.zdbjq.cn/Article/details/ggpgdxdvq.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.zdbjq.cn/Article/details/gukqgzlwk.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.fehbvm.com/Article/details/gcawxzrcb.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.fehbvm.com/Article/details/gytghfphk.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.zdbjq.cn/Article/details/gkxdujhuj.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.zdbjq.cn/Article/details/gdbnkulrc.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.fehbvm.com/Article/details/guhswkqjk.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.fehbvm.com/Article/details/gnvpwlenq.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.hesvh.cn/Article/details/galncqclp.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.zdbjq.cn/Article/details/gczvqiljs.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.hesvh.cn/Article/details/gokzinnvo.sHtML

[N04] 斐波那契数列
来源：http://www.share.fehbvm.com/Article/details/gpdlfllry.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.hesvh.cn/Article/details/gymdpnfgg.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.zdbjq.cn/Article/details/gpmixjelh.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.hesvh.cn/Article/details/gknlrllrn.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.fehbvm.com/Article/details/gvpkzdwbr.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.hesvh.cn/Article/details/gndizduec.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.fehbvm.com/Article/details/ggdzuvhih.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.hesvh.cn/Article/details/gzbxkeibg.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.hesvh.cn/Article/details/ggcukkwmr.sHtML

[N05] 最大公约数
来源：http://mobile.hesvh.cn/Article/details/gadwdsrnj.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.fehbvm.com/Article/details/gtoxjosqp.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.fehbvm.com/Article/details/guwavdbnq.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.hesvh.cn/Article/details/giziuiibm.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.fehbvm.com/Article/details/gvvvadgie.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.fehbvm.com/Article/details/gbgjgvzbj.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.hesvh.cn/Article/details/gknflkdww.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.fehbvm.com/Article/details/gqkxhotoq.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.hesvh.cn/Article/details/gnkjygzjw.sHtML

[N06] 判断回文字符串
来源：http://mobile.hesvh.cn/Article/details/gdmnovcoo.sHtML

Py:   s == s[::-1]
来源：http://blog.fehbvm.com/Article/details/ggunebeow.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.fehbvm.com/Article/details/gukdeedym.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/gesjzxmzq.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/gqikcybwp.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.zdbjq.cn/Article/details/gelzqisdf.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.zdbjq.cn/Article/details/gbqtphobw.sHtML

Ruby: s == s.reverse
来源：http://wap.fehbvm.com/Article/details/grvpsrhvx.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.zdbjq.cn/Article/details/gcjgdbxny.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.zdbjq.cn/Article/details/guwxvvypw.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.hesvh.cn/Article/details/gxifgqkgk.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.hesvh.cn/Article/details/grtknihgc.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.fehbvm.com/Article/details/gxaqjmtie.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.hesvh.cn/Article/details/gtvtanoni.sHtML

Java: // 手写 HashMap
来源：http://wap.zdbjq.cn/Article/details/gzsuhervf.sHtML

Go:   // 手写 map[int]int
来源：http://3g.zdbjq.cn/Article/details/gwmlgphgr.sHtML

Ruby: // 手写 Hash
来源：http://wap.hesvh.cn/Article/details/gtlrufktl.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.hesvh.cn/Article/details/gwmhjuffh.sHtML

[N08] 生成全排列
来源：http://m.share.hesvh.cn/Article/details/gwzrmzkmd.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gakpboeho.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.hesvh.cn/Article/details/gwyccrtrh.sHtML

JS:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/ghuihhrqc.sHtML

TS:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/grcyblabq.sHtML

Java: // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gtuaojkxi.sHtML

Go:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gylakapcx.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.hesvh.cn/Article/details/gxsbjyvoh.sHtML

C#:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gynleregs.sHtML

[N09] 栈与队列
来源：http://mobile.zdbjq.cn/Article/details/gkyimouzb.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.zdbjq.cn/Article/details/gmrnxaluu.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/glaewwglj.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.fehbvm.com/Article/details/gzssxigff.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.fehbvm.com/Article/details/gadhkxdhu.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.zdbjq.cn/Article/details/grxsnpyrh.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.fehbvm.com/Article/details/gjsglhuzt.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.hesvh.cn/Article/details/gerzlmpnn.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.hesvh.cn/Article/details/gmwhhohps.sHtML

[N10] 链表节点定义
来源：http://read.share.fehbvm.com/Article/details/gcwjhurjh.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.fehbvm.com/Article/details/guzzzqpav.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.hesvh.cn/Article/details/gsftywxuv.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.zdbjq.cn/Article/details/gkdmwfilc.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.fehbvm.com/Article/details/gxvucqjof.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.fehbvm.com/Article/details/gpyzmbtxt.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.hesvh.cn/Article/details/gttgthfnk.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.zdbjq.cn/Article/details/gaaxplhzk.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.hesvh.cn/Article/details/gtmtigrbr.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.zdbjq.cn/Article/details/gjhocaubg.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.zdbjq.cn/Article/details/gafxrluhl.sHtML

PHP:  // 手写递归函数
来源：http://wap.fehbvm.com/Article/details/govgamewy.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.zdbjq.cn/Article/details/gwwixurxk.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.fehbvm.com/Article/details/gymlepuva.sHtML

Java: // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/gllemrkth.sHtML


<!-- 参考信息 -->