代发 wailian999

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mobile.zdbjq.cn/Article/details/gkxsseoke.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.share.zdbjq.cn/Article/details/gvgzefveq.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://3g.fehbvm.com/Article/details/gjatibixd.sHtML

[K05] 深拷贝对象
来源：http://read.share.hesvh.cn/Article/details/gbyeebztv.sHtML

Py:   copy.deepcopy(obj)
来源：http://mobile.hesvh.cn/Article/details/gqkyjqqgc.sHtML

PHP:  unserialize(serialize($obj));
来源：http://mobile.fehbvm.com/Article/details/gxqvocmbn.sHtML

JS:   structuredClone(obj)
来源：http://mobile.zdbjq.cn/Article/details/gqufjfqts.sHtML

TS:   structuredClone(obj)
来源：http://mobile.hesvh.cn/Article/details/gsvpkuryx.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://wap.fehbvm.com/Article/details/glexoivqy.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://m.share.zdbjq.cn/Article/details/ghnapvysp.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.share.zdbjq.cn/Article/details/giboirdis.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://read.share.zdbjq.cn/Article/details/gzrwdgrhn.sHtML

[K06] 解析 URL 查询串
来源：http://read.share.zdbjq.cn/Article/details/ggcvddicj.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mobile.fehbvm.com/Article/details/gvgmmnwde.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.blog.fehbvm.com/Article/details/gqumrnkfy.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.fehbvm.com/Article/details/geaydtfkk.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.hesvh.cn/Article/details/gwadzgfin.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://blog.zdbjq.cn/Article/details/gotdsxhws.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.blog.zdbjq.cn/Article/details/gkdcrxlet.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://m.share.zdbjq.cn/Article/details/glfafpgcz.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.hesvh.cn/Article/details/gzuogtttz.sHtML

[K07] 进制转换
来源：http://blog.zdbjq.cn/Article/details/gigbfyosh.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.fehbvm.com/Article/details/gqfnnvbjr.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://blog.hesvh.cn/Article/details/gtnyyaerk.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mobile.hesvh.cn/Article/details/gtbkmojfv.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wap.fehbvm.com/Article/details/gkkxdeuhs.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.fehbvm.com/Article/details/gsilxzfgs.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.zdbjq.cn/Article/details/gmhwjumuy.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.m.share.hesvh.cn/Article/details/gijefbmpa.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.share.fehbvm.com/Article/details/gjkfvptic.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.fehbvm.com/Article/details/gwavcocpr.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.zdbjq.cn/Article/details/gfvjdaivr.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.hesvh.cn/Article/details/gozqcgras.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://mobile.zdbjq.cn/Article/details/giyiwujyz.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.blog.zdbjq.cn/Article/details/gbtyydvqx.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.hesvh.cn/Article/details/gfmmimubx.sHtML

Go:   encoding/gob
来源：http://www.m.share.zdbjq.cn/Article/details/gemydvybh.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.hesvh.cn/Article/details/gshupsakd.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.fehbvm.com/Article/details/gpcukbngh.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gogvfuvxw.sHtML

L. 网络请求
来源：http://blog.fehbvm.com/Article/details/gfblibxyp.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gaigrpooj.sHtML

[L01] 发送 GET 请求
来源：http://www.share.hesvh.cn/Article/details/gcfwmtxzk.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.share.hesvh.cn/Article/details/gybsoouug.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.m.share.fehbvm.com/Article/details/gykfcxzun.sHtML

JS:   await fetch(url)
来源：http://read.share.fehbvm.com/Article/details/gznwsoehx.sHtML

TS:   await fetch(url)
来源：http://www.blog.fehbvm.com/Article/details/ggeuuqpls.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.fehbvm.com/Article/details/gwvqrhyid.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.zdbjq.cn/Article/details/gyeqdkuyi.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.m.share.fehbvm.com/Article/details/galhmyfum.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.fehbvm.com/Article/details/gvtcqntrg.sHtML

[L02] 发送 POST JSON
来源：http://baike.fehbvm.com/Article/details/gwqyarbny.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://read.share.hesvh.cn/Article/details/ggspljevg.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.hesvh.cn/Article/details/gptowddgx.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.zdbjq.cn/Article/details/grvkzqfqb.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.hesvh.cn/Article/details/gqumdwpyx.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.m.share.fehbvm.com/Article/details/gbablkhxf.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mobile.hesvh.cn/Article/details/gvqyjltsy.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.fehbvm.com/Article/details/gngotksmg.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.zdbjq.cn/Article/details/gdqepgkio.sHtML

