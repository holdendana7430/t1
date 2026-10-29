代发 wailian999

JS:   JSON.stringify(obj, null, 2)
来源：http://mobile.hesvh.cn/Article/details/gmsjkqklw.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://3g.fehbvm.com/Article/details/gfsonezle.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://3g.zdbjq.cn/Article/details/gjepciqgg.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://read.share.hesvh.cn/Article/details/gqzzmalys.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://m.share.zdbjq.cn/Article/details/gzrhszdpg.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://3g.fehbvm.com/Article/details/glmpjgpug.sHtML

[K04] 读取 JSON 文件
来源：http://www.blog.hesvh.cn/Article/details/gwqbikvhn.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wap.hesvh.cn/Article/details/gwhyegiju.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.m.share.hesvh.cn/Article/details/gargzuwhv.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.hesvh.cn/Article/details/gjubcmkdb.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.fehbvm.com/Article/details/gvehrsvog.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://m.share.hesvh.cn/Article/details/gsexbrvdr.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://3g.fehbvm.com/Article/details/gpxnjyxox.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://read.share.hesvh.cn/Article/details/ginzkrxlh.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://3g.hesvh.cn/Article/details/ghkljagbh.sHtML

[K05] 深拷贝对象
来源：http://m.share.hesvh.cn/Article/details/gpvxlldrd.sHtML

Py:   copy.deepcopy(obj)
来源：http://read.share.hesvh.cn/Article/details/gfajlfrrp.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.fehbvm.com/Article/details/gxmbvvuri.sHtML

JS:   structuredClone(obj)
来源：http://read.share.hesvh.cn/Article/details/gzuvjschb.sHtML

TS:   structuredClone(obj)
来源：http://blog.fehbvm.com/Article/details/guknxvafq.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://mobile.hesvh.cn/Article/details/gxaswnlyw.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.share.hesvh.cn/Article/details/grfuwqpgd.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.blog.zdbjq.cn/Article/details/gsukdpupe.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.m.share.fehbvm.com/Article/details/gbopixuuy.sHtML

[K06] 解析 URL 查询串
来源：http://m.share.zdbjq.cn/Article/details/gdoenbdra.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.share.hesvh.cn/Article/details/ghhjvqxqz.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wap.hesvh.cn/Article/details/guthdbglp.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.fehbvm.com/Article/details/grvkkimez.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.fehbvm.com/Article/details/gjyjwwnpf.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.blog.fehbvm.com/Article/details/giedlugyf.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://m.share.hesvh.cn/Article/details/gowaablmz.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.fehbvm.com/Article/details/gfpyjxsuv.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.hesvh.cn/Article/details/gvtgjnnpy.sHtML

[K07] 进制转换
来源：http://read.share.hesvh.cn/Article/details/gawpowtvf.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.zdbjq.cn/Article/details/gynnomxvc.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.hesvh.cn/Article/details/gsxcqfxcf.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wap.hesvh.cn/Article/details/gtsypnrqj.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.blog.hesvh.cn/Article/details/gawfhwzlq.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://read.share.fehbvm.com/Article/details/gzxanijzy.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wap.fehbvm.com/Article/details/gwltgssrs.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://3g.zdbjq.cn/Article/details/gdmkynhtg.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.blog.fehbvm.com/Article/details/ggvqbrqes.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.hesvh.cn/Article/details/gxigezueu.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.zdbjq.cn/Article/details/gkvjgybru.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://3g.hesvh.cn/Article/details/ghlukuwej.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.fehbvm.com/Article/details/gqfmrisgo.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.m.share.zdbjq.cn/Article/details/gliefzguq.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mobile.zdbjq.cn/Article/details/gfxabammx.sHtML

Go:   encoding/gob
来源：http://www.blog.fehbvm.com/Article/details/gnhdmjsnu.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.share.zdbjq.cn/Article/details/gavamenys.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://read.share.hesvh.cn/Article/details/gfnwhruse.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gfdamveoc.sHtML

L. 网络请求
来源：http://blog.zdbjq.cn/Article/details/gwyxuivpk.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/giwalpugt.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.hesvh.cn/Article/details/gwololdjm.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.hesvh.cn/Article/details/gdierysus.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.fehbvm.com/Article/details/gzweqoubm.sHtML

JS:   await fetch(url)
来源：http://read.share.hesvh.cn/Article/details/gywxcppcw.sHtML

