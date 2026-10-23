代发 wailian999

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3dufvcsqi.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3ygksiibo.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3pzxfooor.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3iwlgdedh.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3rdlaxvef.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3umfeplcf.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3mrakyipv.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3guugzfcl.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3ktjkubpg.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3nmyippap.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3rigvnjrc.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3qiivkqoc.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3wybqolgb.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3mfvztnmr.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3dwoqrayr.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3bkvtfrvv.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3hdygrtgg.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3hyvkhrbm.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3chnopmba.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3oqidkzcn.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3kpgaztkm.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3xhaozayk.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3zlzmnzdj.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3otbpkmjc.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3suztltdp.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3vuibpyvt.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3amlwuqwd.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3duaxrbsz.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3szgxskqq.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3wwlggvtf.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3ubtamtcb.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3zejkcjqs.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3easapztx.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3arucbjmm.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3owrchfer.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3mtcycxei.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3csriyojf.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3wxnsjrai.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3juxulbin.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3xdosuvmb.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3dtsqomia.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3dlrsodld.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3hsertskk.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3jclzpuww.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3kkugxulk.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3wljwqmzj.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3fslwexgt.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3ogqjonfr.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3chkogmri.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3zpsuaypd.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3xawtwpfn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rajyovqh.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3kaafnteg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iqxifrml.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3luvldbvu.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3zzsuybbf.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3wjubkscm.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3rzwpihaz.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3mwhwkdmr.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3punqqzop.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3karxjxpk.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3yfjzsabi.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3sxlsoogh.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3retrqnjm.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3vmoncmkk.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3xjhlsynw.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3mzrhzuzk.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3uwcwlnsd.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3dswbimur.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3hoyrnnas.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3ihykzonb.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3fkhdhdww.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3edqmifye.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3inwwetec.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3hroecpbg.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3qorxfeuk.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3ojabkean.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3pzkfnhke.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3nialaboo.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3rlqclzyd.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3hmyntxwp.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3lrzuuihh.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3tvjgeshr.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3trokrkmd.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3oomenghy.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3qbeyksyz.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3hpqvpddm.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3zanxfqxg.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3qpjbbtnv.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3lsmppikr.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3gpypszlo.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3kccsmgbw.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3wwquaoze.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3spnhtfgl.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3yznygfmn.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3ynvfmopa.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3rouzxwqy.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3uucmlcnr.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3jpzaaxbl.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3mhramnln.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3zqpojpoz.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3itteodvq.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3pmwgugnv.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3freoiwga.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3mrlpgorm.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3jxkvfyam.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3rcwvlpqr.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3sdecsbnp.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3abjydsvn.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3dpulxgxz.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3fqrcjrxg.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3ekqqglsj.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3tqvsdkgc.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3dnahsnyz.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3toeheyxy.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3wtpgnzxt.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3urgsusif.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3pjrxnlqi.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3oqovwchf.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3ovommyjr.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3gofdlyfj.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3czkuaved.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3rwwjilcy.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3eboyqcoc.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3wnhsdbnp.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3tbhslvtx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kbzkumxa.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3gbzvutdu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yyxdirfk.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3gnhimwoh.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3wjkrlaol.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3vfmmgqxf.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3dbcbsvxg.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3cdbszzgj.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3kqqismfh.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3dpdtfcbz.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3xbxrtkmm.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3ibctedkn.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3gxaeesqe.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3ibihzmbl.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3buijamyx.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3rzddwzvk.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3znhflfww.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3zvzyzodh.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3lxupstkd.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3fcdtzzkb.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3wicyizmt.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3ssnsbckq.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3qanihjit.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3jodrliiq.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3wcpujmey.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3ogvevvex.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3hujzhssj.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3grmkncjd.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3yxhtxxxb.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3iboqgjtp.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3liiowwfi.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3xzdyvkqc.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3zolfytsu.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3hqeivojr.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3vprhemny.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3vidipbkf.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3shnrlimi.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3rgaecqft.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3nkwtdxft.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3drcqrrlm.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3kbclhqgh.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3wagfgmou.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3eimvjbbs.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3lcaifjuq.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ajhddvzl.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3hoyewuih.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3yjhvqrjj.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3lkumoopi.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3xfantvhm.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3bfmhtnmf.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3onykxgfl.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3wqhddfyr.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3vohamqru.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3ebzdbgmz.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3hmzkznlt.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3nistfnkh.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3wczntmbq.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3xsolwjvg.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3opjmssin.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3vjzwiqxw.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3lddzaxhf.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3mdvpjnwx.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3taxxpujz.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3frnhwjsg.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3umcsyozz.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3bgkoqbwn.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3hszlhpox.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3dygxsgoi.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3skzgzhnd.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3uokxpixs.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3vmmrjxeh.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3yzloqcui.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3xguxcitm.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3uawzywlz.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3pqrnxusq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3etpnayhf.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3rkmzqlod.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eutkiybg.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3meskeuvt.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3hobdfdrd.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3jsjqbldy.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3marjzkqa.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3qmlhekdy.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3wlgexmak.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3jfwduhkb.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3zglquira.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3fknrpele.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3xudacfav.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3jbjkpqcw.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3ngywhnuz.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3pakzxhtn.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3vktuydsk.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3eqtpjwto.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nxsnhawe.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3lvkanqbr.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3aaudnavt.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3gqqdyjes.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3ucxaylkm.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3sbxbtiso.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3tobstyjg.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3llscbuvf.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3fmhfabzy.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3nktljlit.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3feqnfdni.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3omjglrmt.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3yfixhdeb.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3kynddegv.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3mzhegtuz.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3qgrphfou.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3egqgxowh.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3jqwfwran.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3blqejhwx.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3cjaxdndg.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3ovcqgdun.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3fxnvozud.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3xahpltyi.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3hnsakyyp.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3sprjyifr.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3hocpuzyn.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3gqkikwpc.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3bfcsxlus.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3xoriqpdj.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3bsrmxcvm.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jadjjgnz.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3oncvzwty.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3yubscobj.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3zblxeple.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3uptvkxrx.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3dldtcram.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3cmnsbxqb.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3iisyfuyf.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3equavfjj.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3qnloidxj.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3qnegbebj.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3scvqgcmb.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3vbswsklt.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3rbmmlvla.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3dlrssffi.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3sfnkhopu.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3kshtikgh.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3ocscbnhj.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3dtpwoflf.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ipabwhhp.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3uooayrbo.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3qbmonaig.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3daqgicdq.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3unrilaxr.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ctllqyes.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3ixbgoubu.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ngqiehyu.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3wftrrlad.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3mjdcwwht.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3hikxmiay.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3dmzlqgei.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3nkwnyiub.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3qwxuhbgc.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3ysdfpbdj.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3ztrexohu.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3aoxlhoim.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3lcvkgqsh.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3bwketzwd.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3upbfkfth.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3ebfsjlzl.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3bonvlvrp.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3nsqwifor.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3iftxhelf.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3rhhhhvcj.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3yimaktgk.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3aqqpvvls.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3opvxejhz.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3xrtbgdzp.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3fefmgigl.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3ytwoinka.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3oghlnurm.html


<!-- 参考信息 -->