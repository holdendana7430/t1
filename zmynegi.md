代发 wailian999

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://read.share.fehbvm.com/Article/details/gtjjyqxon.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://wap.hesvh.cn/Article/details/gujyswzum.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.share.fehbvm.com/Article/details/gqmreecrq.sHtML

[K05] 深拷贝对象
来源：http://www.m.share.zdbjq.cn/Article/details/gaovktaxg.sHtML

Py:   copy.deepcopy(obj)
来源：http://wap.hesvh.cn/Article/details/gtrrqjdtr.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.share.fehbvm.com/Article/details/gnvhaipno.sHtML

JS:   structuredClone(obj)
来源：http://read.share.fehbvm.com/Article/details/gysofmrup.sHtML

TS:   structuredClone(obj)
来源：http://www.blog.fehbvm.com/Article/details/grxodajye.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.share.fehbvm.com/Article/details/gptkxbqnu.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://3g.hesvh.cn/Article/details/gnsjnlaeo.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://3g.hesvh.cn/Article/details/gwylmmzyl.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://mobile.fehbvm.com/Article/details/gxputjfcw.sHtML

[K06] 解析 URL 查询串
来源：http://m.share.fehbvm.com/Article/details/ghznzotgc.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://m.share.fehbvm.com/Article/details/gevcqyzgz.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.blog.fehbvm.com/Article/details/gwoedwnjs.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.zdbjq.cn/Article/details/gxuyrmsxs.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.zdbjq.cn/Article/details/gmlpvlnba.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://m.share.zdbjq.cn/Article/details/gzmezhwgi.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://read.share.fehbvm.com/Article/details/gogyvgear.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.fehbvm.com/Article/details/gwjhgdntp.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mobile.hesvh.cn/Article/details/gkmoxxrcj.sHtML

[K07] 进制转换
来源：http://baike.fehbvm.com/Article/details/ghkzliqvm.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mobile.hesvh.cn/Article/details/gnhcvfluv.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.share.hesvh.cn/Article/details/ggzoekcux.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.hesvh.cn/Article/details/gbyypdpar.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wap.zdbjq.cn/Article/details/gttslpzoj.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.hesvh.cn/Article/details/gdhobxbih.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.zdbjq.cn/Article/details/glmltxozn.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://baike.fehbvm.com/Article/details/ghfkauccn.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mobile.zdbjq.cn/Article/details/ghqmxnodq.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.zdbjq.cn/Article/details/glmrafycb.sHtML

Py:   pickle.dumps(obj)
来源：http://wap.zdbjq.cn/Article/details/gnadplcsn.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://baike.hesvh.cn/Article/details/gbpgqxbip.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.zdbjq.cn/Article/details/gdfbmmpat.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://mobile.hesvh.cn/Article/details/gmwtuzxrk.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.hesvh.cn/Article/details/grskcaloe.sHtML

Go:   encoding/gob
来源：http://blog.hesvh.cn/Article/details/gdyebuuae.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.zdbjq.cn/Article/details/gmdieamkn.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.fehbvm.com/Article/details/gtjkuxhtb.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gekeldnnw.sHtML

L. 网络请求
来源：http://mobile.hesvh.cn/Article/details/gylclsbtu.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gvaxwbbgm.sHtML

[L01] 发送 GET 请求
来源：http://mobile.zdbjq.cn/Article/details/gqxkxumbb.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.hesvh.cn/Article/details/gcardcyjs.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.m.share.hesvh.cn/Article/details/gmjqpmuaz.sHtML

JS:   await fetch(url)
来源：http://blog.fehbvm.com/Article/details/gnfhkwdhd.sHtML

TS:   await fetch(url)
来源：http://m.share.fehbvm.com/Article/details/gdrdhnqho.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.m.share.zdbjq.cn/Article/details/gbbwdvzwu.sHtML

Go:   resp, err := http.Get(url)
来源：http://mobile.zdbjq.cn/Article/details/gsmyjyepy.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.m.share.fehbvm.com/Article/details/gphhxacqn.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.zdbjq.cn/Article/details/gxioekbnm.sHtML

