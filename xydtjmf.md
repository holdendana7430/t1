代发 wailian999

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://m.share.hesvh.cn/Article/details/glqcymcyv.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.hesvh.cn/Article/details/gdyuaxwtz.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.zdbjq.cn/Article/details/gbvhzezof.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.share.hesvh.cn/Article/details/gjitbmibo.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://baike.zdbjq.cn/Article/details/gbbjtxzde.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.m.share.fehbvm.com/Article/details/gztgmfdet.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.share.hesvh.cn/Article/details/galoojryi.sHtML

[K05] 深拷贝对象
来源：http://blog.zdbjq.cn/Article/details/gasdxzngr.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.zdbjq.cn/Article/details/gjnmbyzhh.sHtML

PHP:  unserialize(serialize($obj));
来源：http://wap.zdbjq.cn/Article/details/ggyvrxpez.sHtML

JS:   structuredClone(obj)
来源：http://wap.zdbjq.cn/Article/details/gpaikurml.sHtML

TS:   structuredClone(obj)
来源：http://www.blog.hesvh.cn/Article/details/gdpwxjiqn.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://blog.zdbjq.cn/Article/details/gzqaujhrb.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://3g.hesvh.cn/Article/details/gooogunzh.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://baike.hesvh.cn/Article/details/gldyebujr.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.m.share.zdbjq.cn/Article/details/gunjrzqyh.sHtML

[K06] 解析 URL 查询串
来源：http://blog.hesvh.cn/Article/details/ggpnoqinw.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wap.zdbjq.cn/Article/details/gqsmojygk.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://m.share.zdbjq.cn/Article/details/gibjsijnk.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.zdbjq.cn/Article/details/gxzewufcz.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.hesvh.cn/Article/details/gzgawnzsv.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.fehbvm.com/Article/details/gxazvvghw.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.fehbvm.com/Article/details/gjogqonag.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.fehbvm.com/Article/details/gjlmonotd.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.hesvh.cn/Article/details/gypxydlzd.sHtML

[K07] 进制转换
来源：http://blog.fehbvm.com/Article/details/gkjlhlqvq.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mobile.zdbjq.cn/Article/details/gvkcofunn.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wap.fehbvm.com/Article/details/glyinagjz.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.blog.hesvh.cn/Article/details/glfobexwl.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://3g.fehbvm.com/Article/details/grrmeyoyb.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.m.share.hesvh.cn/Article/details/gsvwvrnbv.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://baike.hesvh.cn/Article/details/gzwynkepu.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://blog.hesvh.cn/Article/details/govqhwoip.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.zdbjq.cn/Article/details/gvajjbzgf.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.blog.fehbvm.com/Article/details/gdesukxvi.sHtML

Py:   pickle.dumps(obj)
来源：http://www.blog.hesvh.cn/Article/details/gycvrxjbh.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://mobile.zdbjq.cn/Article/details/grfmttxdn.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.hesvh.cn/Article/details/glfdfuidb.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://blog.zdbjq.cn/Article/details/gdwcmhhvg.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.hesvh.cn/Article/details/gcgzqmyil.sHtML

Go:   encoding/gob
来源：http://read.share.fehbvm.com/Article/details/gehevwevl.sHtML

Ruby: Marshal.dump(obj)
来源：http://m.share.fehbvm.com/Article/details/gfqouednh.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://baike.fehbvm.com/Article/details/gzvtkeshg.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gtuzaswyf.sHtML

L. 网络请求
来源：http://read.share.zdbjq.cn/Article/details/gibwqslej.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gzxsksvie.sHtML

[L01] 发送 GET 请求
来源：http://read.share.zdbjq.cn/Article/details/glppkwmmx.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.hesvh.cn/Article/details/giyvqhtij.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.fehbvm.com/Article/details/gqhidadaj.sHtML

JS:   await fetch(url)
来源：http://wap.fehbvm.com/Article/details/ghrkwukum.sHtML

TS:   await fetch(url)
来源：http://www.share.fehbvm.com/Article/details/glxjpwlsj.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.fehbvm.com/Article/details/gosoypmcu.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.fehbvm.com/Article/details/gfrjdcayr.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://m.share.hesvh.cn/Article/details/gapnfafzy.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.fehbvm.com/Article/details/gpoyxakwn.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.zdbjq.cn/Article/details/gwmutiahn.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.zdbjq.cn/Article/details/ggqgduatx.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://baike.hesvh.cn/Article/details/gzycfzbsz.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.zdbjq.cn/Article/details/gboepkcgv.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.fehbvm.com/Article/details/gnibcodxw.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.fehbvm.com/Article/details/gmgaqjlne.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mobile.zdbjq.cn/Article/details/gkhdfydpc.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.hesvh.cn/Article/details/ghpfgurjk.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.hesvh.cn/Article/details/gzvscdgmb.sHtML

