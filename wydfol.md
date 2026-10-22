代发 wailian999

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ptzwwqze.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2aifnrjec.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2zypbpsge.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2mrnvviqs.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2vmwzzkyc.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2lukbxhal.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2qavqgsjf.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2nxloaisu.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2rkkvvrbe.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2axnxejnf.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2vcqtdfcc.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2ctzsqygt.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2vnggtoxl.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2edtvhstm.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2ktscyqkl.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2vqcmzbxs.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2vbpvltwz.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2wsoomesj.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2qovwfuvb.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2tnnegnit.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2acyyrzoh.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2lvgocjwm.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2wxyjofgo.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2wfphzhne.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2qqznxhtm.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2fmmtwwrr.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2zttycypi.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2wfkfvzuh.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2xiwlwunz.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2onwcicyl.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2rwkgwwoi.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2fmhmudry.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2adplzsoo.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2uglbkejw.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2wwvsidva.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2psjwpkcn.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2aqnlzyjt.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2sewztbmr.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2aijldlbq.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2ezsejaba.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2fezkdazi.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2hbycgcds.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2jnfsbtix.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2ecfsqtsm.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2qvnwsvbo.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2dejlidvm.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2pjwtwiba.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2wbtklisj.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2qhnwafek.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2uoxkbcyj.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2hekiavgh.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2umidthyl.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2tgettcic.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ecrrjqxu.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2jwejmwcs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zthptbbx.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2vzuvwujl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vvbqpgyz.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2ueleehay.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2zvnehayf.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2xcdrxiud.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2cvljhwqp.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2fpxqzlaz.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2afgxgodx.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2yclsvpiu.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2ugreujhp.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2nlqhjpnl.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2rwgqtfrk.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2hckwjkhq.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2leqjnvpg.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2ibcchzfp.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2umxrytwd.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2zlrzqrvq.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2xkrpzjac.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2mqmkvcqo.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2ssvuaplu.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2vluruhyt.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2acekqbpr.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2kvamjdrn.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2ijvbafoq.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2zentxhyl.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2rhnecyqc.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2onfoomij.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2zobiwgku.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2wbtiwkbj.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2bgiqradl.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2qhcphttt.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2kiowprpd.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2icxzuyeu.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2bfhqyybl.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2uwbmnbhm.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2ynpdnokl.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2auxqlmxt.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2fbvirhuq.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2llciwxmi.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2pwroxqgq.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2uvbeikte.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2hwvmaalc.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2zxamfkhe.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2lkmpeldf.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2fvyequwf.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2fqcistbg.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2wohnxnbn.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2bxbxqtbn.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2skohqlqp.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2wzvcyory.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2netcgicd.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2agidnmbz.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2hrflrtqa.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2zbbqhhxm.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2sszgedwc.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2asxkbtjq.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2yocfvbfx.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2vwpzgbyp.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2xzdqeilr.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2kgfdpanm.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2xyjieyxo.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2mkufahep.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2xxmlcmlf.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2yxvdatqh.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2mgfcfvco.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2tslzregn.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2aentisux.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2qwlpyveo.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2dbvbfwos.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2aamtzjoh.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2ualzsbig.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2iwgfjoqr.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2xdomjqyx.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2tklxnkda.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uuiflsxb.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2rfglhnln.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oaxrcrkq.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2lgxtytks.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2awplinyu.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2zlpawtwd.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2nhsooyco.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2mgpgcxeb.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2lnijrllx.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2ktviagrj.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2orlfaifk.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2hdqweari.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2ocralkhj.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2epujgglq.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2edwbikpp.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2xrjwzzdu.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2zdwmuhvn.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ibgakwyo.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2xadwnama.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2phrzviqv.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2cxyzhdzs.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2nhjevzbb.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2zetowxft.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2wgrvcvxc.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2irzsaqjh.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2nysmravj.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2tlvyzleq.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2agmkngfd.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2mnhcdbdh.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2zoatklta.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2oydnljus.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2vtplepdc.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2okvnzydf.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2hqutowel.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2pevgohss.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2bqagbugk.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2uaabcjfg.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2beapzjkz.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2anqnfsfe.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2nirzcilt.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2dqoqzgie.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2jykuwlwj.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2uqqovkym.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2mqrpktus.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2vrlinihc.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2qnerppcm.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2dueqtica.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2zaqkqznl.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2igetjyhq.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2djbcygov.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2mlqqxfmq.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2unmbfzmv.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2smcaouwl.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2hwgmvvvr.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2spbmrrsb.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2stlyvhbi.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2ygvoxhqu.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2pglupfnm.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2ntpeemmy.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2oljzouei.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2hfrtsahw.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2bpmsvwxp.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2xlfdkxxu.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2yuwynkbr.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2nprgttdh.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2gmucklat.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2rbyzueim.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2hdocqici.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2ytkjgbwy.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2cfqjxxus.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2oluvpfnc.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2pandmqwh.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2vjsamswj.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2nbrvqxcm.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2bfrdjsoh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mzhisseh.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2dugqxzck.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2luioeipv.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2ijyrdnak.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2upfkeuim.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2rsvyhtxw.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2ummiiual.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2hwfldbky.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2wctnkcrj.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2alkhbcow.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2kafniyqs.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2uhkmwuqa.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2syhdqlwn.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2zhohubsl.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2ydatlmds.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2pmfrngnj.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2hnhikmzm.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2bmqmhpek.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2xpmrkyrv.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2detlezdp.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2igewkvgm.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2zbgstqbx.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2jmdznmyl.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2sttxyphe.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2lxkzfklf.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2pcrstyzs.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2aswpftjh.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2fpvpgcvc.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2wezqnljw.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2kweyjgjq.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2dclvdjfe.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2voceutvr.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2oaelxdpd.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2hovanxoz.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2poxichpr.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2zyjiszgc.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2vwhzsxpj.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mbbtdnsa.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2halfjayl.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2ixjocidn.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2hfdpuljj.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2sowpoumy.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2jjpqcllm.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2qblpovit.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2yvihmfzs.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2edbhzphu.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2haaylksc.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2nesgssyj.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2tnhdypsa.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2jtrudmrk.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2exoruwdz.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2lyzwfeqj.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2dexcjrxm.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2lvorkhus.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2bmmkiguo.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2ifghormz.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2xdakyuwo.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2qdrjpqlv.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2tlqzbxfg.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2nizuvsga.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2ipafprwf.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2qjqcigcp.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2jgkcoilm.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2alfelrot.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2lwxvsdel.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2ztchzsjn.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2rkboojqo.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2gtcbstez.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2razczvpy.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2cctfmrve.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ocbxibfx.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2hmtcoijd.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ygnzdice.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2dpaeqyqn.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2pywajesg.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2lmsqxisl.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2yelxzbzc.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2njqqcuku.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2vdyvcqoc.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2wlmqjdhw.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2taaywwdp.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2zskzwoyz.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2pspejviq.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2udjakhoq.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2jddymqvt.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2xmmyzuxw.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2mjkimlcz.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2sfokteqq.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2njwwgacx.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2ncurrged.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2ckjrdhmj.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2ietsplth.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2fmxakrax.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2gkmjnzvy.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2jtyhrwfx.html


<!-- 参考信息 -->