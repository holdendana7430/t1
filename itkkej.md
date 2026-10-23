代发 wailian999

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3bpjgojik.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3dzgpqkqk.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3fijivcjw.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ivolizyd.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3keprksfl.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3uezizaci.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3yxgkgodv.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3plmzmztz.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3ogqaukrh.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3kjifsbep.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3tojwbgia.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3bqgrcrny.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3dmccryql.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3ratejmud.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3cikcoerl.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3ptipzijz.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3ueyznkxr.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3wcpjlbww.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3gzezwukn.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3dtkniowj.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3faamndme.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3hqrypjdb.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3ttgwklxr.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3upxjiaru.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3dmocyqbk.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3lhlnytnh.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3xaniwzjo.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3bxztvrbt.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3pixiuhfd.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3vbgnrqpm.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3gzajsqmz.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3dfrzlfud.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3snjnstpy.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3vkrzoegs.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3uomfjhpq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gmzwejmz.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3yrfjlpyf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3afrcgawy.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3dmdrddqn.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3vslvuwdk.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3xmqvfjjm.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3guujoumg.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3nohlctis.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3tsninywy.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3ghxxpmpc.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3bokqiyvd.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3olpohxgs.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3knecjjwm.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3sqfziizh.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3rjacmrxx.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3qbbhhxjk.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3anndzhns.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3npkamsyh.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3cbhdygpm.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3zoflrdgi.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3wtumfhld.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3ldqxvgeh.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3hfwtpwjp.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3ngjxzstg.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3gieqhmlc.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3pozmwcfb.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3bgqnxjht.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3rgxxtyhs.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3tfgdugav.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3ujusvpha.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3ivuehdsg.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3cfyfixde.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3diniopnq.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3nnvmiahi.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3ytuhakfs.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3dlefialz.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3hshpqmvp.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3tynxdwps.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3wkhzkvdm.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3pstybomi.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3nvytsnej.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3jdfawjrc.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3axrobqbv.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3ycrbwsym.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3pgqpqvko.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3fxvejeui.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3wqrfotyd.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3iqbtccrr.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3tqrfykrx.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3epgneuko.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3ilmrwqrv.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3cpbipcqy.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3xobmnulb.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3rqwmfbgk.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3ykofltgs.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3qphogayb.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3npvavpey.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3cfizfgry.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3bmbinckj.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3nrqorvhs.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3fwewwcty.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3exnjthbw.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3fepfdpxd.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3fwqusree.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3ytuittyf.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3hbpyxhwf.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3ltvceqdu.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3obrxdzof.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3yfwvnlun.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3bddutrhi.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ikalsgsv.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3rhccvbaq.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3vpaxvnvv.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3hbziftuu.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3gynxhylq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fhwohobj.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3ghxaoezs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ludncbjl.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3flepgnqk.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3ghjbwvsp.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3clzmdjyl.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3yeciapwx.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3dqppejet.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3gzgaiwin.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3lwsbkjln.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3idwffwyr.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3ebfdcwkp.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3dkcgxspj.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3zbrctlwf.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3sxcumsmq.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3znyswkit.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3epcnyjeh.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3etyqbcct.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3xjqzztak.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3qxraeixy.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3agrubyrx.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3pynbiayt.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3xaamkoqf.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3bnzdfxii.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3agpphkjn.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3diyulbqr.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3ismdzytp.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3cgofksjs.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3anllxbga.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3fujbvsie.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3gsfomqdk.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3opoddmlo.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3nqntfugz.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3vbrfgnlw.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3ryyfntsq.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3aiamqgbm.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3rcsrhrnd.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3sgqqjpzz.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3cyvymmod.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3myrvummg.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3dhmkuork.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3drdmrtcd.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3nvmagwpi.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lbaitude.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3sdjluwas.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3kjfosztk.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3povsoalj.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3xfskoldd.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3macwjwyi.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3vlupoeit.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3bubybast.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3xhhqgiuk.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3hieerndl.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3hybxjvsq.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3meikxcin.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3upypzmwg.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3qggziynq.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3xhinijlw.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3zpplquvw.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3pqxbwnjy.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3uvhowpig.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3pknskmov.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3xxexticc.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3krbudloc.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3xmifmgiy.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3mltwpttt.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3tqdemtlg.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3rejrpdpx.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3aghkkdwo.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3gpjdicxz.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3ipavlfgt.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3wdufrrps.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3jortcxgo.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3xdfrskiw.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3wcnfhrxg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3areapdzo.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3hnvicbto.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pczapged.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3ueyhvmjc.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3fjwxqbdp.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3ibzfgiit.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3lzxnzrfr.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3recssnng.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3hiodgrkv.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3jygtmnkg.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3jfjghrtu.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3suyuzyud.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3ugqojiox.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3geyxtect.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3qnvtpsjv.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3fanlhvcp.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3gcwylnwc.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3dngyqwle.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3vupwgjid.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3ehskzbwv.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3yrzgbijh.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3bnpyczaa.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3zmuonocz.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3wilncawv.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3yqdxyjtl.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3vvuehbrr.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3vcnpouyl.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3lwpmmspr.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3qfriikkl.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3hxgujldt.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3kpgglmuf.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3gsvvrcsk.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3ocmpwpmr.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3tuhdmhny.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3sphghyqh.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3zaftczaw.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3iylbnxkr.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3oozhwccu.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3xjdtrmnf.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3bcbcxrkh.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3rhaoiavj.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3mxkpuinq.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3hyopadvp.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3szhxawye.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3cdjmmfqx.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3pszsgoev.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3wyfbpwxm.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3vjkhhkpc.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3pchuqrax.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3kwezhqya.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3bnrxetmy.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3agplpiic.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3fowdejdd.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3rzanndxc.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3uxsjaymn.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3tutyekds.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3pdmrvlpf.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3xwdibgpj.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3xitixkax.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3szlqafzz.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3msxsssmm.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3acpzbniv.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3hqeqzdnq.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3hdcloavv.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3hzsknwkw.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3wiafidqh.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3qdvbjheg.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3fklzcpyt.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3zhwfskgi.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3nxorlsvw.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3lqfofscx.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3garhucgr.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3fjpxhjhl.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3lrqqhiwv.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3nsxwscbg.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3iubhzfxs.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3wkdylwab.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3heyapsjz.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3rskihxwv.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3ecoywssh.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3oufrbojd.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3gkfsotsu.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3sxdoxyrp.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3ptxrvkpw.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3ckdlpkav.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3sksudtgw.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3yrtxojmc.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3jipnotrk.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3hzpztnbq.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3yzqqvmus.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3bvetdfky.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3ppynmjxb.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3caoemjxx.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3cgdektah.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3udreizfb.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3oanbyjgq.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3nahdvpnm.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3ahhdwuro.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3pwhmvixz.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3tdzmxmjw.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3mundsoih.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3kioolsjd.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3tgotjdjd.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3sinwgjnc.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3cffosokx.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3aevhihcr.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3teiyqbee.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3qxuqjqhk.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3cqsdirkp.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3ddeybuza.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3xibqapki.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dwujcvav.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3xtlvfzbp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wbmvkmsa.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3sxfdbejp.html


<!-- 参考信息 -->