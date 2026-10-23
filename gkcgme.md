代发 wailian999

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3basmqtfi.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3ftavbvyg.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3ndhxuyua.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3excjqczw.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3unnjtowr.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3onepekdl.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3kddyfimg.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3uexwsvln.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3gobwpkif.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3pagntwnx.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3oxqddjdy.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3fajfkarm.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3mqnkpbxg.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3wewlrxwd.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3exicfgmm.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3ewbwilsq.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3olrnmomw.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3eazdxvol.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3sljcprit.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3codfsufo.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3fxfnyedq.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3fxjeisga.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3agldblpl.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3jfkrigym.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3ecoxsqxn.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3jnymshqe.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3rdvxakyh.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3xoeglvpd.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3efeboocm.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3mhwfpzgn.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3sljczhjq.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3ufelngdu.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3iclpvuwo.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3sgrremjy.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ctsfcwdg.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3zasepltf.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3xydjajoc.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3komutocd.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3enqpnacw.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3ifyyrrek.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3rxpshemg.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3jxahtdyu.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3vjgyvqcc.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3pskorwwa.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3kxlarfbk.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3kfibbiin.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3gnbkvawf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xxyedksh.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3cacojcyh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3opvqpvno.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3bcnqmpve.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3gfhxnyxf.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3xvkfsgwl.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3jyccfzlo.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3dnqxowxj.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3pdtfpszn.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3nponrhdc.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3hvtihkdp.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3uytylhmr.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3fukxybav.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3gsujggdu.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3ztwngqrv.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3xidrmild.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3ssbwziae.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3ztunycui.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3ycxszyno.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3fmvrwssg.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3tmsemcyw.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3ozixcugb.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3zhavimgv.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3aylutndt.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3sevssnkd.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3apqicnbs.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3golopmbs.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3sgxtenzx.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3umuiuvhv.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3pmzhbscq.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3jnhfcnzd.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3yybuxstt.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3wnzirrbr.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3esrolnrw.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3mssbujim.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3euuifzgm.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3fcjzkunb.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3gwmfqusl.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3rorduibs.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3iueyyqjg.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3skjbhuis.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3qijqowzx.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3ffemrobu.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3znurwmzl.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3kytaqwoj.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3blmawubh.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3hgspzpoa.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3hkqlgqbj.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3qnowkezv.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3ycdhyvcy.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3thvmhpmc.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3ckkbkrfp.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3udbmfavk.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3lntflsrf.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3zzeqensq.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3sokpvyjf.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3wfapmldk.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3cihjleqz.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3onpvfult.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3wluhsdtq.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3qltfdiwb.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3oolpgwgv.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3mncoancd.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3zycdbxwd.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3kcshvaqg.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3hwqpqiiy.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3xbojjqkd.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3iecjjpqz.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3jlqtzfsw.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3pknzzsew.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3nufotmju.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3scdjirdf.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3vvvexpjh.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3psdyieha.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3izjpgyjj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nnatyajr.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3wvxupymt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qxxtwlcu.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3vwythihu.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3xjxwzzcy.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3plrxddzm.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3vylhlvts.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3vbmjnkdd.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3odqereqq.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3fqycthai.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3wcmyuszu.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3ppzggygz.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3eeehwunp.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3szrmvzpr.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3sdukziny.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3ikmzqnvy.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3mebqpwkz.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3pshbwyqh.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3nhwjtrbc.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3vqdfnbso.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3onshdins.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3jjibofjc.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3hfunydmj.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3qpogfeqe.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3jzpfxhyr.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3phrtrwit.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3crkiqnng.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3hbdsuduu.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3fsgchlln.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3lnbxvaqq.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3uyhalqel.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3mmixdlhz.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3olbigssy.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3pdywiixl.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3jmshedyo.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3wqdkeghk.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3igtufxrq.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3gvilyyvb.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3sbknycyt.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3qcoxhvyn.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xtizxrji.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3zfqkxafs.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3maswolhy.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3iuhjhunc.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ghqexqol.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3okkpvhol.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3blegodqi.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3pgogehej.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3xjxppftl.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3sytzrhma.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3hwsqutxn.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3bcuocucr.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3mghdbryo.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3nrpaerwb.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3gvnzivuk.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3zbggnwvg.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3fzqevzec.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3liyxagwv.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3pelzpxwb.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3isjpedvv.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3lelaegwy.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3vkefydaf.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3rpjniqgc.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3qjhrokup.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3qlmzzmvi.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3pgobpwxx.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3dkvixhys.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3neqzypvz.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3ovmpqage.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3bycrmbjh.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3udftsflv.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3ztlgesfo.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3jdvjzmsr.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3dqfqyodc.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3ydgsihbc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jyvcobag.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3xvpvygqg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3aibbhmgf.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3orhgpbjx.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3bqfcxxtw.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3cefiycnk.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3aeegbinf.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3jiygxgjz.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3gpyitojc.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3lvgtoauf.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3gmgarzcn.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3muycmlqw.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3kxgvwejh.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3zltmazsd.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3yzwvmndp.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3kbkblivu.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3ehwswlgb.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3runickqg.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3devzsxwl.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3hswmtizh.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3mnzqceyi.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3gkslhogi.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3lfzxzoeb.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3pbbyemoz.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3uoolzote.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3anaukhrw.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3hclmmily.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3aqzplucg.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3ktoicaty.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3pihmglnh.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3mqqkwuts.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3eoeycecq.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3zpytbxzx.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3ujykmmbh.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3khaiwfso.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3kingnftp.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3lmnnslvn.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dzqwtaru.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3glfxafch.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3whluwzyk.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3prnkfkax.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3bpfxagoc.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3gozhgszu.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3lyqtmnhz.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3usldivjy.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3pypowrwf.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3kdfwijgw.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3pbkuzvpr.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3mgewcpqy.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3hstxytrn.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3qseznniz.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3lycfqvfk.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3yuyacdrl.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3uhuteiiu.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3tzxvywuu.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3qmtbduqh.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3qhvccftc.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3dpsmwwrj.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3wubiwcjq.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3nzkwfzwh.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3luvlzfys.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3jrgixxyw.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3upwxtmzj.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3xsvtdiie.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3rvbjgips.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3mfcjkquk.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3purnglku.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3juksnozy.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3shhmzgxs.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3cdaxudjs.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3bzetnaro.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3wutexycl.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3khokthmo.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3vzvhyphn.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3nacdlpla.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3ddvntwef.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3wponlesv.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3awmplbew.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3igslhhhn.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3ajptgzak.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3jqwynfrg.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3eybawmcp.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3tcjkxfoc.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3lfcxeoay.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3prkmxooc.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3haxjkvmq.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3hmcuengh.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3gayrsipw.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3yeryzglb.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3izvbofst.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3jgkwfdlb.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3bgyweiga.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3izztehrn.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3nlhwfdmr.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3xanzowda.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3vspyqnrf.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3ucemmssa.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3sbuxphlu.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3dsxrahpa.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3dihbkiew.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3mnunswfx.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3kgndoyoi.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3lgfbpard.html


<!-- 参考信息 -->