TS:   await fetch(url)
来源：http://baike.hesvh.cn/Article/details/giuuhkgrl.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://baike.zdbjq.cn/Article/details/ghlpercym.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.zdbjq.cn/Article/details/gjicqqnvm.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://baike.hesvh.cn/Article/details/gdxlfnqgx.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.zdbjq.cn/Article/details/gwifgsdov.sHtML

[L02] 发送 POST JSON
来源：http://wap.zdbjq.cn/Article/details/gzgwblfwm.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.share.zdbjq.cn/Article/details/gbedpugtp.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://read.share.hesvh.cn/Article/details/gxhssixkl.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.fehbvm.com/Article/details/gvzkrcuwe.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.hesvh.cn/Article/details/glgyxrnzw.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://read.share.hesvh.cn/Article/details/gjavtedud.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.zdbjq.cn/Article/details/gftupbeen.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.zdbjq.cn/Article/details/gelvbwwoj.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.fehbvm.com/Article/details/gbhyqmivk.sHtML

[L03] 设置自定义请求头
来源：http://wap.hesvh.cn/Article/details/gkcicbvpx.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.fehbvm.com/Article/details/glxjtmnvi.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.zdbjq.cn/Article/details/gauhisbag.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.hesvh.cn/Article/details/gvrggdtag.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.fehbvm.com/Article/details/grdsyushb.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.zdbjq.cn/Article/details/ghvkjektr.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.hesvh.cn/Article/details/glaxmzubg.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.fehbvm.com/Article/details/genwjkxtk.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.hesvh.cn/Article/details/gzqsnadmj.sHtML

[L04] 设置超时
来源：http://m.share.hesvh.cn/Article/details/gupxidxqr.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.hesvh.cn/Article/details/gtqadsyms.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.zdbjq.cn/Article/details/gwhzpkmkm.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.hesvh.cn/Article/details/gepnydkiz.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.hesvh.cn/Article/details/ggxzytzuh.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.hesvh.cn/Article/details/gkqfepotf.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.hesvh.cn/Article/details/gomiwcfji.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.fehbvm.com/Article/details/gmxiiojbw.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.fehbvm.com/Article/details/gvabethqe.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.hesvh.cn/Article/details/gzralwuml.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://read.share.zdbjq.cn/Article/details/gbbrunzlm.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.fehbvm.com/Article/details/gtkawvwyo.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blog.zdbjq.cn/Article/details/gdfcwlcit.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.fehbvm.com/Article/details/gukinsknu.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.fehbvm.com/Article/details/gzgftomus.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.fehbvm.com/Article/details/gtjlbgpaj.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.hesvh.cn/Article/details/gieqeuvhl.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.fehbvm.com/Article/details/gnzghcbrq.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.fehbvm.com/Article/details/gidtfbmys.sHtML

Py:   resp.json()
来源：http://mobile.fehbvm.com/Article/details/ginjdmxug.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.hesvh.cn/Article/details/gzpmceesz.sHtML

JS:   await resp.json()
来源：http://baike.fehbvm.com/Article/details/gwutodjqa.sHtML

TS:   await resp.json()
来源：http://blog.fehbvm.com/Article/details/goaalpwej.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.hesvh.cn/Article/details/gwjzmxwlh.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.hesvh.cn/Article/details/gevjodlyj.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.zdbjq.cn/Article/details/gtfpcuioh.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.hesvh.cn/Article/details/gyplmhvhv.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.fehbvm.com/Article/details/gwaxwphzc.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.fehbvm.com/Article/details/ghttcjvri.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.hesvh.cn/Article/details/gbcohvhnh.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.fehbvm.com/Article/details/gjytgfbbw.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.zdbjq.cn/Article/details/gsdqubwmw.sHtML

Java: resp.statusCode()
来源：http://www.m.share.hesvh.cn/Article/details/gcmfepqzg.sHtML

Go:   resp.StatusCode
来源：http://3g.fehbvm.com/Article/details/ggdzhpuvm.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.fehbvm.com/Article/details/gggotbodc.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.fehbvm.com/Article/details/gwugofzop.sHtML

[L08] 并发请求多个地址
来源：http://wap.fehbvm.com/Article/details/ggxgqcmbq.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.hesvh.cn/Article/details/gebdtvzvl.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.fehbvm.com/Article/details/glrrefyni.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fehbvm.com/Article/details/gbggumykc.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.hesvh.cn/Article/details/gbfjzjxnv.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.fehbvm.com/Article/details/gpgvtgbyv.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.fehbvm.com/Article/details/gvvdfxltu.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.zdbjq.cn/Article/details/glrqjbnxq.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.fehbvm.com/Article/details/ghbyvyqzy.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gedejecje.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.zdbjq.cn/Article/details/gesgkflyw.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gzynqlmus.sHtML