[L03] 设置自定义请求头
来源：http://baike.fehbvm.com/Article/details/gazcyyygq.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://read.share.hesvh.cn/Article/details/gngzytesn.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.zdbjq.cn/Article/details/gwguupgqm.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.fehbvm.com/Article/details/gkdgbipck.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.hesvh.cn/Article/details/gkffuypaj.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.fehbvm.com/Article/details/gxybqkusr.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.zdbjq.cn/Article/details/guohkxbhd.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.fehbvm.com/Article/details/gxwryzgwu.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wap.fehbvm.com/Article/details/gzuqayksg.sHtML

[L04] 设置超时
来源：http://m.share.fehbvm.com/Article/details/gbaqzimqi.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.hesvh.cn/Article/details/gtoozhlok.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.fehbvm.com/Article/details/gfxbpaljn.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.zdbjq.cn/Article/details/ghrjdrjel.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.fehbvm.com/Article/details/gdmobmnph.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.hesvh.cn/Article/details/gxgxkcgns.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.fehbvm.com/Article/details/gkplhlnzy.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.hesvh.cn/Article/details/glvwqlghh.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.zdbjq.cn/Article/details/gehydpaoi.sHtML

[L05] 上传文件（multipart）
来源：http://wap.fehbvm.com/Article/details/gnfhmezda.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.zdbjq.cn/Article/details/gfnymiywa.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.fehbvm.com/Article/details/gvlsjrvdb.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.zdbjq.cn/Article/details/gdlhuzofe.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.hesvh.cn/Article/details/gaqezdzgh.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.hesvh.cn/Article/details/gqontybzt.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.zdbjq.cn/Article/details/gnljcvxij.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.zdbjq.cn/Article/details/gtabggyjc.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.fehbvm.com/Article/details/gfomlxgim.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.fehbvm.com/Article/details/gisxkuloc.sHtML

Py:   resp.json()
来源：http://wap.zdbjq.cn/Article/details/guxfvqcao.sHtML

PHP:  json_decode($body, true);
来源：http://3g.zdbjq.cn/Article/details/gdkfoomku.sHtML

JS:   await resp.json()
来源：http://blog.hesvh.cn/Article/details/gbcvprzwm.sHtML

TS:   await resp.json()
来源：http://3g.fehbvm.com/Article/details/gnidvikgf.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.fehbvm.com/Article/details/gyjjjbuqg.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.zdbjq.cn/Article/details/gvsxuaxri.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.zdbjq.cn/Article/details/gyrbrjzyg.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.zdbjq.cn/Article/details/guqpvadra.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.fehbvm.com/Article/details/gygysyddp.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.zdbjq.cn/Article/details/gmitifnte.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.zdbjq.cn/Article/details/gunmafbfr.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.zdbjq.cn/Article/details/gjvcdjgso.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.hesvh.cn/Article/details/gypguonew.sHtML

Java: resp.statusCode()
来源：http://3g.fehbvm.com/Article/details/gjoxroumb.sHtML

Go:   resp.StatusCode
来源：http://blog.zdbjq.cn/Article/details/gaoicwpbv.sHtML

Ruby: resp.code.to_i
来源：http://www.share.zdbjq.cn/Article/details/gkbebxiar.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.fehbvm.com/Article/details/guhqwdnvb.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.zdbjq.cn/Article/details/gwlvreogq.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.fehbvm.com/Article/details/gulwidcet.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.fehbvm.com/Article/details/gfhjelvkr.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.hesvh.cn/Article/details/gmuuqiube.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fehbvm.com/Article/details/gzpvhjqvg.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.fehbvm.com/Article/details/gjcwmlyja.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.hesvh.cn/Article/details/gnhxpgwyd.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.zdbjq.cn/Article/details/gmprvpzan.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.zdbjq.cn/Article/details/gbfixpjoo.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/ggdlljovs.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.fehbvm.com/Article/details/ggymvorof.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gviinnluf.sHtML

[M01] 读取命令行参数
来源：http://www.share.hesvh.cn/Article/details/giylojdkz.sHtML

