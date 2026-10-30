代发 wailian999

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wap.fehbvm.com/Article/details/gsamaggrl.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://read.share.zdbjq.cn/Article/details/gmyhggqea.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://m.share.fehbvm.com/Article/details/gbvdreuad.sHtML

[K05] 深拷贝对象
来源：http://www.m.share.zdbjq.cn/Article/details/gdvisbdux.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.zdbjq.cn/Article/details/gqjodrrdq.sHtML

PHP:  unserialize(serialize($obj));
来源：http://read.share.fehbvm.com/Article/details/ggmgbfxmj.sHtML

JS:   structuredClone(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gzcsvbgoa.sHtML

TS:   structuredClone(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gxybnvwjb.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.zdbjq.cn/Article/details/gcwjrlxkc.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.blog.fehbvm.com/Article/details/gndzifpex.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.share.fehbvm.com/Article/details/guovcjqih.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://3g.fehbvm.com/Article/details/geerwpcox.sHtML

[K06] 解析 URL 查询串
来源：http://wap.zdbjq.cn/Article/details/gvmlavxbr.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.share.fehbvm.com/Article/details/ggzykcmdj.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wap.zdbjq.cn/Article/details/gsxjpzlll.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.hesvh.cn/Article/details/glqscjhgt.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.zdbjq.cn/Article/details/gmccmdzuc.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.blog.fehbvm.com/Article/details/ggyxdtzce.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://baike.fehbvm.com/Article/details/gnnyekjxl.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://m.share.zdbjq.cn/Article/details/githgbogw.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.m.share.zdbjq.cn/Article/details/gjokrzrrq.sHtML

[K07] 进制转换
来源：http://mobile.hesvh.cn/Article/details/gvaguioyn.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mobile.hesvh.cn/Article/details/gaobxlhph.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.fehbvm.com/Article/details/gypyxjuyj.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.m.share.hesvh.cn/Article/details/gccvrdnzr.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://baike.zdbjq.cn/Article/details/gahihwgkf.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.m.share.fehbvm.com/Article/details/gtkgjhdgx.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.fehbvm.com/Article/details/gywnqzogg.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://baike.zdbjq.cn/Article/details/gvvhppsam.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.fehbvm.com/Article/details/gtgpzlmms.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://wap.hesvh.cn/Article/details/gumewyoim.sHtML

Py:   pickle.dumps(obj)
来源：http://www.blog.hesvh.cn/Article/details/gaqnwaolx.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://mobile.fehbvm.com/Article/details/gehotsgqg.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://mobile.hesvh.cn/Article/details/gvagwumyc.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://read.share.fehbvm.com/Article/details/gnbrocrtn.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mobile.hesvh.cn/Article/details/gdvnqvvnq.sHtML

Go:   encoding/gob
来源：http://m.share.hesvh.cn/Article/details/glbmrdire.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gkexmeadv.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.fehbvm.com/Article/details/gfkjljbdt.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gpwlxotqh.sHtML

L. 网络请求
来源：http://3g.zdbjq.cn/Article/details/gkswtyjcj.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gbzeuqvch.sHtML

[L01] 发送 GET 请求
来源：http://wap.zdbjq.cn/Article/details/gqujxbasf.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.hesvh.cn/Article/details/gxostltvy.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.zdbjq.cn/Article/details/gcokcngba.sHtML

JS:   await fetch(url)
来源：http://wap.fehbvm.com/Article/details/guxdgpkuw.sHtML

TS:   await fetch(url)
来源：http://baike.hesvh.cn/Article/details/gowxizqal.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.hesvh.cn/Article/details/ggfkqjarh.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.fehbvm.com/Article/details/gyyaklwsh.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.zdbjq.cn/Article/details/ghvgdzkfc.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://blog.zdbjq.cn/Article/details/gnbtryavb.sHtML

[L02] 发送 POST JSON
来源：http://mobile.zdbjq.cn/Article/details/gmfahjtnp.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.share.zdbjq.cn/Article/details/gtgrefqaq.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.hesvh.cn/Article/details/gklgkrnqn.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.zdbjq.cn/Article/details/gqpbmvlth.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.fehbvm.com/Article/details/gshitbqel.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.zdbjq.cn/Article/details/gdcwduckt.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.fehbvm.com/Article/details/gugtievlz.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.zdbjq.cn/Article/details/gputkbwqa.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.zdbjq.cn/Article/details/gbtivusbg.sHtML

[L03] 设置自定义请求头
来源：http://baike.zdbjq.cn/Article/details/gmxybyemg.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.hesvh.cn/Article/details/gmwieusyn.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.zdbjq.cn/Article/details/gdhtamsxm.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.zdbjq.cn/Article/details/ghyedrqhb.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.hesvh.cn/Article/details/gokwruhfr.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.zdbjq.cn/Article/details/gzzhdwqoa.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.blog.hesvh.cn/Article/details/gutgxqnle.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.hesvh.cn/Article/details/gddjvsqxh.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.zdbjq.cn/Article/details/gtewgutfb.sHtML

[L04] 设置超时
来源：http://baike.zdbjq.cn/Article/details/gwsbiivza.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.zdbjq.cn/Article/details/gwjeoznta.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.zdbjq.cn/Article/details/gwmflbxbj.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.hesvh.cn/Article/details/gkexaxsar.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.fehbvm.com/Article/details/gzfdhgnlg.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.hesvh.cn/Article/details/gdtbllmqt.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.fehbvm.com/Article/details/gxriajtcq.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.zdbjq.cn/Article/details/gaawsyuhu.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.zdbjq.cn/Article/details/gywtvkmkh.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.fehbvm.com/Article/details/gisumwvop.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.fehbvm.com/Article/details/gysjycyhi.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.fehbvm.com/Article/details/gusfbnzdc.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.zdbjq.cn/Article/details/grbjgqowe.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.zdbjq.cn/Article/details/ginphiyoj.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.zdbjq.cn/Article/details/geqokimht.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.fehbvm.com/Article/details/gcrmoqooe.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.hesvh.cn/Article/details/gxlitywmr.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.zdbjq.cn/Article/details/ggovzccwy.sHtML

[L06] 解析响应为 JSON
来源：http://wap.hesvh.cn/Article/details/gkysmgkmj.sHtML

Py:   resp.json()
来源：http://read.share.fehbvm.com/Article/details/grdrsabci.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.fehbvm.com/Article/details/gxfcfgvtb.sHtML

JS:   await resp.json()
来源：http://www.m.share.zdbjq.cn/Article/details/glkscmvfx.sHtML

TS:   await resp.json()
来源：http://www.m.share.fehbvm.com/Article/details/grftjduie.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.fehbvm.com/Article/details/gaqnlbwsu.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.fehbvm.com/Article/details/grliuafnu.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.fehbvm.com/Article/details/gxewrgyll.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.fehbvm.com/Article/details/gotqplhnl.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.hesvh.cn/Article/details/gninykbyd.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.hesvh.cn/Article/details/guuoitxgr.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.zdbjq.cn/Article/details/gugufashf.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.zdbjq.cn/Article/details/gkwmluwtd.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.fehbvm.com/Article/details/gqvexozmv.sHtML

Java: resp.statusCode()
来源：http://m.share.fehbvm.com/Article/details/gdrxtgtud.sHtML

Go:   resp.StatusCode
来源：http://wap.hesvh.cn/Article/details/gqysppyjp.sHtML

Ruby: resp.code.to_i
来源：http://baike.fehbvm.com/Article/details/goeiazbpp.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.fehbvm.com/Article/details/gesypqflw.sHtML

[L08] 并发请求多个地址
来源：http://m.share.fehbvm.com/Article/details/gxyklcihg.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.fehbvm.com/Article/details/grofjbpzi.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.hesvh.cn/Article/details/gwpttaklk.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fehbvm.com/Article/details/gekvywhyu.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fehbvm.com/Article/details/gezxqzehp.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.hesvh.cn/Article/details/gemzdkfqr.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.fehbvm.com/Article/details/gxnqngmzj.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.hesvh.cn/Article/details/gyjopidfg.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.zdbjq.cn/Article/details/gfnsojiyn.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/grdtxaaxg.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.fehbvm.com/Article/details/grnagyqse.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/ghhbzcuya.sHtML

[M01] 读取命令行参数
来源：http://baike.hesvh.cn/Article/details/gqyqryhvf.sHtML

Py:   sys.argv[1:]
来源：http://read.share.zdbjq.cn/Article/details/gaamamisa.sHtML

PHP:  $argv;  $argc;
来源：http://baike.zdbjq.cn/Article/details/gypijmiil.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.fehbvm.com/Article/details/geimnrpnq.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.zdbjq.cn/Article/details/gyvmokjbq.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.zdbjq.cn/Article/details/gwtnbfzgm.sHtML

Go:   os.Args[1:]
来源：http://www.blog.zdbjq.cn/Article/details/gjsdndens.sHtML

Ruby: ARGV
来源：http://m.share.hesvh.cn/Article/details/goxzpxxic.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.zdbjq.cn/Article/details/gndmuirfa.sHtML

[M02] 读取环境变量
来源：http://www.blog.hesvh.cn/Article/details/gldjpgyxn.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.hesvh.cn/Article/details/gptzwuvss.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.fehbvm.com/Article/details/geeyjsfdd.sHtML

JS:   process.env.HOME
来源：http://www.m.share.zdbjq.cn/Article/details/grbzgsora.sHtML

TS:   process.env.HOME
来源：http://wap.hesvh.cn/Article/details/gqybfnrbk.sHtML

Java: System.getenv("HOME")
来源：http://blog.hesvh.cn/Article/details/gdnhfahtw.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.hesvh.cn/Article/details/gfkgmfhgl.sHtML

Ruby: ENV["HOME"]
来源：http://3g.zdbjq.cn/Article/details/gunvspcpc.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.zdbjq.cn/Article/details/gjaevwcqt.sHtML

[M03] 执行外部命令
来源：http://read.share.zdbjq.cn/Article/details/goojzyotj.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.zdbjq.cn/Article/details/gqowgsezr.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.hesvh.cn/Article/details/gxgfxporo.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.hesvh.cn/Article/details/gidphsbev.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.hesvh.cn/Article/details/gkhpnwzsp.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.zdbjq.cn/Article/details/gjkxfzjbd.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.fehbvm.com/Article/details/gogtjckuv.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.hesvh.cn/Article/details/gulrlucnz.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.fehbvm.com/Article/details/giexvcgpn.sHtML

[M04] 获取当前工作目录
来源：http://baike.zdbjq.cn/Article/details/gamygyozm.sHtML

Py:   os.getcwd()
来源：http://www.share.fehbvm.com/Article/details/guxoziywz.sHtML

PHP:  getcwd();
来源：http://baike.hesvh.cn/Article/details/gnsbpfgai.sHtML

JS:   process.cwd()
来源：http://read.share.hesvh.cn/Article/details/guyjbowml.sHtML

TS:   process.cwd()
来源：http://www.share.fehbvm.com/Article/details/gfynioyqn.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.zdbjq.cn/Article/details/gvniukjxk.sHtML

Go:   os.Getwd()
来源：http://www.blog.fehbvm.com/Article/details/gcjdhqptg.sHtML

Ruby: Dir.pwd
来源：http://www.blog.zdbjq.cn/Article/details/gzfkonlkq.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.zdbjq.cn/Article/details/gdqajptvl.sHtML

[M05] 设置退出码
来源：http://blog.hesvh.cn/Article/details/gqdewlfqz.sHtML

Py:   sys.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gvtmrepan.sHtML

PHP:  exit(1);
来源：http://www.blog.fehbvm.com/Article/details/gzyfrtggp.sHtML

JS:   process.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/goqtmwuep.sHtML

TS:   process.exit(1)
来源：http://www.share.hesvh.cn/Article/details/gfxgddqhq.sHtML

Java: System.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gkbwjprsn.sHtML

Go:   os.Exit(1)
来源：http://baike.fehbvm.com/Article/details/gjuqeoupk.sHtML

Ruby: exit 1
来源：http://www.m.share.zdbjq.cn/Article/details/ggcquawsx.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.hesvh.cn/Article/details/gbevvwzff.sHtML

[M06] 向标准错误输出
来源：http://wap.zdbjq.cn/Article/details/gqpmmiwph.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.zdbjq.cn/Article/details/ggfzmzrwo.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.hesvh.cn/Article/details/gevvupegx.sHtML

JS:   console.error("err")
来源：http://baike.fehbvm.com/Article/details/gqxubeasy.sHtML

TS:   console.error("err")
来源：http://wap.fehbvm.com/Article/details/gwsdwphrd.sHtML

Java: System.err.println("err")
来源：http://read.share.zdbjq.cn/Article/details/gjpdgcuak.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.hesvh.cn/Article/details/gjvmlplmz.sHtML

Ruby: warn "err"
来源：http://mobile.fehbvm.com/Article/details/gacbhevug.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.hesvh.cn/Article/details/gagtjmrzn.sHtML

[M07] 判断是否为主入口
来源：http://wap.fehbvm.com/Article/details/gxdxxbiva.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.fehbvm.com/Article/details/grryaiqgt.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.zdbjq.cn/Article/details/gmyrdutcw.sHtML

JS:   require.main === module
来源：http://mobile.hesvh.cn/Article/details/gamcconat.sHtML

TS:   require.main === module
来源：http://mobile.hesvh.cn/Article/details/gukxhdexw.sHtML

Java: public static void main(String[] args)
来源：http://blog.hesvh.cn/Article/details/gxmwoywpv.sHtML

Go:   func main()
来源：http://wap.zdbjq.cn/Article/details/giuhlknhq.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.fehbvm.com/Article/details/gxfcrxzzr.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.fehbvm.com/Article/details/gezfpwlrb.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.hesvh.cn/Article/details/gqlotfncc.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.fehbvm.com/Article/details/gyfjjylwg.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.fehbvm.com/Article/details/gazasgqls.sHtML

JS:   process.platform;  process.version
来源：http://3g.hesvh.cn/Article/details/glgzgfgqd.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.fehbvm.com/Article/details/gqtrddxzg.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.fehbvm.com/Article/details/goqnkshbj.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.fehbvm.com/Article/details/grobnjnxf.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.fehbvm.com/Article/details/gwwioziyx.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.zdbjq.cn/Article/details/gxgfqwshu.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gjbwlptvd.sHtML

N. 数据结构与算法
来源：http://www.share.fehbvm.com/Article/details/gqwcbzvsh.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gekbonxbi.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.hesvh.cn/Article/details/gigfwtvbi.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/ghlkpfszy.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.zdbjq.cn/Article/details/garvrbysc.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.hesvh.cn/Article/details/glvqgnbya.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.hesvh.cn/Article/details/grqaknian.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gaactywrs.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gflmumtkt.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.zdbjq.cn/Article/details/guzylufox.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.fehbvm.com/Article/details/gbephammc.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.zdbjq.cn/Article/details/gmnbhxmwu.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.fehbvm.com/Article/details/gpltnassg.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.fehbvm.com/Article/details/gityjmeff.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.hesvh.cn/Article/details/getwpqdto.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.zdbjq.cn/Article/details/gjumeobnc.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.hesvh.cn/Article/details/gihocasjj.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.hesvh.cn/Article/details/gzjnshimh.sHtML

Ruby: arr.sort
来源：http://3g.fehbvm.com/Article/details/ghadazhci.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.hesvh.cn/Article/details/gxudurgak.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.fehbvm.com/Article/details/gaekdfwmx.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.fehbvm.com/Article/details/gqvvjryir.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.zdbjq.cn/Article/details/gddjhtyso.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.fehbvm.com/Article/details/gbaskbgdh.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.zdbjq.cn/Article/details/gojtwjeoc.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.fehbvm.com/Article/details/gwaraydjf.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.zdbjq.cn/Article/details/grsnfjyfd.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.fehbvm.com/Article/details/gclnasekl.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.zdbjq.cn/Article/details/gvfrsaeqy.sHtML

[N04] 斐波那契数列
来源：http://www.blog.zdbjq.cn/Article/details/ggbzrquwn.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.hesvh.cn/Article/details/gysbcfztw.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.hesvh.cn/Article/details/grwizrssv.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.hesvh.cn/Article/details/gutvzzlsj.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.hesvh.cn/Article/details/gpbssrzps.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.fehbvm.com/Article/details/ggtkgolyq.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.zdbjq.cn/Article/details/gagiltfnk.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.zdbjq.cn/Article/details/glbpblmog.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/gywxtnmik.sHtML

[N05] 最大公约数
来源：http://www.share.zdbjq.cn/Article/details/guxkvllum.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.hesvh.cn/Article/details/gygidyhsh.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.zdbjq.cn/Article/details/gniiborbb.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.fehbvm.com/Article/details/gykyzfelm.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.fehbvm.com/Article/details/gqpvjmxkq.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.hesvh.cn/Article/details/grhaowcyd.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.zdbjq.cn/Article/details/gemqrliyn.sHtML

Ruby: a.gcd(b)
来源：http://baike.hesvh.cn/Article/details/guflcupqw.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.fehbvm.com/Article/details/gzxyzspcl.sHtML

[N06] 判断回文字符串
来源：http://3g.hesvh.cn/Article/details/gnxctjxnr.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.fehbvm.com/Article/details/gepycuiix.sHtML

PHP:  $s === strrev($s);
来源：http://blog.hesvh.cn/Article/details/geqjyahwd.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/gnrkappit.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/gmzfxkjwy.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.fehbvm.com/Article/details/gmbsvrrwx.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.fehbvm.com/Article/details/glpitiakr.sHtML

Ruby: s == s.reverse
来源：http://baike.zdbjq.cn/Article/details/gnifyxytm.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.hesvh.cn/Article/details/gxudleemw.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.hesvh.cn/Article/details/gkjjrvlyf.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.fehbvm.com/Article/details/gqpybcpon.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.zdbjq.cn/Article/details/gkugsbakg.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.zdbjq.cn/Article/details/gbnlwtina.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.fehbvm.com/Article/details/gteenclsz.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.hesvh.cn/Article/details/gmcaefvpx.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.zdbjq.cn/Article/details/guhbbbtxg.sHtML

Ruby: // 手写 Hash
来源：http://mobile.fehbvm.com/Article/details/gyycaatqy.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.zdbjq.cn/Article/details/ghqtagofa.sHtML

[N08] 生成全排列
来源：http://m.share.hesvh.cn/Article/details/gcxsuqrze.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.zdbjq.cn/Article/details/gmypdirym.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.fehbvm.com/Article/details/gneikdqfm.sHtML

JS:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gkvrshspf.sHtML

TS:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/ghbxtmsio.sHtML

Java: // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gflwhqpnb.sHtML

Go:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gilufrjhr.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.fehbvm.com/Article/details/grswrnbgs.sHtML

C#:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gmumwclso.sHtML

[N09] 栈与队列
来源：http://wap.hesvh.cn/Article/details/ggevpkitr.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.zdbjq.cn/Article/details/grvqxmvjj.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.zdbjq.cn/Article/details/gpctrutus.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.hesvh.cn/Article/details/glrxncsxr.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.zdbjq.cn/Article/details/gjzjmgztp.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.zdbjq.cn/Article/details/gwojgjtrt.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.hesvh.cn/Article/details/gcjfahyxr.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.fehbvm.com/Article/details/geryqpezq.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.fehbvm.com/Article/details/ghevnvlkz.sHtML

[N10] 链表节点定义
来源：http://www.share.fehbvm.com/Article/details/gslmudvvm.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.fehbvm.com/Article/details/gyeypzjne.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.fehbvm.com/Article/details/gvluwezqg.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.hesvh.cn/Article/details/gctlsaswb.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.zdbjq.cn/Article/details/gkpdjnwlp.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.fehbvm.com/Article/details/gxydfyweg.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.hesvh.cn/Article/details/gezmtdawc.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.zdbjq.cn/Article/details/gsssejuha.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.hesvh.cn/Article/details/gdekbqpaw.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.zdbjq.cn/Article/details/gysguvtzj.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.hesvh.cn/Article/details/gejspydhe.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.fehbvm.com/Article/details/gukmwziro.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.hesvh.cn/Article/details/gzrmvalix.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.fehbvm.com/Article/details/gsqeuxdap.sHtML

Java: // 手写递归
来源：http://wap.fehbvm.com/Article/details/ggtzxweox.sHtML

Go:   // 手写递归
来源：http://3g.fehbvm.com/Article/details/gafggkkol.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.fehbvm.com/Article/details/gpnfcneuk.sHtML

C#:   // 手写递归
来源：http://3g.fehbvm.com/Article/details/gmfhuyrij.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.zdbjq.cn/Article/details/gbefuabfs.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.hesvh.cn/Article/details/gemupjqjk.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.fehbvm.com/Article/details/ggsxlpgjm.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.zdbjq.cn/Article/details/gaecsbezn.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.fehbvm.com/Article/details/gxvymugex.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.fehbvm.com/Article/details/gzhswpplf.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.zdbjq.cn/Article/details/gbczgbtbd.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.hesvh.cn/Article/details/ggfhiigyv.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.zdbjq.cn/Article/details/gegqouavr.sHtML


<!-- 参考信息 -->