[L03] 设置自定义请求头
来源：http://3g.fehbvm.com/Article/details/gvmdbnibz.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.fehbvm.com/Article/details/ghikuznpo.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.fehbvm.com/Article/details/geqtshpum.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.hesvh.cn/Article/details/gprfrvccy.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.hesvh.cn/Article/details/guglzqjqj.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.fehbvm.com/Article/details/gjstjespy.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.hesvh.cn/Article/details/gxcwqfbcg.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.fehbvm.com/Article/details/gnotuyapk.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.hesvh.cn/Article/details/gnjyrjhfl.sHtML

[L04] 设置超时
来源：http://www.share.hesvh.cn/Article/details/ghtyorqlx.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.hesvh.cn/Article/details/glhmzicgz.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.zdbjq.cn/Article/details/gozgicocw.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.hesvh.cn/Article/details/ggmvtltae.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.hesvh.cn/Article/details/ghaxvpzzv.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.hesvh.cn/Article/details/gbjnlnsma.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.fehbvm.com/Article/details/gqqhonvii.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.hesvh.cn/Article/details/gzhztlijk.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.hesvh.cn/Article/details/glnhrqvjz.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.zdbjq.cn/Article/details/gljbddnod.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.hesvh.cn/Article/details/gcyjwzytf.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.hesvh.cn/Article/details/gbrroliqc.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.fehbvm.com/Article/details/gcexrgppz.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.hesvh.cn/Article/details/gsnvgabnb.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.fehbvm.com/Article/details/ggqlwqqsj.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.hesvh.cn/Article/details/gbarhrsun.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.hesvh.cn/Article/details/gvzdudlgq.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gruxkycuw.sHtML

[L06] 解析响应为 JSON
来源：http://baike.fehbvm.com/Article/details/gmfutvzab.sHtML

Py:   resp.json()
来源：http://www.m.share.hesvh.cn/Article/details/gksyukxin.sHtML

PHP:  json_decode($body, true);
来源：http://blog.hesvh.cn/Article/details/getearkxd.sHtML

JS:   await resp.json()
来源：http://3g.fehbvm.com/Article/details/gslmnpgiv.sHtML

TS:   await resp.json()
来源：http://m.share.zdbjq.cn/Article/details/gaawgyfjb.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.fehbvm.com/Article/details/gigeabadt.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.fehbvm.com/Article/details/gapzrxcsg.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.fehbvm.com/Article/details/gsiopjilu.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.zdbjq.cn/Article/details/ggwjmsqym.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.hesvh.cn/Article/details/gunmguhsv.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.zdbjq.cn/Article/details/gifcxcsxw.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.fehbvm.com/Article/details/grevzftmv.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.zdbjq.cn/Article/details/gfsmaztxw.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.zdbjq.cn/Article/details/gdlozobvj.sHtML

Java: resp.statusCode()
来源：http://www.blog.hesvh.cn/Article/details/gcruhrpjv.sHtML

Go:   resp.StatusCode
来源：http://mobile.fehbvm.com/Article/details/gnpnilfvm.sHtML

Ruby: resp.code.to_i
来源：http://3g.fehbvm.com/Article/details/gygdtwmho.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.zdbjq.cn/Article/details/gpxrisgyi.sHtML

[L08] 并发请求多个地址
来源：http://wap.zdbjq.cn/Article/details/ggzeyrbkp.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.zdbjq.cn/Article/details/gomvrxpha.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.fehbvm.com/Article/details/gsmdwwpnt.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.zdbjq.cn/Article/details/gtjkryeql.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fehbvm.com/Article/details/gjehcmgvv.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.hesvh.cn/Article/details/gnmwrlhov.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.fehbvm.com/Article/details/gaznixyiq.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.zdbjq.cn/Article/details/gqykmchdx.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.zdbjq.cn/Article/details/gjdxvdqte.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gwijzaepx.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.hesvh.cn/Article/details/gbbrylwkw.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gvytbeuct.sHtML

[M01] 读取命令行参数
来源：http://m.share.zdbjq.cn/Article/details/gjwijwzdc.sHtML

Py:   sys.argv[1:]
来源：http://baike.hesvh.cn/Article/details/gbeyzyirb.sHtML

PHP:  $argv;  $argc;
来源：http://wap.fehbvm.com/Article/details/gzwqawlci.sHtML

