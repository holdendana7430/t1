代发 wailian999

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3jvpxinud.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3ucfqwilt.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3bcipyinu.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3rcwmlqlk.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3ebusggqz.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3deypxgrr.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3qeeoskcl.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3ukrtulpe.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3rkclnpah.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3wcgekytu.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ayzdrcni.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3mhnphzdx.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3dzhtblch.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3jsiwtska.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3rjwmuruj.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3btahbhvr.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3vuqgdnaf.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3otjaonjq.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3fcmllojy.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3keawufzo.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3afutxazp.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3bkouonoc.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3nurtefbx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rsxakvfk.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3xibdowbn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bqnzwdjv.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3lrfrfjcf.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3mukoenlm.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3fjezhyla.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3jopqosec.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3jqsrqnkx.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3fmmzyvrn.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3vtcedydj.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3fffszeka.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3lmhxomgt.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3yfdcfxjp.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3lppsphun.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3tpijvtyg.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3qckicwio.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3ajkyqtfc.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3kxdaccfr.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3zblsjsuy.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3muqhsebz.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3izjnkokb.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3yovycuoz.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3xgvtgyqp.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ewyyweju.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3gjexnxtx.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3aydqnffj.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3yevtshiv.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3lqkaemnq.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3tgagdznr.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3llnvlxan.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3mbnkipvl.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3mdhcnlre.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3eynrswlo.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3yfyigbxb.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3shcsjfso.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3mserlkui.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3sooxajmq.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3xumsnzsf.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3yjxtubyz.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3mzrtvsmd.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3ajirelku.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3danmcofd.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3vbbdenay.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3tuujqqhy.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3shcxrqwi.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3krhvgdes.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3zagciuim.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ntndqzkq.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3owkpgjoz.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3wglqyudn.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3tqvbpdlx.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3rmaurpyz.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3icfsrbzi.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3hiizrpdz.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3upwxxihw.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3whirabbz.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3oxfgpvsj.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3yfczihxi.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3nhvrphbi.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3bijnffix.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3hkyliicm.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3daxxwghx.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3orrimpio.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3wrnmrgle.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3hhzmzptf.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3fbghgdug.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3qgzffzfw.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3cxpxcqin.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3qhsxrlhg.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3xnizcufn.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3bskqluch.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3gjkzhxbr.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3nanninxi.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3yptqeltm.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3nanxjogk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mpvgresk.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3stdlsidh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fmxtwuuq.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3kpzfarzq.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3mnjbypzy.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3cvbyngzu.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3zbqfzeqe.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3cmofulbi.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3nqcuwjfa.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3lnenqmff.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3amfkcewq.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3icmvbntm.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3fvyhszmv.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3femqqphq.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3airzhwwa.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3xruzhzax.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3hvdojkrl.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3pbhsuduc.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3ifzenogh.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3odkytsom.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3shnkicrp.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3jzncpqhg.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3lhmlszgw.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3yhtpmlgc.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3hgjzbate.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3ihqzpzgt.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3pkfollai.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3qfqtahdi.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3pqzeowuz.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3lkaablpx.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3itgfypea.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3yfhviiqm.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3wqovojfj.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3koctwyuz.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3lbrnechp.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3wkvziizj.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3khvzicsg.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3dkchcbfl.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3dmljjklv.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3pxytzzzh.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3pcantatn.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3wdmwogsa.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3dfgqxjde.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rrrebmxb.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3oikyflvm.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3qlardvaj.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3brtdltvd.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3oftqctul.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3puzbhlyy.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3uvpfswsh.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3hzvwdrch.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3uorytlvj.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3cyyxbixl.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3zedavbgr.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3jeodwrza.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3hbdkfywp.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3cwdjisvz.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3mrpckupf.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3girracde.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3qyzjijnt.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3qogytagd.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3qzaqvyzq.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3itauaegr.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3rnoojxlc.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3tiajluyq.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3ejpeimpq.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3ovsmbocb.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3lnaadvwx.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3xwfdkqba.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3cnkvkqpu.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3srxyizek.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3rjfevnev.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3jtvzinjr.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3rxpzbovr.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3qvigpexm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hrtyohcw.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3yrazwxew.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bwxvnvel.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3ibokbnnq.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3pwbokqnz.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3kibtcuow.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3kxcsrfyb.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3kgmgbuem.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3agsmfgjk.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3sdocsrej.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3bbhfbevu.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3divicesu.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3albswlzj.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3gvsaujny.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3nqvvypvp.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3zcfpkywi.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3tccwajch.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3wyejvxvq.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3cgqfohmz.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3vvrgkxkk.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3qhbdqroz.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3xknmxwxk.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3rbqkzhjp.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3wmltwsix.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3svxzzfuj.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3kwzafnce.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3jopumlrr.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3gzfjjryp.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3abtgogui.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3grsyrjkv.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3olipyvqu.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rfbxfsjn.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3xhwlwgko.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3rgfisqhm.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3usmxmfbe.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3ajrwbdwc.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3ttpneern.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3utgebued.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3hknjezrz.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3jvmjxwlg.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3qazzilqf.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3rveomgvy.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3qtwovndc.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3ljodzchc.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3xbdifqjk.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3tvnfmkyn.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3vwhvmvcc.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3nsvjvhtk.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3tfhcntjd.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3wpqjpsjb.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3pkqmimbx.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3sgospkcq.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3igypykxn.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3bqrghhjv.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3ujutipap.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3hyuzjltz.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3lgcodtfj.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3ibrzlpik.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3kpnlsrxc.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3gaeecsoy.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3fbxvwoof.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3eokevrtg.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3deblzwbf.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3pekpnuul.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3ujxziwlm.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3pfmsheci.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3ignthjlh.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ahjwbfnw.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3asotluia.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3zgxvntmb.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3rfmnzhnx.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3xyvwspox.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3bujwngrw.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3ihqisetl.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3jaqwgukn.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3ainkerbe.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3hniquwsg.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3bsnkvuug.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3gxiopzfh.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3dfmuaiet.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3czcipkcg.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3yfbjsams.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3txgdwige.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3daweudnn.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3exhaduqb.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3sclajmgr.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3faixjgyx.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3wmnysiwa.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3jwtspvtz.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3eeybaudn.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3tptvqlyu.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3bhrdbvpy.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3jvvrjfrf.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ymmpkbzr.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3gsrxeqdn.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3dakwpcoo.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3giqgvlca.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3qbxmettn.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3bjpnbbee.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3rwyednjz.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3sprklkcw.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3jtyfocoo.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3bxvkeott.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3hdpgsbqn.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3lbdhbbkk.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3lqpvtlkg.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3vfrhphiv.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3wwzoyndz.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3ixmvsnma.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3rkbemjhf.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3kfgivcph.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3grfyyehw.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3kkngtxoo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pkrkvfql.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3sjozuhsg.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3vijomuve.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3atmdtwkb.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3zohktvxi.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3byfatviy.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3uiyuctms.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3prdjhgwg.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3gzsbbqhk.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3bygympft.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3kioitwjz.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3ngwmhbng.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3xzsphjvq.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3hlpwicic.html


<!-- 参考信息 -->