[L02] 发送 POST JSON
来源：http://wap.fehbvm.com/Article/details/gjcpgnjdt.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.share.hesvh.cn/Article/details/gftvycftv.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://baike.fehbvm.com/Article/details/gdxmqglpa.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.fehbvm.com/Article/details/giynyzomo.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.zdbjq.cn/Article/details/gobulgxhk.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.fehbvm.com/Article/details/ggyydvbhl.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.hesvh.cn/Article/details/ghbbgkemi.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://blog.zdbjq.cn/Article/details/gpvnowqda.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.zdbjq.cn/Article/details/gkmaktqqg.sHtML

[L03] 设置自定义请求头
来源：http://blog.fehbvm.com/Article/details/gvgwttoff.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.hesvh.cn/Article/details/gvzrmvmja.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.hesvh.cn/Article/details/ghpvmkphx.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.zdbjq.cn/Article/details/getvjdpxz.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.fehbvm.com/Article/details/gwkwhflli.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.hesvh.cn/Article/details/gyueossev.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.blog.hesvh.cn/Article/details/gxmssdlow.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.hesvh.cn/Article/details/gspqwctbv.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.hesvh.cn/Article/details/gonakaxuu.sHtML

[L04] 设置超时
来源：http://baike.hesvh.cn/Article/details/gfnjcrdre.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.zdbjq.cn/Article/details/gffbxjofw.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.zdbjq.cn/Article/details/gzlneneqt.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.zdbjq.cn/Article/details/gwnvkbron.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.fehbvm.com/Article/details/gfiojtjyy.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.fehbvm.com/Article/details/grscpwehj.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.zdbjq.cn/Article/details/ganzirqea.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.fehbvm.com/Article/details/gobkmlntr.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.fehbvm.com/Article/details/glregyfxl.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.hesvh.cn/Article/details/ghnajpbif.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://read.share.fehbvm.com/Article/details/gtmospyxr.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.zdbjq.cn/Article/details/gegbblgud.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.zdbjq.cn/Article/details/gcgmhdhky.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.hesvh.cn/Article/details/gitddivrr.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.zdbjq.cn/Article/details/gjgsyaytv.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.fehbvm.com/Article/details/gebdulbye.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.hesvh.cn/Article/details/gavegvlxg.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.hesvh.cn/Article/details/gnfsaxooa.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.hesvh.cn/Article/details/grmmjsgsb.sHtML

Py:   resp.json()
来源：http://baike.zdbjq.cn/Article/details/gseoiveuz.sHtML

PHP:  json_decode($body, true);
来源：http://blog.zdbjq.cn/Article/details/gcrckkxyh.sHtML

JS:   await resp.json()
来源：http://blog.hesvh.cn/Article/details/gckgrgynk.sHtML

TS:   await resp.json()
来源：http://www.blog.fehbvm.com/Article/details/gmnjqsdie.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.hesvh.cn/Article/details/gxkwqaxyd.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.hesvh.cn/Article/details/gfjkhptkf.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.fehbvm.com/Article/details/gopurpeda.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.fehbvm.com/Article/details/gzqqghpfm.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.fehbvm.com/Article/details/gzzdodthf.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.zdbjq.cn/Article/details/galttmiwh.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.fehbvm.com/Article/details/geaykmwwf.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.hesvh.cn/Article/details/gndfooeqm.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.fehbvm.com/Article/details/giiajotbd.sHtML

Java: resp.statusCode()
来源：http://3g.fehbvm.com/Article/details/giwiwauzw.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.zdbjq.cn/Article/details/giawvkbfy.sHtML

Ruby: resp.code.to_i
来源：http://read.share.zdbjq.cn/Article/details/gnxuubqze.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.fehbvm.com/Article/details/gzbyhgvst.sHtML

[L08] 并发请求多个地址
来源：http://www.share.fehbvm.com/Article/details/gdnjnsjxw.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.hesvh.cn/Article/details/gbixazooz.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.zdbjq.cn/Article/details/gmdqjoxsr.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.hesvh.cn/Article/details/gjrzvzhbz.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.hesvh.cn/Article/details/ghqywbrot.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.zdbjq.cn/Article/details/ggwcaixwu.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.zdbjq.cn/Article/details/gglsrtset.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.fehbvm.com/Article/details/gopydhtwr.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.hesvh.cn/Article/details/gfnbhvajk.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gbzbmkonn.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.fehbvm.com/Article/details/gatbxsxgj.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gvvpojhrx.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.zdbjq.cn/Article/details/gpntmqggs.sHtML