JS:   process.argv.slice(2)
来源：http://baike.zdbjq.cn/Article/details/gugbumxgo.sHtML

TS:   process.argv.slice(2)
来源：http://3g.fehbvm.com/Article/details/gkevxemzx.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.fehbvm.com/Article/details/gcpbhgazy.sHtML

Go:   os.Args[1:]
来源：http://m.share.fehbvm.com/Article/details/gudicglrp.sHtML

Ruby: ARGV
来源：http://wap.hesvh.cn/Article/details/gxpwmoobn.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.hesvh.cn/Article/details/gzevoczti.sHtML

[M02] 读取环境变量
来源：http://3g.fehbvm.com/Article/details/givnamcfr.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.fehbvm.com/Article/details/gsxdgsnzn.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.fehbvm.com/Article/details/gpnpeihdv.sHtML

JS:   process.env.HOME
来源：http://www.m.share.fehbvm.com/Article/details/gfoxksvfp.sHtML

TS:   process.env.HOME
来源：http://baike.zdbjq.cn/Article/details/gasephogj.sHtML

Java: System.getenv("HOME")
来源：http://blog.hesvh.cn/Article/details/gitsqeyjx.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.fehbvm.com/Article/details/gvhxzmmmd.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.hesvh.cn/Article/details/gpssvnper.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.fehbvm.com/Article/details/ghqotnefn.sHtML

[M03] 执行外部命令
来源：http://m.share.hesvh.cn/Article/details/gmavqbtgt.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.zdbjq.cn/Article/details/gfexicaoc.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.hesvh.cn/Article/details/gnwxsjyaq.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.zdbjq.cn/Article/details/gbammrlzp.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.hesvh.cn/Article/details/gjqxufqzt.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.hesvh.cn/Article/details/gxhunhxtt.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.hesvh.cn/Article/details/glneeacay.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.fehbvm.com/Article/details/gxwhbcooi.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.zdbjq.cn/Article/details/gpfzltjve.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.zdbjq.cn/Article/details/gljqcnwzo.sHtML

Py:   os.getcwd()
来源：http://read.share.hesvh.cn/Article/details/gdajquvgt.sHtML

PHP:  getcwd();
来源：http://m.share.zdbjq.cn/Article/details/gjmfpjxys.sHtML

JS:   process.cwd()
来源：http://www.m.share.zdbjq.cn/Article/details/gzegelmgm.sHtML

TS:   process.cwd()
来源：http://m.share.zdbjq.cn/Article/details/gorvihibr.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.zdbjq.cn/Article/details/gqhgrslqy.sHtML

Go:   os.Getwd()
来源：http://www.share.fehbvm.com/Article/details/gghdvhncu.sHtML

Ruby: Dir.pwd
来源：http://3g.hesvh.cn/Article/details/gwlkbssgw.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.hesvh.cn/Article/details/gejjkwiyp.sHtML

[M05] 设置退出码
来源：http://baike.hesvh.cn/Article/details/gcwqlrqzk.sHtML

Py:   sys.exit(1)
来源：http://3g.zdbjq.cn/Article/details/geezhknwj.sHtML

PHP:  exit(1);
来源：http://baike.hesvh.cn/Article/details/grntmckln.sHtML

JS:   process.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gknodjbmk.sHtML

TS:   process.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/ghzcwrcca.sHtML

Java: System.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/geigdvupl.sHtML

Go:   os.Exit(1)
来源：http://baike.hesvh.cn/Article/details/gjffhedui.sHtML

Ruby: exit 1
来源：http://blog.zdbjq.cn/Article/details/glacsyyjg.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.fehbvm.com/Article/details/gpiadkjki.sHtML

[M06] 向标准错误输出
来源：http://3g.zdbjq.cn/Article/details/ghbjpkafv.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.fehbvm.com/Article/details/gycadvqwh.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.zdbjq.cn/Article/details/ggsptkxit.sHtML

JS:   console.error("err")
来源：http://3g.fehbvm.com/Article/details/gzxpxnmmn.sHtML

TS:   console.error("err")
来源：http://baike.zdbjq.cn/Article/details/gwavcfjjj.sHtML

Java: System.err.println("err")
来源：http://wap.hesvh.cn/Article/details/gqgeizykv.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.zdbjq.cn/Article/details/grwzxbmud.sHtML

Ruby: warn "err"
来源：http://m.share.hesvh.cn/Article/details/ghjvpsgsz.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.hesvh.cn/Article/details/gfhbhnyqy.sHtML

