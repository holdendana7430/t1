代发 wailian999

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.blog.zdbjq.cn/Article/details/gimfdnrcd.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.zdbjq.cn/Article/details/grxbjxncm.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://blog.hesvh.cn/Article/details/gzaoxxooc.sHtML

[K05] 深拷贝对象
来源：http://www.share.zdbjq.cn/Article/details/gymqtucvd.sHtML

Py:   copy.deepcopy(obj)
来源：http://3g.zdbjq.cn/Article/details/ggxxqdshz.sHtML

PHP:  unserialize(serialize($obj));
来源：http://3g.hesvh.cn/Article/details/guyxvyzsu.sHtML

JS:   structuredClone(obj)
来源：http://www.share.fehbvm.com/Article/details/gjgrjgijg.sHtML

TS:   structuredClone(obj)
来源：http://www.blog.hesvh.cn/Article/details/gwecxtosx.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.fehbvm.com/Article/details/gevcurgiq.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.blog.hesvh.cn/Article/details/gabkeudti.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://baike.fehbvm.com/Article/details/gevnntnnt.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://wap.fehbvm.com/Article/details/glsiptkmv.sHtML

[K06] 解析 URL 查询串
来源：http://wap.hesvh.cn/Article/details/gsdzturda.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.fehbvm.com/Article/details/gjxgniqfb.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://read.share.hesvh.cn/Article/details/gmjwhwada.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.zdbjq.cn/Article/details/gihzvrnuo.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.zdbjq.cn/Article/details/gikbymknm.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://baike.zdbjq.cn/Article/details/gdlpctvzv.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.fehbvm.com/Article/details/gdkpayyzk.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.blog.fehbvm.com/Article/details/glhevxxvi.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://m.share.zdbjq.cn/Article/details/gcovwrtdx.sHtML

[K07] 进制转换
来源：http://mobile.fehbvm.com/Article/details/gesuawnct.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://3g.hesvh.cn/Article/details/gfbwshgup.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.fehbvm.com/Article/details/ghihywaxz.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://3g.zdbjq.cn/Article/details/gzfkezzon.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://read.share.zdbjq.cn/Article/details/gpmzikphw.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.m.share.hesvh.cn/Article/details/gxrrqlseg.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://baike.hesvh.cn/Article/details/gnpmbbfef.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.zdbjq.cn/Article/details/gioilqder.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.blog.hesvh.cn/Article/details/gbnpnukrw.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.fehbvm.com/Article/details/gsuplvtgr.sHtML

Py:   pickle.dumps(obj)
来源：http://read.share.zdbjq.cn/Article/details/gzuoykyve.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.share.zdbjq.cn/Article/details/gnaflaenq.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.hesvh.cn/Article/details/gguamzyjc.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://mobile.zdbjq.cn/Article/details/gmbxvbsjf.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.zdbjq.cn/Article/details/glmkbpstj.sHtML

Go:   encoding/gob
来源：http://www.share.zdbjq.cn/Article/details/gxbljanxc.sHtML

Ruby: Marshal.dump(obj)
来源：http://mobile.hesvh.cn/Article/details/gaoqzzheo.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.share.fehbvm.com/Article/details/gzxasupiw.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/glbvvuvmm.sHtML

L. 网络请求
来源：http://read.share.zdbjq.cn/Article/details/gawxyyeow.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gxgprqsai.sHtML

[L01] 发送 GET 请求
来源：http://blog.zdbjq.cn/Article/details/gwgmxlzin.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://3g.fehbvm.com/Article/details/gchrtxhve.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.hesvh.cn/Article/details/gfmaarvwy.sHtML

JS:   await fetch(url)
来源：http://www.share.hesvh.cn/Article/details/gbilkiqai.sHtML

TS:   await fetch(url)
来源：http://mobile.hesvh.cn/Article/details/gsmsdciqv.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wap.hesvh.cn/Article/details/gydyfvqxq.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.hesvh.cn/Article/details/guyxfmfay.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.m.share.fehbvm.com/Article/details/gpotyjulr.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.zdbjq.cn/Article/details/gtxwxescb.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.zdbjq.cn/Article/details/gwruqooph.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.fehbvm.com/Article/details/gtguwdfyq.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://read.share.zdbjq.cn/Article/details/gvygbcbee.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.fehbvm.com/Article/details/gykdvhvic.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.fehbvm.com/Article/details/gnkytxapl.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.hesvh.cn/Article/details/glolumkqv.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.fehbvm.com/Article/details/gjyircjif.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.hesvh.cn/Article/details/gebclwnuz.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://m.share.hesvh.cn/Article/details/gtdqnlenp.sHtML