Py:   sys.argv[1:]
来源：http://wap.zdbjq.cn/Article/details/ggfogiapo.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.zdbjq.cn/Article/details/gzqqbpfvm.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.fehbvm.com/Article/details/gkceriujk.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.zdbjq.cn/Article/details/gchlnhpuc.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.zdbjq.cn/Article/details/guccijhuz.sHtML

Go:   os.Args[1:]
来源：http://read.share.hesvh.cn/Article/details/gydzsvmis.sHtML

Ruby: ARGV
来源：http://www.share.zdbjq.cn/Article/details/ggvhfbkpc.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.fehbvm.com/Article/details/gbfvmnluy.sHtML

[M02] 读取环境变量
来源：http://baike.zdbjq.cn/Article/details/ggghuhguv.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.hesvh.cn/Article/details/gwncjdmlg.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.fehbvm.com/Article/details/giotymysp.sHtML

JS:   process.env.HOME
来源：http://m.share.fehbvm.com/Article/details/gebhorjpe.sHtML

TS:   process.env.HOME
来源：http://wap.fehbvm.com/Article/details/gpfaopvvn.sHtML

Java: System.getenv("HOME")
来源：http://3g.fehbvm.com/Article/details/gjdijpaoj.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.zdbjq.cn/Article/details/gtsgqtgkb.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.hesvh.cn/Article/details/gdvhikfws.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/gfzzsokrr.sHtML

[M03] 执行外部命令
来源：http://blog.zdbjq.cn/Article/details/gclwgbets.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.hesvh.cn/Article/details/gjutmadex.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.fehbvm.com/Article/details/gpqgrmree.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.hesvh.cn/Article/details/grefqgzrd.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.hesvh.cn/Article/details/gpmpbqqtm.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.zdbjq.cn/Article/details/ggwaoafvs.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.zdbjq.cn/Article/details/gnhurxiwt.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.zdbjq.cn/Article/details/gclcldvhq.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.fehbvm.com/Article/details/gqxxwifgj.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.zdbjq.cn/Article/details/ggabaejyz.sHtML

Py:   os.getcwd()
来源：http://read.share.hesvh.cn/Article/details/guvekvpqu.sHtML

PHP:  getcwd();
来源：http://www.blog.hesvh.cn/Article/details/ggnfhxsrv.sHtML

JS:   process.cwd()
来源：http://wap.fehbvm.com/Article/details/gdadvediv.sHtML

TS:   process.cwd()
来源：http://www.m.share.hesvh.cn/Article/details/goajxpvlk.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.hesvh.cn/Article/details/gizkbieti.sHtML

Go:   os.Getwd()
来源：http://www.share.fehbvm.com/Article/details/gzyyortlh.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.zdbjq.cn/Article/details/gecrepfnt.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.hesvh.cn/Article/details/gfyssxolr.sHtML

[M05] 设置退出码
来源：http://mobile.fehbvm.com/Article/details/gpdfsxars.sHtML

Py:   sys.exit(1)
来源：http://wap.zdbjq.cn/Article/details/gxwhkuhdb.sHtML

PHP:  exit(1);
来源：http://m.share.hesvh.cn/Article/details/gsyhfoehh.sHtML

JS:   process.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gjqrqlowj.sHtML

TS:   process.exit(1)
来源：http://mobile.hesvh.cn/Article/details/gzeovzsxs.sHtML

Java: System.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gljfiuskw.sHtML

Go:   os.Exit(1)
来源：http://www.share.hesvh.cn/Article/details/glykwflxf.sHtML

Ruby: exit 1
来源：http://www.share.hesvh.cn/Article/details/gahdyejuf.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.fehbvm.com/Article/details/gaquzaieb.sHtML

[M06] 向标准错误输出
来源：http://3g.fehbvm.com/Article/details/gerswzsxa.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.zdbjq.cn/Article/details/gdafccfht.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.fehbvm.com/Article/details/gkhuahdyp.sHtML

JS:   console.error("err")
来源：http://3g.fehbvm.com/Article/details/gmmeytdkw.sHtML

TS:   console.error("err")
来源：http://3g.hesvh.cn/Article/details/gqcmnlfwc.sHtML

Java: System.err.println("err")
来源：http://m.share.hesvh.cn/Article/details/gkpfhneng.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.zdbjq.cn/Article/details/gfksdqpzy.sHtML