[M07] 判断是否为主入口
来源：http://baike.fehbvm.com/Article/details/gauheriic.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.hesvh.cn/Article/details/gxfjitqmw.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.fehbvm.com/Article/details/gopzyqrou.sHtML

JS:   require.main === module
来源：http://m.share.fehbvm.com/Article/details/gzivajoyb.sHtML

TS:   require.main === module
来源：http://read.share.hesvh.cn/Article/details/gnmtlqjbk.sHtML

Java: public static void main(String[] args)
来源：http://read.share.fehbvm.com/Article/details/gzjilrxps.sHtML

Go:   func main()
来源：http://3g.zdbjq.cn/Article/details/gwtfoukum.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.zdbjq.cn/Article/details/gejxfyzqe.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.zdbjq.cn/Article/details/gqdgzypsy.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.hesvh.cn/Article/details/gbonupzqi.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.hesvh.cn/Article/details/gigirylir.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.zdbjq.cn/Article/details/ggdplqcbi.sHtML

JS:   process.platform;  process.version
来源：http://read.share.zdbjq.cn/Article/details/gbsihueeh.sHtML

TS:   process.platform;  process.version
来源：http://mobile.hesvh.cn/Article/details/gguzjvvjc.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.zdbjq.cn/Article/details/gtoftwzxu.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.hesvh.cn/Article/details/gfagtxgsp.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.hesvh.cn/Article/details/gtzfhmlzi.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.zdbjq.cn/Article/details/gxdrajdzy.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gwhhqsbes.sHtML

N. 数据结构与算法
来源：http://www.blog.hesvh.cn/Article/details/gbjmwytdc.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/glduzshto.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.zdbjq.cn/Article/details/goeuqfqva.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.hesvh.cn/Article/details/ghnnzshqf.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.hesvh.cn/Article/details/gvwzxqvqm.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.fehbvm.com/Article/details/gvcfgxcoh.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.zdbjq.cn/Article/details/gxhhsskod.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.fehbvm.com/Article/details/gsxuefbmh.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.fehbvm.com/Article/details/gqavwpljr.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.hesvh.cn/Article/details/gkpzxyvmp.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gddadpekj.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.fehbvm.com/Article/details/gjlsflldp.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.hesvh.cn/Article/details/gldugxkjv.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.fehbvm.com/Article/details/gwutdpcib.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.zdbjq.cn/Article/details/gqsddmxsx.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.hesvh.cn/Article/details/gzvlkdfzv.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.zdbjq.cn/Article/details/gyrarhctf.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gljorhdur.sHtML

Ruby: arr.sort
来源：http://blog.fehbvm.com/Article/details/gjklcqhmy.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.hesvh.cn/Article/details/gfatleled.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.hesvh.cn/Article/details/gsbrprxcr.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.zdbjq.cn/Article/details/gssternyu.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.hesvh.cn/Article/details/gvblbyxvs.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.zdbjq.cn/Article/details/giukxkqxi.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.fehbvm.com/Article/details/gfmzfoepr.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.fehbvm.com/Article/details/gkkpofaww.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.fehbvm.com/Article/details/gamjdyjbp.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.fehbvm.com/Article/details/grzjkjogw.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.zdbjq.cn/Article/details/gzqhokvww.sHtML

[N04] 斐波那契数列
来源：http://baike.fehbvm.com/Article/details/gicdlcnhh.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.zdbjq.cn/Article/details/gtylvbqpn.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.hesvh.cn/Article/details/geuyhwtkq.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.zdbjq.cn/Article/details/gxtimjdhi.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.zdbjq.cn/Article/details/gqsvgayuy.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.fehbvm.com/Article/details/ghxbredum.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.hesvh.cn/Article/details/gnkqexwgr.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.zdbjq.cn/Article/details/ggkmsyewh.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.fehbvm.com/Article/details/gdjxljkhw.sHtML

[N05] 最大公约数
来源：http://www.share.zdbjq.cn/Article/details/gsqavpksz.sHtML

Py:   math.gcd(a, b)
来源：http://blog.fehbvm.com/Article/details/gtlcuavwh.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.fehbvm.com/Article/details/ggasziqhm.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.fehbvm.com/Article/details/gxiqmqoxc.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.zdbjq.cn/Article/details/gugrzrlti.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.fehbvm.com/Article/details/geacvceyk.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.zdbjq.cn/Article/details/ggotqfpjj.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gnqnetyww.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.fehbvm.com/Article/details/gmyzbxikt.sHtML