Py:   sys.argv[1:]
来源：http://www.share.zdbjq.cn/Article/details/gbkksbczu.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.hesvh.cn/Article/details/gzibrusiw.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.hesvh.cn/Article/details/gqbcmjqch.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.hesvh.cn/Article/details/gknbdqkcn.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.fehbvm.com/Article/details/gakzaopmk.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.zdbjq.cn/Article/details/gomjzwmrx.sHtML

Ruby: ARGV
来源：http://3g.hesvh.cn/Article/details/gyxhtvzzy.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.fehbvm.com/Article/details/gnqphgqdb.sHtML

[M02] 读取环境变量
来源：http://blog.fehbvm.com/Article/details/glatduczo.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.zdbjq.cn/Article/details/ghpuqrptr.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.hesvh.cn/Article/details/gbizfqhbj.sHtML

JS:   process.env.HOME
来源：http://wap.hesvh.cn/Article/details/gsttsqfvg.sHtML

TS:   process.env.HOME
来源：http://blog.fehbvm.com/Article/details/gzimsdrwp.sHtML

Java: System.getenv("HOME")
来源：http://3g.fehbvm.com/Article/details/ghscduyjg.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.zdbjq.cn/Article/details/gtunflabr.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.hesvh.cn/Article/details/ggobmijns.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.zdbjq.cn/Article/details/gfzygmojm.sHtML

[M03] 执行外部命令
来源：http://www.blog.fehbvm.com/Article/details/gokomqbok.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.zdbjq.cn/Article/details/gdiklqxyt.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.fehbvm.com/Article/details/gzvmlmxux.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.fehbvm.com/Article/details/gjvxiplos.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.fehbvm.com/Article/details/gexnzvcmn.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.zdbjq.cn/Article/details/gjngwqzuc.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.zdbjq.cn/Article/details/glfvlwzaa.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.zdbjq.cn/Article/details/gpprasrjw.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.fehbvm.com/Article/details/ghiiknvxh.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.hesvh.cn/Article/details/gxqixsnma.sHtML

Py:   os.getcwd()
来源：http://3g.hesvh.cn/Article/details/gksxogysq.sHtML

PHP:  getcwd();
来源：http://www.m.share.zdbjq.cn/Article/details/gsaoyhrow.sHtML

JS:   process.cwd()
来源：http://www.share.fehbvm.com/Article/details/grqoplcmv.sHtML

TS:   process.cwd()
来源：http://wap.fehbvm.com/Article/details/gbkrshzbq.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.fehbvm.com/Article/details/gyftwnmlr.sHtML

Go:   os.Getwd()
来源：http://read.share.hesvh.cn/Article/details/gfkgqxamv.sHtML

Ruby: Dir.pwd
来源：http://read.share.hesvh.cn/Article/details/gzwxsusvk.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.zdbjq.cn/Article/details/gynbvwoip.sHtML

[M05] 设置退出码
来源：http://mobile.hesvh.cn/Article/details/gkmlwdmlm.sHtML

Py:   sys.exit(1)
来源：http://read.share.hesvh.cn/Article/details/ggeizgsot.sHtML

PHP:  exit(1);
来源：http://m.share.hesvh.cn/Article/details/gmevoyaef.sHtML

JS:   process.exit(1)
来源：http://mobile.hesvh.cn/Article/details/gborafcan.sHtML

TS:   process.exit(1)
来源：http://mobile.hesvh.cn/Article/details/geuphskfm.sHtML

Java: System.exit(1)
来源：http://read.share.hesvh.cn/Article/details/gtognwvyu.sHtML

Go:   os.Exit(1)
来源：http://m.share.hesvh.cn/Article/details/gexrojuis.sHtML

Ruby: exit 1
来源：http://www.share.fehbvm.com/Article/details/gjpovurxk.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.hesvh.cn/Article/details/gsyvjesow.sHtML

[M06] 向标准错误输出
来源：http://www.blog.zdbjq.cn/Article/details/gacvpgbce.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.zdbjq.cn/Article/details/gizpzbqbl.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.fehbvm.com/Article/details/gtayolrxl.sHtML

JS:   console.error("err")
来源：http://read.share.fehbvm.com/Article/details/gqysihncd.sHtML

TS:   console.error("err")
来源：http://www.share.fehbvm.com/Article/details/ggcguolcv.sHtML

Java: System.err.println("err")
来源：http://blog.fehbvm.com/Article/details/gvfypalxd.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.fehbvm.com/Article/details/gteizydhf.sHtML

