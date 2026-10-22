代发 wailian999

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2jpsjjuhx.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2keirxnxk.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2mhfdadlp.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2bexscjkj.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2nkpgywoh.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2kadxjtip.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2sbvpqwsf.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2syuooxrm.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2mvcfmvjh.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2ynfntbsu.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2ntpnyrao.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2aqypncli.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2fwrzmpwe.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2gynhlewu.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2phtknzdw.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2qruoawtr.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2mimjkabw.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2obsmxamk.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2thoacbdq.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2jxvfcjtm.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2ncwsphsy.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2vkxhwbhz.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2ncqkpque.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2bcgbcoqr.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2dlmmfwal.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2upahophy.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2nzxjqhjg.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2rfiwrsfh.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2yddpoqmn.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2bbbhgxxc.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2updwvbmk.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2rejswusr.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2dlxnpotw.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2uafkxchu.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2lmiapgxz.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2waridgjb.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2lpcvlyoi.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ikzezwxw.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2hgroblma.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2altziyua.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2wulymuji.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2xrrtiaqr.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2vgqhrbdx.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2zmvadolz.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2xzptckes.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2tbhqbjuh.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2sziwydvc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yrgetyji.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2oqdnonnz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wxfwsbma.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2whfjnpgs.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2ncsnqgvc.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2lmgrwsxm.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2xanrcloj.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2kwiyhpgd.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2ibkodtxx.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2gugsakxl.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2lvrxyfgu.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2fpzgtwdd.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2dfdgxmyl.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2wmcflczl.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2tmernpwl.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2bmukypkj.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2sjnqjnvj.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2bysxszef.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2xvybwlng.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2zhmwmtew.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2iuofzirt.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2waatzpex.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2dhekypgs.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2dgqcxyrj.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2hplxoitb.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2ilizonhq.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2xwiuvagi.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2figsbqfm.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2scgrblhq.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2apmrbusn.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2fyjtpwic.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2bbanjutp.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2sjoruwfg.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2ctgydacl.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2bxfrfpuw.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2qitzkmrk.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2zmqfmoyv.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2prhsrvtg.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2kpdiltxq.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2kirquyke.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2haaaykic.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2hgvleola.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2jbxygkxp.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2zbxfezxo.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2ylifysqw.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2tfdfwwxk.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2knowiawg.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2wpnlzahn.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2hvisalga.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2qgdsaiyv.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2rdmfynpy.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2ebnvktvi.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2nhvqcnnb.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2eaquoorm.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2qqhaflab.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2rnlxlgwp.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2nfjvvrkr.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2fyuncroj.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2opktcqqq.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2qcpdxtjj.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2qszslepr.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2dzlceswb.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2yydmpofw.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2hqdwfhaz.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2vzihsqxk.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2kjdmyjnk.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2kwrntcgy.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2kjgffycy.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2nlrfvtvc.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2mxiycpft.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2jbwkqvhf.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2ttgovqin.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2pamdgnlq.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2lcbuxrvn.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2gvzuqais.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uxqfwnij.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2bjemwuet.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2guwiltxh.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2vpujqmye.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2pkaczboi.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2znwqznpg.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2cwhkqwbp.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2leckbbrl.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2myjqdevd.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2pffmagmg.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2fcaropcb.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2pziiemui.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2xhnsfmmx.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2wloeaimo.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2zhmarrlp.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2ysxwyblw.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2skjjpifz.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2xombagvs.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2elzzuxgh.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2nyjbhnjc.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2nniivltv.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2kcgxcxvj.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2dukmebba.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2ieesyzxi.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2udrglsps.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2lmjhjsll.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2xxchhwyl.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2adhqrvyq.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2hsvvkeub.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2mclabdkg.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2xopuzoln.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2srfcnqon.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2liwhuiow.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2urqbsyob.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2hnqpowry.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2easgsqdm.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2pyelkndz.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2hcrviiea.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2kxqgyvdn.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2evgifdau.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2cwvexdso.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2mofpxiay.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qypdnyiy.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2awlwiffs.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2lnkarfyo.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2aarwgayo.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2yceaigoo.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2mmwltyev.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2khdpjojc.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2uudfffux.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2oyfipeti.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2ojeznelw.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2smhdbwgl.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2dkibykon.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2lguuwpdr.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2nrivcvdx.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2waestsms.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2oladzldp.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2zxghduri.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2odbwoobd.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2oowmlyoo.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2iyyvsjuo.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2semzwgag.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2gqmahgjd.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2iudwyeqm.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2lkdasful.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2hgzluvwz.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2yyslxyqx.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2gnrmoovz.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2hhnbopzy.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2kgfsrdnc.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2oyjuhohz.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2ydawtaud.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2yhzstzon.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2qzwirgpt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ihawefmx.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2ecwcowtn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bdeevrve.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2mimlgokj.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2aiozixko.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2ksihlcvx.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2yiqygptq.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2cctptllt.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2vdzvdyyw.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2cklctqnx.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2gopmbeyj.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2xcunyixg.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2kuiwistd.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2hsuhmauf.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2oqonzlkb.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2rfwzrnra.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2nglpxbat.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2tnqnmasu.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2kjmewrds.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2kjmjwjjp.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2mtclvrbo.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2jozjpamj.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2imrlaazp.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2tnolhraw.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2crrpboae.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2ziknyzet.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2vqsaqqxm.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2lopcgcry.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2hukizmil.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2eefgdhlr.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2vugentng.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2qzvaptau.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2tqhcdvxx.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2gxbclanc.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2cewsussx.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2fkyzjdks.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2kbnxtbdo.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2kdmpzlxb.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2nuhmnvpe.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2mjffhdkw.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2wbehegeg.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2otnllvgj.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2bwqkzeqj.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2lvuradko.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2kdtxzvpb.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2jnydkizb.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2daoxsmev.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2nechocfz.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2kamaxzwq.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2yooscczu.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2wdhjvfnv.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2xqkkzbiz.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2zefwovkk.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2qtyjxzko.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2lewstmbg.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2prplrvwx.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2yxdbcgbh.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2uchqbnov.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2hawtgato.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2ptdrdpno.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2hzafchks.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2ctdoiwqp.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2mkvcxgue.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2udrgypro.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2enlafaim.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2qebcehdr.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2bscifnuw.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2wtahtepp.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2fmczvmfl.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2uskyxhdh.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2uxoefnzj.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2gmtnmhzr.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2kzrrlrio.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2jwvrcpyh.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2neprhvjr.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2msvuxhyk.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2gllxarho.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2lravceio.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2frfphlwb.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2yacaxgzw.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2ebaugyqm.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2tzbeajhf.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2pnafandw.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2abayauig.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2gqsldbka.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2lhtrqbfk.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2ryfmslbc.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2iegkjnrc.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2emksnigt.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2tvielvvv.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2gwoiwujx.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2qyvjftux.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2mnpdshpz.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2ggejlfzb.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2sphndsei.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2kohqrlml.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2iazkbsql.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2hxlwgius.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2eylyxzuc.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2olxaswfu.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2tzilmsgz.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2quvoqbpu.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2urxcevtx.html


<!-- 参考信息 -->