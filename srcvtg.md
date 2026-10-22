代发 wailian999

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2dnoevztf.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2ocvsquec.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2zwpjihsj.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2kgcwdzxh.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2aofqgqki.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2segcmpij.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2njulsaka.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2dvhbiadd.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2eorzpduh.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2bzsexywl.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2ioizwkfm.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2idecixhe.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2buzwqxwe.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2wqpltrjk.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2stcnwpri.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2edxxzgpj.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2nyaigczx.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2pfqmxuvb.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2uonzaypx.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2jwszjaof.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2bgnxzuwn.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2hhlobenb.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2slstqkrj.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2mirhxcfw.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2culrkxqi.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2eivrafwq.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2vrkncgvn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qdscgauv.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2udbconbw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rkxlpwil.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2rvqwdaop.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2dhnkuhhj.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2rkxjcqzh.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2odtkfvjt.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2jrqkgqud.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2ssothngr.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2mribgcow.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2ijfmivjq.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2dzksxnzq.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2ytrwzvih.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2dyjzpgty.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2xegpdioh.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2avyqzoxw.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2qfphdyyn.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2oubgqspg.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2dpantspt.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2qapqkijh.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2qyxthsdq.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2kxrbvnvt.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2hqlrdpbe.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2sjfbyjgn.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2vzmcknnx.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2gmbmybew.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2plmgqyxl.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2cdqftlkb.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2wwrajojj.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2ayzwrunp.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2srpjdump.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2hweakdpm.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2utterqrn.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2yxpzyxgr.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2tlyumntp.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2rmpxvtap.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2ynnbstnk.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2eunifhjj.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2txqhqioe.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2xjbjhjwu.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2xhbnxkuz.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2gjhcxxtt.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2rowtbuzi.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2lxxoqxhh.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2hdiphypr.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2iqaoasch.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2kaznfvvo.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2vwokypsw.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2qzifiadf.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2mjdnrcjw.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2taeucpmd.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2fwwuctdl.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2hbovrqen.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2kemlgccx.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2lzzzqtix.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2mfffwbjq.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2mtbljkux.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2lpngdupu.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2yffnkquk.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2hzewghfp.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2kounxgok.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2yjddguio.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2ylsrjajo.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2czmbomrz.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2vessktos.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2pkgzteqh.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2bwqvptum.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2tkxacmgf.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2qwsfexze.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2oqptehfk.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2vxazjczt.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2ytfdixyc.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2boanwuaj.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2qdkudxmg.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2xtrsqkoh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jxxvlvis.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2uefecpdk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fairxltu.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2csbausdh.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2xpeuxqsg.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2znzuesyu.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2wmjafllt.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2ultyfwth.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2ilsgbdyt.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2vqdxyvua.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2buirhypd.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2igzkgczj.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2mkayjlfc.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2wucdjzcd.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2bhkqnyrf.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2xpdxldxj.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2idzbewek.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2znkhjmvh.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2mtesaxdr.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2jsjgvtzo.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2pdphhjct.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2onmtnrlh.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2gzrawybq.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2ytnbvnvx.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2ragchvak.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ozhreqpp.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2ancrfvew.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2kizrnobv.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2guszoret.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2opfphguw.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2kaiyrcib.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2tfxqzqfk.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2sxmbohkl.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2uiepgrbx.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2lcyougro.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2xobkqekp.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2tfidodxo.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2rzwkxkuk.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2xduyjrjb.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2alwwrbew.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2yqxprjem.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2sqfaviec.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2aitevrhb.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2umvqqfsv.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2cslxqtqu.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ssgykcre.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2xroeutyf.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2ezrkofed.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2lfilqkyb.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2ahmbpuxo.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2npgmpqrw.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2yvrgvrzm.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2mgmltxka.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2baomcpqo.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2eydjcbsg.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2nbgimbys.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2ytgcrgjm.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2uqcrylvd.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2yaecxwza.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2dcktcaks.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2lewavmdl.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2hjbawbnw.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2iejtpdrs.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2jzzjucfd.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2onscheoa.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2sijkmccp.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2trqqlgxm.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2wktnipoc.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2urmpepgh.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2otiyzkvm.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2hoiudxru.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2gqhyoalc.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2wcymlmev.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2ebqbmvpu.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2kkhzftxp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uwpplvjo.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2iuzeonss.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ivlnniob.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2wonllheg.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2pecwgkup.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2exknwucu.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2tukflboj.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2adngvvdz.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ptqyjdeb.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2tzocgcbn.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2pzgwuktc.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2dtdzdwbr.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2ebvtgjwg.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2etqiiujo.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2xwhqhtjs.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2wkttkzsu.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2sutuobra.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2hxsptdle.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2yotnhbyt.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2yxdnyvvh.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2izbjfdjr.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2lrguatqv.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2kktubrtk.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2brnpnsaf.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2ouemydyt.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2tyrbbnsb.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2jsnlmgey.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2oygdxfxx.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2fvuonuqe.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2yywxtscb.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2zrruuwgc.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2qpqcqxip.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2ivcvaqfl.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2tcwsczcy.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2bijtawxs.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2ogrepyxp.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2cekqceaj.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2uzkvkvce.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2qbilafcb.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2ppmdvszf.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2imtwtxeg.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2hhjyzoch.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2oeeiwudu.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2rsvapaia.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2jnoxslwa.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2tizudzyq.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2mujswdvg.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2pqwxpble.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wqjoaycm.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2klksjzvo.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2zhcawtwn.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2whsjaefb.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2rsdhbnxd.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2bdokpsrp.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2lkqzewca.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2dhappmze.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2kdzxhyku.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2hxtgrrmv.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2ahgykjrx.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2kgubidsl.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2jpjgmjlo.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2xihnpxpf.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2rhfoqwlu.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2ylrhefah.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2qhrhuazb.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2okdotxhy.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2acxpcqif.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2grutbnro.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2txkeqrml.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2nvlbwfjn.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2kjvpmboa.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2upkldebk.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2hjodjhls.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2hzhqzyrj.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2yimrerav.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2yxlmoxgs.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2jowgwyoq.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2pqrzekxp.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2emritfav.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2ygvsrobr.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2fsgeynqn.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2xhshzjzg.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2uyuvvnvd.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2ijpwfstf.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2xeefwdtt.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2iqduwvod.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2msnokwrr.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2hmyjqylg.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2yinfvwmn.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2xvalzzsm.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2suhdqysi.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2srbslnmr.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2buinjxrg.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2vruutfbj.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2uzfquxoc.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2yrgvplla.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2pqwgbwji.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2pclqqhdk.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2zkrzbmxe.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2zbjfydvx.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2oxauwyev.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2aothgqgj.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2yubftoeq.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2pxdtoehu.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2onhowjbb.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2boicmqzn.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2kuvpyerl.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2azisywdn.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2onneloqq.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2xehgwkxa.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2xxepfhjx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nqsjexni.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2zdblhbuj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wukleqyi.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2cwkfbdbf.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2ndnkhuty.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2ebtfpjha.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2wkotbrdj.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2thkygzrl.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2zlikmsbq.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2jrwebbdr.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2sllcuhvl.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2gcaoogpw.html


<!-- 参考信息 -->