代发 wailian999

Ruby: JSON.pretty_generate(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gexhgwrlg.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://3g.zdbjq.cn/Article/details/gykrhwyoi.sHtML

[K04] 读取 JSON 文件
来源：http://wap.fehbvm.com/Article/details/gpnusjyrv.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://baike.hesvh.cn/Article/details/gmupeukgr.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wap.hesvh.cn/Article/details/gbjeklgvl.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.zdbjq.cn/Article/details/grkklkqkg.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.fehbvm.com/Article/details/gzitulbkn.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://m.share.hesvh.cn/Article/details/gedrxdgcu.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://m.share.hesvh.cn/Article/details/guzmcdoei.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://read.share.zdbjq.cn/Article/details/gpzzsxern.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.share.zdbjq.cn/Article/details/grylujbhp.sHtML

[K05] 深拷贝对象
来源：http://3g.zdbjq.cn/Article/details/glpobwnmz.sHtML

Py:   copy.deepcopy(obj)
来源：http://blog.hesvh.cn/Article/details/gzhdchnjd.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.fehbvm.com/Article/details/gqanhaauj.sHtML

JS:   structuredClone(obj)
来源：http://www.share.zdbjq.cn/Article/details/gefzcrkly.sHtML

TS:   structuredClone(obj)
来源：http://www.share.fehbvm.com/Article/details/gzejgyrrd.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.zdbjq.cn/Article/details/gprfdewax.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://baike.fehbvm.com/Article/details/godtkqthw.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.share.zdbjq.cn/Article/details/gxiylxilx.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.share.hesvh.cn/Article/details/gngustpmk.sHtML

[K06] 解析 URL 查询串
来源：http://3g.fehbvm.com/Article/details/gxwobusxy.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://read.share.hesvh.cn/Article/details/gavgzqhzi.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://m.share.fehbvm.com/Article/details/gqnbttcdt.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.zdbjq.cn/Article/details/grzffivlb.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.zdbjq.cn/Article/details/gbmenjpsd.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.share.hesvh.cn/Article/details/gygktxcem.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://read.share.zdbjq.cn/Article/details/gxpayvyab.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://m.share.fehbvm.com/Article/details/glzszevee.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://baike.hesvh.cn/Article/details/gsjsoshfc.sHtML

[K07] 进制转换
来源：http://www.blog.zdbjq.cn/Article/details/gyaenmwag.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://baike.zdbjq.cn/Article/details/gcvwunagm.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://m.share.fehbvm.com/Article/details/gvogihfwn.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://m.share.fehbvm.com/Article/details/gumszonlb.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.m.share.hesvh.cn/Article/details/gywrxcujx.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.share.fehbvm.com/Article/details/ggizqowgn.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://3g.fehbvm.com/Article/details/gurtgbvba.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wap.hesvh.cn/Article/details/gguvzouol.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.hesvh.cn/Article/details/gtywsbjcf.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://wap.fehbvm.com/Article/details/gcuosizbu.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gxejskxsy.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://mobile.fehbvm.com/Article/details/ghopsxvdn.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.share.hesvh.cn/Article/details/geibnzpaf.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.blog.hesvh.cn/Article/details/gkjbiythv.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.zdbjq.cn/Article/details/gvmklqfea.sHtML

Go:   encoding/gob
来源：http://www.m.share.zdbjq.cn/Article/details/gwebmenrl.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.blog.zdbjq.cn/Article/details/geounylgi.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.zdbjq.cn/Article/details/gvevmarxu.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gpbrljaat.sHtML

L. 网络请求
来源：http://3g.fehbvm.com/Article/details/gobekozrq.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gpgdlzvyp.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.zdbjq.cn/Article/details/gzuqcwahw.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.hesvh.cn/Article/details/gbivfqpcp.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.zdbjq.cn/Article/details/gktmnszaa.sHtML

JS:   await fetch(url)
来源：http://wap.hesvh.cn/Article/details/gslmbbkco.sHtML

TS:   await fetch(url)
来源：http://www.blog.zdbjq.cn/Article/details/gimoqfobi.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://baike.fehbvm.com/Article/details/gzsytwsux.sHtML

Go:   resp, err := http.Get(url)
来源：http://baike.fehbvm.com/Article/details/gebbxgpbs.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.zdbjq.cn/Article/details/guydqvqzi.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.zdbjq.cn/Article/details/gfbmwbmtk.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.hesvh.cn/Article/details/gqfoibrpl.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://read.share.fehbvm.com/Article/details/gbssczyey.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.fehbvm.com/Article/details/gmukcfedp.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.hesvh.cn/Article/details/ggbgcooji.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.hesvh.cn/Article/details/gybeizagq.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.m.share.zdbjq.cn/Article/details/gosfrswes.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://m.share.zdbjq.cn/Article/details/gfunbuucz.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.zdbjq.cn/Article/details/ggefqytgb.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.hesvh.cn/Article/details/gravitxuf.sHtML

[L03] 设置自定义请求头
来源：http://wap.fehbvm.com/Article/details/gprbebmby.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://read.share.zdbjq.cn/Article/details/gsrufecnk.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.hesvh.cn/Article/details/gjxwbidfk.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.fehbvm.com/Article/details/gvfxpunes.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.hesvh.cn/Article/details/gjvemmoiy.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.zdbjq.cn/Article/details/gfdtqlmjk.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.zdbjq.cn/Article/details/ghembfren.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.zdbjq.cn/Article/details/gudwnynrh.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.hesvh.cn/Article/details/ggpppndcd.sHtML

[L04] 设置超时
来源：http://3g.zdbjq.cn/Article/details/gdmxepsmn.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.hesvh.cn/Article/details/gzjgqcraa.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.zdbjq.cn/Article/details/geziheqfi.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.zdbjq.cn/Article/details/gqndgkdcc.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.zdbjq.cn/Article/details/gjsfzqesd.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.hesvh.cn/Article/details/gajdaqpjb.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.hesvh.cn/Article/details/gbfetygcg.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.zdbjq.cn/Article/details/gfguefsoc.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.fehbvm.com/Article/details/gseclgpxy.sHtML

[L05] 上传文件（multipart）
来源：http://baike.zdbjq.cn/Article/details/gegupgibo.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.hesvh.cn/Article/details/gnxkwhitl.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wap.hesvh.cn/Article/details/gaxrctfnl.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.fehbvm.com/Article/details/gehjaaksr.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.fehbvm.com/Article/details/ghmkgodnj.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.fehbvm.com/Article/details/gflijplmd.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.zdbjq.cn/Article/details/gbnvplssg.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.zdbjq.cn/Article/details/gsvbvuynd.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.zdbjq.cn/Article/details/gyqnfsyeb.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.hesvh.cn/Article/details/gixvhwfwz.sHtML

Py:   resp.json()
来源：http://3g.zdbjq.cn/Article/details/gousqbekw.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.zdbjq.cn/Article/details/gfpzrpjzr.sHtML

JS:   await resp.json()
来源：http://www.blog.fehbvm.com/Article/details/giphragqn.sHtML

TS:   await resp.json()
来源：http://wap.zdbjq.cn/Article/details/gghrsroel.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.zdbjq.cn/Article/details/gyutqdhcw.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.fehbvm.com/Article/details/gzhkgoppt.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.hesvh.cn/Article/details/gtllvkucg.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.hesvh.cn/Article/details/gzvshtzwu.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.zdbjq.cn/Article/details/gyhwtchhv.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.hesvh.cn/Article/details/gwcrymdcp.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.hesvh.cn/Article/details/gbrcepqmc.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.fehbvm.com/Article/details/gbdpzofbx.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.zdbjq.cn/Article/details/gvydrhhpu.sHtML

Java: resp.statusCode()
来源：http://www.m.share.zdbjq.cn/Article/details/ggatausww.sHtML

Go:   resp.StatusCode
来源：http://3g.hesvh.cn/Article/details/gqsvovusx.sHtML

Ruby: resp.code.to_i
来源：http://m.share.fehbvm.com/Article/details/gyxrmozeq.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.hesvh.cn/Article/details/gswxthocx.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.hesvh.cn/Article/details/giiteiwll.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.zdbjq.cn/Article/details/gsocyzyjk.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.fehbvm.com/Article/details/gdrqonxjc.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.zdbjq.cn/Article/details/gyfavczzo.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.hesvh.cn/Article/details/godnctchk.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.fehbvm.com/Article/details/gykjcflpm.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.hesvh.cn/Article/details/grmhyypcl.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.hesvh.cn/Article/details/gswnqznsq.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.fehbvm.com/Article/details/gfsuyonlv.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gvwfhbvus.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.fehbvm.com/Article/details/gastruojp.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gvjlrlzjx.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.hesvh.cn/Article/details/gpagrpfuv.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.fehbvm.com/Article/details/gsfdbjjrb.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.hesvh.cn/Article/details/goemjsqtk.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.hesvh.cn/Article/details/gylghdqxp.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.hesvh.cn/Article/details/gliomojrh.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.fehbvm.com/Article/details/geofyjxiv.sHtML

Go:   os.Args[1:]
来源：http://www.blog.hesvh.cn/Article/details/ganevilwc.sHtML

Ruby: ARGV
来源：http://mobile.fehbvm.com/Article/details/gnwnwlimr.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.hesvh.cn/Article/details/gexqylpqr.sHtML

[M02] 读取环境变量
来源：http://m.share.hesvh.cn/Article/details/gwpomszml.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.zdbjq.cn/Article/details/geffndgan.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.hesvh.cn/Article/details/gjnyiaczi.sHtML

JS:   process.env.HOME
来源：http://www.share.fehbvm.com/Article/details/gvulygyki.sHtML

TS:   process.env.HOME
来源：http://www.blog.hesvh.cn/Article/details/gtqakziyj.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/ghaynqpuw.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.zdbjq.cn/Article/details/gaqyhnowu.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.fehbvm.com/Article/details/gqmtphnvx.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.fehbvm.com/Article/details/ggqgnrjso.sHtML

[M03] 执行外部命令
来源：http://mobile.hesvh.cn/Article/details/gefecljmk.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.zdbjq.cn/Article/details/gmmkfkimj.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.hesvh.cn/Article/details/gqkqkiotq.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.fehbvm.com/Article/details/gikbbloti.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.fehbvm.com/Article/details/gvqbdtkkh.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.zdbjq.cn/Article/details/golsquygw.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.zdbjq.cn/Article/details/gvzbqwoeo.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.zdbjq.cn/Article/details/gtlgmudoa.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.hesvh.cn/Article/details/gdupovkso.sHtML

[M04] 获取当前工作目录
来源：http://blog.zdbjq.cn/Article/details/gmldblgeu.sHtML

Py:   os.getcwd()
来源：http://www.m.share.fehbvm.com/Article/details/grpujgxmk.sHtML

PHP:  getcwd();
来源：http://wap.fehbvm.com/Article/details/gotrbaxez.sHtML

JS:   process.cwd()
来源：http://wap.fehbvm.com/Article/details/gaerpqcdf.sHtML

TS:   process.cwd()
来源：http://blog.hesvh.cn/Article/details/gypaftzcj.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.zdbjq.cn/Article/details/ghgjosrxr.sHtML

Go:   os.Getwd()
来源：http://read.share.fehbvm.com/Article/details/gfvoligwn.sHtML

Ruby: Dir.pwd
来源：http://m.share.hesvh.cn/Article/details/gjrcbdoib.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.zdbjq.cn/Article/details/gosyfyvnr.sHtML

[M05] 设置退出码
来源：http://wap.zdbjq.cn/Article/details/gqtvgxlwr.sHtML

Py:   sys.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gjiuojnko.sHtML

PHP:  exit(1);
来源：http://wap.hesvh.cn/Article/details/gjnpbudat.sHtML

JS:   process.exit(1)
来源：http://baike.zdbjq.cn/Article/details/gdbjkpyru.sHtML

TS:   process.exit(1)
来源：http://baike.fehbvm.com/Article/details/gsegsuldr.sHtML

Java: System.exit(1)
来源：http://blog.hesvh.cn/Article/details/gwxhkppis.sHtML

Go:   os.Exit(1)
来源：http://read.share.zdbjq.cn/Article/details/ggnqehtuk.sHtML

Ruby: exit 1
来源：http://www.blog.hesvh.cn/Article/details/gcswvzzac.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.hesvh.cn/Article/details/gcpnjvosv.sHtML

[M06] 向标准错误输出
来源：http://3g.hesvh.cn/Article/details/gdxamppmf.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.fehbvm.com/Article/details/gjthabkff.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.fehbvm.com/Article/details/gxdjedyrk.sHtML

JS:   console.error("err")
来源：http://www.m.share.fehbvm.com/Article/details/gblbsqwho.sHtML

TS:   console.error("err")
来源：http://wap.hesvh.cn/Article/details/gbrtgbvzt.sHtML

Java: System.err.println("err")
来源：http://blog.hesvh.cn/Article/details/gfxcjsfai.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.zdbjq.cn/Article/details/gkucwiqem.sHtML

Ruby: warn "err"
来源：http://mobile.zdbjq.cn/Article/details/giitxifhm.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.zdbjq.cn/Article/details/gplbnxwxw.sHtML

[M07] 判断是否为主入口
来源：http://baike.hesvh.cn/Article/details/gvasaezyb.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.hesvh.cn/Article/details/gbeytsidu.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.fehbvm.com/Article/details/gyqghrnku.sHtML

JS:   require.main === module
来源：http://3g.fehbvm.com/Article/details/gccgjiysm.sHtML

TS:   require.main === module
来源：http://www.share.fehbvm.com/Article/details/gsdccfjuv.sHtML

Java: public static void main(String[] args)
来源：http://m.share.hesvh.cn/Article/details/gyshwavts.sHtML

Go:   func main()
来源：http://www.m.share.zdbjq.cn/Article/details/gjnczzyzh.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.zdbjq.cn/Article/details/gwdktmbsj.sHtML

C#:   static void Main(string[] args)
来源：http://wap.hesvh.cn/Article/details/gbhjaoxqo.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.fehbvm.com/Article/details/gocaozyif.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.zdbjq.cn/Article/details/ganzqoobz.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.hesvh.cn/Article/details/grkyziznr.sHtML

JS:   process.platform;  process.version
来源：http://3g.fehbvm.com/Article/details/gadgaaibv.sHtML

TS:   process.platform;  process.version
来源：http://blog.hesvh.cn/Article/details/gwwjsoluz.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.zdbjq.cn/Article/details/gmpyehbqy.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.hesvh.cn/Article/details/gprbxmtxi.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.hesvh.cn/Article/details/gadnhvprt.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.hesvh.cn/Article/details/gupimbdow.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/ggwxxwndb.sHtML

N. 数据结构与算法
来源：http://www.m.share.hesvh.cn/Article/details/gkszuazvz.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gyrprzsoe.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.hesvh.cn/Article/details/gxuudzbqq.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/girdwuave.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.zdbjq.cn/Article/details/gzhkteobu.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.hesvh.cn/Article/details/gjoyizrgp.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.zdbjq.cn/Article/details/gtyiqracu.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gjgzdedon.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gjfkgapld.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.fehbvm.com/Article/details/gnhgkcobs.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/giaswntum.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.fehbvm.com/Article/details/gzfspogcj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.zdbjq.cn/Article/details/gvwvwizbx.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.fehbvm.com/Article/details/gixrzncge.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.hesvh.cn/Article/details/gactoucly.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.zdbjq.cn/Article/details/gezcluhse.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.fehbvm.com/Article/details/gryyczzsb.sHtML

Go:   slices.Sort(arr)
来源：http://blog.hesvh.cn/Article/details/glvgnmaum.sHtML

Ruby: arr.sort
来源：http://wap.zdbjq.cn/Article/details/grrpqaada.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.fehbvm.com/Article/details/gyvqztfsx.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.hesvh.cn/Article/details/gzsnpnpzf.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.fehbvm.com/Article/details/ghkieouil.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.fehbvm.com/Article/details/gflpcmylh.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.zdbjq.cn/Article/details/gwadqusnz.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.fehbvm.com/Article/details/goabefzeg.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.fehbvm.com/Article/details/gitorhvke.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.hesvh.cn/Article/details/gtwxgbvci.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.zdbjq.cn/Article/details/gghoacybv.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.hesvh.cn/Article/details/gvgvkarog.sHtML

[N04] 斐波那契数列
来源：http://www.share.zdbjq.cn/Article/details/gcbzytvdc.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.zdbjq.cn/Article/details/gooxtfcbo.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.zdbjq.cn/Article/details/gzotiqoiq.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/ggnyscsps.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/gekbkrcia.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.zdbjq.cn/Article/details/gnibgfzwa.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.zdbjq.cn/Article/details/galpdwksg.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.fehbvm.com/Article/details/gdffzqkqa.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.hesvh.cn/Article/details/gmsupvhll.sHtML

[N05] 最大公约数
来源：http://baike.fehbvm.com/Article/details/gkuqralav.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.zdbjq.cn/Article/details/gclnrtmhk.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.hesvh.cn/Article/details/grwxzphpf.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.hesvh.cn/Article/details/gqjarvpnz.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.zdbjq.cn/Article/details/ggnpltwyk.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.zdbjq.cn/Article/details/gfgkzpwgo.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.hesvh.cn/Article/details/gewmtgmxs.sHtML

Ruby: a.gcd(b)
来源：http://www.share.hesvh.cn/Article/details/glokcciwa.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.fehbvm.com/Article/details/gvvllwqbj.sHtML

[N06] 判断回文字符串
来源：http://mobile.zdbjq.cn/Article/details/gazapswpx.sHtML

Py:   s == s[::-1]
来源：http://read.share.hesvh.cn/Article/details/geslophxe.sHtML

PHP:  $s === strrev($s);
来源：http://blog.fehbvm.com/Article/details/gzkipupkz.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/gnqtxbpbt.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/gcfvraqea.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.hesvh.cn/Article/details/gvujvtqze.sHtML

Go:   // 双指针从两端比较
来源：http://wap.hesvh.cn/Article/details/gkrzcvuyu.sHtML

Ruby: s == s.reverse
来源：http://read.share.fehbvm.com/Article/details/gfskyxxdo.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.fehbvm.com/Article/details/ggnovmfam.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.hesvh.cn/Article/details/gmazssimx.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.hesvh.cn/Article/details/gzmdhilsb.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.fehbvm.com/Article/details/gkhsiveeo.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.zdbjq.cn/Article/details/gbizdpwqy.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.zdbjq.cn/Article/details/gjuvxtwes.sHtML

Java: // 手写 HashMap
来源：http://www.share.zdbjq.cn/Article/details/gbnuamiyh.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.fehbvm.com/Article/details/gqlicedmy.sHtML

Ruby: // 手写 Hash
来源：http://read.share.hesvh.cn/Article/details/gfmbusgof.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.hesvh.cn/Article/details/glxhksvyr.sHtML

[N08] 生成全排列
来源：http://wap.zdbjq.cn/Article/details/gvspvzvjv.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.hesvh.cn/Article/details/gxykzfjgg.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.zdbjq.cn/Article/details/gvlyongnu.sHtML

JS:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gihzqzvyr.sHtML

TS:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gmzlnftrc.sHtML

Java: // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/ghrmrohrf.sHtML

Go:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gvyqkwhfz.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.fehbvm.com/Article/details/gldqcfxmv.sHtML

C#:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gxkczejor.sHtML

[N09] 栈与队列
来源：http://read.share.hesvh.cn/Article/details/gaxulsxrq.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.zdbjq.cn/Article/details/gaqnxzutr.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.hesvh.cn/Article/details/guttyxkiq.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.fehbvm.com/Article/details/ggiobhwst.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.zdbjq.cn/Article/details/gmjitgbuu.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.zdbjq.cn/Article/details/gvgzjgibj.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.hesvh.cn/Article/details/gkfpfdjri.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.hesvh.cn/Article/details/gfbqgzmzw.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.zdbjq.cn/Article/details/gsgfwsmoo.sHtML

[N10] 链表节点定义
来源：http://baike.zdbjq.cn/Article/details/gqthorgcw.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.fehbvm.com/Article/details/gxhgellry.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.zdbjq.cn/Article/details/gtjzmpeno.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.hesvh.cn/Article/details/gtiajtrzd.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.hesvh.cn/Article/details/gzuejbmje.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.hesvh.cn/Article/details/gikqcfzjf.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.hesvh.cn/Article/details/gfdbkrifj.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.hesvh.cn/Article/details/gwwptfznn.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.hesvh.cn/Article/details/gcowpqbym.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.fehbvm.com/Article/details/gevnzrsnr.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.fehbvm.com/Article/details/gnrquvatg.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.fehbvm.com/Article/details/gmexbiurr.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.zdbjq.cn/Article/details/gmnfowxab.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.zdbjq.cn/Article/details/goaxvqokb.sHtML

Java: // 手写递归
来源：http://www.share.fehbvm.com/Article/details/gixxqexjc.sHtML

Go:   // 手写递归
来源：http://baike.zdbjq.cn/Article/details/gyktupqvo.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.zdbjq.cn/Article/details/gaujaegyc.sHtML

C#:   // 手写递归
来源：http://www.share.fehbvm.com/Article/details/gcjzlsqzq.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.hesvh.cn/Article/details/gjkcdswmy.sHtML


<!-- 参考信息 -->