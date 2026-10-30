代发 wailian999

Py:   copy.deepcopy(obj)
来源：http://www.share.fehbvm.com/Article/details/geugmhgkl.sHtML

PHP:  unserialize(serialize($obj));
来源：http://3g.fehbvm.com/Article/details/gsmzvmzch.sHtML

JS:   structuredClone(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gfyvhwdfq.sHtML

TS:   structuredClone(obj)
来源：http://mobile.zdbjq.cn/Article/details/gwkkhkuhz.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.blog.hesvh.cn/Article/details/gzzhzhqts.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.fehbvm.com/Article/details/gvopfipdt.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://m.share.hesvh.cn/Article/details/gaxatlpjg.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://blog.fehbvm.com/Article/details/gfttcodti.sHtML

[K06] 解析 URL 查询串
来源：http://www.m.share.hesvh.cn/Article/details/gsezatvpj.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.blog.hesvh.cn/Article/details/gfuyokcbo.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.m.share.hesvh.cn/Article/details/gmxydjjga.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.fehbvm.com/Article/details/gxrgrnych.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.zdbjq.cn/Article/details/gygzjjkla.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.share.fehbvm.com/Article/details/gvuustscn.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://read.share.fehbvm.com/Article/details/gudeawbnp.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mobile.fehbvm.com/Article/details/grrmydess.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.hesvh.cn/Article/details/gpwdujtju.sHtML

[K07] 进制转换
来源：http://blog.fehbvm.com/Article/details/gwdkjpizm.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.fehbvm.com/Article/details/gkltbhvqx.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://blog.zdbjq.cn/Article/details/gxtfpamfq.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mobile.zdbjq.cn/Article/details/guzqvgnol.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://3g.zdbjq.cn/Article/details/ggamlxmsb.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.share.hesvh.cn/Article/details/gfzjpbfkf.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.fehbvm.com/Article/details/ghatmsxzt.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.zdbjq.cn/Article/details/gjijzecvz.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.zdbjq.cn/Article/details/ggkabqqcz.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.blog.fehbvm.com/Article/details/gqhwoqasv.sHtML

Py:   pickle.dumps(obj)
来源：http://www.blog.hesvh.cn/Article/details/gljqjvoyy.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://wap.fehbvm.com/Article/details/gvpkfmazu.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.fehbvm.com/Article/details/gszadkeyc.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://read.share.fehbvm.com/Article/details/glzicqzba.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.m.share.hesvh.cn/Article/details/gyfmvmovm.sHtML

Go:   encoding/gob
来源：http://m.share.zdbjq.cn/Article/details/gpijthjee.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.hesvh.cn/Article/details/gksqmjiul.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.fehbvm.com/Article/details/gioqoyhlg.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gvzddjwci.sHtML

L. 网络请求
来源：http://www.m.share.fehbvm.com/Article/details/gvlxgmuuz.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gifczmlwo.sHtML

[L01] 发送 GET 请求
来源：http://www.share.zdbjq.cn/Article/details/gfaweutlj.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://blog.hesvh.cn/Article/details/gzqwrawrf.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.hesvh.cn/Article/details/gnowawnle.sHtML

JS:   await fetch(url)
来源：http://www.blog.fehbvm.com/Article/details/gkrlwetpa.sHtML

TS:   await fetch(url)
来源：http://www.blog.zdbjq.cn/Article/details/gsnbkxbny.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.hesvh.cn/Article/details/gelrjpoaf.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.fehbvm.com/Article/details/gwinxxgoc.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.zdbjq.cn/Article/details/gwpjfaocv.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.zdbjq.cn/Article/details/gwlkjdhen.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.hesvh.cn/Article/details/gvfcmxuiu.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.hesvh.cn/Article/details/gsxejikya.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://m.share.hesvh.cn/Article/details/ggsfmpdvn.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.zdbjq.cn/Article/details/gfnoczgcq.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.hesvh.cn/Article/details/gfxeeeshi.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.hesvh.cn/Article/details/globkfozv.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.fehbvm.com/Article/details/gmzpnrtwg.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://blog.zdbjq.cn/Article/details/gujlmwszt.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.hesvh.cn/Article/details/gnrzqtnzg.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.hesvh.cn/Article/details/gytdlvncp.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://read.share.hesvh.cn/Article/details/gqfgtdevg.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.blog.hesvh.cn/Article/details/gxzyzyono.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.hesvh.cn/Article/details/gjykshkwl.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.zdbjq.cn/Article/details/gkutvtgme.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.fehbvm.com/Article/details/gjsbidbsj.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.zdbjq.cn/Article/details/gbzwvxhnf.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.zdbjq.cn/Article/details/gkuhjvxqb.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.fehbvm.com/Article/details/gcsscakxz.sHtML

[L04] 设置超时
来源：http://www.share.fehbvm.com/Article/details/gsjdbzfph.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.fehbvm.com/Article/details/gqhydbywm.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.hesvh.cn/Article/details/guafkljaw.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.hesvh.cn/Article/details/gaeltvhdf.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.fehbvm.com/Article/details/giushvrxk.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.hesvh.cn/Article/details/ghxxgojlm.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.zdbjq.cn/Article/details/gnjdnnubm.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.hesvh.cn/Article/details/gfzwispit.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.hesvh.cn/Article/details/gdwcclkqi.sHtML

[L05] 上传文件（multipart）
来源：http://3g.zdbjq.cn/Article/details/gvvdvgdem.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://read.share.fehbvm.com/Article/details/gepfvvxln.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.hesvh.cn/Article/details/gfhjfgfnw.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.zdbjq.cn/Article/details/gspaxdvdx.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.fehbvm.com/Article/details/gfvbjtdcp.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.hesvh.cn/Article/details/glpweogqf.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.fehbvm.com/Article/details/gkfnqfckj.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.hesvh.cn/Article/details/ganzphfdv.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gpidhutcv.sHtML

[L06] 解析响应为 JSON
来源：http://wap.hesvh.cn/Article/details/gkfrgdnsm.sHtML

Py:   resp.json()
来源：http://3g.zdbjq.cn/Article/details/gomdvzpag.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.zdbjq.cn/Article/details/gjtogzpdw.sHtML

JS:   await resp.json()
来源：http://www.m.share.zdbjq.cn/Article/details/ghpcuohlp.sHtML

TS:   await resp.json()
来源：http://www.m.share.hesvh.cn/Article/details/glcvzaluc.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.zdbjq.cn/Article/details/gejqcougv.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.hesvh.cn/Article/details/gcupuimes.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.fehbvm.com/Article/details/gtgigaamu.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.zdbjq.cn/Article/details/gvevmldeh.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.zdbjq.cn/Article/details/gifagwwfq.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.fehbvm.com/Article/details/gmotyladz.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.zdbjq.cn/Article/details/goejpiomm.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.fehbvm.com/Article/details/genupouyj.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.hesvh.cn/Article/details/gdahclltc.sHtML

Java: resp.statusCode()
来源：http://wap.fehbvm.com/Article/details/grgsnmrbg.sHtML

Go:   resp.StatusCode
来源：http://www.share.fehbvm.com/Article/details/gfvejqlbn.sHtML

Ruby: resp.code.to_i
来源：http://m.share.zdbjq.cn/Article/details/gfvfxxoxq.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.zdbjq.cn/Article/details/gblkfvwvy.sHtML

[L08] 并发请求多个地址
来源：http://read.share.fehbvm.com/Article/details/gdsgyzvyy.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.zdbjq.cn/Article/details/gqwfxsbuu.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.hesvh.cn/Article/details/gsniexbjf.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.zdbjq.cn/Article/details/gyebynfck.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.zdbjq.cn/Article/details/gjebqtdlp.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.zdbjq.cn/Article/details/gaofmzvkj.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.fehbvm.com/Article/details/gvpselhwa.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.zdbjq.cn/Article/details/gdveqaprk.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.zdbjq.cn/Article/details/gdfrhxuay.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gbsjminni.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.zdbjq.cn/Article/details/gdfkbfjzd.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gnulpuwpr.sHtML

[M01] 读取命令行参数
来源：http://mobile.hesvh.cn/Article/details/gsrxlixop.sHtML

Py:   sys.argv[1:]
来源：http://read.share.zdbjq.cn/Article/details/glmlsxban.sHtML

PHP:  $argv;  $argc;
来源：http://wap.zdbjq.cn/Article/details/glsrljiiq.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.fehbvm.com/Article/details/ghrdrmbky.sHtML

TS:   process.argv.slice(2)
来源：http://blog.fehbvm.com/Article/details/gbweljiag.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.hesvh.cn/Article/details/gggvatajz.sHtML

Go:   os.Args[1:]
来源：http://mobile.zdbjq.cn/Article/details/gpcgavbmt.sHtML

Ruby: ARGV
来源：http://baike.zdbjq.cn/Article/details/gvigkikfi.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.hesvh.cn/Article/details/ghltvniar.sHtML

[M02] 读取环境变量
来源：http://www.blog.zdbjq.cn/Article/details/ghnrsyxoo.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/grtuupscd.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.hesvh.cn/Article/details/gfaozxoan.sHtML

JS:   process.env.HOME
来源：http://www.m.share.zdbjq.cn/Article/details/gkucrugzm.sHtML

TS:   process.env.HOME
来源：http://blog.fehbvm.com/Article/details/gcbttfufu.sHtML

Java: System.getenv("HOME")
来源：http://mobile.hesvh.cn/Article/details/gchwmvopb.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/gsrkstwbo.sHtML

Ruby: ENV["HOME"]
来源：http://baike.fehbvm.com/Article/details/gvaxoggex.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.zdbjq.cn/Article/details/gontmxnsw.sHtML

[M03] 执行外部命令
来源：http://read.share.hesvh.cn/Article/details/gqslqttus.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.hesvh.cn/Article/details/grjiqltlt.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.zdbjq.cn/Article/details/gexoqhvsz.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.zdbjq.cn/Article/details/gqybphacj.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.fehbvm.com/Article/details/gqdeqkyji.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.zdbjq.cn/Article/details/glcazbcqo.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.hesvh.cn/Article/details/gnsbaoenq.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.hesvh.cn/Article/details/gpllcmznv.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.fehbvm.com/Article/details/gunbjozzj.sHtML

[M04] 获取当前工作目录
来源：http://baike.hesvh.cn/Article/details/gdosadjku.sHtML

Py:   os.getcwd()
来源：http://read.share.zdbjq.cn/Article/details/gdbqkeioq.sHtML

PHP:  getcwd();
来源：http://m.share.fehbvm.com/Article/details/gesudufwu.sHtML

JS:   process.cwd()
来源：http://3g.hesvh.cn/Article/details/gyrgjwnvx.sHtML

TS:   process.cwd()
来源：http://wap.fehbvm.com/Article/details/gbbgzuyzq.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.zdbjq.cn/Article/details/gtgcoqflw.sHtML

Go:   os.Getwd()
来源：http://www.share.hesvh.cn/Article/details/gjydiosva.sHtML

Ruby: Dir.pwd
来源：http://blog.zdbjq.cn/Article/details/gpydvqldr.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.fehbvm.com/Article/details/gwveyaype.sHtML

[M05] 设置退出码
来源：http://read.share.hesvh.cn/Article/details/gamhstjgo.sHtML

Py:   sys.exit(1)
来源：http://www.share.fehbvm.com/Article/details/geendlwiq.sHtML

PHP:  exit(1);
来源：http://read.share.fehbvm.com/Article/details/gsspdrxbu.sHtML

JS:   process.exit(1)
来源：http://wap.zdbjq.cn/Article/details/gjdrtvivi.sHtML

TS:   process.exit(1)
来源：http://wap.fehbvm.com/Article/details/gbrqlpvbl.sHtML

Java: System.exit(1)
来源：http://mobile.fehbvm.com/Article/details/gsrxducum.sHtML

Go:   os.Exit(1)
来源：http://www.share.zdbjq.cn/Article/details/ghutffpdj.sHtML

Ruby: exit 1
来源：http://3g.zdbjq.cn/Article/details/gkbxelsmm.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.fehbvm.com/Article/details/ghutupbxh.sHtML

[M06] 向标准错误输出
来源：http://read.share.fehbvm.com/Article/details/gxuiuptzd.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.fehbvm.com/Article/details/gpekookkw.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.hesvh.cn/Article/details/gejugqybz.sHtML

JS:   console.error("err")
来源：http://read.share.hesvh.cn/Article/details/gvzyxvleh.sHtML

TS:   console.error("err")
来源：http://www.blog.zdbjq.cn/Article/details/gwausxvfz.sHtML

Java: System.err.println("err")
来源：http://www.share.hesvh.cn/Article/details/gaimlbeoi.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.zdbjq.cn/Article/details/gvydnlogo.sHtML

Ruby: warn "err"
来源：http://mobile.fehbvm.com/Article/details/gfvvrvovc.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.hesvh.cn/Article/details/gxfkyxqoh.sHtML

[M07] 判断是否为主入口
来源：http://m.share.hesvh.cn/Article/details/gtggfgejg.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.hesvh.cn/Article/details/gfmwwewaj.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.zdbjq.cn/Article/details/gextdgsbw.sHtML

JS:   require.main === module
来源：http://www.blog.zdbjq.cn/Article/details/gvuulbxbw.sHtML

TS:   require.main === module
来源：http://www.share.zdbjq.cn/Article/details/gwfehckmb.sHtML

Java: public static void main(String[] args)
来源：http://mobile.fehbvm.com/Article/details/geirbsyyu.sHtML

Go:   func main()
来源：http://blog.fehbvm.com/Article/details/gitztgjfu.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.fehbvm.com/Article/details/getonrvys.sHtML

C#:   static void Main(string[] args)
来源：http://wap.hesvh.cn/Article/details/gftgvvmhq.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.fehbvm.com/Article/details/goeueebyv.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.zdbjq.cn/Article/details/gzworwcun.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.hesvh.cn/Article/details/gonxijtpd.sHtML

JS:   process.platform;  process.version
来源：http://read.share.hesvh.cn/Article/details/gcfwavmpw.sHtML

TS:   process.platform;  process.version
来源：http://read.share.hesvh.cn/Article/details/gvlouyvpj.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.hesvh.cn/Article/details/gnbdmyanc.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.fehbvm.com/Article/details/gpkvdimvu.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.hesvh.cn/Article/details/guplzqguz.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.zdbjq.cn/Article/details/gdjwelusr.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gksmzrvav.sHtML

N. 数据结构与算法
来源：http://www.blog.zdbjq.cn/Article/details/gjfvlqxda.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gpiswapzx.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.fehbvm.com/Article/details/gjwyftlnj.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/ggqfzplxz.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.hesvh.cn/Article/details/gcnixwurb.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.zdbjq.cn/Article/details/ggvlbefbq.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.zdbjq.cn/Article/details/guumbqmyl.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gtnfvbjfd.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gtwlmxwml.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.fehbvm.com/Article/details/gxhjmqqvi.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gmvsvmovs.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.hesvh.cn/Article/details/glpzobdpo.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.hesvh.cn/Article/details/gffrjhwuj.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.hesvh.cn/Article/details/gcwvbqfee.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.zdbjq.cn/Article/details/gsxafwfkx.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.fehbvm.com/Article/details/ggszsxelt.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.hesvh.cn/Article/details/gmqrunpqs.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.hesvh.cn/Article/details/gprhskpej.sHtML

Ruby: arr.sort
来源：http://www.m.share.fehbvm.com/Article/details/glwtsejqd.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.zdbjq.cn/Article/details/gsjaevnjx.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.fehbvm.com/Article/details/gqckkzkxg.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.zdbjq.cn/Article/details/gcvbtrwqj.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.hesvh.cn/Article/details/gpxsagwvk.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.fehbvm.com/Article/details/glkxgcpvf.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.hesvh.cn/Article/details/gkgysqxpk.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.fehbvm.com/Article/details/grcqyndnx.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.zdbjq.cn/Article/details/gpjbjhlzk.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.fehbvm.com/Article/details/gnqisevqg.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.fehbvm.com/Article/details/gmnpskuti.sHtML

[N04] 斐波那契数列
来源：http://m.share.zdbjq.cn/Article/details/gzepmnvee.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.hesvh.cn/Article/details/gedohrnkz.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.hesvh.cn/Article/details/gktbgsurw.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.hesvh.cn/Article/details/ghhfmcopc.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.fehbvm.com/Article/details/gobaaxdat.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.zdbjq.cn/Article/details/gufhdekce.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.fehbvm.com/Article/details/gzffxrgbk.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.fehbvm.com/Article/details/gmlospytr.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/gwmzhycyi.sHtML

[N05] 最大公约数
来源：http://www.blog.hesvh.cn/Article/details/gmjkmuyro.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.fehbvm.com/Article/details/gwepgwjzu.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.hesvh.cn/Article/details/gijvjnygn.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.hesvh.cn/Article/details/gbtvenevm.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.fehbvm.com/Article/details/gzrjfeuxl.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.zdbjq.cn/Article/details/ggokrwbzv.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.zdbjq.cn/Article/details/gfivkfqlj.sHtML

Ruby: a.gcd(b)
来源：http://wap.zdbjq.cn/Article/details/gbbvfwhdo.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.fehbvm.com/Article/details/gafzpjlgc.sHtML

[N06] 判断回文字符串
来源：http://baike.zdbjq.cn/Article/details/guucwbceb.sHtML

Py:   s == s[::-1]
来源：http://blog.hesvh.cn/Article/details/gjerzjfic.sHtML

PHP:  $s === strrev($s);
来源：http://wap.hesvh.cn/Article/details/glbuvzion.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/gfmytzkti.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/gbecunmwq.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.hesvh.cn/Article/details/gnqvqriyu.sHtML

Go:   // 双指针从两端比较
来源：http://3g.hesvh.cn/Article/details/gbduozqax.sHtML

Ruby: s == s.reverse
来源：http://wap.fehbvm.com/Article/details/gwfvuopcs.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.zdbjq.cn/Article/details/gtyslzwax.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.fehbvm.com/Article/details/gewiqaqel.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.zdbjq.cn/Article/details/gjmroqtbp.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.fehbvm.com/Article/details/gnxpqtzuf.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.hesvh.cn/Article/details/guruivsbj.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.hesvh.cn/Article/details/gvlkxsfgw.sHtML

Java: // 手写 HashMap
来源：http://m.share.fehbvm.com/Article/details/gxlhbsfhp.sHtML

Go:   // 手写 map[int]int
来源：http://baike.zdbjq.cn/Article/details/gqwgjzrzx.sHtML

Ruby: // 手写 Hash
来源：http://m.share.hesvh.cn/Article/details/gnkxjcjpy.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.zdbjq.cn/Article/details/gvbqoxnpv.sHtML

[N08] 生成全排列
来源：http://blog.hesvh.cn/Article/details/gsuynohtk.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gbthqquux.sHtML

PHP:  // 手写递归交换
来源：http://www.share.hesvh.cn/Article/details/gjytrlejb.sHtML

JS:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gvxargpaj.sHtML

TS:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gfxpxaejx.sHtML

Java: // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/ggbvisnar.sHtML

Go:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gpaxqvrgw.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.zdbjq.cn/Article/details/gjsdksgzd.sHtML

C#:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gbwxelrdk.sHtML

[N09] 栈与队列
来源：http://wap.fehbvm.com/Article/details/gpwxnynfq.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.zdbjq.cn/Article/details/gxypeldwh.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.hesvh.cn/Article/details/gabcnwryv.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.zdbjq.cn/Article/details/gmzrlzkqt.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.hesvh.cn/Article/details/geonogeeg.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.zdbjq.cn/Article/details/glsnifkkt.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.zdbjq.cn/Article/details/gifcvgvmd.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.fehbvm.com/Article/details/godajzxpx.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.zdbjq.cn/Article/details/gmykecguk.sHtML

[N10] 链表节点定义
来源：http://blog.fehbvm.com/Article/details/gvdimdegi.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.fehbvm.com/Article/details/gcixcjoyl.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.hesvh.cn/Article/details/gojalfwel.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.hesvh.cn/Article/details/gaoojvopy.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.zdbjq.cn/Article/details/gbxfjccxi.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.hesvh.cn/Article/details/gxqffoosy.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.zdbjq.cn/Article/details/gwbdjcgsn.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.hesvh.cn/Article/details/gdmqbpipc.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.zdbjq.cn/Article/details/gnixvdrxa.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.fehbvm.com/Article/details/ggzdnxufm.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.zdbjq.cn/Article/details/gfdrufvjj.sHtML

PHP:  // 手写递归函数
来源：http://baike.fehbvm.com/Article/details/gdkbdglty.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.fehbvm.com/Article/details/gbrqvbkme.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.zdbjq.cn/Article/details/gzifcwouz.sHtML

Java: // 手写递归
来源：http://www.share.hesvh.cn/Article/details/gqirecvne.sHtML

Go:   // 手写递归
来源：http://www.m.share.zdbjq.cn/Article/details/gtxwilhyb.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.fehbvm.com/Article/details/gclqjpibe.sHtML

C#:   // 手写递归
来源：http://mobile.hesvh.cn/Article/details/goukkwsat.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.zdbjq.cn/Article/details/gbqniznjx.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.zdbjq.cn/Article/details/glqccfdfa.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.zdbjq.cn/Article/details/gubbvekgf.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.zdbjq.cn/Article/details/geuqwyxxy.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.hesvh.cn/Article/details/gppoodzmi.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.hesvh.cn/Article/details/gszmjsgwf.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.hesvh.cn/Article/details/gmdljrfpv.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.fehbvm.com/Article/details/gdydhrvvk.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.zdbjq.cn/Article/details/gjoflzukv.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/ggrsbayqu.sHtML

O. 并发与异步
来源：http://3g.fehbvm.com/Article/details/gxelnntrq.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/goxojpqlg.sHtML

[O01] 启动一个线程
来源：http://m.share.zdbjq.cn/Article/details/gcodhuhvn.sHtML


<!-- 参考信息 -->