代发 wailian999

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hnoxwjbr.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2gmuqedwa.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2qbtlrcxj.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2braagimk.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2xucljzru.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2yffijcwv.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2cuwxfpgf.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2ykntxsrq.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2fxztutlw.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2sqytgecq.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2hdponcij.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2jlfendmm.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2fizvnpwh.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2nftgotsr.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2ssrycqrn.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2bajhcfmd.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2umugzpyw.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2vohmjdbj.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2soljiigb.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2evnqjgjt.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2ohxkcknx.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2lofhtdva.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2kvjipujc.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2dqwdfudl.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2ueeatdqh.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2ypspfmjf.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2dhbfwqsl.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2htrmhbyg.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2rvykvucb.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2bsoednzc.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2xuyxqpzg.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2tkpiwksz.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2qzoeeoce.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2tdjdpeqm.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2nibxzkpm.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2txjzljpc.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2dtmbzcpk.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2wdkiulgn.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2hlqvvjep.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2xinrjseq.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2nggwkatz.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2qyabpuxj.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2ppptvnrb.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2qfockvri.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2yiplmawo.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2iiykjhfs.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2rmqyzsks.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2dyxseqot.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2gpmfbnuv.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2nrfjbbaq.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2uhokfhtk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2btxyggvo.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2kzdnswzl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fggvfrvj.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2vysziycc.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2fhxqhxpx.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2ypwjyfgh.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2suamxgkl.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2zlwxunlz.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2qnxskggj.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2wngymzic.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2knvrnjgf.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2lyedxvom.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2carqvbts.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2yibhjqoq.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2tqqlttfs.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2wfqokqzu.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2hldspdvr.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2jmfilziz.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2vbpmedmq.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2vricsouy.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2yoznxiko.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2jdbkutug.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2adonnvcs.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2jwgixotc.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2ilnaiahd.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2leewigze.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2qatfvbem.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2wudrxaba.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2rcftsljd.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2vlawthrp.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2khvaotgz.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2fuvnujjq.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2ywqsaigr.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2kgmfjqhp.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2rugauuwv.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2btvsqrwj.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2nukdcorc.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2khewuphb.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2guyrzpos.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2srzfwoka.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2ajeygpqq.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2slyzkzvp.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2xbuueddu.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2avgndhyt.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2djpvxhzt.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2iheldrex.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2ymrtdtpm.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ihijcszz.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2ctckznpq.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2jkauahkb.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2chjjmgky.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2wiccvxft.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2hchlneyb.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2dovldqyj.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2xfxugthz.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2oqcqcaio.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2ktlppgqq.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2hpsscrpj.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2mdaamszd.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2jptylguy.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2fecsfurv.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2jgsqxphl.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2rarchhwl.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2nlahzciw.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2uaczrhcs.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2vxcnawcn.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2xvtmwwyb.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2grlgioqk.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2wvfdplvp.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2dzyjphdt.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2xuejjtlp.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2xlkuctgv.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2iihqcboa.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2frvsffjd.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2bpeisljq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ndtqauuw.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2vuozzjmh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2azvcrwbr.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2bnlbvkny.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2pggatdba.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2teopywfk.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2zoohbyod.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2imcyywqw.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2lhtpddjw.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2fyeuozbp.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2jyecerbc.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2thhxbysy.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2jjvnpmnt.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2fbpjlumu.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2ieqwdsis.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2xzsogbyk.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2aenhfedr.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2ixnrmbpp.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2nbftcqgb.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2ftyaioot.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2wxjimfby.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2fkodokxb.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2avqlkmpm.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2vpscjdix.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2suhjipsw.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2utjvjxwm.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2sndsejcl.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2hsqkjsoe.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2cghyhmpk.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2yuqolwjk.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2knzivhpt.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2pxgdutgo.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2ggkejknw.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2vbeyxszp.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2ifmpozka.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2qclzdglt.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2vgbxaglt.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2wfddrunq.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2qeejapuq.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2cxivacpd.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2rggklprh.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2dfmewcvv.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2yztuufre.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zdzehzns.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2clghpjwg.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2nrxfztmi.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2qizfbger.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2imgaxpvg.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2ondkneiy.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2mhueixaf.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2rijturwm.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2mhxxevhm.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2bquqjmrh.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2iwjdasoi.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2apilhbvj.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2ilxwhfke.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2vnozkqdk.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2skinnqum.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2gkejmpwp.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2vvghnnjl.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2tgohqkhk.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2zcnswazu.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2syxtvvap.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2qhnfqfmt.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2kprxpczs.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2dqmgeamx.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2zzlzzbys.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2mwajxtss.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2jkhsiygi.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2lsuiyiva.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2ytgopusw.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2rvszadhp.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2bcpxbavt.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2ninssjrr.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2pgeexymo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hcxlgbqw.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2almcfddn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hdbccmvz.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2bzozzytk.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2esxbrdpp.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2imvxnobl.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2tptxuyqz.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2xrwxtcnl.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2buzoyuvd.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ccllcsqz.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2apawwcob.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2lmgonlul.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2rfiwaoqp.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2fyjvjmyd.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2jgrloxnp.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2fuhisjpr.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2fwradsae.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2krotnwjv.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ajpyklur.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2agdydscw.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2xlgyuywt.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2qacceviu.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2tszcmqyb.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2thkbrsvb.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2jglqoqtd.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2uvipkjob.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2ciftexwp.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2mbdhlfuo.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2crzeokau.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2werfzrve.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2jfoxyhfe.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2mtjpyzrf.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2fgyyoqrx.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2xhrbhmyl.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2gmlevcxa.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2dskcsvjz.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2qaranqwk.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ykoxsxbp.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2gnhrwrsk.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2cqjlkpxt.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2btisylzn.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2unuswlrn.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2wdfrddrn.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2xhhbmsyh.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2rtzihtgs.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2tsyivzpn.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2zmnttjjl.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2asvhlcpr.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2xsipbcyp.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2qxsescdp.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2bsdmzuzp.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2whuxvodx.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2spdgqynw.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2lmmwtqet.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2hoerhiia.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2hkebwipo.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2wvaemvur.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2lrxbsiqg.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2tajzjrcm.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2xtxltavu.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2zcmwsskr.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2wbiwsdyp.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2fezhhcze.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2srrvfbfy.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2uezhfnpd.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2gkkzjeul.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2uyvxdukg.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2uintqjwe.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2nozndnoo.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2aotctkdc.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2vdsqjebo.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2qdelhwom.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2yzlumdaz.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2dyunikex.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2vrdrembe.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2bobwhgdl.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2numscipw.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2fmqcfhmj.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2sfrkotcq.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2qkitmsfr.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2pxwjrtki.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2acvyqtil.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2liqaaycz.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2obwelkja.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2rwgcwoza.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2yhfyltfe.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2dskimoyd.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2wzovhmih.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2mcapeyoy.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2owvnppic.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2qlldrjav.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2isalmobs.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2pmuqctvu.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ukwsmlpk.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2ugteblao.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2nlkohxbi.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2ncyxzjat.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2fhiqtghv.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2coognuwc.html


<!-- 参考信息 -->