代发 wailian999

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.fehbvm.com/Article/details/gvcvgmhxw.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.blog.zdbjq.cn/Article/details/gdqdmetmt.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wap.zdbjq.cn/Article/details/gvkwhgzse.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.m.share.zdbjq.cn/Article/details/grhxplxwe.sHtML

[K06] 解析 URL 查询串
来源：http://blog.zdbjq.cn/Article/details/giqyookwr.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://baike.zdbjq.cn/Article/details/gypxnyhmn.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://read.share.hesvh.cn/Article/details/gnujzywll.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.hesvh.cn/Article/details/gmcfiyrvv.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.zdbjq.cn/Article/details/gpbhsnupe.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.zdbjq.cn/Article/details/gkqasyfpy.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://wap.hesvh.cn/Article/details/geygurmir.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.zdbjq.cn/Article/details/gzrziftwl.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://baike.zdbjq.cn/Article/details/ghdgnohac.sHtML

[K07] 进制转换
来源：http://mobile.zdbjq.cn/Article/details/grbwjibft.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.zdbjq.cn/Article/details/ghksvupxq.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.m.share.zdbjq.cn/Article/details/gfuiwyhsg.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://baike.hesvh.cn/Article/details/gmczpqceq.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://baike.hesvh.cn/Article/details/gvxsqlkqn.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.m.share.zdbjq.cn/Article/details/gphzlvzeg.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.m.share.zdbjq.cn/Article/details/gidtzwfhb.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.zdbjq.cn/Article/details/gjayzsamv.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.share.zdbjq.cn/Article/details/glsektdgh.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.share.hesvh.cn/Article/details/goealypom.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/glmfuyvea.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gqbmkfveb.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.zdbjq.cn/Article/details/gbbuyryjp.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.fehbvm.com/Article/details/guixwtqrn.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.hesvh.cn/Article/details/gkyabqzbl.sHtML

Go:   encoding/gob
来源：http://wap.fehbvm.com/Article/details/geikkewie.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.zdbjq.cn/Article/details/gnqfhjmrx.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.fehbvm.com/Article/details/gkgwqgjwe.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gfprhdjzn.sHtML

L. 网络请求
来源：http://www.m.share.fehbvm.com/Article/details/gyylronad.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gxfhjnacp.sHtML

[L01] 发送 GET 请求
来源：http://wap.hesvh.cn/Article/details/gzmmsbcoc.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.hesvh.cn/Article/details/grbzxlxqe.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.zdbjq.cn/Article/details/gkqomzgqc.sHtML

JS:   await fetch(url)
来源：http://read.share.hesvh.cn/Article/details/gozgtthsi.sHtML

TS:   await fetch(url)
来源：http://www.blog.zdbjq.cn/Article/details/gaamyqolx.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.hesvh.cn/Article/details/glfevvsrj.sHtML

Go:   resp, err := http.Get(url)
来源：http://mobile.hesvh.cn/Article/details/gixttpklb.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.hesvh.cn/Article/details/gxkfjjhxe.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.hesvh.cn/Article/details/gmcqxcxby.sHtML

[L02] 发送 POST JSON
来源：http://mobile.fehbvm.com/Article/details/gnlrrhphu.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://read.share.zdbjq.cn/Article/details/gdwrcdltr.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.zdbjq.cn/Article/details/gqfaetlsb.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.zdbjq.cn/Article/details/gxroyalnr.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.zdbjq.cn/Article/details/ghfavycuz.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.zdbjq.cn/Article/details/gfizioifo.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.zdbjq.cn/Article/details/gknbzcbhm.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.zdbjq.cn/Article/details/ggmhqgang.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.fehbvm.com/Article/details/gvsvpgpdf.sHtML

[L03] 设置自定义请求头
来源：http://baike.zdbjq.cn/Article/details/ggtzggebc.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.hesvh.cn/Article/details/gcatgdaad.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.hesvh.cn/Article/details/gsfeqvpol.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.fehbvm.com/Article/details/gtftlrjhh.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.zdbjq.cn/Article/details/gevganovy.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.fehbvm.com/Article/details/goqqivgkg.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.zdbjq.cn/Article/details/gxfwpvrhj.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.zdbjq.cn/Article/details/gtetaiiet.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.hesvh.cn/Article/details/gipwxizdp.sHtML

