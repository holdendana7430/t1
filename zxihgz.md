代发 wailian999

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2uyekrjgs.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2ctupkkkj.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2txnvzgat.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2gryczhzv.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2ryppbzfc.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2rilxkzve.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2pdzvxruw.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2gqyvomxy.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2nacfkkwq.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2tnxtdflw.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2uxkrvaos.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2lmlvshdk.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2dttfwrxj.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2mspzhvnb.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2majjrsqu.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2dbtfnnmt.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2kqjogxnb.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2enlsbxig.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2qrwyodno.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2jluelzgi.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2hkhlfjxi.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2nmpupfvi.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2ywfpxobc.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2gjsdezix.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2blxbflpm.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2abepfwbn.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2rtdzziic.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2vgdmwdni.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2uzqnlvok.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2ysgvgjln.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2cakcuore.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2gflbspwg.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2ipqtwujj.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2ldeotxyi.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2rhhccfte.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2uefttqmq.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2yldyribl.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ndzsbceq.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2thiudcrk.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2repizbsu.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2cenmlejl.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2gwiqnwup.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2zzkkifwh.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2zhhmndmq.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2vmycfwyj.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2yqcdbezd.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2nsfjlwvu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iuvhssde.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2pixkxiib.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ppkgxipj.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2cnmdfaqq.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2puwjnwbv.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2inbxqqgq.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2voreftpv.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2wahnxagu.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2sutjnlum.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2lcbhamsk.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2gekjvsmv.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2jpotofks.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2tjcbccwc.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2dbwpreaw.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2bnkflaue.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2sfrpuqec.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2yhwxciis.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2adoyunzc.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2ebrssuci.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2xlhwsdkm.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2kxrbbnga.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2svedckzc.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2yxbsrqde.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2pgpjghle.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2fbukxpmo.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2fvvgjsvs.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2slkxoeqk.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2brzxlhmr.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2txwzonhm.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2mieqifek.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2irnqgjrs.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2udglyyvy.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2mklnaaoi.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2eabtdefd.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2mbxbzwci.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2jkzvtxiz.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2wuvkdbfx.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2goqsegan.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2bzwiknuw.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2dkmywdtd.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2xgvegnwt.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2papykdhr.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2genjjirt.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2vpwhiocc.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2abcimtku.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2vjbwmozw.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2lstuhaiv.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2csipnsdq.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2ofnwemaz.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2fycckwve.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2kdqqrhcx.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2qtbrtwnn.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2kopvlvjd.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2flrxamzc.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2mdcuwmgi.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2czpwggqs.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2apftwcvx.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2lzgirxjb.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2ddzanvao.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2uxqpfymh.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2jwxzmpcv.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2jrkgkfex.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2duszzuvj.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2snpcvtid.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2ruqmccrz.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2wsszoyci.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2sowvvepy.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2bqyphgeu.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2kpqndxzb.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2isxuocsm.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2raysdnuq.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2hhlxmkqe.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2efncqlhp.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2tjncpzcy.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2gqfmsxbz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yikzucom.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2iwvywewx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jiqheatl.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2kagogxnc.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2kryzjuyp.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2ejscgmox.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2rzzqooop.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2stujemud.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2crntenho.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2znzopjhr.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2qbttulxr.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2dwbxvbls.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2idnodifi.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2gizyvoji.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2dgdorcwc.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2viitnfqq.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2gtsigwtj.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ttqtrrvr.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2nkjvsdyt.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2zclnsldf.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2pmmjizfl.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2jxroaukq.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2mhwlbejr.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2oxjuqcxd.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2vnobzxoc.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2tmpqmqju.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2pgdmocit.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2xbgchtti.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2onvkmpxv.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2naraxhlq.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2nyzbzldi.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2mynzjkcj.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2bknqosjd.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2tchzjugo.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2bbnjwqdw.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2nduxsvmo.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ydpzvfqb.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2wqeldskj.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2hzakoeut.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2sxdmpsmd.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2myhxjoqw.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2xjenkoav.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2kwgnxjms.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2dvlmukqp.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2mkhaiqwz.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2bkhmuzxl.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2rbkmtsgb.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2norpmdpk.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2zhyzymjf.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2luxazsql.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2mielppcm.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2vhlshqhr.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2lgngldmu.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2irtrnddl.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2kvmrtwzr.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2evkxrgqm.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2owdrctoj.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2qtfolfvh.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2rjovzahs.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2rzdreqts.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2hrgqbdsn.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2boeydapn.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2pfaipspz.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2ofjvrpos.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2pzcfnimi.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2ljtucery.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2iqyavjzi.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2hfsmpwwi.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2vidowccq.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2kudzhmwl.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2fahfozsd.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2nmgnlrlg.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2flrpmama.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2odwzzmgr.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2octrzwhq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rmgzolcy.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2ybvfsktk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cgpmawbx.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2dwsetpqn.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ttiscvik.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2pcuqfllp.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2ozlcagoq.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2oqdjhkzj.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2yrakacsx.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ccuhgjyz.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2hssqpixj.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2fkhrkxbf.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2uurgdcqg.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2tlktxmsj.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2mpklzyhg.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2tsmeorch.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2gklfflew.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2wuttclnh.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2ltjhxzdd.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2bjeepgoy.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2gbftdnrh.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2vwjfzidn.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2ieovsbib.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2xcfsgwin.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2psbalyiq.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2bynvgmhb.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2jbhicwky.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2izoavgjo.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2mhpwzybu.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2yrtzwlop.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2gbdwkssn.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2kiqlcbge.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2atmrphmq.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2slqxhzgd.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2encoccge.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2sadcumnc.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2hfrkshcj.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2xjmgiytk.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2phxqwquj.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2caqrqlgc.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2fsqnvelp.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2ikotfhar.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2uiphbtmy.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2bpotwsbs.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2ajmlifwp.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2zdotufko.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2khtmkkbu.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2oqutoptj.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ssalnlzr.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2ogcfpiyh.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2lvsonzaw.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2zasybvsl.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2kaimkkvm.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2rdzfrzlm.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2izqwqcyz.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2qwwtezoe.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2khkagcnf.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2kjwmwkjk.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2tnadrkiz.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2vlofupmb.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2drlbhdth.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2svyybdvb.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2kpmpcuve.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2vuksywgh.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2cuytqojq.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2gedxmpxl.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2lnfotagq.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2ixmkhmzt.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2hhytytri.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2fkvidjvl.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2vktmsbyg.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2yeokushw.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2takrmgfk.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2imvlbdzu.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2njoxless.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2abrsheov.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2zgcoivfe.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2eyadcuix.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2vhhaurgu.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2xpelbqsy.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2mycjuwxv.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2inucxewx.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2cltqyalu.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2udlfowir.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2xqpmqiwx.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2bqggtwjg.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2ratncqzb.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2fkempsqb.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2hvqkaqrg.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2cirbehle.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2ehuodjfl.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2elplxnqq.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2ujcufttb.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2qetxymlm.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2zedjpbze.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2ncjhtfrr.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2psgauyry.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2lelozioo.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2ygtngjlw.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2bxgmsrsl.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2iwaleebb.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2qaajpqkf.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2tdvnlonb.html


<!-- 参考信息 -->