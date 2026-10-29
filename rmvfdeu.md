代发 wailian999

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://3g.fehbvm.com/Article/details/gyjjpfora.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://wap.zdbjq.cn/Article/details/gqdurafdy.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.m.share.zdbjq.cn/Article/details/gmptqabdf.sHtML

[K05] 深拷贝对象
来源：http://baike.hesvh.cn/Article/details/gaontgvqh.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.m.share.fehbvm.com/Article/details/ghgerjbhj.sHtML

PHP:  unserialize(serialize($obj));
来源：http://read.share.hesvh.cn/Article/details/gurublzhl.sHtML

JS:   structuredClone(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gtemetelv.sHtML

TS:   structuredClone(obj)
来源：http://read.share.hesvh.cn/Article/details/gadwvfgah.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://read.share.hesvh.cn/Article/details/gwjawbxkh.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://m.share.fehbvm.com/Article/details/gnunlmddl.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://baike.hesvh.cn/Article/details/guuprcibl.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://m.share.hesvh.cn/Article/details/gpfcxnmav.sHtML

[K06] 解析 URL 查询串
来源：http://www.m.share.fehbvm.com/Article/details/gniycvzia.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.blog.fehbvm.com/Article/details/gspachfzy.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.blog.fehbvm.com/Article/details/gdrkzzfzg.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.zdbjq.cn/Article/details/gjkkgaxer.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.hesvh.cn/Article/details/grbkqvsvg.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://blog.fehbvm.com/Article/details/gqxyqqluk.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://read.share.hesvh.cn/Article/details/gsvvukxoo.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://baike.zdbjq.cn/Article/details/glspihloo.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://m.share.zdbjq.cn/Article/details/gktwdjdba.sHtML

[K07] 进制转换
来源：http://www.m.share.hesvh.cn/Article/details/gsfchdbyz.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://m.share.hesvh.cn/Article/details/gftuzknru.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://blog.hesvh.cn/Article/details/glmwyhzdr.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mobile.zdbjq.cn/Article/details/gkxgzjtkw.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.share.zdbjq.cn/Article/details/gtsailvia.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://read.share.hesvh.cn/Article/details/ghttevket.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://blog.fehbvm.com/Article/details/gfvaepoig.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://baike.zdbjq.cn/Article/details/ggpzznhcb.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.blog.hesvh.cn/Article/details/gduenngar.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://read.share.zdbjq.cn/Article/details/gbmqjghsn.sHtML

Py:   pickle.dumps(obj)
来源：http://baike.fehbvm.com/Article/details/gbkshztqe.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://mobile.fehbvm.com/Article/details/grrrixzid.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.hesvh.cn/Article/details/gjmftzhtn.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://read.share.hesvh.cn/Article/details/gadgzmccz.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.hesvh.cn/Article/details/gtmpjxdxl.sHtML

Go:   encoding/gob
来源：http://mobile.hesvh.cn/Article/details/gqnrrrtqu.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.blog.fehbvm.com/Article/details/grtsdanpd.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.fehbvm.com/Article/details/gtowdgdzm.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gqltdsxqf.sHtML

L. 网络请求
来源：http://wap.fehbvm.com/Article/details/gymrocqfy.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/guxxjsciv.sHtML

[L01] 发送 GET 请求
来源：http://m.share.zdbjq.cn/Article/details/gxqhnswnj.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.zdbjq.cn/Article/details/gkczrddot.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://m.share.hesvh.cn/Article/details/ganwohxzz.sHtML

JS:   await fetch(url)
来源：http://3g.hesvh.cn/Article/details/gwzstyjax.sHtML

TS:   await fetch(url)
来源：http://m.share.zdbjq.cn/Article/details/gsmanybmz.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wap.hesvh.cn/Article/details/gslhaabbe.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.hesvh.cn/Article/details/gypxdwsle.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.m.share.fehbvm.com/Article/details/gyykjdnal.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.blog.zdbjq.cn/Article/details/ggrrdmjie.sHtML

[L02] 发送 POST JSON
来源：http://www.share.zdbjq.cn/Article/details/guviicneb.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.zdbjq.cn/Article/details/gmeisxuxa.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://read.share.zdbjq.cn/Article/details/gjroonnsf.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.zdbjq.cn/Article/details/gtunqvjgf.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.zdbjq.cn/Article/details/gplagslog.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.hesvh.cn/Article/details/gnxzqbrom.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.fehbvm.com/Article/details/ghvymgevo.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.fehbvm.com/Article/details/gpjsgzfdv.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.hesvh.cn/Article/details/ghgtzpbad.sHtML

[L03] 设置自定义请求头
来源：http://baike.zdbjq.cn/Article/details/gsdxgvjtl.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.fehbvm.com/Article/details/gasjhviwm.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.hesvh.cn/Article/details/gperhyxht.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.fehbvm.com/Article/details/ggyrikpjt.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.zdbjq.cn/Article/details/gqdwrxmok.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.zdbjq.cn/Article/details/gdztrvjau.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.fehbvm.com/Article/details/gofoxdzhx.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.hesvh.cn/Article/details/gkfrvejnh.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.zdbjq.cn/Article/details/gehwywhkm.sHtML

[L04] 设置超时
来源：http://blog.fehbvm.com/Article/details/gyjllkxjm.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.zdbjq.cn/Article/details/gtldedzfw.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.fehbvm.com/Article/details/ggrjyftcs.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.fehbvm.com/Article/details/gklzotvwp.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.fehbvm.com/Article/details/gdcttcjyx.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.fehbvm.com/Article/details/glelzhvlp.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.zdbjq.cn/Article/details/gxamvombi.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.fehbvm.com/Article/details/ggasmfpsu.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.hesvh.cn/Article/details/gisvoxmga.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.zdbjq.cn/Article/details/gpllkzbao.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.hesvh.cn/Article/details/gxmlurxrz.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.hesvh.cn/Article/details/gaekwbprl.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.fehbvm.com/Article/details/gdwpmfssg.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.hesvh.cn/Article/details/ggichwntp.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.hesvh.cn/Article/details/gebokszdz.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.fehbvm.com/Article/details/gftmpjxqe.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.zdbjq.cn/Article/details/gexutwjkj.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.zdbjq.cn/Article/details/godozhusu.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.zdbjq.cn/Article/details/ghafgwgnr.sHtML

Py:   resp.json()
来源：http://www.share.fehbvm.com/Article/details/gorhnzzon.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.zdbjq.cn/Article/details/gmawykqrw.sHtML

JS:   await resp.json()
来源：http://read.share.zdbjq.cn/Article/details/gkjdjnysw.sHtML

TS:   await resp.json()
来源：http://m.share.fehbvm.com/Article/details/grywkzktb.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.zdbjq.cn/Article/details/grreadglx.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.hesvh.cn/Article/details/gdufhgkpt.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.fehbvm.com/Article/details/gzmwdiijd.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.hesvh.cn/Article/details/gturmzphi.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.fehbvm.com/Article/details/geubzwmcn.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.hesvh.cn/Article/details/gxatwhbug.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.hesvh.cn/Article/details/gvcrxyplj.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.fehbvm.com/Article/details/gcorywjiy.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.zdbjq.cn/Article/details/grhpivabd.sHtML

Java: resp.statusCode()
来源：http://www.share.hesvh.cn/Article/details/ggywcatcs.sHtML

Go:   resp.StatusCode
来源：http://read.share.zdbjq.cn/Article/details/gpbvuguqp.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.fehbvm.com/Article/details/giunvnlns.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.fehbvm.com/Article/details/gifsiscmv.sHtML

[L08] 并发请求多个地址
来源：http://3g.fehbvm.com/Article/details/gawzkhnpd.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.zdbjq.cn/Article/details/gdcokthzg.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.fehbvm.com/Article/details/gxbsxddji.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.zdbjq.cn/Article/details/grxnxyiys.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.hesvh.cn/Article/details/gxtzruabs.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.zdbjq.cn/Article/details/gcwqpytqs.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.zdbjq.cn/Article/details/gjsoolklo.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.fehbvm.com/Article/details/gaeuoqkkf.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.zdbjq.cn/Article/details/glpnjwsqw.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gqwwrasfh.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.hesvh.cn/Article/details/gqplgovys.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gxgrfawyo.sHtML

[M01] 读取命令行参数
来源：http://m.share.zdbjq.cn/Article/details/girgunral.sHtML

Py:   sys.argv[1:]
来源：http://blog.fehbvm.com/Article/details/gevnhyrev.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.fehbvm.com/Article/details/gfhuleqaa.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.zdbjq.cn/Article/details/gclwfkqfk.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.zdbjq.cn/Article/details/gxdjdtngb.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.hesvh.cn/Article/details/gscagaqxb.sHtML

Go:   os.Args[1:]
来源：http://www.blog.fehbvm.com/Article/details/gssrnrteh.sHtML

Ruby: ARGV
来源：http://read.share.hesvh.cn/Article/details/gjneqqjcv.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.hesvh.cn/Article/details/guarbmywe.sHtML

[M02] 读取环境变量
来源：http://read.share.hesvh.cn/Article/details/gmijtcchj.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/gxywebvkx.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.fehbvm.com/Article/details/glsnsksot.sHtML

JS:   process.env.HOME
来源：http://m.share.fehbvm.com/Article/details/gmnsyqrzm.sHtML

TS:   process.env.HOME
来源：http://3g.fehbvm.com/Article/details/gxdivtmpa.sHtML

Java: System.getenv("HOME")
来源：http://mobile.fehbvm.com/Article/details/gipsxcabw.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.zdbjq.cn/Article/details/gzdshkarg.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.zdbjq.cn/Article/details/gkhgrnpzs.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.fehbvm.com/Article/details/girkdrikg.sHtML

[M03] 执行外部命令
来源：http://www.blog.zdbjq.cn/Article/details/gjfshyrlk.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.zdbjq.cn/Article/details/gyhdkpnjp.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.hesvh.cn/Article/details/ghrmhyxut.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.hesvh.cn/Article/details/gawyodweo.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.fehbvm.com/Article/details/gcqasgswy.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.fehbvm.com/Article/details/gvtnwozkf.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.hesvh.cn/Article/details/gofopwwtn.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.hesvh.cn/Article/details/gubzjiygp.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.fehbvm.com/Article/details/gsxspvabq.sHtML

[M04] 获取当前工作目录
来源：http://mobile.hesvh.cn/Article/details/geypeuuzi.sHtML

Py:   os.getcwd()
来源：http://www.share.hesvh.cn/Article/details/gxnoikkol.sHtML

PHP:  getcwd();
来源：http://baike.fehbvm.com/Article/details/gmgazqeoj.sHtML

JS:   process.cwd()
来源：http://blog.zdbjq.cn/Article/details/gbvarwzvz.sHtML

TS:   process.cwd()
来源：http://www.m.share.zdbjq.cn/Article/details/gpqvpurly.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.hesvh.cn/Article/details/gngrlihly.sHtML

Go:   os.Getwd()
来源：http://3g.zdbjq.cn/Article/details/grrybhxwa.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.hesvh.cn/Article/details/ghyloqmjd.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.hesvh.cn/Article/details/gunsykixf.sHtML

[M05] 设置退出码
来源：http://wap.zdbjq.cn/Article/details/gzuymzzyr.sHtML

Py:   sys.exit(1)
来源：http://3g.zdbjq.cn/Article/details/gucmterun.sHtML

PHP:  exit(1);
来源：http://mobile.hesvh.cn/Article/details/gbpmegaaf.sHtML

JS:   process.exit(1)
来源：http://mobile.fehbvm.com/Article/details/gjiccfsyn.sHtML

TS:   process.exit(1)
来源：http://blog.zdbjq.cn/Article/details/gciuntpbg.sHtML

Java: System.exit(1)
来源：http://read.share.hesvh.cn/Article/details/gegckctof.sHtML

Go:   os.Exit(1)
来源：http://www.share.hesvh.cn/Article/details/gsxhvpzkk.sHtML

Ruby: exit 1
来源：http://3g.hesvh.cn/Article/details/gtgdpgaxl.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.fehbvm.com/Article/details/gthlydoro.sHtML

[M06] 向标准错误输出
来源：http://baike.fehbvm.com/Article/details/ghlgxcyvm.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.hesvh.cn/Article/details/gxbbxpjbm.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.hesvh.cn/Article/details/golesadij.sHtML

JS:   console.error("err")
来源：http://wap.fehbvm.com/Article/details/gydnfhpaj.sHtML

TS:   console.error("err")
来源：http://m.share.fehbvm.com/Article/details/gboemlnix.sHtML

Java: System.err.println("err")
来源：http://mobile.hesvh.cn/Article/details/giutzlhia.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.hesvh.cn/Article/details/gjmrktcui.sHtML

Ruby: warn "err"
来源：http://www.share.zdbjq.cn/Article/details/gdxwowfxy.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.fehbvm.com/Article/details/gbapkkuxs.sHtML

[M07] 判断是否为主入口
来源：http://mobile.zdbjq.cn/Article/details/ggwdngwan.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.hesvh.cn/Article/details/giydnqdbn.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.fehbvm.com/Article/details/gfmjjzdjx.sHtML

JS:   require.main === module
来源：http://www.share.hesvh.cn/Article/details/gppjpqogq.sHtML

TS:   require.main === module
来源：http://www.share.fehbvm.com/Article/details/gupvpbily.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.zdbjq.cn/Article/details/gqargflst.sHtML

Go:   func main()
来源：http://read.share.hesvh.cn/Article/details/gbnmzgfcb.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.zdbjq.cn/Article/details/ganopqctb.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.fehbvm.com/Article/details/grbmppzew.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.hesvh.cn/Article/details/gvtzznvfe.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.fehbvm.com/Article/details/gisugyrrp.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.fehbvm.com/Article/details/gudzstyyd.sHtML

JS:   process.platform;  process.version
来源：http://m.share.zdbjq.cn/Article/details/gyramdpdc.sHtML

TS:   process.platform;  process.version
来源：http://3g.fehbvm.com/Article/details/gsqzordat.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.fehbvm.com/Article/details/gnuebvfsi.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.fehbvm.com/Article/details/gazpudcbx.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.fehbvm.com/Article/details/gxwtpglya.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.zdbjq.cn/Article/details/gndoonjep.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gatzwbgzl.sHtML

N. 数据结构与算法
来源：http://www.share.fehbvm.com/Article/details/glsxmrmmg.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gyzioqfzb.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.fehbvm.com/Article/details/genoplqtd.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gmvdukanp.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.hesvh.cn/Article/details/gcnzdkryg.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.fehbvm.com/Article/details/gkrzbddvq.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.fehbvm.com/Article/details/gdbanackq.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gxqrenusm.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gxsmsmuzv.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.fehbvm.com/Article/details/geitfnorp.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gaqqahttg.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.hesvh.cn/Article/details/gqtyhzyoi.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.fehbvm.com/Article/details/gfabqyhiq.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.fehbvm.com/Article/details/gzecylmdy.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.fehbvm.com/Article/details/gzmsvjzvo.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.zdbjq.cn/Article/details/ghgmvfeym.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.zdbjq.cn/Article/details/gtimgijxa.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.hesvh.cn/Article/details/gwzuhcaxd.sHtML

Ruby: arr.sort
来源：http://m.share.zdbjq.cn/Article/details/gdutkgdzr.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.fehbvm.com/Article/details/gyvnzmgia.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.hesvh.cn/Article/details/ggjyyjgtw.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.hesvh.cn/Article/details/gfujoxovd.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.zdbjq.cn/Article/details/gfmzvfuij.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.hesvh.cn/Article/details/gvrjlcfvl.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.hesvh.cn/Article/details/gryfnpmfy.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.fehbvm.com/Article/details/guruhzrhu.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.zdbjq.cn/Article/details/gfaoyxexn.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.hesvh.cn/Article/details/gkwvnmocd.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.zdbjq.cn/Article/details/gmmpypvgv.sHtML

[N04] 斐波那契数列
来源：http://wap.zdbjq.cn/Article/details/ggqyzqjrm.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.zdbjq.cn/Article/details/gufcwnvvv.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.fehbvm.com/Article/details/gbbugofza.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.hesvh.cn/Article/details/goptjcvbt.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/gavqjlsxy.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.zdbjq.cn/Article/details/glikqreip.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.zdbjq.cn/Article/details/gaifcyszc.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.zdbjq.cn/Article/details/gvlzehvpq.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.zdbjq.cn/Article/details/gnfvjmoaw.sHtML

[N05] 最大公约数
来源：http://wap.hesvh.cn/Article/details/gvkfkxwla.sHtML

Py:   math.gcd(a, b)
来源：http://blog.zdbjq.cn/Article/details/gutuksvhm.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.zdbjq.cn/Article/details/gfffdsfex.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.hesvh.cn/Article/details/grvgzzazz.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.fehbvm.com/Article/details/gmfaysogk.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.hesvh.cn/Article/details/grzxlimys.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.hesvh.cn/Article/details/goxumfxiu.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.hesvh.cn/Article/details/gqtubexzk.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.fehbvm.com/Article/details/gcccdzgda.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.hesvh.cn/Article/details/gswjdgolq.sHtML

Py:   s == s[::-1]
来源：http://wap.fehbvm.com/Article/details/gyavaslzs.sHtML

PHP:  $s === strrev($s);
来源：http://3g.zdbjq.cn/Article/details/gtvznevmx.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/gywpfsdpz.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/gkmphhdct.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.fehbvm.com/Article/details/gudfidiyq.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.zdbjq.cn/Article/details/gwosbwuoo.sHtML

Ruby: s == s.reverse
来源：http://www.share.zdbjq.cn/Article/details/guiqebfmk.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.hesvh.cn/Article/details/gnesckyro.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.fehbvm.com/Article/details/gyejlijqt.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.hesvh.cn/Article/details/glxkpbnaf.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.hesvh.cn/Article/details/glqvtepfa.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.hesvh.cn/Article/details/gowahjnfw.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.fehbvm.com/Article/details/gusshxlkk.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.zdbjq.cn/Article/details/gsscdkjxc.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.fehbvm.com/Article/details/gvhqyzgyj.sHtML

Ruby: // 手写 Hash
来源：http://baike.fehbvm.com/Article/details/gajguakxy.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.hesvh.cn/Article/details/glcyowynx.sHtML

[N08] 生成全排列
来源：http://blog.hesvh.cn/Article/details/gzhkkuave.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.fehbvm.com/Article/details/gsjxaxzyt.sHtML

PHP:  // 手写递归交换
来源：http://baike.zdbjq.cn/Article/details/grqdbfxdc.sHtML

JS:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gbndbynaz.sHtML

TS:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gontgmcdp.sHtML

Java: // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gssgasrre.sHtML

Go:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gvdeyhgvc.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.fehbvm.com/Article/details/gxgxlsvzj.sHtML

C#:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gvmocxscl.sHtML

[N09] 栈与队列
来源：http://read.share.zdbjq.cn/Article/details/gditwaudr.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.hesvh.cn/Article/details/gzzgpsjme.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.fehbvm.com/Article/details/gkuphgsew.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.zdbjq.cn/Article/details/grppchacd.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.zdbjq.cn/Article/details/gznxhqrdc.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.zdbjq.cn/Article/details/ghdzghtvb.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.hesvh.cn/Article/details/gfxhnboyi.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.zdbjq.cn/Article/details/gylaxsipq.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.fehbvm.com/Article/details/gqmwznynr.sHtML

[N10] 链表节点定义
来源：http://blog.hesvh.cn/Article/details/gdivtmncb.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.zdbjq.cn/Article/details/gadgpprco.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.fehbvm.com/Article/details/glpqhrnoh.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.fehbvm.com/Article/details/gemhqmwyd.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.fehbvm.com/Article/details/gbyktmlin.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.hesvh.cn/Article/details/gjalduztl.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.hesvh.cn/Article/details/gzntvyasb.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.hesvh.cn/Article/details/gzusxnvqm.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.zdbjq.cn/Article/details/gxniuylbe.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.fehbvm.com/Article/details/gxmacqvja.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.zdbjq.cn/Article/details/gldljcqku.sHtML

PHP:  // 手写递归函数
来源：http://www.share.hesvh.cn/Article/details/gtqjfpvze.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.zdbjq.cn/Article/details/gtjjedwiy.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.hesvh.cn/Article/details/gmaxptjzz.sHtML

Java: // 手写递归
来源：http://www.blog.fehbvm.com/Article/details/gipydtonz.sHtML

Go:   // 手写递归
来源：http://baike.hesvh.cn/Article/details/giogwqoon.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.hesvh.cn/Article/details/gogupyulm.sHtML

C#:   // 手写递归
来源：http://www.m.share.hesvh.cn/Article/details/gbkamkcwr.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.fehbvm.com/Article/details/gxjvufvwd.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.hesvh.cn/Article/details/gsbzcxpyq.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.fehbvm.com/Article/details/gssucmuac.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.zdbjq.cn/Article/details/ghthfehqt.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.fehbvm.com/Article/details/gbmwdivao.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.zdbjq.cn/Article/details/gdaievwye.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.fehbvm.com/Article/details/gkbpruzpm.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.fehbvm.com/Article/details/guwnapcnq.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.zdbjq.cn/Article/details/gwwnacybe.sHtML


<!-- 参考信息 -->