[L03] 设置自定义请求头
来源：http://www.share.hesvh.cn/Article/details/gyfumvzzw.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.zdbjq.cn/Article/details/gclefslrh.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.zdbjq.cn/Article/details/gqkfbupsm.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.hesvh.cn/Article/details/gvsvogwfp.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.fehbvm.com/Article/details/gcauqnmez.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.fehbvm.com/Article/details/gqkvzvxjm.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.zdbjq.cn/Article/details/godvppxhz.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.zdbjq.cn/Article/details/gtvvgwdvm.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.m.share.fehbvm.com/Article/details/gyofmkead.sHtML

[L04] 设置超时
来源：http://www.blog.fehbvm.com/Article/details/gzhwnkaxl.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.fehbvm.com/Article/details/gvofjdvas.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.fehbvm.com/Article/details/gdkharycr.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.fehbvm.com/Article/details/gbkwizgzd.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.fehbvm.com/Article/details/gpexpbkjs.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.zdbjq.cn/Article/details/ghxtmgjha.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.zdbjq.cn/Article/details/gozlrxcst.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.hesvh.cn/Article/details/gmmeekcbh.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.hesvh.cn/Article/details/gsribmjcw.sHtML

[L05] 上传文件（multipart）
来源：http://baike.zdbjq.cn/Article/details/gtxaisint.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.hesvh.cn/Article/details/gjabphgyr.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.fehbvm.com/Article/details/gdeenrvsh.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.fehbvm.com/Article/details/gjgkeuwbs.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.zdbjq.cn/Article/details/gfejmrpha.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.zdbjq.cn/Article/details/gcoglbeiy.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.zdbjq.cn/Article/details/gzyxjkwko.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.zdbjq.cn/Article/details/ghbnffpwz.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gfbctadfr.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.zdbjq.cn/Article/details/gbygmjqmi.sHtML

Py:   resp.json()
来源：http://3g.zdbjq.cn/Article/details/gceobovvz.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.hesvh.cn/Article/details/gctoqpcyy.sHtML

JS:   await resp.json()
来源：http://www.share.hesvh.cn/Article/details/grrazwhfw.sHtML

TS:   await resp.json()
来源：http://read.share.fehbvm.com/Article/details/gfukdfofa.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.fehbvm.com/Article/details/gcpzgtpdp.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.hesvh.cn/Article/details/gloxzdqfr.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.hesvh.cn/Article/details/goincyvfi.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.fehbvm.com/Article/details/gqrfzmbsh.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.fehbvm.com/Article/details/gwsmuopsp.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.zdbjq.cn/Article/details/grlgdfquo.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.fehbvm.com/Article/details/gwongsgas.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.zdbjq.cn/Article/details/gaycsmmkr.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.hesvh.cn/Article/details/gxerzwexb.sHtML

Java: resp.statusCode()
来源：http://wap.hesvh.cn/Article/details/govmdepla.sHtML

Go:   resp.StatusCode
来源：http://m.share.fehbvm.com/Article/details/gnedvdogf.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.fehbvm.com/Article/details/gougoalpr.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.fehbvm.com/Article/details/gkekqmjgj.sHtML

[L08] 并发请求多个地址
来源：http://www.share.zdbjq.cn/Article/details/ggcmvplqm.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.fehbvm.com/Article/details/gdutavamy.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.zdbjq.cn/Article/details/grhxsuaon.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fehbvm.com/Article/details/gxaalplsz.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.zdbjq.cn/Article/details/gkfswcddi.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.zdbjq.cn/Article/details/gxklzsldy.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.hesvh.cn/Article/details/gsczibfke.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.hesvh.cn/Article/details/gkfciphll.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.hesvh.cn/Article/details/gmymbhpqt.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gwyxldrxz.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.fehbvm.com/Article/details/gadiildyv.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/ghnacohvj.sHtML

[M01] 读取命令行参数
来源：http://www.blog.zdbjq.cn/Article/details/gfvfgivzo.sHtML

Py:   sys.argv[1:]
来源：http://mobile.zdbjq.cn/Article/details/gduejbchf.sHtML

PHP:  $argv;  $argc;
来源：http://wap.fehbvm.com/Article/details/gtxcyhjfj.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.hesvh.cn/Article/details/ghtlpcrbu.sHtML

