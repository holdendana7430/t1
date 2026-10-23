代发 wailian999

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3lsuwurrc.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3pinnswsc.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3jxlrfeap.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3hrrjrwzt.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3nhbjztoq.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3sepabnjm.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3paplsnfi.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3aeuzsccy.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3bbbipeum.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3sfgcmzkj.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3wsgxxsbm.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3whwotobk.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3kyurkllg.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3ctnwqaye.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3ddnqpbyu.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3mtxztykz.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3nzktqcts.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3jbrxmrey.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3hijcdbnt.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3ivyttcvv.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3fatqrqod.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3vcmjfhgb.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3ojacvkxo.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3waogkamy.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3ttcmtqla.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3tdcrivpj.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3cmgafkgn.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3mamsyvch.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3ignvviht.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3kqbgycvz.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3jszklbjw.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3iybaunnb.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3ugxevvrb.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3gynnahuv.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3fhsjggzz.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ajnwfauj.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ftgkbwcz.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3yzmtsnjt.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3wgfxoxwu.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3paswjxhn.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3hxjgpboq.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ywjavtja.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3pufbszeh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fcrtjong.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3kaxgpzon.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ppbmywbd.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3lzevftsp.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3pofkzktx.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3pnymebgx.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3ctelpjcw.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3acvmcgsg.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3edvtxjov.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3ibsaftxy.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3dxfldinx.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3tjrtzajj.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3jfcbfxtq.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3sxhsoqje.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3ocpbsryl.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3faizzafv.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3ssnepaow.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3thmtqkhs.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3zvcusbwr.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3xiftvggt.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3icslkyug.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3kntvofdp.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3jvqsbrxe.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3fruhcheq.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3ptmutdsf.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3hrunzuye.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3jdphjsmo.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3fmxoxwmb.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3spcsicja.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3mtjjtfpi.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3lxlfegxa.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3qnkuxhep.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3sobcfquy.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3oodjfohg.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3twnpkvvu.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3kkobywcc.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3gihkyaue.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3suxaxvkr.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3gidaptzl.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3kkfxdbed.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3qtuokybl.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3ssztiqgh.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3igtvhceg.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3xtzrtykc.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3bljknroo.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3adnqneco.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3hsmrgfac.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3rjqptroe.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3riyebpla.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3ptvwaqzm.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3hktjwijy.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3qukcminm.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3qdemuuwk.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3urxossrm.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3fkrbabbu.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3gsdfscgj.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3uqaeuxlz.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3raupbutt.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3cskxykgl.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3eiilwymd.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3hcjenhak.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3tcattrje.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3oguuraxp.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3pdfydcef.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3zobhvisf.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3withjmim.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3qkpfpazu.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3heskjxyx.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3vbxrjdqc.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3nbtkparu.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3kyepmirc.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3fsnvvzrk.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3pzbsnaxo.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3mrmhplcs.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3eowmwzel.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3krxaibnj.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3femzxxxu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dglxurfc.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3tyfkcjgo.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3sdpelqsx.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3kqzhpjaa.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3mbvpovjn.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3suzpqege.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3wclwwfsq.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3jshallig.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3wfwffynb.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3lhurqeoc.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3bsrgbilu.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3ipdxntwq.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3tjryuluc.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3qbttdqsy.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3zwqkucrj.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3vddvkbah.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3dvlymnts.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3epcponcp.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3dbabjwyt.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3ucfpbmkl.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ffnndars.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3xjluyobm.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3depylzfe.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3ipgouovh.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3lgyuunfb.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3jykozaoc.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3oqdmkpcg.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3wlpfxlon.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3psalndqi.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3asbweyaa.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3mrhappbz.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3nrqrcmre.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3nuxitpgw.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3rytlpzvw.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3afntyyuz.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3qerejptc.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3rdoekzcm.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3vjeecpuh.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3brozclza.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3iiyokorx.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zdrdxkvj.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3cwhpepzz.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3cdtnuzue.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ufcrtzzu.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3ysifdrph.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3jlhwfqjb.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3bhhkmbfa.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3txcuayvc.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3mfmleusx.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3yzacxmdk.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3kvkitnwf.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3nogrqucp.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3twbbbptj.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3rtyhlbhe.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3hlsqjpmr.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3nueatsjs.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3niwznper.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3ajjlxolm.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3jzijyyyl.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3hukqhiqd.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3tdfvbhtp.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3xwhyvuxb.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3twtdzfeh.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3wneirbgx.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3yjfobxsu.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3lcifejsb.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3irnmpxfb.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3ogxlgabs.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3fwduihxt.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3nuptcxee.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3fddeuttn.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3csultdes.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3kvfidrxo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tcvowcle.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3nswaotlw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ijshqsyq.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3hhmiusvd.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3crwivnwn.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3lyodccku.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3heqdmmot.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3ngkgryos.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3vppccbga.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3gxgefjqc.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3fwpqutnn.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ljhnflqh.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3kghblwqr.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3urvtydsb.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3okxfvzcr.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3zlpyybcp.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3piicumei.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3evzffvfn.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3oynzohbz.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3ncuwciga.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3dwyyjlvt.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3ztmgpvue.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3ujmedhhy.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3pmoyumbi.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3dolsdyfc.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3fsdyxcyy.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3qtbszyuk.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3guzjfffa.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3wizykpfy.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3uoemndbr.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3otbguyip.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3livlhkig.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3ujyailmk.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3qmjfmfqm.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3qrmvdthn.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3hpvonseb.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3mrxrtefd.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3aohqgjic.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ibypzlcl.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3igsfwwio.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3tieegolh.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3surtydfh.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3eppyjnyz.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3pegdkehc.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3jsajkdsv.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3livxcphj.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3hctvkwbo.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3hbjgqran.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3rxgudosd.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3wtjfdtbw.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3azjgneun.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3xazrufob.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3zlosuivl.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3xvnocinj.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3jfshzgkc.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3miititnj.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3drdadivc.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3mtnmvppk.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3mcqvehzi.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3nrpygkkm.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3glafwcod.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3hikhvqcg.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3bijdfvne.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3lyppwgce.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3pwwjpmgm.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3oozipalf.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3henpbgxi.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3btincwmy.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3yynlmnrp.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ucdyhpzv.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ryzewbqj.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3erekncxw.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3cdxcczsz.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3pxehtybd.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3tewkxuwe.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3gypsvjfp.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3uiunosni.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3amesdouj.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3irsjajqy.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3splupyau.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3kfggxzpj.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3knnnrrpk.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3pszghmgk.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3nlddfmaa.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3tmjqmdjd.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3jbmfzjja.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3xqdreqze.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3jfxbypmw.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3jjzvpamj.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3oqoquaah.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3cbweviwl.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3mtfsqzaj.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3ldizseob.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3mfewuuxh.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3mzhvhntd.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3zmfgippp.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3wpeamcrk.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3xwwqfpdq.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3ymtdiaic.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3vrrhjpcr.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3pyopbzrb.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3dzrjspgw.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3bcnckold.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3lncoqqqc.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3faraietk.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3sktlmuqf.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3xjxccajy.html


<!-- 参考信息 -->