Ruby: warn "err"
来源：http://mobile.zdbjq.cn/Article/details/gmziwvqic.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.fehbvm.com/Article/details/giniuodjn.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.fehbvm.com/Article/details/gfgkvzspb.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.hesvh.cn/Article/details/gfdkjbwgq.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.fehbvm.com/Article/details/gyzumjnpa.sHtML

JS:   require.main === module
来源：http://www.m.share.zdbjq.cn/Article/details/gegcldwsi.sHtML

TS:   require.main === module
来源：http://read.share.hesvh.cn/Article/details/gnsnncodu.sHtML

Java: public static void main(String[] args)
来源：http://baike.fehbvm.com/Article/details/gqrakypdf.sHtML

Go:   func main()
来源：http://www.blog.hesvh.cn/Article/details/geokupqys.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.zdbjq.cn/Article/details/gdmjstlka.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.fehbvm.com/Article/details/gqikuiznl.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.zdbjq.cn/Article/details/gildxnspu.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.fehbvm.com/Article/details/gboqdlmqn.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.zdbjq.cn/Article/details/giudjcxxc.sHtML

JS:   process.platform;  process.version
来源：http://m.share.fehbvm.com/Article/details/glnqdkomo.sHtML

TS:   process.platform;  process.version
来源：http://blog.fehbvm.com/Article/details/gqqermyma.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.hesvh.cn/Article/details/gfdcdihlq.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.fehbvm.com/Article/details/gupkfloyo.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.hesvh.cn/Article/details/gqlkgpgjr.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.fehbvm.com/Article/details/gjhbauilq.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/goximwpkh.sHtML

N. 数据结构与算法
来源：http://mobile.fehbvm.com/Article/details/gzsvdxren.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/guqqjgfvo.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.hesvh.cn/Article/details/gtvmybetr.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/grplwgkde.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.hesvh.cn/Article/details/gjbaqlbcy.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.hesvh.cn/Article/details/gwfmiavzy.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.zdbjq.cn/Article/details/guidogzlw.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gqtisfded.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gutnkfoob.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.hesvh.cn/Article/details/gktkevkmk.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gatgslznc.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.hesvh.cn/Article/details/ghhugblka.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.hesvh.cn/Article/details/gugjoxvjd.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.fehbvm.com/Article/details/gpfsgvslu.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.zdbjq.cn/Article/details/gotfxtbcx.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.fehbvm.com/Article/details/gzfvnbfkk.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.fehbvm.com/Article/details/gwgomusqt.sHtML

Go:   slices.Sort(arr)
来源：http://blog.fehbvm.com/Article/details/gmgybtatt.sHtML

Ruby: arr.sort
来源：http://wap.fehbvm.com/Article/details/gfgzbxknf.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.zdbjq.cn/Article/details/gjiizbfmd.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.zdbjq.cn/Article/details/gjunqfpav.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.hesvh.cn/Article/details/ggeatzgfz.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.hesvh.cn/Article/details/gtzfavxox.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.hesvh.cn/Article/details/glxrysmmc.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.fehbvm.com/Article/details/goetabdnz.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.fehbvm.com/Article/details/gmgmujvlo.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.fehbvm.com/Article/details/gtirzpjcb.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.hesvh.cn/Article/details/ghdkoyoqq.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.zdbjq.cn/Article/details/gxkusmgev.sHtML

[N04] 斐波那契数列
来源：http://wap.hesvh.cn/Article/details/gulhoktto.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.zdbjq.cn/Article/details/gpckleexz.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.fehbvm.com/Article/details/gvvhjmyor.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.fehbvm.com/Article/details/gvspccbfs.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.zdbjq.cn/Article/details/gugqgwgxs.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.fehbvm.com/Article/details/gfgzsniwu.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.zdbjq.cn/Article/details/gvisozoro.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.fehbvm.com/Article/details/gcjyspcov.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/gseerjmfv.sHtML

[N05] 最大公约数
来源：http://www.share.fehbvm.com/Article/details/ghychrbhc.sHtML

Py:   math.gcd(a, b)
来源：http://baike.zdbjq.cn/Article/details/gixobwkih.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.hesvh.cn/Article/details/gcdatpenh.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.fehbvm.com/Article/details/gavvaohtz.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.zdbjq.cn/Article/details/gmbmnbzif.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.fehbvm.com/Article/details/gpztdwtne.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.hesvh.cn/Article/details/gnwqzgumm.sHtML

Ruby: a.gcd(b)
来源：http://read.share.hesvh.cn/Article/details/grxlactrl.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.fehbvm.com/Article/details/gzcezjtlj.sHtML

