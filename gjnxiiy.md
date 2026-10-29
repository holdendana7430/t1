代发 wailian999

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mobile.hesvh.cn/Article/details/gjqapfaud.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.hesvh.cn/Article/details/gohzwlgen.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.zdbjq.cn/Article/details/ghfcyobyw.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mobile.hesvh.cn/Article/details/gmxbhuser.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.m.share.fehbvm.com/Article/details/gmkdygopv.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.m.share.zdbjq.cn/Article/details/gssxwzmjh.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://3g.fehbvm.com/Article/details/gqmordbif.sHtML

[K05] 深拷贝对象
来源：http://www.m.share.fehbvm.com/Article/details/gknbuzvxj.sHtML

Py:   copy.deepcopy(obj)
来源：http://baike.hesvh.cn/Article/details/gjrwabgqv.sHtML

PHP:  unserialize(serialize($obj));
来源：http://mobile.hesvh.cn/Article/details/gojrvatap.sHtML

JS:   structuredClone(obj)
来源：http://www.share.fehbvm.com/Article/details/gqovhkixz.sHtML

TS:   structuredClone(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gafterjwh.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.zdbjq.cn/Article/details/grdhpxiun.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.hesvh.cn/Article/details/gsudvldqh.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://blog.fehbvm.com/Article/details/gtjnamtxj.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://wap.fehbvm.com/Article/details/gcdtyysfg.sHtML

[K06] 解析 URL 查询串
来源：http://www.blog.zdbjq.cn/Article/details/gvkbyxork.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.blog.fehbvm.com/Article/details/gnjktxuup.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.share.hesvh.cn/Article/details/gzxxuujtq.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.fehbvm.com/Article/details/ghmgabahx.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.zdbjq.cn/Article/details/gihcqphsj.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://m.share.zdbjq.cn/Article/details/gkrwhhxcy.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://3g.fehbvm.com/Article/details/geipvegff.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.m.share.hesvh.cn/Article/details/gnusqgzni.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.share.hesvh.cn/Article/details/gyibqvnxd.sHtML

[K07] 进制转换
来源：http://3g.fehbvm.com/Article/details/gembjzksx.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.zdbjq.cn/Article/details/gkvxeevzz.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://read.share.zdbjq.cn/Article/details/gpdcswxku.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.share.zdbjq.cn/Article/details/gpnfwpdwz.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://m.share.zdbjq.cn/Article/details/gdmsfahyk.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.fehbvm.com/Article/details/gvmqhfhup.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://blog.fehbvm.com/Article/details/gdshyxdqv.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.hesvh.cn/Article/details/gmbtnmrxx.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://m.share.hesvh.cn/Article/details/ggkhmozzp.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://read.share.fehbvm.com/Article/details/gxguyqtig.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.zdbjq.cn/Article/details/gqivuqjuf.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.hesvh.cn/Article/details/gelxibwht.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://3g.fehbvm.com/Article/details/gkjflydjd.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.hesvh.cn/Article/details/gwiaxdnnj.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.fehbvm.com/Article/details/gcbuyuxar.sHtML

Go:   encoding/gob
来源：http://blog.fehbvm.com/Article/details/gdcxdtpdr.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.hesvh.cn/Article/details/gduziwkdj.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://3g.zdbjq.cn/Article/details/gjhgfuqab.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gwqrnblkb.sHtML

L. 网络请求
来源：http://www.blog.zdbjq.cn/Article/details/gnqictous.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/godecsbff.sHtML

[L01] 发送 GET 请求
来源：http://3g.fehbvm.com/Article/details/gpvnfvwmm.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.hesvh.cn/Article/details/gttaaukcn.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.zdbjq.cn/Article/details/gogtsbkne.sHtML

JS:   await fetch(url)
来源：http://www.blog.fehbvm.com/Article/details/ggvwnaegs.sHtML

TS:   await fetch(url)
来源：http://www.blog.zdbjq.cn/Article/details/gudjqsrot.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.fehbvm.com/Article/details/gbufuyabm.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.fehbvm.com/Article/details/gbxrexuvh.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.hesvh.cn/Article/details/gizkrapak.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.zdbjq.cn/Article/details/gzmauklcq.sHtML

[L02] 发送 POST JSON
来源：http://baike.fehbvm.com/Article/details/gaubhfekc.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.fehbvm.com/Article/details/ghgynjbtr.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://read.share.hesvh.cn/Article/details/gctqulzdb.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.hesvh.cn/Article/details/gybmxfqgk.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.fehbvm.com/Article/details/gatkychvu.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.fehbvm.com/Article/details/gytbhukyc.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.zdbjq.cn/Article/details/glqqimido.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.zdbjq.cn/Article/details/gknsulqsi.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://read.share.zdbjq.cn/Article/details/gjzyetqpq.sHtML

[L03] 设置自定义请求头
来源：http://read.share.fehbvm.com/Article/details/gfryrpsth.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.hesvh.cn/Article/details/gslezvwew.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.blog.hesvh.cn/Article/details/ghqczierg.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.fehbvm.com/Article/details/gupavlftw.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.fehbvm.com/Article/details/gxroqtduz.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.zdbjq.cn/Article/details/gjlzappwc.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.zdbjq.cn/Article/details/ggfvtonhx.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.zdbjq.cn/Article/details/gcryncbxp.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.m.share.zdbjq.cn/Article/details/gjsorieda.sHtML

[L04] 设置超时
来源：http://baike.hesvh.cn/Article/details/gcgyufimg.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.hesvh.cn/Article/details/gpqvbfwyt.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.fehbvm.com/Article/details/gfibzsnav.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.hesvh.cn/Article/details/gqosmmtvw.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.fehbvm.com/Article/details/gnanrbrku.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.fehbvm.com/Article/details/gbwbrbptb.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.hesvh.cn/Article/details/gccsntjfy.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.fehbvm.com/Article/details/gpdejfwxd.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.fehbvm.com/Article/details/gdxnzyrll.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.hesvh.cn/Article/details/ggiajbron.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.hesvh.cn/Article/details/gevmrtqqn.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.zdbjq.cn/Article/details/ghdyfwkpm.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.hesvh.cn/Article/details/gmvfwagrq.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.zdbjq.cn/Article/details/gkxcrcrbk.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.zdbjq.cn/Article/details/gpjustojp.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.hesvh.cn/Article/details/gplzdklwd.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.zdbjq.cn/Article/details/gryfuxbpl.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.fehbvm.com/Article/details/gznfqbszy.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.fehbvm.com/Article/details/gwpsurbxn.sHtML

Py:   resp.json()
来源：http://baike.zdbjq.cn/Article/details/gdkyhwodm.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.fehbvm.com/Article/details/gcebetsjb.sHtML

JS:   await resp.json()
来源：http://blog.zdbjq.cn/Article/details/grtppzhdd.sHtML

TS:   await resp.json()
来源：http://www.m.share.zdbjq.cn/Article/details/gujdahwkk.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.hesvh.cn/Article/details/gptoigacy.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.zdbjq.cn/Article/details/gznixhlzs.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.fehbvm.com/Article/details/gkyxrnbfv.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.fehbvm.com/Article/details/guzqmngcw.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.fehbvm.com/Article/details/gbhlpufrp.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.hesvh.cn/Article/details/gapgjunek.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.hesvh.cn/Article/details/gcdqikaxh.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.fehbvm.com/Article/details/gtrlhzger.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.hesvh.cn/Article/details/gkgvnpuyr.sHtML

Java: resp.statusCode()
来源：http://mobile.fehbvm.com/Article/details/gjyzrfzol.sHtML

Go:   resp.StatusCode
来源：http://wap.fehbvm.com/Article/details/gcvdpdhxf.sHtML

Ruby: resp.code.to_i
来源：http://read.share.fehbvm.com/Article/details/gkteaewwj.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.fehbvm.com/Article/details/gcachklzr.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.fehbvm.com/Article/details/gsletygrg.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.fehbvm.com/Article/details/grjfzcwus.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.hesvh.cn/Article/details/gadkzfprg.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fehbvm.com/Article/details/gydonxbqr.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.zdbjq.cn/Article/details/gclchmuxv.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.fehbvm.com/Article/details/gxcwydjcc.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.fehbvm.com/Article/details/gafstdcjv.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.hesvh.cn/Article/details/gmrnoqfpa.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.fehbvm.com/Article/details/gtjhickms.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gulwtmsfc.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.fehbvm.com/Article/details/gcflykvcv.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/geytytmht.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.hesvh.cn/Article/details/ghrahhcer.sHtML

Py:   sys.argv[1:]
来源：http://mobile.zdbjq.cn/Article/details/ggxfxuzxk.sHtML

PHP:  $argv;  $argc;
来源：http://3g.hesvh.cn/Article/details/gybbmhnlr.sHtML

JS:   process.argv.slice(2)
来源：http://wap.hesvh.cn/Article/details/gyxgpxeaf.sHtML

TS:   process.argv.slice(2)
来源：http://wap.zdbjq.cn/Article/details/gghmzlmja.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.fehbvm.com/Article/details/gnvfjztzf.sHtML

Go:   os.Args[1:]
来源：http://baike.fehbvm.com/Article/details/ggdkdpzlw.sHtML

Ruby: ARGV
来源：http://www.blog.zdbjq.cn/Article/details/geebjhyig.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.zdbjq.cn/Article/details/gyuvwyiuc.sHtML

[M02] 读取环境变量
来源：http://mobile.fehbvm.com/Article/details/gbmvbyqox.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.hesvh.cn/Article/details/goiynaxib.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.zdbjq.cn/Article/details/gqdyuyydf.sHtML

JS:   process.env.HOME
来源：http://blog.hesvh.cn/Article/details/gymymmuzw.sHtML

TS:   process.env.HOME
来源：http://m.share.hesvh.cn/Article/details/gxrfmxfcl.sHtML

Java: System.getenv("HOME")
来源：http://3g.fehbvm.com/Article/details/gentldklw.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.hesvh.cn/Article/details/ggqvvutqd.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.fehbvm.com/Article/details/ggnbyndhr.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.zdbjq.cn/Article/details/gejmxhwmn.sHtML

[M03] 执行外部命令
来源：http://read.share.zdbjq.cn/Article/details/gcfzkdqns.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.hesvh.cn/Article/details/gusuhzans.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.fehbvm.com/Article/details/ghemlvdzq.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.hesvh.cn/Article/details/gcdvhpcot.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.fehbvm.com/Article/details/gmakrvvzh.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.fehbvm.com/Article/details/gtdaridue.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.hesvh.cn/Article/details/goglpijuq.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.zdbjq.cn/Article/details/gjnerccje.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.fehbvm.com/Article/details/gndiwjpyu.sHtML

[M04] 获取当前工作目录
来源：http://read.share.fehbvm.com/Article/details/gzeqohujl.sHtML

Py:   os.getcwd()
来源：http://www.m.share.fehbvm.com/Article/details/gvgzhdjwy.sHtML

PHP:  getcwd();
来源：http://www.m.share.fehbvm.com/Article/details/gpmhxrsvy.sHtML

JS:   process.cwd()
来源：http://www.m.share.hesvh.cn/Article/details/guifltzvd.sHtML

TS:   process.cwd()
来源：http://blog.fehbvm.com/Article/details/gqfcpmeci.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.hesvh.cn/Article/details/ghlxqmzpm.sHtML

Go:   os.Getwd()
来源：http://www.blog.fehbvm.com/Article/details/gojgunmid.sHtML

Ruby: Dir.pwd
来源：http://www.blog.fehbvm.com/Article/details/gxryyydzx.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.hesvh.cn/Article/details/gbayxouus.sHtML

[M05] 设置退出码
来源：http://mobile.fehbvm.com/Article/details/gaomeazel.sHtML

Py:   sys.exit(1)
来源：http://wap.hesvh.cn/Article/details/gawxwsrxv.sHtML

PHP:  exit(1);
来源：http://www.share.fehbvm.com/Article/details/gqggwvyfm.sHtML

JS:   process.exit(1)
来源：http://blog.fehbvm.com/Article/details/gobfjrjam.sHtML

TS:   process.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gbfhixhan.sHtML

Java: System.exit(1)
来源：http://read.share.fehbvm.com/Article/details/gcxxwgxlb.sHtML

Go:   os.Exit(1)
来源：http://wap.hesvh.cn/Article/details/gbdwwmupn.sHtML

Ruby: exit 1
来源：http://www.m.share.hesvh.cn/Article/details/gboqayrcf.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.hesvh.cn/Article/details/glhmcenti.sHtML

[M06] 向标准错误输出
来源：http://blog.zdbjq.cn/Article/details/gexrvzljn.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.hesvh.cn/Article/details/guwkkteja.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.fehbvm.com/Article/details/gkgtlceul.sHtML

JS:   console.error("err")
来源：http://3g.hesvh.cn/Article/details/gkpgbwaao.sHtML

TS:   console.error("err")
来源：http://read.share.fehbvm.com/Article/details/gnottykuh.sHtML

Java: System.err.println("err")
来源：http://www.blog.fehbvm.com/Article/details/gzndlixsq.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.hesvh.cn/Article/details/gypmjwjpm.sHtML

Ruby: warn "err"
来源：http://wap.hesvh.cn/Article/details/gsmcwpiee.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.hesvh.cn/Article/details/gtrdpbint.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.hesvh.cn/Article/details/geefxotgl.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.hesvh.cn/Article/details/gnqaadeyk.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.fehbvm.com/Article/details/gliucuctd.sHtML

JS:   require.main === module
来源：http://www.m.share.zdbjq.cn/Article/details/gwwpyxywm.sHtML

TS:   require.main === module
来源：http://wap.zdbjq.cn/Article/details/glnwclcke.sHtML

Java: public static void main(String[] args)
来源：http://mobile.zdbjq.cn/Article/details/gwnhyfqnj.sHtML

Go:   func main()
来源：http://read.share.hesvh.cn/Article/details/govuovaps.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.zdbjq.cn/Article/details/gqfelsazx.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.hesvh.cn/Article/details/glduwvtio.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.fehbvm.com/Article/details/gtgqzydou.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.zdbjq.cn/Article/details/guphoayin.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.zdbjq.cn/Article/details/gkgnlsvxg.sHtML

JS:   process.platform;  process.version
来源：http://read.share.fehbvm.com/Article/details/glgbpjdmo.sHtML

TS:   process.platform;  process.version
来源：http://blog.fehbvm.com/Article/details/gtpnnccau.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.zdbjq.cn/Article/details/gnksnrtmy.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.hesvh.cn/Article/details/grysvxpwn.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.fehbvm.com/Article/details/gpjovjkfn.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.zdbjq.cn/Article/details/gswlfgekx.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gjcsdosgc.sHtML

N. 数据结构与算法
来源：http://www.m.share.fehbvm.com/Article/details/gplpywnzx.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gjiaqqurd.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.fehbvm.com/Article/details/gybziynvb.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.fehbvm.com/Article/details/gzenowjef.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.zdbjq.cn/Article/details/geytftjpn.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.zdbjq.cn/Article/details/gvwrwdnoj.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.hesvh.cn/Article/details/giqxvhytg.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gdxvygjyy.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/giwgbgfqo.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.hesvh.cn/Article/details/gddhwhajw.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gtemgixep.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.zdbjq.cn/Article/details/gkpieackr.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.zdbjq.cn/Article/details/gzgsozuvp.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.hesvh.cn/Article/details/gfuxakdkw.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.zdbjq.cn/Article/details/gavzwnhvc.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.zdbjq.cn/Article/details/gtwtrgmid.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.hesvh.cn/Article/details/gthslobjs.sHtML

Go:   slices.Sort(arr)
来源：http://blog.zdbjq.cn/Article/details/gqzycvlue.sHtML

Ruby: arr.sort
来源：http://www.blog.zdbjq.cn/Article/details/giuiekdhn.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.zdbjq.cn/Article/details/gfstuabll.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.hesvh.cn/Article/details/ggqscmige.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.hesvh.cn/Article/details/gopkhjwro.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.fehbvm.com/Article/details/gigujbfeu.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.zdbjq.cn/Article/details/gborvcvyf.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.zdbjq.cn/Article/details/gjelxzyit.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.zdbjq.cn/Article/details/ggjmtwsdx.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.fehbvm.com/Article/details/ggeaeczax.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.fehbvm.com/Article/details/girekxnnb.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.fehbvm.com/Article/details/gliazujnc.sHtML

[N04] 斐波那契数列
来源：http://read.share.hesvh.cn/Article/details/gzpwtjzys.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.fehbvm.com/Article/details/gbribhxzh.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.hesvh.cn/Article/details/gpoahhsfi.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.zdbjq.cn/Article/details/gelqjvycx.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.zdbjq.cn/Article/details/gnqdzkibw.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.hesvh.cn/Article/details/gjopgaupu.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.fehbvm.com/Article/details/gtizktlyu.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.zdbjq.cn/Article/details/ghpmmawoi.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.zdbjq.cn/Article/details/gteyifsek.sHtML

[N05] 最大公约数
来源：http://baike.hesvh.cn/Article/details/ghgyzxlka.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.zdbjq.cn/Article/details/giokvfjqk.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.hesvh.cn/Article/details/ghdvxizpf.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.zdbjq.cn/Article/details/gkqbyhwlv.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.zdbjq.cn/Article/details/gdbhuamnh.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.fehbvm.com/Article/details/gdsckmkfh.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.zdbjq.cn/Article/details/gliadejen.sHtML

Ruby: a.gcd(b)
来源：http://wap.fehbvm.com/Article/details/gsbevdosl.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.fehbvm.com/Article/details/gwqskftet.sHtML

[N06] 判断回文字符串
来源：http://mobile.fehbvm.com/Article/details/gbwxenqvu.sHtML

Py:   s == s[::-1]
来源：http://3g.fehbvm.com/Article/details/gnpebrael.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.fehbvm.com/Article/details/gxzgvvzol.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/goegpxdkw.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gpokxbtof.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.zdbjq.cn/Article/details/gwzfjmjwf.sHtML

Go:   // 双指针从两端比较
来源：http://3g.hesvh.cn/Article/details/grgvindii.sHtML

Ruby: s == s.reverse
来源：http://read.share.hesvh.cn/Article/details/gbiulzqom.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.fehbvm.com/Article/details/gzzosdvcm.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.zdbjq.cn/Article/details/grxqsyiwf.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.zdbjq.cn/Article/details/gdbfojdwm.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.zdbjq.cn/Article/details/glpgdztfb.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.zdbjq.cn/Article/details/guhzdzkit.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.fehbvm.com/Article/details/gqsoszref.sHtML

Java: // 手写 HashMap
来源：http://baike.hesvh.cn/Article/details/gumxfpmha.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.zdbjq.cn/Article/details/gjnojtghm.sHtML

Ruby: // 手写 Hash
来源：http://read.share.zdbjq.cn/Article/details/gkcrkxrab.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.zdbjq.cn/Article/details/gvbfkhmet.sHtML

[N08] 生成全排列
来源：http://www.m.share.hesvh.cn/Article/details/gzssvzyog.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.hesvh.cn/Article/details/gfhpaobfm.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.zdbjq.cn/Article/details/gfeqebvfl.sHtML

JS:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gafmkeglq.sHtML

TS:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gtvwnywor.sHtML

Java: // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/ghturmnng.sHtML

Go:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gfdwaitln.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.fehbvm.com/Article/details/gzmxdrcue.sHtML

C#:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gngdopipb.sHtML

[N09] 栈与队列
来源：http://wap.hesvh.cn/Article/details/gyfdxpxly.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.fehbvm.com/Article/details/gncrgckvd.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.fehbvm.com/Article/details/gaqjadxgg.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.fehbvm.com/Article/details/gfbqffooq.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.fehbvm.com/Article/details/gfhkhdvrj.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.fehbvm.com/Article/details/gosqtvvce.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.fehbvm.com/Article/details/geozdeatg.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.zdbjq.cn/Article/details/gvlawmjld.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.hesvh.cn/Article/details/gksezwwfe.sHtML

[N10] 链表节点定义
来源：http://blog.zdbjq.cn/Article/details/gveyqesxl.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.hesvh.cn/Article/details/gaczomeut.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.zdbjq.cn/Article/details/gtcccuklo.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.fehbvm.com/Article/details/gnnitrjez.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.zdbjq.cn/Article/details/gghqggezt.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.fehbvm.com/Article/details/gegkyffvq.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.zdbjq.cn/Article/details/gggdhtjaf.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.hesvh.cn/Article/details/gvkzbsrrl.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.zdbjq.cn/Article/details/gnsmthcle.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.zdbjq.cn/Article/details/giucswyyj.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.zdbjq.cn/Article/details/gccpoamlw.sHtML

PHP:  // 手写递归函数
来源：http://mobile.hesvh.cn/Article/details/gkfqicqwx.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.fehbvm.com/Article/details/ghytwrgso.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.hesvh.cn/Article/details/gouszxqxd.sHtML

Java: // 手写递归
来源：http://www.m.share.zdbjq.cn/Article/details/glijmfxuy.sHtML

Go:   // 手写递归
来源：http://wap.zdbjq.cn/Article/details/gmixfwfgn.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.hesvh.cn/Article/details/gapldmaua.sHtML

C#:   // 手写递归
来源：http://mobile.fehbvm.com/Article/details/gsqfqykci.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.fehbvm.com/Article/details/gtmumnvns.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.zdbjq.cn/Article/details/gzdwwzimt.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.hesvh.cn/Article/details/gzmelkatq.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.hesvh.cn/Article/details/gegftfmkr.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.zdbjq.cn/Article/details/gzpbnbtwe.sHtML


<!-- 参考信息 -->