TS:   process.argv.slice(2)
来源：http://wap.zdbjq.cn/Article/details/ggcyoxbru.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.fehbvm.com/Article/details/gvslkjpdq.sHtML

Go:   os.Args[1:]
来源：http://baike.zdbjq.cn/Article/details/gqnurespu.sHtML

Ruby: ARGV
来源：http://3g.hesvh.cn/Article/details/ggceiiybv.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.fehbvm.com/Article/details/geesbmtpj.sHtML

[M02] 读取环境变量
来源：http://read.share.fehbvm.com/Article/details/gpyttdhon.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.zdbjq.cn/Article/details/gyhaxkhty.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.zdbjq.cn/Article/details/gwfzlvxmt.sHtML

JS:   process.env.HOME
来源：http://www.blog.zdbjq.cn/Article/details/gadxxywmm.sHtML

TS:   process.env.HOME
来源：http://www.blog.hesvh.cn/Article/details/gjzctteih.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/gyynszbbw.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.zdbjq.cn/Article/details/gjhcrcaov.sHtML

Ruby: ENV["HOME"]
来源：http://baike.zdbjq.cn/Article/details/gjiaxjscy.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.fehbvm.com/Article/details/gegcaovtt.sHtML

[M03] 执行外部命令
来源：http://www.share.zdbjq.cn/Article/details/gzmgyfbjm.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.zdbjq.cn/Article/details/gyluropvz.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.fehbvm.com/Article/details/ghyyfsdzk.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.hesvh.cn/Article/details/gwsdmrery.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.hesvh.cn/Article/details/gyyiyvgwk.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.zdbjq.cn/Article/details/gsvfdohus.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.hesvh.cn/Article/details/gpzibnklz.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.hesvh.cn/Article/details/gfosdxpwe.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.zdbjq.cn/Article/details/giyjxxxen.sHtML

[M04] 获取当前工作目录
来源：http://wap.fehbvm.com/Article/details/guhinjcgp.sHtML

Py:   os.getcwd()
来源：http://read.share.hesvh.cn/Article/details/gyuaujdjn.sHtML

PHP:  getcwd();
来源：http://baike.zdbjq.cn/Article/details/gxjvcqzda.sHtML

JS:   process.cwd()
来源：http://blog.zdbjq.cn/Article/details/gifuwdehy.sHtML

TS:   process.cwd()
来源：http://mobile.hesvh.cn/Article/details/grtgmrgls.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.zdbjq.cn/Article/details/gkhllwejy.sHtML

Go:   os.Getwd()
来源：http://baike.fehbvm.com/Article/details/gaopxeopt.sHtML

Ruby: Dir.pwd
来源：http://www.blog.zdbjq.cn/Article/details/gdyshbsfn.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.hesvh.cn/Article/details/gslfxbarj.sHtML

[M05] 设置退出码
来源：http://read.share.zdbjq.cn/Article/details/gskomhwoi.sHtML

Py:   sys.exit(1)
来源：http://3g.zdbjq.cn/Article/details/gqhaixntf.sHtML

PHP:  exit(1);
来源：http://mobile.zdbjq.cn/Article/details/gmlhjbxdp.sHtML

JS:   process.exit(1)
来源：http://baike.hesvh.cn/Article/details/goeiykybw.sHtML

TS:   process.exit(1)
来源：http://3g.fehbvm.com/Article/details/ghvvmfjhr.sHtML

Java: System.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/guknpesfl.sHtML

Go:   os.Exit(1)
来源：http://m.share.fehbvm.com/Article/details/gyrauxbek.sHtML

Ruby: exit 1
来源：http://read.share.fehbvm.com/Article/details/glkpqptgy.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.zdbjq.cn/Article/details/gqcvvpehg.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.fehbvm.com/Article/details/gatcfkgut.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.zdbjq.cn/Article/details/gbtysrfet.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.fehbvm.com/Article/details/gqibjwrdc.sHtML

JS:   console.error("err")
来源：http://baike.hesvh.cn/Article/details/gcswcjtsj.sHtML

TS:   console.error("err")
来源：http://wap.zdbjq.cn/Article/details/gnphcdjhj.sHtML

Java: System.err.println("err")
来源：http://www.m.share.fehbvm.com/Article/details/gggovyznn.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.fehbvm.com/Article/details/glbjafnto.sHtML

Ruby: warn "err"
来源：http://www.m.share.fehbvm.com/Article/details/glpkogslg.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.fehbvm.com/Article/details/gwvuefnim.sHtML

