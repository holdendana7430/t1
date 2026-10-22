代发 wailian999

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2faoaitsi.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2qucfdllk.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2vqnkgmbm.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2pntscxzy.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2zwqkfcxb.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2ohezzwrl.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2yxtmgrrw.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2crtkedtn.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2nbwzhdhi.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2ptcqnljh.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2jwzdlfwd.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2qdxpvrze.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2cgiueric.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2mpqdgvfj.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2puhnulxt.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2hcfnvyoe.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2uqzteesj.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2snlplvfq.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2kktewvec.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2jsbttvme.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2oagisepf.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2agyvxxed.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2gglmlswf.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2fwhxwyds.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2kcknshzz.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2cpjcwetg.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2lmbmmcqy.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2ffiilpmt.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2jydgniqi.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2ueaqielc.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2betozdwy.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2rdiwtncc.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2xwddgshy.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2xxgbscqa.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2ezkqkfrl.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ceshhhwb.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2khrleppw.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2nofhfson.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2bwliyxfq.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2texkjjmw.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2soaahniz.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2kcltpwqu.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2apoqvdmj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dkmswhlq.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2cecdsslb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cvxashxz.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2lslwxhqu.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2dnxskrcp.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2lkrxqchh.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2gvemvgkf.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2bnxexrgl.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2uehhivgk.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2hspvvfdh.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2zrdndicp.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2okottswu.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2frvgvken.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2baqubhcl.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2tqjrreuk.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2kaleenmb.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2hpndisoq.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2oxfzqlxa.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2nkmjuvwj.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2snuvgvth.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2gsznrpuk.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2krdjfhyb.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2fhubrmak.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2ajnerhic.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2ygjuevqq.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2kzoggoum.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2qdkbysam.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2cykvcfpd.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2popingib.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2myyjyepm.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2qagwvrhj.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2cacirqro.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2fgnfruyj.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2nbumnxsn.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2bkcpskal.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2qpgierhu.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2wfqlpgwn.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2wljbogey.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2eouqeatf.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2mjdiqgss.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2fkoaxrik.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2xwnpuktf.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2lsptmevq.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2tfltvhfu.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2tswwqhsb.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2vteyhodh.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2kfivhsiw.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2auvwxzbl.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2yojnnhby.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2kraneroe.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2helcfcan.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2avgtxpko.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2rogfdtho.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2msqlrmtv.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2kfxthgur.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2gjqlnjtg.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2izsniorv.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2uhweafeh.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2cuvdpvif.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2catpezcf.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2zunxlued.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2aehlvktk.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2tqgvoyxu.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2mgvptxfw.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2jfkhoton.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2yimaaugt.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2cyizatzu.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2qdibqmkk.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2lqsatviz.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2eysztctp.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2fmtnxkda.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2fgaawlox.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2fenijjbw.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2ogpydxbk.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2djvhwmjs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fjvznmec.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2bobckxlw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yhkqgnzc.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2woxeatki.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2qizfoyzu.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2cewzenfm.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2uxlknfpd.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2dpfguyfv.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2dqjtsdrk.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2fxrhdlsk.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2qvqhcskd.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2oichtbrq.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2qegjaiqf.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2pokxujmq.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2msxlfnto.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2eglsxaof.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2bdikpwyn.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2uvpliyrb.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2ksxasvpb.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2ylfeorsq.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2rbcpwdqy.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2jtnsdnhs.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2iwbnovmd.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2jmoqyjdk.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2moqodkoh.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2tstemzho.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2rtwcfmlc.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2hassagkh.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2epcsbcqt.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2ywrafhxh.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2tfgkvxiy.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2pfptlkjt.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2uydtgvuu.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2xzfkjqqt.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ssvciigx.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2vrpbucxe.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2pawffdrq.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2itqyplzs.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2dfsdnwnt.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2khtxzvek.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2yqxyzmyr.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2poozskco.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2kyyyudch.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2kcdlnuyt.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2myatbdsx.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2habmdvsh.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2amohedqm.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2gsrqcugz.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2gugufccr.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2fjfomisj.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2sgsonmrv.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2eqlpedcx.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2pdvrgplo.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2ugijhamr.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2tyefgtnk.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2kxwcdxai.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2toynlyrr.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2tyseckwa.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2yyponisj.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2qcqzairl.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2bavojvag.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2tailluqs.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2kkydwuny.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2kmkqkqjm.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2cxzgexkg.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2hpsujivm.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2uhhaxwbx.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2svyexehl.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2cufehesz.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2conhjuep.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2lpittkkv.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2vrkzqgax.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2pzfpqsbh.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2gxoiwbnm.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2zmeijprg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tglcudeb.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2jdrggwaf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2raulvshr.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2utvommln.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2hrzxmnlc.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2hyihnhgp.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2nshhvvep.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2wwlyukjq.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2iyotkgrn.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2zvatkkwx.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2ccazytbh.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2qfbkyzqm.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2pfnlugek.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2jyuilhhm.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2zussudvt.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2fymklkjc.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2ryaksdhd.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2rlcbysir.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2uzugebcn.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2hjalwciw.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2hglqozck.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2oevaauep.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2tsnsuhnl.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2iyeiizni.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2vqlogqfq.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2zkfgblcz.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2dkpcsarz.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2ldzsqfqn.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2exaxcbwy.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2pdoscdla.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2obpjgocm.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ugtexgbk.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2crbtzoqr.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2nyqmwqxs.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2qhamjvqr.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2lizwcizc.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2xqpfcsdz.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2fmhcquat.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2tulqfnbt.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2cfvywlnj.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2kdvtqxve.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2tdkjxopq.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2brbefjwm.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2tfsskkrj.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2nzdlplxc.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2whgqopoh.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2mtknctoe.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2pjnengtj.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2crurjopr.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2mdijatak.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2rsmheaai.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2ivzfyhce.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2kulhpijr.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2drsjdgsn.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2ajgqtqjd.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2flgthask.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2loewywnh.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2eidjfqnr.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2hrqhxuui.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2kesgkwcm.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2xghkecfo.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2lefshhsh.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2xshthcsg.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2ghaevrwc.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2uryxhqhd.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2cgqozrcq.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2bivgkeia.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2fxgjedab.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2ctbxyhar.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2usxxrfys.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2iprvjbbu.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2yikfdqfe.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2zwhdvjsf.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2lhofaiak.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2gebzeryq.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2fhmxvpfe.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2crlrpmpp.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2ctizoqlo.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2zseszwow.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2uoqzhdwz.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2hragphxn.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2ezhdkhvz.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2kyeqfwgw.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2oqddxicm.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2zolgxtkh.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2ydqjlwaz.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2ygkmpujc.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2mrjopntv.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2knxjedki.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2yolzmlbp.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2mahxrmpo.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2vcxsskne.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2aclinpup.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2jkhpnufm.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2njnwbxrq.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2issuhvjy.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2lprhobkb.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2rdefrxog.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2qttjpnbi.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2rfmfsosm.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2vpoliqff.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2gbejrubf.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2fyoevdrm.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2ivvrewlo.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2ypprglcu.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2okxpjxdc.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2unbvxenh.html


<!-- 参考信息 -->