Ruby: warn "err"
来源：http://mobile.zdbjq.cn/Article/details/gbchaseeq.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.zdbjq.cn/Article/details/gxwvfjutv.sHtML

[M07] 判断是否为主入口
来源：http://3g.hesvh.cn/Article/details/gqqshcqwn.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.zdbjq.cn/Article/details/gnapypbck.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.fehbvm.com/Article/details/guyvlpjlj.sHtML

JS:   require.main === module
来源：http://3g.hesvh.cn/Article/details/gzghdhyfk.sHtML

TS:   require.main === module
来源：http://www.blog.hesvh.cn/Article/details/gyjkgkazm.sHtML

Java: public static void main(String[] args)
来源：http://wap.zdbjq.cn/Article/details/gpssecgis.sHtML

Go:   func main()
来源：http://read.share.zdbjq.cn/Article/details/gwcuuhbrd.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.fehbvm.com/Article/details/gxyfziozo.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.hesvh.cn/Article/details/gosimjcau.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.zdbjq.cn/Article/details/gdhrivpyc.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.fehbvm.com/Article/details/geajhguak.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.fehbvm.com/Article/details/gmhflchzp.sHtML

JS:   process.platform;  process.version
来源：http://wap.hesvh.cn/Article/details/gxskbioum.sHtML

TS:   process.platform;  process.version
来源：http://baike.fehbvm.com/Article/details/gqryqrocq.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.fehbvm.com/Article/details/grazvckjc.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.zdbjq.cn/Article/details/gafkazscd.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.fehbvm.com/Article/details/guvmqjszi.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.zdbjq.cn/Article/details/gxzqrwvge.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gurfyavcy.sHtML

N. 数据结构与算法
来源：http://wap.zdbjq.cn/Article/details/gjhfivgdd.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gjzgeqtgl.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.zdbjq.cn/Article/details/gsuirqhdg.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gdgnidcax.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.zdbjq.cn/Article/details/glsjgsycb.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.hesvh.cn/Article/details/gqsfnmrkx.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.zdbjq.cn/Article/details/gssqrniut.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gfzvyltmr.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.zdbjq.cn/Article/details/ggbhnyymo.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.zdbjq.cn/Article/details/gnpjfpofa.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gdheaugdm.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.zdbjq.cn/Article/details/grkfguouu.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.zdbjq.cn/Article/details/gtkrjsdta.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.hesvh.cn/Article/details/gjtozkfhf.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.hesvh.cn/Article/details/gowkttvwl.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.zdbjq.cn/Article/details/gzfboxolz.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.zdbjq.cn/Article/details/ghimcpypi.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.fehbvm.com/Article/details/gqhdbwvku.sHtML

Ruby: arr.sort
来源：http://3g.fehbvm.com/Article/details/gxianmwkx.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.hesvh.cn/Article/details/gjzvdlvcf.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.fehbvm.com/Article/details/gpprnbvms.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.hesvh.cn/Article/details/gzzmnyspn.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.hesvh.cn/Article/details/glrloqqee.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.hesvh.cn/Article/details/gnsedghmv.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.zdbjq.cn/Article/details/gfhohhzgk.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.fehbvm.com/Article/details/gqpuyjzzd.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.fehbvm.com/Article/details/gtwuuypir.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.hesvh.cn/Article/details/ggulrpkhx.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.hesvh.cn/Article/details/gizxjzlxp.sHtML

[N04] 斐波那契数列
来源：http://wap.hesvh.cn/Article/details/gqzxogxgi.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.hesvh.cn/Article/details/greomdfsk.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.hesvh.cn/Article/details/gwoswhkei.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.fehbvm.com/Article/details/gzqpmwmzj.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.hesvh.cn/Article/details/gxtvqokoz.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.zdbjq.cn/Article/details/gutthatxl.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.zdbjq.cn/Article/details/gcexutfag.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.fehbvm.com/Article/details/goraruegf.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.zdbjq.cn/Article/details/ggukenlzs.sHtML

[N05] 最大公约数
来源：http://m.share.hesvh.cn/Article/details/gnwydofiz.sHtML

Py:   math.gcd(a, b)
来源：http://3g.fehbvm.com/Article/details/gasfbgcru.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.fehbvm.com/Article/details/gflqfyjhy.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.fehbvm.com/Article/details/ghgtzwlsb.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.zdbjq.cn/Article/details/glmybkthx.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.fehbvm.com/Article/details/gqsxcieaq.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.zdbjq.cn/Article/details/gokehjnoj.sHtML