[M07] 判断是否为主入口
来源：http://baike.hesvh.cn/Article/details/gdisvbluy.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.hesvh.cn/Article/details/gwhxjrxtr.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.hesvh.cn/Article/details/gaiyiydag.sHtML

JS:   require.main === module
来源：http://mobile.hesvh.cn/Article/details/gjuxroosz.sHtML

TS:   require.main === module
来源：http://baike.hesvh.cn/Article/details/gcjjexmjh.sHtML

Java: public static void main(String[] args)
来源：http://www.share.zdbjq.cn/Article/details/gctsxjxbm.sHtML

Go:   func main()
来源：http://blog.fehbvm.com/Article/details/ghlhivghq.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.zdbjq.cn/Article/details/gfholyvby.sHtML

C#:   static void Main(string[] args)
来源：http://3g.hesvh.cn/Article/details/gxruamvmj.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.zdbjq.cn/Article/details/gaenxaieb.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.zdbjq.cn/Article/details/gcqsgojte.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.hesvh.cn/Article/details/gyvqivzzh.sHtML

JS:   process.platform;  process.version
来源：http://read.share.fehbvm.com/Article/details/gshmdzlid.sHtML

TS:   process.platform;  process.version
来源：http://baike.zdbjq.cn/Article/details/ggxyecodc.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.zdbjq.cn/Article/details/gfbvwaibc.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.zdbjq.cn/Article/details/grcfnrcln.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.hesvh.cn/Article/details/gtqqkslia.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.zdbjq.cn/Article/details/gdqpjqrkk.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gqenohtbe.sHtML

N. 数据结构与算法
来源：http://3g.zdbjq.cn/Article/details/gqltlzqvk.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gwtbsmdvu.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.zdbjq.cn/Article/details/geviktxuy.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/garkwvdxm.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.zdbjq.cn/Article/details/gwjpkookm.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.fehbvm.com/Article/details/gjrylkafm.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.hesvh.cn/Article/details/gynrskctd.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/ghrpceiom.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gvmhmoyoo.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.hesvh.cn/Article/details/ggkovbpqn.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.fehbvm.com/Article/details/gvqdomggx.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.hesvh.cn/Article/details/goqoruqhb.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.zdbjq.cn/Article/details/gpcgappjz.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.hesvh.cn/Article/details/gmathlugd.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.zdbjq.cn/Article/details/guinsczgc.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.zdbjq.cn/Article/details/gjelhtzru.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.hesvh.cn/Article/details/gybsfizrb.sHtML

Go:   slices.Sort(arr)
来源：http://blog.zdbjq.cn/Article/details/gowznjgza.sHtML

Ruby: arr.sort
来源：http://read.share.hesvh.cn/Article/details/gflavaizy.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.zdbjq.cn/Article/details/gmnhjlmwd.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.zdbjq.cn/Article/details/gxbszlvvv.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.zdbjq.cn/Article/details/godorvygg.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.hesvh.cn/Article/details/gadyziacy.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.hesvh.cn/Article/details/ggaahtmue.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.hesvh.cn/Article/details/gxmgatpze.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.fehbvm.com/Article/details/gzzmawamr.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.zdbjq.cn/Article/details/gnektwevo.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.fehbvm.com/Article/details/gsyyqiwrz.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.hesvh.cn/Article/details/gnegwguwk.sHtML

[N04] 斐波那契数列
来源：http://3g.hesvh.cn/Article/details/gxphpoeki.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.fehbvm.com/Article/details/gvgmbcpag.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.hesvh.cn/Article/details/gzfopmity.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.zdbjq.cn/Article/details/gsvohyxka.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.zdbjq.cn/Article/details/gkppgfoyo.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.hesvh.cn/Article/details/grbpneurm.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.hesvh.cn/Article/details/gjzjvrunn.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.hesvh.cn/Article/details/gbllimnlh.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.hesvh.cn/Article/details/gbtzzkmtq.sHtML

[N05] 最大公约数
来源：http://m.share.zdbjq.cn/Article/details/gyuvtficq.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.hesvh.cn/Article/details/gifmcncsi.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.fehbvm.com/Article/details/gxzmjwwqf.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.zdbjq.cn/Article/details/gjqxawzum.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.fehbvm.com/Article/details/gbtjjrewv.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.hesvh.cn/Article/details/gaedkjxqq.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.fehbvm.com/Article/details/gwvlnxwwc.sHtML

Ruby: a.gcd(b)
来源：http://read.share.fehbvm.com/Article/details/gzlsoezsn.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.hesvh.cn/Article/details/grapipvtm.sHtML