[L04] 设置超时
来源：http://baike.fehbvm.com/Article/details/gqajxwffh.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.zdbjq.cn/Article/details/grxtohwwj.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.hesvh.cn/Article/details/gxvmajiix.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.hesvh.cn/Article/details/gmsbifuni.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.zdbjq.cn/Article/details/gefwfxubw.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.hesvh.cn/Article/details/gmyijedta.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.zdbjq.cn/Article/details/gcittjhmh.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.fehbvm.com/Article/details/girsoudxu.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.zdbjq.cn/Article/details/gyiofsjrr.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.fehbvm.com/Article/details/gtfjqbhcc.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.hesvh.cn/Article/details/gmttjeoul.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.fehbvm.com/Article/details/ghihvglof.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blog.hesvh.cn/Article/details/gohxqgklx.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.hesvh.cn/Article/details/gpivwceje.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.hesvh.cn/Article/details/ghfocoyju.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.fehbvm.com/Article/details/gzuiicdpu.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.fehbvm.com/Article/details/gpcockuco.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gqvmchukl.sHtML

[L06] 解析响应为 JSON
来源：http://3g.hesvh.cn/Article/details/grinwnlmu.sHtML

Py:   resp.json()
来源：http://baike.hesvh.cn/Article/details/gexxavmxb.sHtML

PHP:  json_decode($body, true);
来源：http://3g.fehbvm.com/Article/details/gezdytegu.sHtML

JS:   await resp.json()
来源：http://www.share.zdbjq.cn/Article/details/gxmgzxkbq.sHtML

TS:   await resp.json()
来源：http://www.m.share.zdbjq.cn/Article/details/gzrkbnzvr.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.zdbjq.cn/Article/details/gcczvrsdx.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.zdbjq.cn/Article/details/gefbexxil.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.hesvh.cn/Article/details/gvhawrher.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.zdbjq.cn/Article/details/gybsilngb.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.zdbjq.cn/Article/details/gyuoduuch.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.hesvh.cn/Article/details/gphchilti.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.zdbjq.cn/Article/details/goqxdsido.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.hesvh.cn/Article/details/gyvacryng.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.hesvh.cn/Article/details/gntjuapmz.sHtML

Java: resp.statusCode()
来源：http://www.m.share.hesvh.cn/Article/details/ghmwbaami.sHtML

Go:   resp.StatusCode
来源：http://www.share.fehbvm.com/Article/details/gvpswxqnx.sHtML

Ruby: resp.code.to_i
来源：http://read.share.zdbjq.cn/Article/details/gqjjgekgv.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.zdbjq.cn/Article/details/gujnbwigh.sHtML

[L08] 并发请求多个地址
来源：http://baike.hesvh.cn/Article/details/gtdtemzzu.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.fehbvm.com/Article/details/gcuxitzlp.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.hesvh.cn/Article/details/gnjsldple.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.hesvh.cn/Article/details/gxdkpwnxy.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fehbvm.com/Article/details/garzihzux.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.fehbvm.com/Article/details/gbjxvkckf.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.fehbvm.com/Article/details/gnlwpdtut.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.fehbvm.com/Article/details/gaaydimkf.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.zdbjq.cn/Article/details/gbggveemt.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gvgxotycc.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.zdbjq.cn/Article/details/gplescdpe.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gdntoghux.sHtML

[M01] 读取命令行参数
来源：http://wap.zdbjq.cn/Article/details/gblsfcqpd.sHtML

Py:   sys.argv[1:]
来源：http://baike.fehbvm.com/Article/details/gdckwktrz.sHtML

PHP:  $argv;  $argc;
来源：http://wap.zdbjq.cn/Article/details/ginusftuv.sHtML

JS:   process.argv.slice(2)
来源：http://3g.hesvh.cn/Article/details/gktwmvexj.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.zdbjq.cn/Article/details/gposghvcg.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.fehbvm.com/Article/details/gciflssbo.sHtML

Go:   os.Args[1:]
来源：http://read.share.fehbvm.com/Article/details/gqpkjkolh.sHtML

Ruby: ARGV
来源：http://read.share.zdbjq.cn/Article/details/gjlfnwger.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.hesvh.cn/Article/details/gavsqsxnz.sHtML

[M02] 读取环境变量
来源：http://baike.zdbjq.cn/Article/details/gdyghumth.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.fehbvm.com/Article/details/gefqvtyug.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.zdbjq.cn/Article/details/gnxrmgzny.sHtML