[N06] 判断回文字符串
来源：http://read.share.zdbjq.cn/Article/details/gbiixcezm.sHtML

Py:   s == s[::-1]
来源：http://3g.hesvh.cn/Article/details/gtdnjjnxy.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.zdbjq.cn/Article/details/gevxuztqj.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/ganaricvz.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/gfiuwyaol.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.fehbvm.com/Article/details/gtmmsstuj.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.zdbjq.cn/Article/details/gwuswjwjt.sHtML

Ruby: s == s.reverse
来源：http://baike.hesvh.cn/Article/details/gdezhurfn.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.zdbjq.cn/Article/details/gnjzjmokz.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.fehbvm.com/Article/details/gseiytkzj.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.hesvh.cn/Article/details/gpqvtkosr.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.hesvh.cn/Article/details/gmrldygcb.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.hesvh.cn/Article/details/guftnwchq.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.hesvh.cn/Article/details/gpspiwohr.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.zdbjq.cn/Article/details/geiacolig.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.hesvh.cn/Article/details/gqmkddawn.sHtML

Ruby: // 手写 Hash
来源：http://m.share.zdbjq.cn/Article/details/gemyefkah.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.fehbvm.com/Article/details/garqzjdkt.sHtML

[N08] 生成全排列
来源：http://m.share.hesvh.cn/Article/details/gcmokcukb.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.fehbvm.com/Article/details/gmxwtermm.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.zdbjq.cn/Article/details/gyyssqseu.sHtML

JS:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/ghhsaifhm.sHtML

TS:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gbtcgyecu.sHtML

Java: // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/ghqcxxucs.sHtML

Go:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gtvvvogqz.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.hesvh.cn/Article/details/gisyjrvvq.sHtML

C#:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gwwoogbsc.sHtML

[N09] 栈与队列
来源：http://m.share.hesvh.cn/Article/details/gjbfelcyh.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.hesvh.cn/Article/details/gjinefegz.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.hesvh.cn/Article/details/gzvjgqvgg.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.zdbjq.cn/Article/details/giwsxybet.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.hesvh.cn/Article/details/gsilrnjbs.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.hesvh.cn/Article/details/gmupzxcjo.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.hesvh.cn/Article/details/ghyyfzrmk.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.zdbjq.cn/Article/details/gpyxnjmzr.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.hesvh.cn/Article/details/grclaqygi.sHtML

[N10] 链表节点定义
来源：http://www.m.share.hesvh.cn/Article/details/guspmrayq.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.hesvh.cn/Article/details/gewtkrbjc.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.fehbvm.com/Article/details/gexowpcft.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.zdbjq.cn/Article/details/gjskmxufh.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.hesvh.cn/Article/details/gdlwvbzox.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.fehbvm.com/Article/details/gpqrrramp.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.hesvh.cn/Article/details/gnkbltjvf.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.fehbvm.com/Article/details/gnxqpdqpb.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.zdbjq.cn/Article/details/gzahkbgaj.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.hesvh.cn/Article/details/ghdriuuoq.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.hesvh.cn/Article/details/gjtftkpku.sHtML

PHP:  // 手写递归函数
来源：http://blog.fehbvm.com/Article/details/gbvukqrof.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.fehbvm.com/Article/details/gqvrvwayu.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.zdbjq.cn/Article/details/gacwqmthp.sHtML

Java: // 手写递归
来源：http://m.share.hesvh.cn/Article/details/guegftidp.sHtML

Go:   // 手写递归
来源：http://mobile.zdbjq.cn/Article/details/gsuosdtby.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.hesvh.cn/Article/details/ghnmvopwz.sHtML

C#:   // 手写递归
来源：http://wap.zdbjq.cn/Article/details/garkqivys.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.fehbvm.com/Article/details/glgwblzhs.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.hesvh.cn/Article/details/gjwnmghwc.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.zdbjq.cn/Article/details/gjdbanqjo.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.hesvh.cn/Article/details/gjixqdbon.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.hesvh.cn/Article/details/giyxvmoco.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.zdbjq.cn/Article/details/grphjpmip.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.hesvh.cn/Article/details/gxsmnyjhh.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.hesvh.cn/Article/details/gzqwzyxrp.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.zdbjq.cn/Article/details/gfetdshnt.sHtML


<!-- 参考信息 -->