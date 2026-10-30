代发 wailian999

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://baike.hesvh.cn/Article/details/gervsbivz.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.fehbvm.com/Article/details/gsvbanfnw.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.hesvh.cn/Article/details/glkwhgvbr.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://m.share.fehbvm.com/Article/details/gulrewhbz.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://3g.fehbvm.com/Article/details/gzdiifdle.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.m.share.fehbvm.com/Article/details/gmwahpssd.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://m.share.hesvh.cn/Article/details/ghnnpqexl.sHtML

[K05] 深拷贝对象
来源：http://www.m.share.zdbjq.cn/Article/details/gxldkimiw.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.share.hesvh.cn/Article/details/gmqkwqwem.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.fehbvm.com/Article/details/gvujepidx.sHtML

JS:   structuredClone(obj)
来源：http://www.blog.hesvh.cn/Article/details/gevteumpx.sHtML

TS:   structuredClone(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gzhwsqdgz.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://m.share.hesvh.cn/Article/details/gnrhtvkqt.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://3g.zdbjq.cn/Article/details/galfpjdyj.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://blog.zdbjq.cn/Article/details/gbehuuago.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://blog.hesvh.cn/Article/details/gumrvpzrn.sHtML

[K06] 解析 URL 查询串
来源：http://www.blog.hesvh.cn/Article/details/gviujaxxo.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://read.share.hesvh.cn/Article/details/gnnsvlnfr.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://blog.hesvh.cn/Article/details/gigogtwuf.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.hesvh.cn/Article/details/gswgzejxr.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.zdbjq.cn/Article/details/ggfiwrdgy.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.blog.fehbvm.com/Article/details/glvbnehkh.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.zdbjq.cn/Article/details/gmwhzzbcg.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://m.share.hesvh.cn/Article/details/grbxjseml.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mobile.fehbvm.com/Article/details/gaboszvpf.sHtML

[K07] 进制转换
来源：http://baike.fehbvm.com/Article/details/gmlxpjxex.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://3g.fehbvm.com/Article/details/gnscvidtw.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://m.share.hesvh.cn/Article/details/gihgxstrc.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.hesvh.cn/Article/details/gtzkizdfg.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://read.share.fehbvm.com/Article/details/goekactpl.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.zdbjq.cn/Article/details/gtasatdgo.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.fehbvm.com/Article/details/gvhplqtqz.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.share.zdbjq.cn/Article/details/gucrxfuak.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.zdbjq.cn/Article/details/gvkvbrucm.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://read.share.fehbvm.com/Article/details/grvwgnlnt.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.fehbvm.com/Article/details/gljtouahl.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://wap.zdbjq.cn/Article/details/gwcvpszkp.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://baike.fehbvm.com/Article/details/gmzhyyojf.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.zdbjq.cn/Article/details/gsbwwdahh.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.zdbjq.cn/Article/details/gxpktbqnj.sHtML

Go:   encoding/gob
来源：http://m.share.fehbvm.com/Article/details/gqvbgqznx.sHtML

Ruby: Marshal.dump(obj)
来源：http://read.share.hesvh.cn/Article/details/gymvfngud.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.hesvh.cn/Article/details/ghfisbcwu.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gdmjzkrbo.sHtML

L. 网络请求
来源：http://read.share.zdbjq.cn/Article/details/gqvhxibgo.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gdoivnyvi.sHtML

[L01] 发送 GET 请求
来源：http://www.share.fehbvm.com/Article/details/ghaxrglri.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://blog.zdbjq.cn/Article/details/gbpclvwax.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.m.share.zdbjq.cn/Article/details/gsdyfxcie.sHtML

JS:   await fetch(url)
来源：http://www.blog.hesvh.cn/Article/details/ggbxehtmj.sHtML

TS:   await fetch(url)
来源：http://www.m.share.fehbvm.com/Article/details/gklqhytoc.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.fehbvm.com/Article/details/gxuxybpmo.sHtML

Go:   resp, err := http.Get(url)
来源：http://read.share.hesvh.cn/Article/details/gclkuavlj.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.fehbvm.com/Article/details/gnicbfiff.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.hesvh.cn/Article/details/gahzjoukb.sHtML

[L02] 发送 POST JSON
来源：http://wap.fehbvm.com/Article/details/gmmkmtdaf.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.hesvh.cn/Article/details/gmumjtjvk.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.zdbjq.cn/Article/details/gfpdmmxvk.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.fehbvm.com/Article/details/gsknswwmu.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.zdbjq.cn/Article/details/ghglbgeiw.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.hesvh.cn/Article/details/gwdwyoaum.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.zdbjq.cn/Article/details/gssizwgzr.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.zdbjq.cn/Article/details/gxigsckaj.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://m.share.hesvh.cn/Article/details/gzwiuefba.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.zdbjq.cn/Article/details/gnluajaug.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.fehbvm.com/Article/details/geengloxy.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.m.share.zdbjq.cn/Article/details/ghnzkeobq.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.hesvh.cn/Article/details/gsrzhwubq.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.hesvh.cn/Article/details/gorqzvvcy.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.hesvh.cn/Article/details/gumijnbgh.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.fehbvm.com/Article/details/gqrzbzzvg.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.hesvh.cn/Article/details/gebkyfxdl.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.hesvh.cn/Article/details/gzrcypygj.sHtML

[L04] 设置超时
来源：http://www.m.share.fehbvm.com/Article/details/gzrgewioz.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.zdbjq.cn/Article/details/getyvlfiz.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.zdbjq.cn/Article/details/gnykfimfl.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.fehbvm.com/Article/details/gafciaoyh.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.zdbjq.cn/Article/details/gjuuednxf.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.zdbjq.cn/Article/details/gdrkmcmmx.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.hesvh.cn/Article/details/goggxiqqm.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.fehbvm.com/Article/details/gnimgecbi.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.hesvh.cn/Article/details/gplqsmobh.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.hesvh.cn/Article/details/grkhwzzui.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.fehbvm.com/Article/details/glrdwteii.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.zdbjq.cn/Article/details/gmsfctyco.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.zdbjq.cn/Article/details/gffmqdbpv.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.fehbvm.com/Article/details/ghqiphkab.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.hesvh.cn/Article/details/gqabbyaus.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.zdbjq.cn/Article/details/grbyebqyx.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.fehbvm.com/Article/details/gzayahtof.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gfkfsarki.sHtML

[L06] 解析响应为 JSON
来源：http://blog.zdbjq.cn/Article/details/gppreuepj.sHtML

Py:   resp.json()
来源：http://blog.fehbvm.com/Article/details/gvtvmjysl.sHtML

PHP:  json_decode($body, true);
来源：http://wap.fehbvm.com/Article/details/gglzqohdl.sHtML

JS:   await resp.json()
来源：http://mobile.hesvh.cn/Article/details/gomehqlqe.sHtML

TS:   await resp.json()
来源：http://read.share.fehbvm.com/Article/details/gpqkdhvtf.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.hesvh.cn/Article/details/gzwjsvaoa.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.zdbjq.cn/Article/details/gvcapeccv.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.hesvh.cn/Article/details/guoawilsw.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.fehbvm.com/Article/details/glmqbjvcf.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.fehbvm.com/Article/details/gzcnmyjdy.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.zdbjq.cn/Article/details/gngmhnmht.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.zdbjq.cn/Article/details/gvekzduor.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.fehbvm.com/Article/details/gnkkijnky.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.fehbvm.com/Article/details/ggteuovbl.sHtML

Java: resp.statusCode()
来源：http://m.share.hesvh.cn/Article/details/gffbqslxt.sHtML

Go:   resp.StatusCode
来源：http://m.share.hesvh.cn/Article/details/gdjojeavw.sHtML

Ruby: resp.code.to_i
来源：http://mobile.fehbvm.com/Article/details/gstcfpsrj.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.zdbjq.cn/Article/details/gitwhhotx.sHtML

[L08] 并发请求多个地址
来源：http://mobile.hesvh.cn/Article/details/ggghyjgll.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.hesvh.cn/Article/details/gdztrzbul.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.hesvh.cn/Article/details/gvpzqsqer.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.hesvh.cn/Article/details/gapswtgir.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.fehbvm.com/Article/details/gdkvgetvd.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.fehbvm.com/Article/details/gnwcumsje.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.fehbvm.com/Article/details/gmfvbvbpu.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.zdbjq.cn/Article/details/gwiipzzdt.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.hesvh.cn/Article/details/gdkhteurl.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gbjqhscub.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.hesvh.cn/Article/details/gaqbhqymt.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gzmruziag.sHtML

[M01] 读取命令行参数
来源：http://blog.hesvh.cn/Article/details/gjcphanem.sHtML

Py:   sys.argv[1:]
来源：http://baike.hesvh.cn/Article/details/gdmwwcwrf.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.fehbvm.com/Article/details/grsgtazzm.sHtML

JS:   process.argv.slice(2)
来源：http://3g.hesvh.cn/Article/details/gbzooldob.sHtML

TS:   process.argv.slice(2)
来源：http://wap.fehbvm.com/Article/details/glbvmndlg.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.zdbjq.cn/Article/details/gggrcthlq.sHtML

Go:   os.Args[1:]
来源：http://blog.fehbvm.com/Article/details/gswigmlfq.sHtML

Ruby: ARGV
来源：http://read.share.fehbvm.com/Article/details/gjtsngztj.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.hesvh.cn/Article/details/gkzuhzije.sHtML

[M02] 读取环境变量
来源：http://3g.fehbvm.com/Article/details/gvqtcmxum.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.hesvh.cn/Article/details/gnuzvpiju.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.hesvh.cn/Article/details/gxswaxmwd.sHtML

JS:   process.env.HOME
来源：http://www.blog.fehbvm.com/Article/details/goclyyant.sHtML

TS:   process.env.HOME
来源：http://blog.hesvh.cn/Article/details/gyisdyirg.sHtML

Java: System.getenv("HOME")
来源：http://www.share.zdbjq.cn/Article/details/gffhzlzjo.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.zdbjq.cn/Article/details/grsqqysme.sHtML

Ruby: ENV["HOME"]
来源：http://3g.zdbjq.cn/Article/details/gbkdedifz.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.hesvh.cn/Article/details/ganjsieax.sHtML

[M03] 执行外部命令
来源：http://blog.hesvh.cn/Article/details/gswaikuug.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.fehbvm.com/Article/details/gxblpxpqy.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.hesvh.cn/Article/details/gmcosxsrn.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.zdbjq.cn/Article/details/gwywugczd.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.hesvh.cn/Article/details/goqphlrvh.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.zdbjq.cn/Article/details/gfdjlmcki.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.fehbvm.com/Article/details/gidezmyvq.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.hesvh.cn/Article/details/giahpaibb.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.hesvh.cn/Article/details/gtakcjzfm.sHtML

[M04] 获取当前工作目录
来源：http://blog.hesvh.cn/Article/details/gqliplulc.sHtML

Py:   os.getcwd()
来源：http://3g.hesvh.cn/Article/details/gxwwhumjv.sHtML

PHP:  getcwd();
来源：http://m.share.fehbvm.com/Article/details/ggpbbdsuk.sHtML

JS:   process.cwd()
来源：http://wap.zdbjq.cn/Article/details/gjhspmqlp.sHtML

TS:   process.cwd()
来源：http://3g.zdbjq.cn/Article/details/guzyrhzhk.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.fehbvm.com/Article/details/gqoekegoj.sHtML

Go:   os.Getwd()
来源：http://read.share.hesvh.cn/Article/details/gmgiygshs.sHtML

Ruby: Dir.pwd
来源：http://mobile.zdbjq.cn/Article/details/geptgowrm.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.zdbjq.cn/Article/details/gjxshsgid.sHtML

[M05] 设置退出码
来源：http://read.share.fehbvm.com/Article/details/gfnfbwcai.sHtML

Py:   sys.exit(1)
来源：http://blog.zdbjq.cn/Article/details/gqjazpzvn.sHtML

PHP:  exit(1);
来源：http://3g.hesvh.cn/Article/details/gkltagyix.sHtML

JS:   process.exit(1)
来源：http://baike.fehbvm.com/Article/details/gnzvacvlr.sHtML

TS:   process.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/grfvuseuo.sHtML

Java: System.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gjervdpmj.sHtML

Go:   os.Exit(1)
来源：http://blog.hesvh.cn/Article/details/gowlqtcfs.sHtML

Ruby: exit 1
来源：http://blog.hesvh.cn/Article/details/gmmwrskrr.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.fehbvm.com/Article/details/gsfilyolk.sHtML

[M06] 向标准错误输出
来源：http://www.blog.fehbvm.com/Article/details/gkkrmbcmr.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.fehbvm.com/Article/details/grawazfwc.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.hesvh.cn/Article/details/ggodvmabr.sHtML

JS:   console.error("err")
来源：http://3g.zdbjq.cn/Article/details/grizzuzwe.sHtML

TS:   console.error("err")
来源：http://www.m.share.fehbvm.com/Article/details/gtmqvvvqm.sHtML

Java: System.err.println("err")
来源：http://www.share.fehbvm.com/Article/details/gjvamxehx.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.zdbjq.cn/Article/details/gnbxgmsxi.sHtML

Ruby: warn "err"
来源：http://read.share.fehbvm.com/Article/details/gupuezcow.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.zdbjq.cn/Article/details/guvdzmzil.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.zdbjq.cn/Article/details/gyfvbnsas.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.fehbvm.com/Article/details/gytnxqgdn.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.hesvh.cn/Article/details/gruxscwao.sHtML

JS:   require.main === module
来源：http://baike.hesvh.cn/Article/details/goqocwvbw.sHtML

TS:   require.main === module
来源：http://mobile.zdbjq.cn/Article/details/gpxpcpocj.sHtML

Java: public static void main(String[] args)
来源：http://read.share.hesvh.cn/Article/details/grargbgbt.sHtML

Go:   func main()
来源：http://wap.fehbvm.com/Article/details/gvlkamzwf.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.fehbvm.com/Article/details/gycbzhsqh.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.zdbjq.cn/Article/details/gxgvchqlx.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.fehbvm.com/Article/details/gimoxmtry.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.zdbjq.cn/Article/details/gtevmesfs.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.zdbjq.cn/Article/details/gcbjnedou.sHtML

JS:   process.platform;  process.version
来源：http://baike.fehbvm.com/Article/details/gfknigedx.sHtML

TS:   process.platform;  process.version
来源：http://mobile.zdbjq.cn/Article/details/gwzzypjec.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.hesvh.cn/Article/details/geexyolbq.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.hesvh.cn/Article/details/glkonrpep.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.hesvh.cn/Article/details/gjsglelpj.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.hesvh.cn/Article/details/ghihgexvw.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gkfznnvgv.sHtML

N. 数据结构与算法
来源：http://m.share.hesvh.cn/Article/details/ghkczfjjb.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gsokexhya.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.zdbjq.cn/Article/details/gdesglzxi.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gkmoxjewt.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.hesvh.cn/Article/details/gzukfgxoj.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.zdbjq.cn/Article/details/gydzracuf.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.hesvh.cn/Article/details/gymmpzdhz.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gmxmzkrnp.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gwdkpombt.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.fehbvm.com/Article/details/gvydiwutp.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.fehbvm.com/Article/details/groniyfwh.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.zdbjq.cn/Article/details/gnituahrz.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.hesvh.cn/Article/details/gtbpcxlaj.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.zdbjq.cn/Article/details/ghqezzzix.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.fehbvm.com/Article/details/grpfwqvjf.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.hesvh.cn/Article/details/grjabicar.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.zdbjq.cn/Article/details/gskxysjnn.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.zdbjq.cn/Article/details/gmzxjbebj.sHtML

Ruby: arr.sort
来源：http://baike.hesvh.cn/Article/details/gutkprhan.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.fehbvm.com/Article/details/gdrbqiryb.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.fehbvm.com/Article/details/gbgnaelbk.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.zdbjq.cn/Article/details/goobujccm.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.fehbvm.com/Article/details/gixougnqq.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.fehbvm.com/Article/details/gjtrovkpm.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.zdbjq.cn/Article/details/gjoixpqlh.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.hesvh.cn/Article/details/gmghyfwla.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.hesvh.cn/Article/details/gfuzsalww.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.zdbjq.cn/Article/details/gsmmtugvp.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.hesvh.cn/Article/details/gghqvgvmb.sHtML

[N04] 斐波那契数列
来源：http://www.blog.fehbvm.com/Article/details/gqhkbiceb.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.hesvh.cn/Article/details/glcfkxcio.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.hesvh.cn/Article/details/gffjitmlt.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.hesvh.cn/Article/details/gnizjtfyk.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.zdbjq.cn/Article/details/gxhrxkhsx.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.zdbjq.cn/Article/details/gjnhnjspi.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.zdbjq.cn/Article/details/gbnttvgvc.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.zdbjq.cn/Article/details/gnklyxshe.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/gwurlinll.sHtML

[N05] 最大公约数
来源：http://3g.hesvh.cn/Article/details/gsbabhtiz.sHtML

Py:   math.gcd(a, b)
来源：http://blog.fehbvm.com/Article/details/gmuwnwsii.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.fehbvm.com/Article/details/gsavoemic.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.fehbvm.com/Article/details/gfsfqefgg.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.zdbjq.cn/Article/details/gyoyjfbnt.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.zdbjq.cn/Article/details/ghrgkcxwj.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.hesvh.cn/Article/details/gloivmsmo.sHtML

Ruby: a.gcd(b)
来源：http://3g.zdbjq.cn/Article/details/gpsffwpze.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.fehbvm.com/Article/details/gfxyytngi.sHtML

[N06] 判断回文字符串
来源：http://blog.hesvh.cn/Article/details/gewncyvwe.sHtML

Py:   s == s[::-1]
来源：http://wap.fehbvm.com/Article/details/gtmjvamzd.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.hesvh.cn/Article/details/gwgrjgelb.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/gxpwhjelt.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/gvrbpnkwy.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.fehbvm.com/Article/details/gsgwtcuey.sHtML

Go:   // 双指针从两端比较
来源：http://3g.hesvh.cn/Article/details/giypeexww.sHtML

Ruby: s == s.reverse
来源：http://read.share.zdbjq.cn/Article/details/ggbhphzoa.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.fehbvm.com/Article/details/gtnukucig.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.fehbvm.com/Article/details/glygsqfbt.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.hesvh.cn/Article/details/ghotumuim.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.hesvh.cn/Article/details/gtmxwehbl.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.hesvh.cn/Article/details/gzjnedfhc.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.zdbjq.cn/Article/details/gmixhofxe.sHtML

Java: // 手写 HashMap
来源：http://www.share.fehbvm.com/Article/details/gxmwlemck.sHtML

Go:   // 手写 map[int]int
来源：http://3g.zdbjq.cn/Article/details/gnxeushgr.sHtML

Ruby: // 手写 Hash
来源：http://3g.fehbvm.com/Article/details/glxhqtbyw.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.fehbvm.com/Article/details/growypofu.sHtML

[N08] 生成全排列
来源：http://read.share.hesvh.cn/Article/details/gyylhktwd.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.fehbvm.com/Article/details/gcqvxbosx.sHtML

PHP:  // 手写递归交换
来源：http://3g.fehbvm.com/Article/details/gvenqhnra.sHtML

JS:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gytfceslp.sHtML

TS:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gbvaxrbdj.sHtML

Java: // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gidnhaogl.sHtML

Go:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gfjisgntn.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.zdbjq.cn/Article/details/gnsrctjjy.sHtML

C#:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gycmroxis.sHtML

[N09] 栈与队列
来源：http://wap.zdbjq.cn/Article/details/gduedsymo.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/gjwvisujy.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.hesvh.cn/Article/details/ghigonqjy.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.hesvh.cn/Article/details/gvytifrjo.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.hesvh.cn/Article/details/gqnawrgrw.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.fehbvm.com/Article/details/gqtmjoejh.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.fehbvm.com/Article/details/gztkurawp.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.hesvh.cn/Article/details/gyxuyqyzr.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.hesvh.cn/Article/details/gvqvxopcd.sHtML

[N10] 链表节点定义
来源：http://read.share.fehbvm.com/Article/details/gfaujpbqj.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.hesvh.cn/Article/details/gaidopabp.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.zdbjq.cn/Article/details/ggmbwlxhz.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.fehbvm.com/Article/details/gphoupwgz.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.fehbvm.com/Article/details/ggswyhpkv.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.zdbjq.cn/Article/details/gligbiixy.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.zdbjq.cn/Article/details/gwiqsoajm.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.zdbjq.cn/Article/details/galztlnlu.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.fehbvm.com/Article/details/gwedraeuy.sHtML

[N11] 二叉树中序遍历
来源：http://blog.fehbvm.com/Article/details/gdkldyhho.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.zdbjq.cn/Article/details/gptwgszct.sHtML

PHP:  // 手写递归函数
来源：http://baike.fehbvm.com/Article/details/grjwfqjux.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.hesvh.cn/Article/details/gaonjephi.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.hesvh.cn/Article/details/gbqhibwzd.sHtML

Java: // 手写递归
来源：http://baike.fehbvm.com/Article/details/ggajwawwu.sHtML

Go:   // 手写递归
来源：http://www.share.fehbvm.com/Article/details/gkwlgrwlc.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.hesvh.cn/Article/details/gogrpqtyr.sHtML

C#:   // 手写递归
来源：http://m.share.hesvh.cn/Article/details/gdrjojdxi.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.hesvh.cn/Article/details/gtyircwmf.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.zdbjq.cn/Article/details/gwsrblhrh.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.fehbvm.com/Article/details/gjutzusce.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.zdbjq.cn/Article/details/goapdbara.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.fehbvm.com/Article/details/gbkluortr.sHtML


<!-- 参考信息 -->