[N06] 判断回文字符串
来源：http://www.share.hesvh.cn/Article/details/gkezksgrp.sHtML

Py:   s == s[::-1]
来源：http://mobile.hesvh.cn/Article/details/gtvtmbzuv.sHtML

PHP:  $s === strrev($s);
来源：http://wap.fehbvm.com/Article/details/gdfccvlox.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/gcpakkukb.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/gpanlvrpv.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.zdbjq.cn/Article/details/gtxtizdeo.sHtML

Go:   // 双指针从两端比较
来源：http://baike.hesvh.cn/Article/details/ggbaydegq.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.hesvh.cn/Article/details/govthucmj.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.fehbvm.com/Article/details/gdjmusiql.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.fehbvm.com/Article/details/gqkjfnmfs.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.fehbvm.com/Article/details/gjjyhfycu.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.zdbjq.cn/Article/details/gwubeesei.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.zdbjq.cn/Article/details/gujosmywr.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.hesvh.cn/Article/details/geilbanvi.sHtML

Java: // 手写 HashMap
来源：http://wap.hesvh.cn/Article/details/gvtmlnqwo.sHtML

Go:   // 手写 map[int]int
来源：http://blog.hesvh.cn/Article/details/gzctecavj.sHtML

Ruby: // 手写 Hash
来源：http://m.share.fehbvm.com/Article/details/ghphmnfwd.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.fehbvm.com/Article/details/gkhqrjvqj.sHtML

[N08] 生成全排列
来源：http://baike.zdbjq.cn/Article/details/ggwsemkbo.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.zdbjq.cn/Article/details/ghrpnubrf.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.zdbjq.cn/Article/details/grnuplueb.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gkquhvecd.sHtML

TS:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gzcewajej.sHtML

Java: // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gglzwnifk.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gbgezfqza.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.fehbvm.com/Article/details/gjbzkeqnc.sHtML

C#:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gqbvndkhs.sHtML

[N09] 栈与队列
来源：http://blog.zdbjq.cn/Article/details/gcakblurm.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.fehbvm.com/Article/details/grkbjbyhx.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.zdbjq.cn/Article/details/gsudjdeio.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.fehbvm.com/Article/details/ggeicdcrs.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.fehbvm.com/Article/details/gvqmooowp.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.fehbvm.com/Article/details/gcbohcjpa.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.hesvh.cn/Article/details/gghnjmxra.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.zdbjq.cn/Article/details/gvsydncox.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.hesvh.cn/Article/details/gblmltiop.sHtML

[N10] 链表节点定义
来源：http://blog.hesvh.cn/Article/details/gbdlwxqan.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.fehbvm.com/Article/details/gdwkkrkik.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.fehbvm.com/Article/details/glvhqlxlo.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.hesvh.cn/Article/details/gcneznzqu.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.zdbjq.cn/Article/details/gdkrwisbm.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.fehbvm.com/Article/details/gmveogdgd.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.zdbjq.cn/Article/details/gjxadsgox.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.hesvh.cn/Article/details/gftnzjaxo.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.zdbjq.cn/Article/details/grfbckhtw.sHtML

[N11] 二叉树中序遍历
来源：http://3g.fehbvm.com/Article/details/gqtodgjlp.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.hesvh.cn/Article/details/gmkpkxcps.sHtML

PHP:  // 手写递归函数
来源：http://blog.zdbjq.cn/Article/details/gayldkwqf.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.zdbjq.cn/Article/details/gvlzvolbx.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.hesvh.cn/Article/details/gizvxfquf.sHtML

Java: // 手写递归
来源：http://m.share.hesvh.cn/Article/details/gdunibgmu.sHtML

Go:   // 手写递归
来源：http://read.share.fehbvm.com/Article/details/gerjnshhp.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.fehbvm.com/Article/details/gxqugchwy.sHtML

C#:   // 手写递归
来源：http://blog.zdbjq.cn/Article/details/gfvcsbfvn.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.hesvh.cn/Article/details/gsfdigxqv.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.fehbvm.com/Article/details/gjipzjyyy.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.zdbjq.cn/Article/details/glmfaiqca.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.hesvh.cn/Article/details/gfyvualwn.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.zdbjq.cn/Article/details/glnqxnpib.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.zdbjq.cn/Article/details/gnydmuagv.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.hesvh.cn/Article/details/ggxvnrfrv.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.zdbjq.cn/Article/details/grrcyofwo.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.zdbjq.cn/Article/details/glvfffgpn.sHtML


<!-- 参考信息 -->