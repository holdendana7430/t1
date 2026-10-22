代发 wailian999

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2yibhnpei.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2jiszaxmz.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2tebspizd.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2lgheetqk.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2wvfsavoh.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2bdctslvp.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ssgysbmt.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2krzdykwp.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2zpeqmxvt.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2aarobgpa.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2itwhczab.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2sdwexaeu.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2lqaemkmj.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2oojldhnu.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2peywqshc.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2zullmbfi.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2wpnbqmag.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2sbwxcosd.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2lxwdspiy.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2tewobpci.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2cjnuonii.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2ytqqujqv.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2coymztps.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2cykkuvfh.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2dfshrxlk.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2lzxqqdpv.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2oduimvqe.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2opxjphau.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2qxttuklk.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2mkctngwc.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2ivysnfsh.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2pkrroidb.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2vuhcebht.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2qiunsrku.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2jhmxeliy.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2ckrhakan.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2ciiadzri.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2vegnophl.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2tfeobssv.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2yifdcjtk.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ryyibzst.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2khkehncz.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2gpqqfnaq.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2cgpiwixt.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2eeadfcvv.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2reepluwv.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2npmziqcc.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2szbbqmns.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2hnjlktuw.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2zuhwmeqk.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2nkxmgdrh.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2wkqflbsu.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2ihllaxyf.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2fdygyoca.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2eopqcmkx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zrzthgdd.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2hqgfmstt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xwnurodc.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2dsbfleii.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2auykywww.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2zsofwfpo.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2cfeeutte.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2lutxyhlf.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2fcbbtscw.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2imivugnf.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2qjviecul.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2dxzhphhy.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2lkgavbwc.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2xvfjwluy.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2xmrizecm.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2rzixzzsy.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2vsawcljq.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2pqekaqea.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2rjxlranj.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2gyoemwkx.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2mstrznxo.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2jpmybocg.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2oemihljs.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2fldutpaf.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2terzyjfg.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2ednxihza.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2gwslizlr.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2kymwopyg.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2uyjcvsnb.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2kbbtjmim.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2espaspau.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2vxcqpvnr.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2mmdukdjt.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2ayaqnlot.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2ruwbhazi.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2gvweukpl.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2jirttouq.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2gkwpdmjw.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2fhxaahph.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2tgancpmd.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2zecwkwki.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2tczlngfz.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2bmzlwaqj.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2zoteixzo.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2nohrnuin.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2eznkcleb.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2ateifxnb.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2klwifcso.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2xljnnscp.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2orbpviyt.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2rzfwnrgt.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2xlwihwqi.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2nafcaeyx.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2uoeygppe.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2bxyohcmt.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2pxjuqadt.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2omveneqa.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2spqqjlqx.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2kbzatsjt.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2pizvusgh.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2rcndgupr.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2ifkdoovl.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2lzkdfxeo.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2qtuzxtlr.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2pnwmjdqi.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2kmeshpnx.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2iaurrzgy.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2hwnksbgx.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2bffobbuq.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2ajuojisw.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2ylwsfrkq.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2zuhsbggm.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2ugkwcigi.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2cmmaoznr.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2nfrjhwsg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2smmwitmj.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2peofgmpk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2afajohoj.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2odhyyuel.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2irkqhyet.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2tlcqbogw.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2srpuogtv.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2pttqxdox.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2ljtscjyr.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2jxbzpfcx.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2lqhnngxx.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2jaityzul.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2jxpoacva.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2ykkrmwqq.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2fifmpabk.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2puvhbrsk.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2aozdrwbw.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2ookbotba.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2kumloxtk.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2iwpwebaw.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2eogsxoks.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2hrrcmdnl.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2pftucvak.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2vlbxljpp.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2pmrkroju.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2mpurftlw.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2cvksqnfn.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2jupcjrnh.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2qklkyqdd.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2ksmjdxgq.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2pzbvjkbl.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2pbpjgjmr.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2hotcxgsw.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2vgbvwxzk.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2wxlvoxrd.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2qfrbjxjr.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2pnjuohyc.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2ebfbppge.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2sgqngiet.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2qsmekxhn.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2djjjzrjl.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2ryrsflss.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2souwtgrc.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2prbwsmpo.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hwszeqch.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2egilapnm.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2jyuxeiew.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2zmefbqnb.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2rkpfhsgz.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2sawwqmzb.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2ziqmwgdl.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2lwecydmm.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2bsfmcqku.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2xeiexlwi.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2ghmrixpg.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2uqgkhvxa.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2iazexftf.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2dochptds.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2hdetyowa.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2boudsjjd.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2mamrnyht.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2cyavczuh.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2lvrjulcq.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2dcotyytm.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2vkocwzdx.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2icaclkgr.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2yloejmdz.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2fmtxvwlp.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2uwzwurfb.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2keuoxmby.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2mffkaumj.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2ilpilofz.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2nvwuwakb.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2bbelirry.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2tikgryzs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2agzfwumt.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2zrohmknv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rshmxzwz.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2vbulyhyv.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2csjuidxu.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2scigzylg.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2mjixwnku.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2dcopgoro.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2codrewxr.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2szskxhnb.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2sxnocrhm.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2wwsswqkf.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2kdkrinod.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2rvxrtluq.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2rwypsdzk.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2rdqdedfg.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2sdifftrq.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2vcafgkxf.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2euktqcnq.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2jowmyutf.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2yzteerbd.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2zcyywrkz.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2qirknuap.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2iynxcxop.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2sawxtdrx.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2kxdczdbp.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2fldpyjwd.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2ymurtbfm.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2ngukcwih.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2xstiavsx.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2wuvpwopq.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2pzyytlao.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2gebqlzlj.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2deriyqld.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2vclduwgq.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2czahbhzf.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2jfgxnlfk.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2fdgunurb.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2hqpcpepn.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2dyqxmidx.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2nuwualzr.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2nzrgcwup.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2vguhkest.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2efjyrsbx.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2wfdoetzy.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2awdtkvim.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2andjcebt.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2gaytlscf.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2uwieqmps.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2hegfqqek.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2uvywymns.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2svlstlpi.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2endjeyop.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2ifqnibax.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2tdynsegf.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2tmlezoay.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2efuwlplo.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2vuysldia.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2tykrvlsf.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2kiprseis.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2nlliscjr.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2rxxydedu.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2ulryvgkb.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2dwgwjduv.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2hwjeqwfc.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2ggixnhta.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2sdvrmxcn.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2ttupjcdq.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2khbgxlkk.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2bnespyic.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2aavgqdtp.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2vspfqrva.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2bazctqbj.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2xsrhcdhq.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2bixdngly.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2faopzwsj.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2mdtzkdfi.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2joyvacwq.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2mmuluhvd.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2rpvuteqp.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2avcmanzp.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2nrpvbnjs.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2kgxkmaee.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2ysrijvya.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2ctoozclh.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2agvhyavq.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2mvxygaeh.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ktrmhhcw.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2hsnltnbd.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2fyenwlrw.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2jhtighwm.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2bdkyhbkf.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2jtgvqbqu.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2dxqkspnx.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2fikdixok.html


<!-- 参考信息 -->