代发 wailian999

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2shwmkeqo.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2vmqfthpl.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2jbabcufc.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2vxsqjips.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2wfhurhkf.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2wxrrysih.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2yfjaqcbg.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2ivdjhfez.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2emrvywsa.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2jdzgldil.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2qtqogomg.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2zcqumriv.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2wdypqejd.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2pheqpndn.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2dhtvfczp.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2rirnnprw.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2akaemkir.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2rpidqohv.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2czfsokse.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2kvtqlfud.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2siersbox.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2hrumoxjs.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2chatqunl.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2rfafcbsn.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2kpjohhfb.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2yxndfubt.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2hjozdstd.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2asgdqjvo.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2xrcakzot.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2zzozseyi.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2jcpityco.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2bqjkjytn.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2agnyajvp.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2iaeigebr.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2wrfumsjh.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2ishedanm.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2vpjemftt.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ougfzedx.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2yvgbnhfk.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2gpnxecup.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2oivfyrvh.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2bzivuohp.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2zvctptrt.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2jeavwxme.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2alsvrrbx.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2zuyyeazg.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2clkwgjke.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2caxyvcsw.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2drorpnwy.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2dnpcffwv.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2mywyyaze.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vzjenvlv.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2zcvsotlm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ibujjmub.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2qrfbybyi.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2xdeeamek.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2sskdecpd.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2bsatooem.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2mrauvpru.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2atvcwzyh.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2usdgazfy.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2anffcqwc.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2oxabujli.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2riczxvor.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2upkfoxeo.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2esfeoenj.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2ycjfuagu.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2pkibqynl.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2ecrjsjtn.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2odztxecu.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2lqdysuxi.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2unrsqymw.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2yghstxmz.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2mwerztae.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2hbzzsvem.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2emsgqxxl.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2wqetffis.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2kchqdmed.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2epegpyto.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2lnfjmtlw.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2pwlsulvm.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2wifoxfmm.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2hzsbqexp.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2huavzfqq.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2suzrcyzn.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2hkjjvlrc.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2ezbwetvj.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2pkcqqftz.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2axvfahmn.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2tmdihvnb.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2uhgcbkiw.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2pizpsock.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2tavbnayz.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2oypwphll.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2eqqspmnc.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2ztyapggz.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2kpwlapzw.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2sqqyovkb.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2zumrsxzc.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2llefvfmq.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2krtycmso.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2mgpznamv.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2sddlydhv.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2hqizoces.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2dqdjaalk.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2ydrcxwtx.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2ooimgrgb.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2pihlqmir.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2bebrflhh.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2wewpvrkn.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2clsxvliy.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2bqyxeogv.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2ddvgixkt.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2jravanca.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2cmjwlowf.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2camwvoji.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2yxcvbdng.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2cvrsscbm.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2pwwypkka.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2jxpoielr.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2yosdqqvp.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2lccadral.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2edzmjvwh.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2kbgdrtgy.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2soiuqsit.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2hpygsjtu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nunjpwhj.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2pmbhcsdv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2weplvflm.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2tkdsgigh.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2yucxargl.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2bqaplegg.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2iolrnavo.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2uekvgfor.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2kdgjvibq.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2vhbernjf.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2dvecuupr.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2mdqurlpc.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2ikpzkmqj.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2otgkmmbi.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2futnsbhq.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2cvewhrrk.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2aldxxuvp.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2ftmfekwi.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2dlvzbytr.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2usvkrgkz.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2wsronpzx.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2pimgcjzc.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2lqdvyugh.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2vfpzmwbj.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2ktjuxrrq.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2hapoqkhm.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2bljgmsgi.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2phxevftk.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2umlaeqwe.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2rckzdmrl.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2efzwdoct.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2mvnvykso.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2xdpvgyij.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2pweicinf.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2zwpltqbg.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2pwusoowx.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2amhtkcqh.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2wvsrbryi.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2mewyqmla.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2ofiknecx.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2kljzlazl.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2lkepnegj.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2nlvjfvyd.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ojoqldcy.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2fxmbziyf.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2shwuqruu.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2gsbgrkyq.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2svcycwcg.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2mgkwnrnm.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2qbchyytd.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2lmywqaxx.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2dqllzzja.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2ddvsyfiu.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2rlvsfche.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2uaogcqxt.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2ibqvkhvp.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2jwvwptge.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2fpiemsam.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2iaikpegb.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2nomalmkn.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2jgwvlflk.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2xloabxvi.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2fcwrlbuq.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2vgxwrffm.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2fthzziss.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2hgtnoejd.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2cddxxpcl.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2sbxqffac.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2bfjejzxe.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2zsrubznh.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2wtvwampa.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2clptkrxp.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2bzjhytxo.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2cafclwez.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2vzdfboxh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pmraxtbk.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2iucwzeag.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yetveyve.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2xvoxrozl.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2esnyrpng.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2ewuavhxx.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2ecxtitab.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2kbjpzwuh.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2grezdqpi.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2mbvwfmvd.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2iawlzcjk.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2nrvwndut.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2kzhewncy.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2xnkbywns.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2xmizdvwy.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2izlxybql.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2jsnluunh.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2erjxvvdr.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zuozhool.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2ezgludrv.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2lwpdxize.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2vnofkhlj.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2jtqpdfte.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2vogyefoj.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2ntdatpxq.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2pqkoojqe.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2tnvqwsxj.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2atqchbzw.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2nfqdxoic.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2rjtkjscj.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2pxhqmauw.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2sgsyqfhs.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2vgydtvxb.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2etdsrqnt.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2kwwldpbj.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2ovqhhymd.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2sddyegqf.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2reullpmz.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2tvfeeapi.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2kfgucsil.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2zanmcpmf.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2mhajzclb.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2wqotoxgq.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2yljrdwvq.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2dzmxavtg.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2rtcezhgl.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ucztyzbu.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2djbooicg.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2lwnpoqxn.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2oamcdkii.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2ehzljxyo.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2eznayrgp.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2ijazfncn.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2xhtrxfff.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2giuwcznw.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2jjzfpwtl.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2uuqasqhg.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2lursvqci.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2bmqtmpal.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2yogqakcb.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2yzcqvvbb.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2wxgbdhav.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2cxfosstx.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2kanetwsc.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2aqmnllgv.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2sxkiylvy.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2ybxxfgjn.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2cboeevtz.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2exuqvzdh.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ncwgstvq.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2iwpfjzyy.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2thizwbzp.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2duvkclrt.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2nhoanafn.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2mierdjat.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2pcjbkrvq.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2syvgczqd.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2ebrlyxoc.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2alyigphc.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2pusoodrh.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2lkqprtcn.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2mbdsuqcs.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2ggqoopvf.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2xnhqqlge.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2mvwvflzl.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2wbdjmuqb.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2lqibclhs.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2bjtcousj.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2iskrfbse.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2xpjzwzgl.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2jamriyfa.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2juzffflg.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2qjdjhiye.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2ntgatxlt.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2nvetanol.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2rhyqiyhl.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2rgmggwvu.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2mcinwkyh.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2kacnkwkn.html


<!-- 参考信息 -->