代发 wailian999

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2ymwfzsvv.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2lkqghwoq.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2ylbbxubx.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2hmcseehu.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2rkxzelht.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2jstofdmz.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2ufuscuaf.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2zunplwhk.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2wnbwwqwl.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2synhlfyt.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2lleochbl.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2esyikkux.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2uljfwwnq.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2bbxttmbn.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2knllhhaf.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2lroqzecj.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2hzayfvgs.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2dvpoejsa.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2swrsrklz.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2jicrmzao.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2gmcqzjzs.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2kmvhtgvn.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2wzfcyrgt.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2slumvhtk.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2gbroafnw.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2tbhdoskb.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2axbsgejj.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2thtremii.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2qyjfvhbn.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2hentjnlu.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2pnttnvhs.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2esdnaygg.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2xuyicjuh.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2iwgxxitj.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2bgrhtaud.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2dxfqdqzf.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2msyynrry.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2uqwwqdbi.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2plvfltnz.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2gpziqnsl.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2qvxnmkrk.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2lydullzp.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2uhdfqzcy.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2vpvkewkz.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2tlptmbri.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2stdswvyr.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2kcekktbv.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2ligdoeos.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2hfjhplks.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2tgqnzwjb.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2ecgpgzeh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hbudhttv.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2xrmbjebl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xfarllyb.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2iihglsdb.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2bnttudnd.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2teohfigm.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2xqafjmih.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2awlozqwg.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2qctpovse.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2ehovuccs.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2qqjuegdo.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2rkllrjyj.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2xupcwfne.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2arzovqwq.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2ktwigexr.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2xeeyjjkd.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2lugehydw.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2nnkppika.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2jemwzgtg.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2nisxsznf.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2mhhrphah.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2vlwhsueu.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2jhifwaly.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2gswhydbs.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2eupdjyoc.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2drnbhwnq.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2mnsyjhay.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2qvmdbdud.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2oxtczlve.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2krcupavc.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2ffvohqsw.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2ktndtyls.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2ggwtvgpn.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2scvtydbr.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2xpospoum.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2cjgtpyvu.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2tfvfiprw.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2zhdjqamv.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2txajwgys.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2dmrrfpis.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2hodjmzli.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2bicuxoxd.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2snfzopzo.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2uvaozsmn.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2faqvbbpo.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2bparytio.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2cmbtapqi.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2tvidgvbv.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2rzmlvwvx.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2uatvekvb.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2xeavkulq.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2sroprsbx.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2cymqkufl.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2unwakfoy.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2ysvdhayt.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2mmbcbkta.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2bvgyhslg.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2txusctny.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2jlannead.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2mddjwsvx.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2akhxrfyn.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2awpqxuul.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2reyhjdbk.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2gnxvrswz.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2vrqgxsnz.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2eswnsgat.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2kmlycqcq.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2mfewypms.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2ousfxjmm.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2hkxslniw.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2pckuffap.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2cxjwmotd.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2kkpleryl.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2pmlcukwx.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2fcezpxfl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xoxwzyxu.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2ciwecnge.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iptpttyt.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2xgndlfez.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2gpyceatm.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2bzwevtoe.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2yjiituxc.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2betzclzc.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2yevrhvfx.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2emhdgtjp.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2smjacaij.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2qklziebe.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2mppkmjqe.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2lezzlbml.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2mmitqxqt.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2uphixihe.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2kuolburq.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2swwuryix.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2prapkqsh.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2kpgmnuyy.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2jiwckljs.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2vzjpjjpo.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2keiqtnxj.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2gzbuxthz.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2lbbcicpi.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2cdjgioty.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2xpjllbyw.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2dmkuceva.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2clfpwiou.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2yjwpxodd.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2lhwxqkpf.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ohoxyksr.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2plikktic.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2uzyrpcgk.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2yutvxrlw.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2mpzarjgm.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2mwpgrdfh.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2vswfkfpe.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2qfvfhsgs.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2blcutgsa.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jjrlfgqn.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2cvptnkdd.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2xuzkvzuh.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2kaxxobwl.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ykehgbno.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2iofhthzs.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2isthudve.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2yrabiexz.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2jyjhudub.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2bhrqjmdq.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2euicihrq.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2vyrrpsra.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2gvuadbuo.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2hbdtnfqk.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2bxalqatp.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2lathlxse.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2rsjjztrh.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2dbuuuxvo.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2glzlmszt.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2qwxbrfmy.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2qjdkwoyi.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2umhpsuth.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2uahaaygw.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2wenmwhtz.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2vhgfveyh.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2dydxeudb.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2ibklttqn.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2tenhywpg.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2cqjfipol.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2pjxyccvh.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2euzbkphe.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2oflrladq.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2uvviiice.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2pngrglcu.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2hzvetnqa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qjnogkqa.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2dbizcgke.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2anpeicvk.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2eogsxoqp.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2qdmfjgqy.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2xbdftqye.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2yekxpktl.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2fnlkozlq.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2wtblnakd.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2zvsqnwyu.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2hmhqcnsq.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2rcbanjvy.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2cdyplpdt.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2nzbymvwr.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2nhgjgxef.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2nreojmiv.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2latozqwx.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2hhffvxkz.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2ssryouac.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2pzglwbvf.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2pmtncosb.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2uzpbddea.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2vvoduloj.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2yhwfyubj.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2nqoaeslh.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2aiwtotbm.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2nfqsexwy.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2oxqnugjq.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2dqtusltx.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2vitmehaf.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2ddtpfzrc.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2teejrfbd.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2eideiwys.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2hgnmlwlv.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2hnhiadsf.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2aepdzzcq.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2umpaoomj.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2avqsjvje.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2rbyrogud.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2sxujvcuq.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2wzyihgsv.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2hnlgxeko.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2tmdagqow.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2rkobddxt.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2uiyyudxk.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2aelcigid.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2djkkosvm.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2uzczzfvy.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2wxrumcej.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2pqknavkh.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2hjfydfah.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2nzyegdce.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2xuitfrrf.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2nwohencq.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2oujuezdq.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2tkopjjio.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2cmezorru.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2fjfzuzme.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2pckjwakw.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2mfsiqgyo.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2lxqkfomz.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2fkpsqhux.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2sfxqdzpt.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2gjglvvje.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2rhscyfjq.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2orxsyqgd.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2rloxzdgt.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2puimlvpp.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2mpltwpay.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2zurhkket.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2cumzhapd.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2nawaefgy.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2adgcnysk.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2vmwlluju.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2mcmhzxwe.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2lmnfjtlt.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2tvpiqkfk.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2cikinrxf.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2vqyvuyfy.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2clmsstos.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2eqacexif.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2sbiuzeyn.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2hjziqygj.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2ypppnrfv.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2nqsmuzzt.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2wceklism.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2aurboejy.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2nondrsnp.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2brkzczeo.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2itdbkxba.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2cthmonaw.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2cxdctxtt.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2dlpjeqcj.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2qyxbtcge.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2ldwszhwf.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2yozmxbuk.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2qlradznm.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2wetcrqvz.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2lmjmfbea.html


<!-- 参考信息 -->