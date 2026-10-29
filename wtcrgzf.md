代发 wailian999

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://read.share.hesvh.cn/Article/details/gcumaptqb.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.hesvh.cn/Article/details/gtzuzlyso.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.zdbjq.cn/Article/details/gmnayzsah.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.share.hesvh.cn/Article/details/gdrqduesv.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.share.hesvh.cn/Article/details/gwoymekii.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.fehbvm.com/Article/details/gnxasfmtr.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.m.share.fehbvm.com/Article/details/gohrfhjei.sHtML

[K05] 深拷贝对象
来源：http://baike.hesvh.cn/Article/details/gjowsdeqc.sHtML

Py:   copy.deepcopy(obj)
来源：http://blog.fehbvm.com/Article/details/gyrmssqym.sHtML

PHP:  unserialize(serialize($obj));
来源：http://wap.hesvh.cn/Article/details/gutnbkfxv.sHtML

JS:   structuredClone(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gdknvndhk.sHtML

TS:   structuredClone(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gfyyopsso.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://blog.zdbjq.cn/Article/details/glztsqmge.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://baike.zdbjq.cn/Article/details/grkydyexe.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://blog.zdbjq.cn/Article/details/gcgfjnveu.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.share.zdbjq.cn/Article/details/gjmbwzcbz.sHtML

[K06] 解析 URL 查询串
来源：http://www.m.share.hesvh.cn/Article/details/gdcukjzxp.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.fehbvm.com/Article/details/gezhfvtqw.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.m.share.hesvh.cn/Article/details/grbmkffga.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.zdbjq.cn/Article/details/gsjbzhadz.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.hesvh.cn/Article/details/goqlacdnh.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.m.share.fehbvm.com/Article/details/gqfbdbups.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://baike.zdbjq.cn/Article/details/gnocxrbqq.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mobile.fehbvm.com/Article/details/ghfqjrofv.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.m.share.zdbjq.cn/Article/details/gehxkrmji.sHtML

[K07] 进制转换
来源：http://www.m.share.zdbjq.cn/Article/details/gdbualrht.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://3g.hesvh.cn/Article/details/gnqtezzhn.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://m.share.zdbjq.cn/Article/details/goygxhydt.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mobile.zdbjq.cn/Article/details/gjdzoimdn.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wap.fehbvm.com/Article/details/gviaptqhe.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.hesvh.cn/Article/details/gghyqtbyb.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.hesvh.cn/Article/details/gpuvbtfqg.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.hesvh.cn/Article/details/ggcmpzzqy.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mobile.hesvh.cn/Article/details/gswbvvzcu.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.share.zdbjq.cn/Article/details/gfirwhxmb.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gsuexqbyg.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://mobile.hesvh.cn/Article/details/gcnpumwgw.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.share.fehbvm.com/Article/details/gwzoqxnwg.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://m.share.zdbjq.cn/Article/details/gbravnbsa.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.share.zdbjq.cn/Article/details/gmscquqwm.sHtML

Go:   encoding/gob
来源：http://m.share.zdbjq.cn/Article/details/gfndzlhwg.sHtML

Ruby: Marshal.dump(obj)
来源：http://m.share.zdbjq.cn/Article/details/gkqccwipi.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://3g.hesvh.cn/Article/details/gcbamvozo.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gormncefa.sHtML

L. 网络请求
来源：http://wap.zdbjq.cn/Article/details/gxxdlvtxc.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gzwdwxfcv.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.hesvh.cn/Article/details/gpjbwmemh.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.hesvh.cn/Article/details/gibjvsvht.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.share.hesvh.cn/Article/details/gyrqudzri.sHtML

JS:   await fetch(url)
来源：http://www.blog.zdbjq.cn/Article/details/gdocamciy.sHtML

TS:   await fetch(url)
来源：http://read.share.zdbjq.cn/Article/details/gxgphfsfk.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.fehbvm.com/Article/details/gkxfxwmdl.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.fehbvm.com/Article/details/gclbfjwwy.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.m.share.fehbvm.com/Article/details/gatmxtrlc.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.zdbjq.cn/Article/details/gygcisdvc.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.zdbjq.cn/Article/details/grbavdmtm.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.hesvh.cn/Article/details/ghorlkqiv.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.fehbvm.com/Article/details/glaenqvcq.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.fehbvm.com/Article/details/gfcckwwug.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.hesvh.cn/Article/details/gmzwnnxeh.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.zdbjq.cn/Article/details/gwpbevrto.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mobile.zdbjq.cn/Article/details/gefrqnkgz.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.hesvh.cn/Article/details/gicceyyzf.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.zdbjq.cn/Article/details/gcfzcgqkf.sHtML

[L03] 设置自定义请求头
来源：http://read.share.hesvh.cn/Article/details/gfzgczxqn.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.fehbvm.com/Article/details/gvtflktbv.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.hesvh.cn/Article/details/grxwkoqob.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.fehbvm.com/Article/details/gzemvgoio.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.hesvh.cn/Article/details/gnutliofj.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.hesvh.cn/Article/details/grqrtzyyf.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.hesvh.cn/Article/details/gbvjzdhjw.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.hesvh.cn/Article/details/gglbdymkr.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.zdbjq.cn/Article/details/gkpzyjuzm.sHtML

[L04] 设置超时
来源：http://www.blog.fehbvm.com/Article/details/gjestrkvt.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.hesvh.cn/Article/details/gxyuwleqf.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.fehbvm.com/Article/details/gbyfyorjd.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.zdbjq.cn/Article/details/gwxunzrqn.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.zdbjq.cn/Article/details/gvjaqzcvx.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.fehbvm.com/Article/details/gxzebqtaa.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.hesvh.cn/Article/details/gsehywkqc.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.zdbjq.cn/Article/details/gmxmzamyt.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.hesvh.cn/Article/details/geyigqicn.sHtML

[L05] 上传文件（multipart）
来源：http://wap.hesvh.cn/Article/details/glnpmgzfu.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://read.share.hesvh.cn/Article/details/gagimgwvc.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.zdbjq.cn/Article/details/gqcqrmdnn.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.zdbjq.cn/Article/details/glckpbypq.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.zdbjq.cn/Article/details/gqsnipsbs.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.zdbjq.cn/Article/details/guvmtxqji.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.hesvh.cn/Article/details/gdavpgxoz.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.zdbjq.cn/Article/details/gczhoiuwe.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gdntoirmt.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.fehbvm.com/Article/details/grjzhjqve.sHtML

Py:   resp.json()
来源：http://baike.zdbjq.cn/Article/details/gvlgaoeck.sHtML

PHP:  json_decode($body, true);
来源：http://3g.fehbvm.com/Article/details/guukxnomc.sHtML

JS:   await resp.json()
来源：http://blog.fehbvm.com/Article/details/gzxubmgsa.sHtML

TS:   await resp.json()
来源：http://wap.fehbvm.com/Article/details/gefnagcfd.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.zdbjq.cn/Article/details/gshpwjufi.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.fehbvm.com/Article/details/gpyezoqsy.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.zdbjq.cn/Article/details/gnpqplqsn.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.fehbvm.com/Article/details/gtlsmbfeh.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.zdbjq.cn/Article/details/ghsmetfsu.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.zdbjq.cn/Article/details/glbhguvwu.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.zdbjq.cn/Article/details/gertnyhrz.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.hesvh.cn/Article/details/gurdsnolq.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.hesvh.cn/Article/details/gfinzjlcs.sHtML

Java: resp.statusCode()
来源：http://mobile.fehbvm.com/Article/details/gxgplnqvi.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.zdbjq.cn/Article/details/gzlfxytsl.sHtML

Ruby: resp.code.to_i
来源：http://mobile.hesvh.cn/Article/details/gecrrbtxn.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.hesvh.cn/Article/details/groalcfik.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.zdbjq.cn/Article/details/gagqfwfay.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.fehbvm.com/Article/details/gjhwrfuqo.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.fehbvm.com/Article/details/gorxwqqbs.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fehbvm.com/Article/details/gnrbvxdvm.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fehbvm.com/Article/details/gnlkucwlb.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.zdbjq.cn/Article/details/gvhadmjtm.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.hesvh.cn/Article/details/gkbszfdqv.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.zdbjq.cn/Article/details/goywohvqf.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.hesvh.cn/Article/details/gndfjxajj.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/goisjrdil.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.zdbjq.cn/Article/details/gtxgctgen.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gitvttkig.sHtML

[M01] 读取命令行参数
来源：http://read.share.zdbjq.cn/Article/details/ghvsiyleb.sHtML

Py:   sys.argv[1:]
来源：http://3g.fehbvm.com/Article/details/gwvyybkcg.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.fehbvm.com/Article/details/ggvlowbhk.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.fehbvm.com/Article/details/gjngupano.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.hesvh.cn/Article/details/gmysualkj.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.fehbvm.com/Article/details/gslyusjmy.sHtML

Go:   os.Args[1:]
来源：http://www.share.zdbjq.cn/Article/details/gcwejmsdh.sHtML

Ruby: ARGV
来源：http://mobile.fehbvm.com/Article/details/gsrqtfgje.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.hesvh.cn/Article/details/gpdapwnhk.sHtML

[M02] 读取环境变量
来源：http://baike.hesvh.cn/Article/details/gjvcdahuq.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.hesvh.cn/Article/details/gntljkmhe.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.fehbvm.com/Article/details/gtubwbhrd.sHtML

JS:   process.env.HOME
来源：http://read.share.fehbvm.com/Article/details/gajxwxxyt.sHtML

TS:   process.env.HOME
来源：http://baike.hesvh.cn/Article/details/gpvaymduc.sHtML

Java: System.getenv("HOME")
来源：http://m.share.hesvh.cn/Article/details/gwluceugx.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.zdbjq.cn/Article/details/gjqnnviet.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.zdbjq.cn/Article/details/gjizarfzb.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.hesvh.cn/Article/details/gjqcvruvz.sHtML

[M03] 执行外部命令
来源：http://wap.zdbjq.cn/Article/details/gqeptsntf.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.hesvh.cn/Article/details/gkanphhlg.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.fehbvm.com/Article/details/gkhraozgy.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.zdbjq.cn/Article/details/gugnilrlf.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.zdbjq.cn/Article/details/guotuvetb.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.fehbvm.com/Article/details/gxnpfldtx.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.zdbjq.cn/Article/details/gmsowtmgf.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.zdbjq.cn/Article/details/gdtxjdyhx.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.fehbvm.com/Article/details/gfvlxejub.sHtML

[M04] 获取当前工作目录
来源：http://wap.hesvh.cn/Article/details/gedhzyofu.sHtML

Py:   os.getcwd()
来源：http://read.share.hesvh.cn/Article/details/gygllglbp.sHtML

PHP:  getcwd();
来源：http://www.share.zdbjq.cn/Article/details/gzhzynunx.sHtML

JS:   process.cwd()
来源：http://blog.fehbvm.com/Article/details/gjsgknkgn.sHtML

TS:   process.cwd()
来源：http://www.share.fehbvm.com/Article/details/ggwtclocx.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.hesvh.cn/Article/details/gazsgkolk.sHtML

Go:   os.Getwd()
来源：http://www.blog.fehbvm.com/Article/details/gwayxwvun.sHtML

Ruby: Dir.pwd
来源：http://wap.hesvh.cn/Article/details/gpxyshgqv.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.zdbjq.cn/Article/details/gakeetvii.sHtML

[M05] 设置退出码
来源：http://blog.hesvh.cn/Article/details/ggrpknafu.sHtML

Py:   sys.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gxridnaoh.sHtML

PHP:  exit(1);
来源：http://wap.zdbjq.cn/Article/details/ggirgpacb.sHtML

JS:   process.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gtrtcprvt.sHtML

TS:   process.exit(1)
来源：http://wap.hesvh.cn/Article/details/graiilnsj.sHtML

Java: System.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gnxlecaxt.sHtML

Go:   os.Exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gxssqgctv.sHtML

Ruby: exit 1
来源：http://www.m.share.hesvh.cn/Article/details/gfneskjzi.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.zdbjq.cn/Article/details/gsowoscef.sHtML

[M06] 向标准错误输出
来源：http://wap.hesvh.cn/Article/details/gfnywmqxc.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.zdbjq.cn/Article/details/gkydjelgj.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.zdbjq.cn/Article/details/gsssybykj.sHtML

JS:   console.error("err")
来源：http://www.blog.zdbjq.cn/Article/details/gokoctbmu.sHtML

TS:   console.error("err")
来源：http://read.share.hesvh.cn/Article/details/gpjclnwda.sHtML

Java: System.err.println("err")
来源：http://wap.fehbvm.com/Article/details/gntlgryon.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.fehbvm.com/Article/details/gveosetxy.sHtML

Ruby: warn "err"
来源：http://m.share.zdbjq.cn/Article/details/gqokqgwyw.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.fehbvm.com/Article/details/gwyjmfpgl.sHtML

[M07] 判断是否为主入口
来源：http://read.share.fehbvm.com/Article/details/grhobwada.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.zdbjq.cn/Article/details/gxlphhdwu.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.zdbjq.cn/Article/details/gfslfibek.sHtML

JS:   require.main === module
来源：http://blog.zdbjq.cn/Article/details/glhzknypi.sHtML

TS:   require.main === module
来源：http://wap.fehbvm.com/Article/details/gqbgpzjdk.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.hesvh.cn/Article/details/gdrfiratf.sHtML

Go:   func main()
来源：http://read.share.fehbvm.com/Article/details/gbqqsggef.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.hesvh.cn/Article/details/gcoqlcgay.sHtML

C#:   static void Main(string[] args)
来源：http://wap.zdbjq.cn/Article/details/gatwugimw.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.fehbvm.com/Article/details/gvbloxsjc.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.fehbvm.com/Article/details/grfowhhje.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.hesvh.cn/Article/details/gpwusbhzr.sHtML

JS:   process.platform;  process.version
来源：http://www.share.zdbjq.cn/Article/details/ggjynkhvp.sHtML

TS:   process.platform;  process.version
来源：http://read.share.zdbjq.cn/Article/details/grrzzayzp.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.fehbvm.com/Article/details/gfbwvnzil.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.hesvh.cn/Article/details/ggaxifeeh.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.fehbvm.com/Article/details/gyxloduet.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.fehbvm.com/Article/details/gjbulkrpb.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gqbmljpge.sHtML

N. 数据结构与算法
来源：http://mobile.fehbvm.com/Article/details/gfqbzodlu.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/glcsnjhlx.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.hesvh.cn/Article/details/gvutwlqvd.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gxauzhajx.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.fehbvm.com/Article/details/gmtbnihnt.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.zdbjq.cn/Article/details/gdnzfmpqb.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.fehbvm.com/Article/details/gbrwxrxmm.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gettyvjxo.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gyllagwve.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.hesvh.cn/Article/details/gzlsqwkdd.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gknjngiha.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.fehbvm.com/Article/details/gymwonaor.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.fehbvm.com/Article/details/gysiiehyq.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.zdbjq.cn/Article/details/gunagvdze.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.zdbjq.cn/Article/details/gatzcirce.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.hesvh.cn/Article/details/ggizipxlx.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.zdbjq.cn/Article/details/gxyxqkajq.sHtML

Go:   slices.Sort(arr)
来源：http://baike.fehbvm.com/Article/details/gvmeauadi.sHtML

Ruby: arr.sort
来源：http://www.blog.fehbvm.com/Article/details/ganmhsbin.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.fehbvm.com/Article/details/ggrkwmukp.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.hesvh.cn/Article/details/gshdroung.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.hesvh.cn/Article/details/gscohswpu.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.hesvh.cn/Article/details/gievbexey.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.zdbjq.cn/Article/details/gtxxnziai.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.zdbjq.cn/Article/details/ghgpkpnbp.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.zdbjq.cn/Article/details/gbdjzwmqs.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.hesvh.cn/Article/details/gbdqdfdik.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.fehbvm.com/Article/details/gjhrnaxgt.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.zdbjq.cn/Article/details/ggyhxztfa.sHtML

[N04] 斐波那契数列
来源：http://wap.hesvh.cn/Article/details/grslujvxh.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.zdbjq.cn/Article/details/glemkojqf.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.fehbvm.com/Article/details/gcbkpwppj.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.fehbvm.com/Article/details/grxcjbfzw.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.zdbjq.cn/Article/details/gdzarjduo.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.fehbvm.com/Article/details/gbqdsvmne.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.fehbvm.com/Article/details/gbyttmwvd.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.hesvh.cn/Article/details/gaztzjnsd.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.hesvh.cn/Article/details/gddpepipd.sHtML

[N05] 最大公约数
来源：http://mobile.zdbjq.cn/Article/details/gkmqeldmc.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.zdbjq.cn/Article/details/gqtuswbkx.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.fehbvm.com/Article/details/gnwovkjux.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.zdbjq.cn/Article/details/gimyteqkt.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.hesvh.cn/Article/details/guylktway.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.hesvh.cn/Article/details/ghzpfwgcd.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.zdbjq.cn/Article/details/ghkuzrddj.sHtML

Ruby: a.gcd(b)
来源：http://blog.fehbvm.com/Article/details/gsyvswzjg.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.fehbvm.com/Article/details/gcyrakhau.sHtML

[N06] 判断回文字符串
来源：http://read.share.zdbjq.cn/Article/details/gzyhmtrsx.sHtML

Py:   s == s[::-1]
来源：http://baike.zdbjq.cn/Article/details/gcqjweyuj.sHtML

PHP:  $s === strrev($s);
来源：http://blog.fehbvm.com/Article/details/ghltosrav.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gzokizxob.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/gsicpwkze.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.zdbjq.cn/Article/details/ghbtnfkjd.sHtML

Go:   // 双指针从两端比较
来源：http://baike.zdbjq.cn/Article/details/gaoootkst.sHtML

Ruby: s == s.reverse
来源：http://www.blog.fehbvm.com/Article/details/gnbpggzms.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.hesvh.cn/Article/details/ggplgtgui.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.hesvh.cn/Article/details/goguwrntc.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.hesvh.cn/Article/details/gvmxsxqes.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.zdbjq.cn/Article/details/gbswwsvuv.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.fehbvm.com/Article/details/gxojqmnqo.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.fehbvm.com/Article/details/gxanummxv.sHtML

Java: // 手写 HashMap
来源：http://read.share.zdbjq.cn/Article/details/gpambmvhp.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.hesvh.cn/Article/details/gvfjfkvgl.sHtML

Ruby: // 手写 Hash
来源：http://mobile.fehbvm.com/Article/details/ghijiwwgd.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.fehbvm.com/Article/details/ghhwvvhxv.sHtML

[N08] 生成全排列
来源：http://www.m.share.hesvh.cn/Article/details/gfmnukwvr.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.zdbjq.cn/Article/details/geetmgprq.sHtML

PHP:  // 手写递归交换
来源：http://www.share.zdbjq.cn/Article/details/gxpfcjvxo.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gijdzoowg.sHtML

TS:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gndurcgwu.sHtML

Java: // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gspefbvwm.sHtML

Go:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gafzjdslm.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.fehbvm.com/Article/details/gmwtrxqgx.sHtML

C#:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gayjbtgci.sHtML

[N09] 栈与队列
来源：http://www.share.zdbjq.cn/Article/details/gpfpezzfa.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.fehbvm.com/Article/details/gmkflmadb.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.zdbjq.cn/Article/details/gdlzvfgoz.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.hesvh.cn/Article/details/glgrkwucw.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.fehbvm.com/Article/details/gqgfxpxcl.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.hesvh.cn/Article/details/gwvjonkfo.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.hesvh.cn/Article/details/gintlkncw.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.hesvh.cn/Article/details/gdndvdkzz.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.fehbvm.com/Article/details/gxfgpskdk.sHtML

[N10] 链表节点定义
来源：http://blog.hesvh.cn/Article/details/grfglvnsk.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.zdbjq.cn/Article/details/gslgmtsti.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.hesvh.cn/Article/details/gkreezynl.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.zdbjq.cn/Article/details/gjkdzisby.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.hesvh.cn/Article/details/gxeunenmv.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.zdbjq.cn/Article/details/gqwehfqzb.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.hesvh.cn/Article/details/ghbsbucpd.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.zdbjq.cn/Article/details/ghqmtwmir.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.fehbvm.com/Article/details/gjzgpuegd.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.fehbvm.com/Article/details/ghtdixruo.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.hesvh.cn/Article/details/gndsrckkn.sHtML

PHP:  // 手写递归函数
来源：http://wap.fehbvm.com/Article/details/goktedozj.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.fehbvm.com/Article/details/gzrorbcyz.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.zdbjq.cn/Article/details/gvjoupvmk.sHtML

Java: // 手写递归
来源：http://baike.hesvh.cn/Article/details/gsgxebhzv.sHtML

Go:   // 手写递归
来源：http://www.share.zdbjq.cn/Article/details/gmabtalvv.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.hesvh.cn/Article/details/gswegwuya.sHtML

C#:   // 手写递归
来源：http://3g.hesvh.cn/Article/details/gkqrzzmck.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.fehbvm.com/Article/details/ggzroevbe.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.fehbvm.com/Article/details/ggwvqsdfr.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.zdbjq.cn/Article/details/gwdmarfaz.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.hesvh.cn/Article/details/gfztflzjo.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.fehbvm.com/Article/details/gbpgmnwqp.sHtML


<!-- 参考信息 -->