[M01] 读取命令行参数
来源：http://3g.hesvh.cn/Article/details/gegoyfdmp.sHtML

Py:   sys.argv[1:]
来源：http://wap.hesvh.cn/Article/details/gmboqbjcu.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.fehbvm.com/Article/details/gzjwiqhgp.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.hesvh.cn/Article/details/ggfwzqcoh.sHtML

TS:   process.argv.slice(2)
来源：http://3g.fehbvm.com/Article/details/gqzjnjufj.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.hesvh.cn/Article/details/gqxuhhnfr.sHtML

Go:   os.Args[1:]
来源：http://read.share.hesvh.cn/Article/details/gmhhvoqml.sHtML

Ruby: ARGV
来源：http://www.m.share.hesvh.cn/Article/details/gyngtmkrs.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.zdbjq.cn/Article/details/glljimbxf.sHtML

[M02] 读取环境变量
来源：http://www.share.hesvh.cn/Article/details/gtjbevblt.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.hesvh.cn/Article/details/gndvyguir.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.hesvh.cn/Article/details/gbwfxdexh.sHtML

JS:   process.env.HOME
来源：http://wap.zdbjq.cn/Article/details/gomxlxyfe.sHtML

TS:   process.env.HOME
来源：http://m.share.zdbjq.cn/Article/details/ggoisjseo.sHtML

Java: System.getenv("HOME")
来源：http://read.share.hesvh.cn/Article/details/grroptlhp.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.fehbvm.com/Article/details/gbydbwfns.sHtML

Ruby: ENV["HOME"]
来源：http://blog.hesvh.cn/Article/details/gwmksntkl.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.fehbvm.com/Article/details/gscpeasxy.sHtML

[M03] 执行外部命令
来源：http://m.share.zdbjq.cn/Article/details/gictslybp.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.hesvh.cn/Article/details/gkxedjcex.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.hesvh.cn/Article/details/gstzabobb.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.zdbjq.cn/Article/details/gakzcbfem.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.zdbjq.cn/Article/details/gdmpvhkaj.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.hesvh.cn/Article/details/gxvknxymd.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.hesvh.cn/Article/details/gkzyngqoz.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.zdbjq.cn/Article/details/gjklurthm.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.fehbvm.com/Article/details/gottbscdr.sHtML

[M04] 获取当前工作目录
来源：http://3g.hesvh.cn/Article/details/glnpappbt.sHtML

Py:   os.getcwd()
来源：http://blog.fehbvm.com/Article/details/gweiauknf.sHtML

PHP:  getcwd();
来源：http://m.share.hesvh.cn/Article/details/gdhxcizcf.sHtML

JS:   process.cwd()
来源：http://read.share.zdbjq.cn/Article/details/gftkhcshx.sHtML

TS:   process.cwd()
来源：http://3g.zdbjq.cn/Article/details/gmpboabzo.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.fehbvm.com/Article/details/gccrubyei.sHtML

Go:   os.Getwd()
来源：http://3g.zdbjq.cn/Article/details/gltxnahxx.sHtML

Ruby: Dir.pwd
来源：http://m.share.fehbvm.com/Article/details/grakgzsnc.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.zdbjq.cn/Article/details/gvnhsyzuw.sHtML

[M05] 设置退出码
来源：http://wap.hesvh.cn/Article/details/gwvtjqwra.sHtML

Py:   sys.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gmksgntcl.sHtML

PHP:  exit(1);
来源：http://www.m.share.fehbvm.com/Article/details/gatsgweko.sHtML

JS:   process.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gffxadcfj.sHtML

TS:   process.exit(1)
来源：http://mobile.fehbvm.com/Article/details/gltvzcwdf.sHtML

Java: System.exit(1)
来源：http://wap.fehbvm.com/Article/details/grbkbpxwf.sHtML

Go:   os.Exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gzkquwxaz.sHtML

Ruby: exit 1
来源：http://blog.hesvh.cn/Article/details/gcfjwzjux.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.fehbvm.com/Article/details/gslyqewvl.sHtML

