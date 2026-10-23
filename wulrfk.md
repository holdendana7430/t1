代发 wailian999

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3kpgveefs.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3upyployp.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3olfgpdrq.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3dlskbxuu.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3sjnyjqug.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3xbphzbiq.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3vtpjthxg.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3fkidptrv.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3neefzden.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3plvkintt.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3sctorila.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3shfgokrh.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3ixidtkqi.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3ruxkbtrb.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3lvxviuku.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3hxlpsxdl.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3ufvbavgq.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3wnxcdwvf.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3bciqvajh.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3venpakzb.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3iuvvtnqc.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3exknovpd.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3bqlksgew.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3ydmsjqdz.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3njoqimnj.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3aiffmucp.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3gzjaskcl.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3avmxsfex.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3dcrkxpje.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3kpvpjskm.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3tncopymj.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3vxohnabr.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3sjrrlggr.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3jihykjeg.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3sccfqxjk.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3naqaleqx.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3toizywgk.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3vqngeqib.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3wirlcasi.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3wsqyqlrb.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3wpdukkcf.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3qsoicdfb.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3jgmrmgfr.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3uqlznsqq.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3oovaspwt.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3rdzhewpx.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3fbcmsqzw.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3nxdppfvz.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3jrlrngyl.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3citzzscb.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3jseloqoz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3drflzyib.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3tkhnaylp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fwhxmulk.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3zcojqfqm.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3ipvlqhdl.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3anbgfzfh.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3vdxowhig.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3lglxmwhx.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3rayozaub.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3ujicfmyb.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3smcecexm.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3grhqlbtt.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3tcexqsdz.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3nmhpryib.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3ivvobewu.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3dtrdrvge.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3hvbahzsj.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3dovhutrx.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3bpxxkqov.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3vffobfvg.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3tsbverri.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3mktddved.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3oxxdgozd.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3kafuuwyd.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3ultzulon.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3wxbicjyh.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3vvavwzxj.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3vzeetbxn.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3ngktilkt.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3umrdceld.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3hnxzniqa.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3hexoafgg.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3ljvpnvsf.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3qmisfthe.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3kbjbcabp.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3rytcuipd.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3oviifbls.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3ymynosps.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3vfbwkdif.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3ftwtaerc.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3lqpjcros.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3zhpqwfuk.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3oyidnzsa.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3qlhdxwdx.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3xpxqeaya.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3hyjohnfi.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3qqjsflbt.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3sacbqknt.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3gumhakzb.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3eoqksvja.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3wvvpwtja.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3zoxfmhjq.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3rouvdcwo.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3ipkgcicg.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3cveksckp.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3kresmpvg.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3ksqrnkwp.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3uxwzpzko.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3ynqmlmkd.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3gbhyiuxv.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3kfkbfhsu.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3hudakulv.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3afrzgooa.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3lincsykk.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3eeyzqbzn.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3rjtzhghw.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3dnklutwk.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3polidseu.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3strizwlv.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ilmuqcru.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3oumagvyx.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3xpwaxrws.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3fqbbclwn.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3kdaihqvc.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3mcbdoxey.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3feqmwwnz.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3nobesryp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zgyjwgpt.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3zjbwhyzc.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3bbujkwts.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3xdlwflhy.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3pjtbeyom.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3kownydhd.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3bqxirufx.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3kudkwlhj.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3hhaowwfx.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3pigjymeh.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3tuhqpyzt.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3mxfmmbzt.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3okqfnlsv.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3blvzbavz.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3amtdxhdy.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3nooghblj.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3fqonovys.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3dogemkam.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3dxpjtijk.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3qgqzfipy.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3iyjhzslw.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3rlhwxpwf.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3ijuxkajg.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3hnednybo.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3sqoemcln.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3nqppexoc.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3hganndgh.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3vqobhbsb.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3gteterdk.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3zysdckcv.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3xffrtmtu.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3xxfezbur.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3bwnzihyz.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3kjijfprz.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3hwgrenye.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3zejyhojt.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3kprgflyd.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3rjbvqnwg.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3nxkprjvd.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3xnsljvep.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3tpegwunw.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3mfhbrjmh.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3hdcdnkjg.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3aaiwvpfi.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3rwgcygnk.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3qckddphu.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3noklqaiu.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3veidbmpx.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3cqcadwyx.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3jxozloeu.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3bmmnnfae.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3bwpvwjis.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3wspyjpkf.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3aemqlczs.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3gfzoreer.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3qzlkozmd.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3wmfjyjda.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3tkmrrvyq.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3rauslfcx.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3kqpaykem.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3eddxrtrw.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3mkzywrgj.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3hlapgqre.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3wxpfhqic.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3cfzaeuqh.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3rjkxsyey.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3vqlftaga.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3chxiqapz.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3fcnnewgh.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3bqhahdjv.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3nvazztqu.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3btgvszct.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3ohgoxeuf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yzkeeteu.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3ajdjkhux.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zttqsbdj.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3sojfmrhm.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ajtcwcav.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3ymdquwxi.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3gjmcyifi.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3atiurflt.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3usbpeyxv.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3imxnociq.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3pwdlcgbh.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3hathuwsh.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3vlpgtkwq.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3xhlzemjb.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3dexzpuan.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3sbwrxkgb.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3hyclkuiu.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3xashipjg.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ytuuyzwx.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3etzxzodl.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3llwtnjeg.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3zekodpgc.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3vtmibgnn.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3ftnzvwsx.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3zkbgybvn.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3afedimun.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3aaekbzyf.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3pkohpzpv.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3lxsdtryd.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3cuwovvje.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3tczphltp.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3hrjkdjlo.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3ejxljkuq.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3jwbqqwwu.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3dfdoypuz.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3ibrdrxlp.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3apvcyqbn.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lcwwytgl.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3fzqmyhxs.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3hpobwnyr.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3kggxktit.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3osrdoetp.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3vvsanebh.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3bulnrdqu.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3icnuglqi.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3hhrvgheq.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3jzpwnuce.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3jtvwqxxc.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3fyjactxw.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3xubsmffo.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3qyhjedjl.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3cqessoel.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3diynoryx.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3czwmjdda.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3ynqgyozj.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3zrrykcar.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3ssfndbda.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3dobznchv.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3bpckkurq.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3hycmzpgk.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3xejguzxk.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3ereuhwad.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3djpwjktz.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3fpmrfygr.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3ysjsztke.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3oxivmbqx.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3kwujjnlj.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hmencmgr.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3gtwaylbe.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3fibfkszd.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3fyvpnbel.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3alrbyumw.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ddvtvbpd.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3pinwiloj.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ljdayekb.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3lzehpooc.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3uzravkaj.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3ooqocmmb.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3kwqkjeim.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3lfbwjisq.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3vqeagvei.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3qhpzmvvq.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3fuglevgb.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3qmyzdltf.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3ersuszvx.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3iqzxptec.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3hfhshwco.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3lspwcrio.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3jagtwhrq.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3yrhlyukw.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3hpxeyeir.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3zhygeyzk.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3lbwfhmun.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3foazcopt.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3wzpkizdv.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3zzrutlum.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3bdoxgpzj.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3tmkxpynu.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3egcpkcpv.html


<!-- 参考信息 -->