JS:   process.env.HOME
来源：http://www.share.zdbjq.cn/Article/details/gyqbrstxx.sHtML

TS:   process.env.HOME
来源：http://www.blog.zdbjq.cn/Article/details/gieqzvbvd.sHtML

Java: System.getenv("HOME")
来源：http://read.share.fehbvm.com/Article/details/gkmrtbavi.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.hesvh.cn/Article/details/grpsrhqeh.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.fehbvm.com/Article/details/gmqnvezir.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/gqjpcicwz.sHtML

[M03] 执行外部命令
来源：http://m.share.hesvh.cn/Article/details/gubdahouw.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.fehbvm.com/Article/details/gowaxeswb.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.fehbvm.com/Article/details/gqwujrvwo.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.fehbvm.com/Article/details/gqjngfgqe.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.fehbvm.com/Article/details/gvlfklzfk.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.fehbvm.com/Article/details/gqyaldgpl.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.fehbvm.com/Article/details/gyiosqgpx.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.fehbvm.com/Article/details/girxdphwo.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.zdbjq.cn/Article/details/gtxbkybwn.sHtML

[M04] 获取当前工作目录
来源：http://baike.hesvh.cn/Article/details/gfkvoukoc.sHtML

Py:   os.getcwd()
来源：http://mobile.zdbjq.cn/Article/details/gfiaaddqc.sHtML

PHP:  getcwd();
来源：http://baike.fehbvm.com/Article/details/gmjjkkbov.sHtML

JS:   process.cwd()
来源：http://www.share.zdbjq.cn/Article/details/gostsvdiq.sHtML

TS:   process.cwd()
来源：http://blog.zdbjq.cn/Article/details/gpsvfcvdh.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.hesvh.cn/Article/details/gylvbdmqt.sHtML

Go:   os.Getwd()
来源：http://mobile.fehbvm.com/Article/details/gwvwywxtd.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.hesvh.cn/Article/details/gjizcfbcz.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.zdbjq.cn/Article/details/ghdcaamgu.sHtML

[M05] 设置退出码
来源：http://www.share.hesvh.cn/Article/details/gzdpismcb.sHtML

Py:   sys.exit(1)
来源：http://blog.fehbvm.com/Article/details/gfuvelhrl.sHtML

PHP:  exit(1);
来源：http://baike.zdbjq.cn/Article/details/grbvnjfgk.sHtML

JS:   process.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gvhgzpatt.sHtML

TS:   process.exit(1)
来源：http://m.share.hesvh.cn/Article/details/gnpvlvgmv.sHtML

Java: System.exit(1)
来源：http://baike.hesvh.cn/Article/details/gmfrsyjio.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gofnozfgp.sHtML

Ruby: exit 1
来源：http://3g.hesvh.cn/Article/details/glnwkurmk.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.hesvh.cn/Article/details/gtcvhbbex.sHtML

[M06] 向标准错误输出
来源：http://www.blog.hesvh.cn/Article/details/gvzrpiwkd.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.zdbjq.cn/Article/details/gteopytrp.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.fehbvm.com/Article/details/grbmdqnrp.sHtML

JS:   console.error("err")
来源：http://baike.fehbvm.com/Article/details/glzqhvutr.sHtML

TS:   console.error("err")
来源：http://3g.fehbvm.com/Article/details/gmsxotdzp.sHtML

Java: System.err.println("err")
来源：http://mobile.zdbjq.cn/Article/details/glqehgvpr.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.hesvh.cn/Article/details/gbwrigomt.sHtML

Ruby: warn "err"
来源：http://www.blog.zdbjq.cn/Article/details/grefpowha.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.zdbjq.cn/Article/details/gbdnnxpny.sHtML

[M07] 判断是否为主入口
来源：http://blog.zdbjq.cn/Article/details/gsvylsvor.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.zdbjq.cn/Article/details/gcyvelahx.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.zdbjq.cn/Article/details/gfcivdktn.sHtML

JS:   require.main === module
来源：http://3g.fehbvm.com/Article/details/gngsqacsh.sHtML

TS:   require.main === module
来源：http://mobile.hesvh.cn/Article/details/gkuuezlgh.sHtML

Java: public static void main(String[] args)
来源：http://read.share.fehbvm.com/Article/details/gvbolsyah.sHtML