[M06] 向标准错误输出
来源：http://m.share.hesvh.cn/Article/details/ghseyyzew.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.fehbvm.com/Article/details/guscjmbgk.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.zdbjq.cn/Article/details/gdtjjyhgu.sHtML

JS:   console.error("err")
来源：http://3g.fehbvm.com/Article/details/gollncypz.sHtML

TS:   console.error("err")
来源：http://m.share.fehbvm.com/Article/details/ghygfqgle.sHtML

Java: System.err.println("err")
来源：http://www.blog.hesvh.cn/Article/details/gqklvqlie.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.fehbvm.com/Article/details/gdglftmfz.sHtML

Ruby: warn "err"
来源：http://read.share.zdbjq.cn/Article/details/gxjrwfvuf.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.hesvh.cn/Article/details/gakztobtz.sHtML

[M07] 判断是否为主入口
来源：http://mobile.zdbjq.cn/Article/details/gqmmhvnxm.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.hesvh.cn/Article/details/gmwvzjspf.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.hesvh.cn/Article/details/gelwwtbzs.sHtML

JS:   require.main === module
来源：http://www.m.share.zdbjq.cn/Article/details/glbkiwgpx.sHtML

TS:   require.main === module
来源：http://www.blog.zdbjq.cn/Article/details/gjfyagmgt.sHtML

Java: public static void main(String[] args)
来源：http://mobile.fehbvm.com/Article/details/gelkwysts.sHtML

Go:   func main()
来源：http://blog.hesvh.cn/Article/details/gblqekrru.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.fehbvm.com/Article/details/gokqesaky.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.hesvh.cn/Article/details/gwpacxfxo.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.zdbjq.cn/Article/details/gqsybmmow.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.fehbvm.com/Article/details/ghzhslrnc.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.zdbjq.cn/Article/details/gbzjdgurv.sHtML

JS:   process.platform;  process.version
来源：http://www.share.fehbvm.com/Article/details/gszcwzdam.sHtML

TS:   process.platform;  process.version
来源：http://m.share.fehbvm.com/Article/details/gdxyslksi.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.zdbjq.cn/Article/details/gcninywxs.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.zdbjq.cn/Article/details/guvanruiz.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.hesvh.cn/Article/details/gesifehpw.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.fehbvm.com/Article/details/gqhsprrrq.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gwzhkcxvx.sHtML

N. 数据结构与算法
来源：http://mobile.zdbjq.cn/Article/details/govbcqhye.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gzvtmobpw.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.hesvh.cn/Article/details/gyyymornk.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.fehbvm.com/Article/details/gleuoxzgh.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.hesvh.cn/Article/details/gakvmvkrv.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.fehbvm.com/Article/details/gvvlpcemp.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.fehbvm.com/Article/details/gnkddiolx.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.fehbvm.com/Article/details/gcjjdedyr.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.fehbvm.com/Article/details/gishrfqvc.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.zdbjq.cn/Article/details/gbrswlvnl.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.fehbvm.com/Article/details/gipwydikh.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.zdbjq.cn/Article/details/gxgesaqzs.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.hesvh.cn/Article/details/gloanuzup.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.zdbjq.cn/Article/details/gfqjbxlqm.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.fehbvm.com/Article/details/gyispegpv.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.fehbvm.com/Article/details/gcrzekwvr.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.hesvh.cn/Article/details/gguqeweoy.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.zdbjq.cn/Article/details/grjtdmonk.sHtML

Ruby: arr.sort
来源：http://wap.fehbvm.com/Article/details/gfciokycc.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.fehbvm.com/Article/details/gpkqmvxyx.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.zdbjq.cn/Article/details/gryziwwat.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.zdbjq.cn/Article/details/gcrmhipnm.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.hesvh.cn/Article/details/ghihsdjgp.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.zdbjq.cn/Article/details/gubwqwdwu.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.zdbjq.cn/Article/details/gmustdnth.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.fehbvm.com/Article/details/gbkvdtykd.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.zdbjq.cn/Article/details/gxrzdtqbd.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.fehbvm.com/Article/details/gaybbzdkw.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.zdbjq.cn/Article/details/gwxfilwzc.sHtML

[N04] 斐波那契数列
来源：http://blog.fehbvm.com/Article/details/gaacpvhwz.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.zdbjq.cn/Article/details/gihntrtyd.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.zdbjq.cn/Article/details/gctonwaku.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.hesvh.cn/Article/details/gphsmwrtp.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.hesvh.cn/Article/details/gmjznnisr.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.zdbjq.cn/Article/details/gpusatnez.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.fehbvm.com/Article/details/gekwmsnyk.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.hesvh.cn/Article/details/ghxkobrgn.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gupfghbcc.sHtML