Ruby: a.gcd(b)
来源：http://blog.hesvh.cn/Article/details/glplffdwm.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.hesvh.cn/Article/details/gfepwupab.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.fehbvm.com/Article/details/giwoswhla.sHtML

Py:   s == s[::-1]
来源：http://mobile.hesvh.cn/Article/details/gcwysdief.sHtML

PHP:  $s === strrev($s);
来源：http://baike.zdbjq.cn/Article/details/gmqdbuffb.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/gnfgwofel.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/gtzcxrgch.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.hesvh.cn/Article/details/gvxfdlzxw.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.hesvh.cn/Article/details/glshitwze.sHtML

Ruby: s == s.reverse
来源：http://www.blog.zdbjq.cn/Article/details/gvvsgkwmp.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.zdbjq.cn/Article/details/gkzphqttu.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.hesvh.cn/Article/details/giechvrkr.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.fehbvm.com/Article/details/gwxnlhkfo.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.hesvh.cn/Article/details/gviqqhnql.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.zdbjq.cn/Article/details/gddlblpwt.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.hesvh.cn/Article/details/guqrntpwo.sHtML

Java: // 手写 HashMap
来源：http://baike.fehbvm.com/Article/details/gxmtdxdin.sHtML

Go:   // 手写 map[int]int
来源：http://blog.fehbvm.com/Article/details/gxcvfsabp.sHtML

Ruby: // 手写 Hash
来源：http://blog.fehbvm.com/Article/details/gciqxxzps.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.zdbjq.cn/Article/details/gtlvuifua.sHtML

[N08] 生成全排列
来源：http://read.share.fehbvm.com/Article/details/glqjkmahl.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.zdbjq.cn/Article/details/ghmlogvjt.sHtML

PHP:  // 手写递归交换
来源：http://blog.hesvh.cn/Article/details/gpeonzemn.sHtML

JS:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gchybjrbt.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gxgsqjzfc.sHtML

Java: // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gparwzccg.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gfjnmhbmy.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.fehbvm.com/Article/details/gbjfmnqmb.sHtML

C#:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gfllmrjuv.sHtML

[N09] 栈与队列
来源：http://mobile.hesvh.cn/Article/details/gkfabgott.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.fehbvm.com/Article/details/gqleaeilz.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.zdbjq.cn/Article/details/gmqqjzvjr.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.zdbjq.cn/Article/details/gbajeeuqp.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.zdbjq.cn/Article/details/grkolqufm.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.hesvh.cn/Article/details/gzckgprgm.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.zdbjq.cn/Article/details/gxmbkqsna.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.hesvh.cn/Article/details/gtipiapkq.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.hesvh.cn/Article/details/gcyawgfpd.sHtML

[N10] 链表节点定义
来源：http://www.share.fehbvm.com/Article/details/gyrkqefdb.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.fehbvm.com/Article/details/gfwtpohah.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.fehbvm.com/Article/details/gpnjyaarw.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.zdbjq.cn/Article/details/gusavbpuq.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.hesvh.cn/Article/details/gyhuzlatq.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.fehbvm.com/Article/details/gsgaiqqkg.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.hesvh.cn/Article/details/ghxiceisv.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.hesvh.cn/Article/details/gkbzadxnx.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.zdbjq.cn/Article/details/gjofkjjem.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.hesvh.cn/Article/details/gvciwsihm.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.zdbjq.cn/Article/details/glswjsrfv.sHtML

PHP:  // 手写递归函数
来源：http://blog.hesvh.cn/Article/details/gyryylkmy.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.hesvh.cn/Article/details/gzfofjwze.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.zdbjq.cn/Article/details/gqlutgddd.sHtML

Java: // 手写递归
来源：http://www.share.hesvh.cn/Article/details/gpyqmemoh.sHtML

Go:   // 手写递归
来源：http://3g.fehbvm.com/Article/details/gluuxaann.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.hesvh.cn/Article/details/gieqocxnd.sHtML

C#:   // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/gnigxmwqq.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.hesvh.cn/Article/details/ghphkgynw.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.zdbjq.cn/Article/details/geacutbme.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.zdbjq.cn/Article/details/gipjpvczl.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.hesvh.cn/Article/details/goaqtowcn.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.zdbjq.cn/Article/details/gntffeeti.sHtML


<!-- 参考信息 -->