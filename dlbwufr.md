代发 wailian999

Ruby: JSON.pretty_generate(obj)
来源：http://wap.fehbvm.com/Article/details/gbdvegzks.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.share.zdbjq.cn/Article/details/ghakrtsbp.sHtML

[K04] 读取 JSON 文件
来源：http://www.m.share.zdbjq.cn/Article/details/gurhvzjbo.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.share.zdbjq.cn/Article/details/gexaktqpk.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.blog.hesvh.cn/Article/details/gfilwafxs.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.hesvh.cn/Article/details/geufhyjcm.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.hesvh.cn/Article/details/glehhoydy.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.share.fehbvm.com/Article/details/gjaqtwuld.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.share.zdbjq.cn/Article/details/gagpjjbgg.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.fehbvm.com/Article/details/glfcworbe.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://baike.hesvh.cn/Article/details/gofbwbxla.sHtML

[K05] 深拷贝对象
来源：http://www.share.hesvh.cn/Article/details/gzgmhpwvk.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.fehbvm.com/Article/details/gcghoirpu.sHtML

PHP:  unserialize(serialize($obj));
来源：http://3g.fehbvm.com/Article/details/gngheesls.sHtML

JS:   structuredClone(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/goozpdqzx.sHtML

TS:   structuredClone(obj)
来源：http://blog.fehbvm.com/Article/details/gpcdydkmr.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://m.share.hesvh.cn/Article/details/gzkcsdfyq.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.m.share.fehbvm.com/Article/details/gnhatrzwm.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://baike.fehbvm.com/Article/details/gkoqcefai.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://wap.zdbjq.cn/Article/details/gqnjfvrca.sHtML

[K06] 解析 URL 查询串
来源：http://3g.fehbvm.com/Article/details/gwhepmnrg.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://blog.fehbvm.com/Article/details/geygtmuxm.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.share.fehbvm.com/Article/details/glmvrobzk.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.hesvh.cn/Article/details/gkztmebnb.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.zdbjq.cn/Article/details/gdurkpfol.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.share.zdbjq.cn/Article/details/gbabuuxpv.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://m.share.hesvh.cn/Article/details/gnedfecoi.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.hesvh.cn/Article/details/gwseknjhp.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.fehbvm.com/Article/details/gueskvvqn.sHtML

[K07] 进制转换
来源：http://baike.hesvh.cn/Article/details/ghifrvjsy.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://m.share.zdbjq.cn/Article/details/gfjhyznai.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.m.share.zdbjq.cn/Article/details/gebmibkhp.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.m.share.zdbjq.cn/Article/details/gtofksacv.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://read.share.zdbjq.cn/Article/details/gtjfvtevq.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wap.fehbvm.com/Article/details/gioterkqz.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.zdbjq.cn/Article/details/getuoevwb.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.zdbjq.cn/Article/details/goztkjewy.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.hesvh.cn/Article/details/glryzxpvv.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.m.share.hesvh.cn/Article/details/gogxfvjsn.sHtML

Py:   pickle.dumps(obj)
来源：http://baike.hesvh.cn/Article/details/gnvsbxzrd.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://read.share.fehbvm.com/Article/details/gvfyujqqk.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.share.zdbjq.cn/Article/details/gcqmvniff.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://3g.fehbvm.com/Article/details/gdhcaxpob.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://blog.fehbvm.com/Article/details/grgbpsxow.sHtML

Go:   encoding/gob
来源：http://blog.fehbvm.com/Article/details/gykcilhdb.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.fehbvm.com/Article/details/gskloqeik.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.hesvh.cn/Article/details/gelyrdmxo.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gvlagirge.sHtML

L. 网络请求
来源：http://www.m.share.hesvh.cn/Article/details/gpueiqdvp.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gzmyfazak.sHtML

[L01] 发送 GET 请求
来源：http://mobile.hesvh.cn/Article/details/ggosbhsaq.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://baike.fehbvm.com/Article/details/gxnaceitl.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.hesvh.cn/Article/details/gtyuddaxh.sHtML

JS:   await fetch(url)
来源：http://mobile.hesvh.cn/Article/details/gkpmxreuj.sHtML

TS:   await fetch(url)
来源：http://wap.zdbjq.cn/Article/details/gvzdzbtnx.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.fehbvm.com/Article/details/gdovfhjix.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.hesvh.cn/Article/details/gdgcnmuvz.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.hesvh.cn/Article/details/gugafqcds.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.zdbjq.cn/Article/details/gsngypivb.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.hesvh.cn/Article/details/gonsusrqr.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://m.share.hesvh.cn/Article/details/gjelukhnp.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://baike.fehbvm.com/Article/details/gyjkvglja.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.hesvh.cn/Article/details/gjwhxuzrm.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.hesvh.cn/Article/details/gkyybnhqs.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.zdbjq.cn/Article/details/gvsxnvazw.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.hesvh.cn/Article/details/gegnvzjgn.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://blog.zdbjq.cn/Article/details/gqwlvjuns.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.fehbvm.com/Article/details/gtoabwovc.sHtML

[L03] 设置自定义请求头
来源：http://www.share.fehbvm.com/Article/details/gaavoovxy.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://read.share.zdbjq.cn/Article/details/gotrtxzpr.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.fehbvm.com/Article/details/gryhnbqwn.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.fehbvm.com/Article/details/grasnzsal.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.fehbvm.com/Article/details/gyqwmeakj.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.hesvh.cn/Article/details/gxeodrfva.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.hesvh.cn/Article/details/ggeptfftv.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.share.hesvh.cn/Article/details/gywgakvho.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.zdbjq.cn/Article/details/gxousjvvt.sHtML

[L04] 设置超时
来源：http://read.share.zdbjq.cn/Article/details/giybnyzne.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.hesvh.cn/Article/details/gdgdfnqij.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.zdbjq.cn/Article/details/ghauqzpad.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.fehbvm.com/Article/details/girnsdvlz.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.zdbjq.cn/Article/details/gaklrhtid.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.zdbjq.cn/Article/details/glramhvln.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.fehbvm.com/Article/details/gqkglpteo.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.fehbvm.com/Article/details/gmkarblse.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.hesvh.cn/Article/details/gxlmzkmur.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.fehbvm.com/Article/details/gnztlhmru.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://read.share.fehbvm.com/Article/details/gvdrnejok.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.hesvh.cn/Article/details/gpwqhrtny.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.hesvh.cn/Article/details/gyndjiqzg.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.fehbvm.com/Article/details/gxmjjgwnw.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.zdbjq.cn/Article/details/gxpjtgnud.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://m.share.fehbvm.com/Article/details/gwojbptfv.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.zdbjq.cn/Article/details/giduiarck.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gnvbvrujp.sHtML

[L06] 解析响应为 JSON
来源：http://wap.fehbvm.com/Article/details/gnqfbtetj.sHtML

Py:   resp.json()
来源：http://www.m.share.hesvh.cn/Article/details/gqowyqaiz.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.zdbjq.cn/Article/details/gvkafhsup.sHtML

JS:   await resp.json()
来源：http://blog.hesvh.cn/Article/details/gdgsecltg.sHtML

TS:   await resp.json()
来源：http://read.share.zdbjq.cn/Article/details/galawqcyy.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.fehbvm.com/Article/details/geuzfedrf.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.zdbjq.cn/Article/details/ghyatctnj.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.fehbvm.com/Article/details/gyerruxki.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.zdbjq.cn/Article/details/gmgsckeyd.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.fehbvm.com/Article/details/gmyaesdty.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.hesvh.cn/Article/details/gzinokzkn.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.hesvh.cn/Article/details/gzehpndbs.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.fehbvm.com/Article/details/gpajamvxl.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.zdbjq.cn/Article/details/gyqyjnjje.sHtML

Java: resp.statusCode()
来源：http://baike.fehbvm.com/Article/details/gpqifhgqs.sHtML

Go:   resp.StatusCode
来源：http://baike.hesvh.cn/Article/details/gxtzbhczy.sHtML

Ruby: resp.code.to_i
来源：http://blog.fehbvm.com/Article/details/gpvopawda.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.hesvh.cn/Article/details/gwidewrgl.sHtML

[L08] 并发请求多个地址
来源：http://blog.zdbjq.cn/Article/details/giuwcnplk.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.zdbjq.cn/Article/details/guhxlzynf.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.hesvh.cn/Article/details/gulqklgbc.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.zdbjq.cn/Article/details/gkmwhgxqb.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.hesvh.cn/Article/details/gwhzakzgj.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.zdbjq.cn/Article/details/gntnbqjqj.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.hesvh.cn/Article/details/grchsuglv.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.hesvh.cn/Article/details/gpqkoibnj.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.hesvh.cn/Article/details/gascafnay.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/grtnyxgjw.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.hesvh.cn/Article/details/glktrhrwt.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gmxtqweqe.sHtML

[M01] 读取命令行参数
来源：http://wap.zdbjq.cn/Article/details/gkiuuyhkn.sHtML

Py:   sys.argv[1:]
来源：http://read.share.zdbjq.cn/Article/details/gtyyweufh.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.fehbvm.com/Article/details/gnvxrueov.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.zdbjq.cn/Article/details/gzbhlvebe.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.hesvh.cn/Article/details/gcrbrcdcv.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.zdbjq.cn/Article/details/gfjnqpznw.sHtML

Go:   os.Args[1:]
来源：http://wap.hesvh.cn/Article/details/guurnwloh.sHtML

Ruby: ARGV
来源：http://www.m.share.hesvh.cn/Article/details/gwbwgabsi.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.hesvh.cn/Article/details/ggkcyptsd.sHtML

[M02] 读取环境变量
来源：http://blog.zdbjq.cn/Article/details/gqlrmrtdc.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.zdbjq.cn/Article/details/gklgkjded.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.fehbvm.com/Article/details/giyrqcmzr.sHtML

JS:   process.env.HOME
来源：http://mobile.hesvh.cn/Article/details/gegywdxcw.sHtML

TS:   process.env.HOME
来源：http://www.blog.hesvh.cn/Article/details/gjrchlyvh.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.zdbjq.cn/Article/details/gkzitgztz.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.zdbjq.cn/Article/details/gcfuxorsq.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.fehbvm.com/Article/details/gffxoeryy.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.hesvh.cn/Article/details/gldyfahpd.sHtML

[M03] 执行外部命令
来源：http://www.share.zdbjq.cn/Article/details/gzqnpoyhi.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.zdbjq.cn/Article/details/gmpjphfke.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.hesvh.cn/Article/details/gvtwbieea.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.hesvh.cn/Article/details/gldmrzisi.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.fehbvm.com/Article/details/galzgzkol.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.hesvh.cn/Article/details/getkvyonp.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.hesvh.cn/Article/details/gherrjzxr.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.zdbjq.cn/Article/details/gyilprmil.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.hesvh.cn/Article/details/ghwdnpsnh.sHtML

[M04] 获取当前工作目录
来源：http://3g.hesvh.cn/Article/details/gwnfxwqir.sHtML

Py:   os.getcwd()
来源：http://read.share.fehbvm.com/Article/details/gatexdotl.sHtML

PHP:  getcwd();
来源：http://www.blog.zdbjq.cn/Article/details/gohrengcl.sHtML

JS:   process.cwd()
来源：http://blog.fehbvm.com/Article/details/gqvjbyhai.sHtML

TS:   process.cwd()
来源：http://mobile.hesvh.cn/Article/details/gnprnskfh.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.hesvh.cn/Article/details/gnctkdtbk.sHtML

Go:   os.Getwd()
来源：http://www.m.share.zdbjq.cn/Article/details/gnnjilccm.sHtML

Ruby: Dir.pwd
来源：http://m.share.zdbjq.cn/Article/details/gaogyarnq.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.hesvh.cn/Article/details/gkoazfhdm.sHtML

[M05] 设置退出码
来源：http://www.m.share.hesvh.cn/Article/details/gwqabvisa.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gdrrxrhiy.sHtML

PHP:  exit(1);
来源：http://mobile.hesvh.cn/Article/details/gggtaorjz.sHtML

JS:   process.exit(1)
来源：http://baike.fehbvm.com/Article/details/glfmhvuxt.sHtML

TS:   process.exit(1)
来源：http://baike.hesvh.cn/Article/details/ggisegjem.sHtML

Java: System.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gnewqkyhv.sHtML

Go:   os.Exit(1)
来源：http://baike.zdbjq.cn/Article/details/gzkxdgoes.sHtML

Ruby: exit 1
来源：http://read.share.hesvh.cn/Article/details/glmjmgrpf.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.zdbjq.cn/Article/details/gvlzeohdr.sHtML

[M06] 向标准错误输出
来源：http://baike.hesvh.cn/Article/details/gwdcaeuyi.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.fehbvm.com/Article/details/ghngdwskk.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.hesvh.cn/Article/details/gpghxydli.sHtML

JS:   console.error("err")
来源：http://baike.hesvh.cn/Article/details/gsremjhgw.sHtML

TS:   console.error("err")
来源：http://wap.fehbvm.com/Article/details/glfozcapz.sHtML

Java: System.err.println("err")
来源：http://www.share.zdbjq.cn/Article/details/geusibwzx.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.fehbvm.com/Article/details/gxariyxnc.sHtML

Ruby: warn "err"
来源：http://wap.zdbjq.cn/Article/details/gztxsojjt.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.zdbjq.cn/Article/details/gxqqixnfw.sHtML

[M07] 判断是否为主入口
来源：http://wap.zdbjq.cn/Article/details/gzwctqhgc.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.hesvh.cn/Article/details/glztuibaj.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.fehbvm.com/Article/details/gszetdgci.sHtML

JS:   require.main === module
来源：http://mobile.zdbjq.cn/Article/details/gucpjdhch.sHtML

TS:   require.main === module
来源：http://3g.fehbvm.com/Article/details/gdgliamvg.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.fehbvm.com/Article/details/gbuxkupun.sHtML

Go:   func main()
来源：http://3g.hesvh.cn/Article/details/gfblymris.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.fehbvm.com/Article/details/gnscbdtmq.sHtML

C#:   static void Main(string[] args)
来源：http://baike.hesvh.cn/Article/details/gpbahhnhx.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.hesvh.cn/Article/details/grdadttzw.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.fehbvm.com/Article/details/gkpemuitj.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.fehbvm.com/Article/details/gbxrxnqqq.sHtML

JS:   process.platform;  process.version
来源：http://3g.fehbvm.com/Article/details/gsbvpqyux.sHtML

TS:   process.platform;  process.version
来源：http://read.share.hesvh.cn/Article/details/gcvyjwxbl.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.fehbvm.com/Article/details/gtnfkbvft.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.fehbvm.com/Article/details/gisyasfjg.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.zdbjq.cn/Article/details/gleliuims.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.zdbjq.cn/Article/details/gkouxmbbq.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/ggpxbdeij.sHtML

N. 数据结构与算法
来源：http://www.share.hesvh.cn/Article/details/gacxwybsi.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gxhlajlyl.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.hesvh.cn/Article/details/gmozofkli.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.hesvh.cn/Article/details/gmhjsyouw.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.fehbvm.com/Article/details/gjqewpsuc.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.fehbvm.com/Article/details/goebcovpj.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.hesvh.cn/Article/details/grseosckw.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gkqgghfwk.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.fehbvm.com/Article/details/ghjezvtlw.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.zdbjq.cn/Article/details/gdoyjttap.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.hesvh.cn/Article/details/gtzrlcxay.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.fehbvm.com/Article/details/gkrmljfgs.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.fehbvm.com/Article/details/gmdalexgx.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.hesvh.cn/Article/details/gfubhsins.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.fehbvm.com/Article/details/gxiekdosv.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.zdbjq.cn/Article/details/geaunsrwq.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.fehbvm.com/Article/details/gvzjcznxq.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.fehbvm.com/Article/details/gfyseucrw.sHtML

Ruby: arr.sort
来源：http://mobile.fehbvm.com/Article/details/gjrrvgpgy.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.fehbvm.com/Article/details/gwtzhbbsa.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.fehbvm.com/Article/details/glanqqarg.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.fehbvm.com/Article/details/gusfxkcsp.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.hesvh.cn/Article/details/gbouuxldb.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.hesvh.cn/Article/details/gqmgawlur.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.fehbvm.com/Article/details/gjstmlpyc.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.zdbjq.cn/Article/details/gkebzgmmw.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.hesvh.cn/Article/details/gnvxavwwj.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.fehbvm.com/Article/details/giuwrziow.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.zdbjq.cn/Article/details/gsxudmqms.sHtML

[N04] 斐波那契数列
来源：http://m.share.zdbjq.cn/Article/details/gsaztqyrb.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.fehbvm.com/Article/details/gttudrrnb.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.fehbvm.com/Article/details/ggxyvwuiw.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.hesvh.cn/Article/details/gewimttug.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.hesvh.cn/Article/details/gsxmbjboy.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.zdbjq.cn/Article/details/gyfbwtesa.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.zdbjq.cn/Article/details/gidvjyhqe.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.fehbvm.com/Article/details/ggjfejiwe.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.hesvh.cn/Article/details/gujcyuswn.sHtML

[N05] 最大公约数
来源：http://www.m.share.zdbjq.cn/Article/details/gzscmtrtk.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.zdbjq.cn/Article/details/gbcdjoxjk.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.fehbvm.com/Article/details/gkqrbtodf.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.fehbvm.com/Article/details/gjnleqlsr.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.hesvh.cn/Article/details/gmuyqraki.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.hesvh.cn/Article/details/gdwupvsqx.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.fehbvm.com/Article/details/gruiywgut.sHtML

Ruby: a.gcd(b)
来源：http://wap.fehbvm.com/Article/details/gxidnmbzq.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.hesvh.cn/Article/details/gonhwzrtf.sHtML

[N06] 判断回文字符串
来源：http://baike.fehbvm.com/Article/details/ghwvjmixk.sHtML

Py:   s == s[::-1]
来源：http://www.share.zdbjq.cn/Article/details/gzumkdeks.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.zdbjq.cn/Article/details/gqtgybxim.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/gqexoukfu.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/glwhfctfl.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.fehbvm.com/Article/details/gkbgutatt.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.zdbjq.cn/Article/details/gtotlxknq.sHtML

Ruby: s == s.reverse
来源：http://blog.fehbvm.com/Article/details/gcfuskfpp.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.zdbjq.cn/Article/details/gjhjrkqil.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.hesvh.cn/Article/details/gmmievbki.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.hesvh.cn/Article/details/gdvkybsof.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.fehbvm.com/Article/details/gyhtxuuia.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.zdbjq.cn/Article/details/ggyrewpcf.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.zdbjq.cn/Article/details/gtoulbvdx.sHtML

Java: // 手写 HashMap
来源：http://m.share.fehbvm.com/Article/details/gbuqkcsjh.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.hesvh.cn/Article/details/gwqomgcqc.sHtML

Ruby: // 手写 Hash
来源：http://www.share.fehbvm.com/Article/details/guwsrklbc.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.zdbjq.cn/Article/details/gafjcwyhp.sHtML

[N08] 生成全排列
来源：http://read.share.hesvh.cn/Article/details/gpkldibuu.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.hesvh.cn/Article/details/gxzcnaysy.sHtML

PHP:  // 手写递归交换
来源：http://blog.fehbvm.com/Article/details/gdwkihuwy.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gjnnkrwgi.sHtML

TS:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gebozwmva.sHtML

Java: // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gpvvyseoj.sHtML

Go:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gezkhpumz.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.hesvh.cn/Article/details/gnfgepolz.sHtML

C#:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gtxtkcwcr.sHtML

[N09] 栈与队列
来源：http://m.share.hesvh.cn/Article/details/gdeqmrqym.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.fehbvm.com/Article/details/gnuwxvmky.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.fehbvm.com/Article/details/gsapvjjup.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.zdbjq.cn/Article/details/grnsydunv.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.zdbjq.cn/Article/details/gixbuowtw.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.zdbjq.cn/Article/details/gblyxptjd.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.fehbvm.com/Article/details/gmdiopjea.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.fehbvm.com/Article/details/gpjbungjz.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.fehbvm.com/Article/details/goowrshzy.sHtML

[N10] 链表节点定义
来源：http://m.share.fehbvm.com/Article/details/gnphnxnea.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.zdbjq.cn/Article/details/ggjkgyiqd.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.zdbjq.cn/Article/details/gwjhubnuq.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.zdbjq.cn/Article/details/ggpoqusrs.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.zdbjq.cn/Article/details/ghpbgetgh.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.zdbjq.cn/Article/details/gmdulpcsl.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.zdbjq.cn/Article/details/gbgzamhgw.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.fehbvm.com/Article/details/ghdngtqil.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.fehbvm.com/Article/details/gqeylbmbq.sHtML

[N11] 二叉树中序遍历
来源：http://blog.zdbjq.cn/Article/details/glgiymvan.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.fehbvm.com/Article/details/gjetfrxvo.sHtML

PHP:  // 手写递归函数
来源：http://wap.zdbjq.cn/Article/details/gjssnvdiu.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.hesvh.cn/Article/details/gnsktroxg.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.zdbjq.cn/Article/details/gzpeqxpou.sHtML

Java: // 手写递归
来源：http://www.share.hesvh.cn/Article/details/gkchweovw.sHtML

Go:   // 手写递归
来源：http://www.blog.zdbjq.cn/Article/details/gjwrdyiub.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.hesvh.cn/Article/details/gzonfdosn.sHtML

C#:   // 手写递归
来源：http://wap.fehbvm.com/Article/details/gqkzaipey.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.fehbvm.com/Article/details/gdqqahqef.sHtML


<!-- 参考信息 -->