[N05] 最大公约数
来源：http://read.share.hesvh.cn/Article/details/gyumnbdjs.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.hesvh.cn/Article/details/glthfelsq.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.fehbvm.com/Article/details/gclzpqhyr.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.fehbvm.com/Article/details/gykhmwixb.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.fehbvm.com/Article/details/geyuqdkqi.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.hesvh.cn/Article/details/gphhgsbns.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.hesvh.cn/Article/details/gglkzukng.sHtML

Ruby: a.gcd(b)
来源：http://m.share.hesvh.cn/Article/details/gwmxxgseh.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.hesvh.cn/Article/details/gaghqhwhn.sHtML

[N06] 判断回文字符串
来源：http://blog.hesvh.cn/Article/details/grxysdvii.sHtML

Py:   s == s[::-1]
来源：http://read.share.zdbjq.cn/Article/details/gypzfxaay.sHtML

PHP:  $s === strrev($s);
来源：http://3g.zdbjq.cn/Article/details/gjpyrpybq.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/gcvakfowe.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/ghqlupely.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.zdbjq.cn/Article/details/guryuqhyi.sHtML

Go:   // 双指针从两端比较
来源：http://3g.fehbvm.com/Article/details/ghunbsvcu.sHtML

Ruby: s == s.reverse
来源：http://baike.hesvh.cn/Article/details/gqxicjtts.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.zdbjq.cn/Article/details/gknknsjnr.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.zdbjq.cn/Article/details/gcfkvdbha.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.fehbvm.com/Article/details/gpwikwliq.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.zdbjq.cn/Article/details/gboqrnkio.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.hesvh.cn/Article/details/gvroobybg.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.fehbvm.com/Article/details/gahsvajbu.sHtML

Java: // 手写 HashMap
来源：http://mobile.zdbjq.cn/Article/details/gaghcluyw.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.zdbjq.cn/Article/details/gzrqwxebd.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.fehbvm.com/Article/details/gtrwsmxbt.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.zdbjq.cn/Article/details/gsrfpifdy.sHtML

[N08] 生成全排列
来源：http://baike.fehbvm.com/Article/details/gionyvjzf.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.zdbjq.cn/Article/details/gdihuryrc.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.zdbjq.cn/Article/details/gqkechpqr.sHtML

JS:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gkiyqcxje.sHtML

TS:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gdpayfheb.sHtML

Java: // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gnvfntotb.sHtML

Go:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gghcmrzof.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.zdbjq.cn/Article/details/gbolvenoh.sHtML

C#:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gbvllmlpa.sHtML

[N09] 栈与队列
来源：http://3g.zdbjq.cn/Article/details/gbljfypvf.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.hesvh.cn/Article/details/gyatskely.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.fehbvm.com/Article/details/gmflhilqx.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.fehbvm.com/Article/details/gwmumeicy.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.fehbvm.com/Article/details/gpqzxcmjg.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.fehbvm.com/Article/details/gzierzipu.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.zdbjq.cn/Article/details/gymsnabmt.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.zdbjq.cn/Article/details/gvelrxpgy.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.fehbvm.com/Article/details/grniipmeg.sHtML

[N10] 链表节点定义
来源：http://baike.zdbjq.cn/Article/details/gxtmdhygu.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.hesvh.cn/Article/details/gogxdfrry.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.hesvh.cn/Article/details/gquwrrqsk.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.hesvh.cn/Article/details/gckkxszcc.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.hesvh.cn/Article/details/gplcjohvs.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.hesvh.cn/Article/details/gdlfnqjlh.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.zdbjq.cn/Article/details/gufkldear.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.zdbjq.cn/Article/details/ghokulnmx.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.fehbvm.com/Article/details/gsgshfeyz.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.fehbvm.com/Article/details/ggveshbki.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.fehbvm.com/Article/details/gercqeclx.sHtML

PHP:  // 手写递归函数
来源：http://baike.fehbvm.com/Article/details/gjtluzlfk.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.fehbvm.com/Article/details/gpozkgfdi.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.zdbjq.cn/Article/details/gnqhjcpov.sHtML

Java: // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/gejobnhby.sHtML


<!-- 参考信息 -->