Go:   func main()
来源：http://3g.fehbvm.com/Article/details/gzvwwtipi.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.zdbjq.cn/Article/details/givbsbppx.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.fehbvm.com/Article/details/grrawvbrb.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.hesvh.cn/Article/details/giyljsdon.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.hesvh.cn/Article/details/gbjnlsupn.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.fehbvm.com/Article/details/gfksqznnd.sHtML

JS:   process.platform;  process.version
来源：http://blog.hesvh.cn/Article/details/geiteueff.sHtML

TS:   process.platform;  process.version
来源：http://mobile.hesvh.cn/Article/details/garksjfyt.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.zdbjq.cn/Article/details/gyebbljxz.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.zdbjq.cn/Article/details/gbnurosgm.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.fehbvm.com/Article/details/gkbpxlyae.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.fehbvm.com/Article/details/gmkuwbvtt.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gsszbvjwb.sHtML

N. 数据结构与算法
来源：http://www.blog.hesvh.cn/Article/details/gychbnljp.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gynhcbpan.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.fehbvm.com/Article/details/gccfbkfbq.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gmnfqojck.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.hesvh.cn/Article/details/grsexezgm.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.hesvh.cn/Article/details/gjilkjrip.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.hesvh.cn/Article/details/giwcdjhet.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.fehbvm.com/Article/details/guvobkunx.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gofxxluuu.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.zdbjq.cn/Article/details/gjsanhmww.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.hesvh.cn/Article/details/gwkdbpygp.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.hesvh.cn/Article/details/gwqkbgbtc.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.zdbjq.cn/Article/details/gkynwydrs.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.fehbvm.com/Article/details/gvqmlwpms.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.zdbjq.cn/Article/details/gnbgrwimk.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.hesvh.cn/Article/details/gcxzlkijt.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.fehbvm.com/Article/details/gvdeofsoy.sHtML

Go:   slices.Sort(arr)
来源：http://3g.fehbvm.com/Article/details/gcfqpxhue.sHtML

Ruby: arr.sort
来源：http://www.m.share.fehbvm.com/Article/details/gyfhggdpv.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.zdbjq.cn/Article/details/gtopczyap.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.hesvh.cn/Article/details/gerdkcebp.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.hesvh.cn/Article/details/gnhwcnhdd.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.fehbvm.com/Article/details/ggpukrbxe.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.hesvh.cn/Article/details/gxgfnosdo.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.hesvh.cn/Article/details/gdaltihas.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.fehbvm.com/Article/details/gdfhbnakl.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.zdbjq.cn/Article/details/gjqpqpxku.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.zdbjq.cn/Article/details/gyozjborf.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.hesvh.cn/Article/details/gelkawyct.sHtML

[N04] 斐波那契数列
来源：http://baike.zdbjq.cn/Article/details/gbazgfvxq.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.zdbjq.cn/Article/details/gukolhbfh.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.hesvh.cn/Article/details/giylxbpla.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/gmnalluwb.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.hesvh.cn/Article/details/glkqdgbyf.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.fehbvm.com/Article/details/gzfsumzqq.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.fehbvm.com/Article/details/gdlvflahx.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.hesvh.cn/Article/details/gswnjjsjm.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.zdbjq.cn/Article/details/gabkclctg.sHtML

[N05] 最大公约数
来源：http://wap.hesvh.cn/Article/details/ghpvzakox.sHtML

Py:   math.gcd(a, b)
来源：http://wap.fehbvm.com/Article/details/gfexxsqto.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.hesvh.cn/Article/details/gsytpodvl.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.fehbvm.com/Article/details/gfzwkavjj.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.fehbvm.com/Article/details/gdeufizoa.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.hesvh.cn/Article/details/gnipftizz.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.zdbjq.cn/Article/details/gajnccqzt.sHtML

Ruby: a.gcd(b)
来源：http://3g.hesvh.cn/Article/details/gpapqsorn.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.fehbvm.com/Article/details/gptlgspuk.sHtML

[N06] 判断回文字符串
来源：http://blog.zdbjq.cn/Article/details/gupaiclge.sHtML

