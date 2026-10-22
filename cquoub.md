代发 wailian999

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2izgbgnlq.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2bzuniyak.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2iuzwpdmw.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2txxsqoqa.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2ajfufcgq.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2fnzdsjvi.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2pvpcqecj.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2dwbhjkfo.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2lruqxszn.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2gqrnchgc.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2eidfbikj.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2dfwqnwhb.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2jmdqthyd.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2aqcujstc.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2inmafsun.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2aogiksyw.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2pzyjqjwe.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2mdgymcnf.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2rwikzcul.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2jadnkdco.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2jawthziw.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2qatccrxg.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2vpqwvcrb.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2kchdtduh.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2odsjzjwf.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2awvtqkns.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2bqtlrutn.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2kccmlbai.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2nhfxmcib.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2hsyuvudo.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2zlxwqbfd.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2avftotzu.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2qdntozep.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2xwhlzrpd.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2kpqatdbs.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2qdddtquq.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2cedhadda.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2zudnhurb.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2ryhbhjnb.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2fhnohmty.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2ypvsdfuh.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2gwrhgmqj.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2mabenacy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zwjvimxc.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2ndehzety.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2taqzphjm.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2phxcodxh.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2qrogbfmp.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2oorjkjwg.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2nlzjvtpg.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2ujwugewg.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2efqadiiz.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2hdxrnftl.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2pvynkfnq.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2xrswaelm.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2yngmrkzz.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2xelskwoc.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2cgafhcod.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2ldnwpcyp.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2beykpyrm.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2piodydoh.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2xaxfxgwv.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2zvetzrun.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2yctamren.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2fudwuxgb.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2jydgjnki.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2hewoxhjl.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2tmlaemyb.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2pwdvwqls.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2nwyvjtvz.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2tkgezpoz.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2hobrcqqe.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2gsshnqvf.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2apvttqtr.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2zldlstmg.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2hgeetxyv.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2rxgskpku.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2ebpwxcgk.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2zwhoxpsh.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2hbjlevyd.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2xrxhtjdk.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2owxsvgqd.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2xoeesxhi.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2tfntmdio.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2aebxchef.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2tlumbevg.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2qfwojhgt.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2yfbdzooa.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2eedrqidg.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2ukspxeim.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2gvqsmiaw.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2exrgzcer.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2zakxnvoa.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2rpcmlylf.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2kavzfrri.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2dmljxdll.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2lgssawnm.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2sbcbxvvd.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2ftwgvewx.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2gzvflwmf.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2cfvirukc.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2vycdcjzq.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2yslmfmen.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2dkxjziiv.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2yxcoqhet.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2ptcxmtqo.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2rbbefzlv.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2zdivfsyo.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2kywxybqn.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2alhcvtst.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2svwpbwzg.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2wlrzksdq.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2lcfwxspu.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2bfnqfoyc.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2wdtpnibr.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2aicywntp.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2kntspptg.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2txprbajt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2setlmfmg.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2zgvshzyq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2makjfmss.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2faennubi.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2eirdxtve.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2dncypiqu.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2bprgmbqn.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2btluxtqv.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2trcvtpij.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2zkpcigwm.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2fbbwtfod.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2uwdxmlin.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2qentklit.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2ewlmjntm.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2szwliyrv.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2mvsgafsl.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2xhqivxiq.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2jyjknagk.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2kjedhish.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2cwkwktlr.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2fdvfkuxr.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2xxpoaezq.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2iqqpybfc.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2hrhvsunb.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2ursclthg.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2oiprxivn.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2ubnsllwl.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2grlkvdte.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2dkqzdkqw.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2ytezzyhk.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2lledcqpn.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2zlgeqpde.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2rfpcnmmf.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2ykipddok.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2mobcpzae.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2cttxevok.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2ijmfkiai.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2sqclidhl.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2iijsmhwx.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2vhmyoaub.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2xhfdvhvs.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2yqjioajt.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vbnrnasq.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xfgefxgy.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wzrqsxjh.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2uxakjaap.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2ivryxcjm.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2hptrvxxp.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2ekraqudf.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2geqewcwf.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2htuksfhg.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2bawodxak.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2rcfpxhpl.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2yhsfamak.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2kbqwjczy.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2plqzzvre.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2jxzdnaxj.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2qbxhwkpo.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2aajxywwq.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2rxbkxdcz.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2trzaexod.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2dolbucml.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2xwewtqwj.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2rzerzqui.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2hnnhcdqp.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2uintebas.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2gkpcdedy.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2hhsmdnqg.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2lztpjnef.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2yztawxho.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2zphvdlqx.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2nsfuxilg.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2slylrgef.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2embaukyw.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2vmcvqehd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dclpqltr.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2acugocwv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ycmmcakr.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2cogskaew.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2wthdaeyt.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2csembwnp.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2uqphubls.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2fjrknmmm.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2epxgoszm.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2vedvmelq.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2qefctwwk.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2mkirkehy.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2rwivipnf.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2zpivgbfb.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2txmbjtil.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2esblhwot.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2cfqzixxe.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2pffzbicg.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2erqsgiqa.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2cjxpwxee.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2veiekulg.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2mejjvyyz.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2npklarpv.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2pdetudls.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2lllylzuu.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2aufdprfd.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2bptdectv.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2qdtlrheu.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2ibdtyuqm.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2hyomdkdj.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2kanffmbg.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2utzsfiuk.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2djecgjno.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ofxayjmj.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2wdsovmiw.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2yjjgdyho.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2udaslqdy.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2crqwvnzf.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2fzrwjnbr.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2gtlwvkdi.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2nzfsgbkx.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2mpaarfza.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2voxojcql.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2nespgkrz.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2ciiouvvu.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2btamgvfj.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2jvioomrc.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2joqyarmf.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2zymhaqnv.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2libdhzyu.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2awvooxmq.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2lbzfpqml.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2gjqnvupf.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2synxxpfu.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2hoqvkgkb.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2yvbghale.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2qkvdldxx.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2bvgvvwrf.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2ajfxauhp.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2sfxcvcmg.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2jeegnuaz.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2yudxkibe.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2sejmjldt.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2gzspyxsa.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2jsysyolt.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2knftllne.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2wwmnzbzq.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2oohpryif.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2suxgvoqd.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2geeqpcmw.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2cizhlrmh.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2goaofzkx.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2mvuffkwj.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2dgfdordr.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2atvwvzwc.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2xhamfbds.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2rlzkzyej.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2gajqohyy.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2nnzwgacg.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2amyswksy.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2mfowqxnx.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2xbjxtzyp.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2tiymyunn.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2vsznpzse.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2fountarh.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2ajudzycp.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2gwhnrsmm.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2dqaaqgfw.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2jsbncswv.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2vcmbrknl.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2lopxyueb.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2jvmtwtck.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2xibzgjsw.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2laytmqoa.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2ytpkkwyi.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2ijadfdwy.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2jgdblalj.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2dteabnvl.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2fjfvvcur.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2jtgaxntz.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2bauetcbc.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2jafswwoj.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2hfzqgwcu.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2nwkcvbzw.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2ezkjhjtj.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2qonsfmhr.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2oirousrt.html


<!-- 参考信息 -->