[N06] 判断回文字符串
来源：http://www.share.hesvh.cn/Article/details/gbnazqoew.sHtML

Py:   s == s[::-1]
来源：http://3g.hesvh.cn/Article/details/grkfnznhg.sHtML

PHP:  $s === strrev($s);
来源：http://wap.hesvh.cn/Article/details/glhnpipyt.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/gpfkzgiso.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/gfesodifl.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.zdbjq.cn/Article/details/gcuadrysc.sHtML

Go:   // 双指针从两端比较
来源：http://wap.fehbvm.com/Article/details/gcfqzhzzc.sHtML

Ruby: s == s.reverse
来源：http://baike.hesvh.cn/Article/details/guhjmrfum.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.hesvh.cn/Article/details/geduqrqig.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.hesvh.cn/Article/details/gtajlmcfw.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.hesvh.cn/Article/details/guuqhytbu.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.fehbvm.com/Article/details/gzrdnnqfu.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.hesvh.cn/Article/details/gvxknmaen.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.zdbjq.cn/Article/details/gyxtzlprm.sHtML

Java: // 手写 HashMap
来源：http://blog.fehbvm.com/Article/details/ghlriawke.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.fehbvm.com/Article/details/ghxapcvwp.sHtML

Ruby: // 手写 Hash
来源：http://www.share.hesvh.cn/Article/details/gsvvcenmw.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.hesvh.cn/Article/details/gicildler.sHtML

[N08] 生成全排列
来源：http://read.share.fehbvm.com/Article/details/gcsqqctgg.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.zdbjq.cn/Article/details/gchdzogba.sHtML

PHP:  // 手写递归交换
来源：http://3g.hesvh.cn/Article/details/ghvnvwadf.sHtML

JS:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gmugxvmgt.sHtML

TS:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gllwhoyrs.sHtML

Java: // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gfhczktaf.sHtML

Go:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gujbxverr.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.zdbjq.cn/Article/details/gipotsplg.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gknfdamee.sHtML

[N09] 栈与队列
来源：http://read.share.fehbvm.com/Article/details/ghcaefhdk.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.hesvh.cn/Article/details/gycnkstft.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.hesvh.cn/Article/details/ggqlbjrbf.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.zdbjq.cn/Article/details/grzofsxuw.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.hesvh.cn/Article/details/gjweosovx.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.zdbjq.cn/Article/details/gvmvyvork.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.zdbjq.cn/Article/details/gywchqjsn.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.fehbvm.com/Article/details/gtwryflfn.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.zdbjq.cn/Article/details/gzdmlsgcf.sHtML

[N10] 链表节点定义
来源：http://baike.hesvh.cn/Article/details/gpedsvryw.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.fehbvm.com/Article/details/gktxuougd.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.fehbvm.com/Article/details/gorsxiyzu.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.fehbvm.com/Article/details/gunimcjtx.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.fehbvm.com/Article/details/gvrahbtyw.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.fehbvm.com/Article/details/guequduvn.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.hesvh.cn/Article/details/gzvniojzh.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.fehbvm.com/Article/details/ggzzwthuj.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.fehbvm.com/Article/details/gaagoxavf.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.hesvh.cn/Article/details/gegmnvbux.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.zdbjq.cn/Article/details/grbdrxiyz.sHtML

PHP:  // 手写递归函数
来源：http://www.share.fehbvm.com/Article/details/gcvcoxixc.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.zdbjq.cn/Article/details/giucxuhbt.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.zdbjq.cn/Article/details/gxvzeugfy.sHtML

Java: // 手写递归
来源：http://mobile.zdbjq.cn/Article/details/gfhxztuvh.sHtML

Go:   // 手写递归
来源：http://wap.fehbvm.com/Article/details/gnglnnoyj.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.hesvh.cn/Article/details/gxlodhwjy.sHtML

C#:   // 手写递归
来源：http://3g.hesvh.cn/Article/details/gkatacftx.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.fehbvm.com/Article/details/gmydfguwz.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.hesvh.cn/Article/details/gvrmyrasx.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.hesvh.cn/Article/details/glhofhuwe.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.hesvh.cn/Article/details/giylbkptb.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.fehbvm.com/Article/details/gmdywdnsf.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.fehbvm.com/Article/details/goyxsesrx.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.hesvh.cn/Article/details/gseofqwvk.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.hesvh.cn/Article/details/ganjaogzh.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.hesvh.cn/Article/details/ggadkwnya.sHtML


<!-- 参考信息 -->