Py:   s == s[::-1]
来源：http://blog.hesvh.cn/Article/details/gmznqoxvs.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.fehbvm.com/Article/details/gwnsddtrz.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/gnxqjjxvr.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/gnwjedfmm.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.hesvh.cn/Article/details/goqnspwgp.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.fehbvm.com/Article/details/gtwhnsxcr.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.fehbvm.com/Article/details/gvdhqznsr.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.hesvh.cn/Article/details/gxhczftnt.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.zdbjq.cn/Article/details/gptouuatr.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.fehbvm.com/Article/details/gvswsknat.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.hesvh.cn/Article/details/gxpkgxjmg.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.zdbjq.cn/Article/details/gzrmkisvf.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.zdbjq.cn/Article/details/giyckymiq.sHtML

Java: // 手写 HashMap
来源：http://www.share.zdbjq.cn/Article/details/goeshrwlo.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.hesvh.cn/Article/details/giduonzxn.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.fehbvm.com/Article/details/gakjyddyy.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.hesvh.cn/Article/details/gzvxivaib.sHtML

[N08] 生成全排列
来源：http://www.m.share.zdbjq.cn/Article/details/gcmmulkso.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.fehbvm.com/Article/details/gumpuzbii.sHtML

PHP:  // 手写递归交换
来源：http://wap.fehbvm.com/Article/details/grnsgpcsz.sHtML

JS:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/guaserizo.sHtML

TS:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/goewccura.sHtML

Java: // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gdxoljabd.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gkzqwupkb.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.fehbvm.com/Article/details/gijbdedcj.sHtML

C#:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/grvqkhuzc.sHtML

[N09] 栈与队列
来源：http://wap.zdbjq.cn/Article/details/gdvxdklhg.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.zdbjq.cn/Article/details/geiwbauux.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.hesvh.cn/Article/details/gurinajty.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.hesvh.cn/Article/details/gngxrtpok.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.zdbjq.cn/Article/details/gticrscdr.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.zdbjq.cn/Article/details/gmmttwmpx.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.hesvh.cn/Article/details/gutljufgm.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.hesvh.cn/Article/details/gmwuohecd.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.fehbvm.com/Article/details/gccpttstc.sHtML

[N10] 链表节点定义
来源：http://www.blog.hesvh.cn/Article/details/gssoxyotx.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.hesvh.cn/Article/details/gevzuvgkj.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.fehbvm.com/Article/details/gnqkmjfpi.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.hesvh.cn/Article/details/gfvycrxhk.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.fehbvm.com/Article/details/gbujbjvym.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.hesvh.cn/Article/details/goioptzqw.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.hesvh.cn/Article/details/gpvdjposy.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.fehbvm.com/Article/details/gzeunncuy.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.hesvh.cn/Article/details/ggzsnywph.sHtML

[N11] 二叉树中序遍历
来源：http://3g.fehbvm.com/Article/details/gvgjniuyo.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.hesvh.cn/Article/details/gpckowlwb.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.zdbjq.cn/Article/details/gnnrfkixq.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.hesvh.cn/Article/details/ggbmurghy.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.fehbvm.com/Article/details/gxdprinmf.sHtML

Java: // 手写递归
来源：http://mobile.hesvh.cn/Article/details/ggbdmubji.sHtML

Go:   // 手写递归
来源：http://www.blog.zdbjq.cn/Article/details/gzdkpkzvr.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.fehbvm.com/Article/details/gnxubzqzz.sHtML

C#:   // 手写递归
来源：http://www.share.hesvh.cn/Article/details/gpqdkifie.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.fehbvm.com/Article/details/gturkpdrr.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.zdbjq.cn/Article/details/gekwyomii.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.zdbjq.cn/Article/details/gloyinucd.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.hesvh.cn/Article/details/gqakvvabl.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.hesvh.cn/Article/details/gllnszdea.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.zdbjq.cn/Article/details/gqepzxqol.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.fehbvm.com/Article/details/gpxzytksy.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.zdbjq.cn/Article/details/gkuehjqwo.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.hesvh.cn/Article/details/gjqmnamlp.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/ghhbbcrqw.sHtML

O. 并发与异步
来源：http://www.blog.zdbjq.cn/Article/details/gidqjsdrn.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gxoftvrjz.sHtML

[O01] 启动一个线程
来源：http://3g.zdbjq.cn/Article/details/gfevrhqel.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.fehbvm.com/Article/details/ghbbhwxoi.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.hesvh.cn/Article/details/gijtyaksf.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.zdbjq.cn/Article/details/gxubjldfh.sHtML

TS:   // 同 JS
来源：http://www.blog.fehbvm.com/Article/details/grhpbetvv.sHtML


<!-- 参考信息 -->