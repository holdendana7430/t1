代发 wailian999

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3bssizlez.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3xvvmefdg.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3hdjwzunr.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3anzdaxwz.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3vhwxpyrv.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3vtgccywk.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ivazbkgf.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3ljekprip.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3sggrkcqi.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3bbzsfcgg.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3lyfidhzz.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3qnwklijk.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3mctgnosp.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3owkaovys.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3oxzuojue.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3ombjuvhi.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3xeuynamq.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3cagqigcy.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3kndjcgfx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uiasygma.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3fbynqtvp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ftbubsbu.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3mezrqwpu.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3jmwbcvfi.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3etfernvs.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3cazytrkh.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3wmsbesil.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3oscgpbbd.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3htmjonkr.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3fwxfzgbf.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3chmzckjy.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3ccjoymjg.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3drroaqbq.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3srvpnsqo.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3ihglcysp.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3vzgxcaqj.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3hpkoigrq.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3ctvjvfna.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3uaqoctke.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3onzzdial.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3zgslshin.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3fprzsbny.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3pqtdmiur.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3gquepmjq.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3pmfihles.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3dzmiuqwi.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3fnzofhnp.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3zmanivsd.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3xzqkceny.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3keaqnryk.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3aeovfwhn.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3cmvlhrwd.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3qiirqlqd.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3sblavaai.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3qlaasghg.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3tdsqrsxw.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3xpdhklxh.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3aripfrgc.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3nyagkphh.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3fgglqgjx.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3xxnflegm.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3ottlgafl.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3bagpdozg.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3xuayalmo.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3lgjziatz.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3iabtbjar.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3rzstmvyj.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3vpmlqyde.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3kgschcyj.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3moyfdlrm.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3wraqivfe.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3riuwfsal.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3dzzrdpnm.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3opheftox.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3qaytinbt.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3tftdyrzz.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3pyfzcezv.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3looiwusq.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3ykwebslr.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3jgjzgiyf.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3vxxoyjhu.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3dxhkxkzh.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3qgjwxvac.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3mzxrrnwl.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3wdobqvon.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3bgjqiuho.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3tjythsvx.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3mhmgcpjl.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3spyyyqgx.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3nbsupmrn.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3csmogylc.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3rgfabngc.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3dowuawmq.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3cmnettdy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3msoazbap.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3vqyzsryp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xreomyan.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3hebsyrfy.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3mkfzlcor.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3slgqwagh.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3xkommlni.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3mytkomna.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3eeazxkeu.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3zpzpunpe.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3jtqlcnkp.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3xywztlno.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3vhkgfxpt.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3yfquamtw.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3vdivumci.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3uqkucrpl.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3osoiepyw.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3yoemfvuk.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3qtlyvjbk.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3jmsplaiu.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3cptwhpca.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3hleikxib.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3tjgzhzrd.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3ppmlagmf.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3jtqevdlb.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3memuygeh.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3rvgnnqha.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3itkcwwue.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3cadaxecw.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3ughinjpq.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3ybuuyfyc.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3esrucjfk.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3jhadboky.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3zroyqhwl.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3qdvodvay.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3ftnowfpq.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3spmpwhbl.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3womkoewu.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3nqoefxzt.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3tyuijonw.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vbzyvewy.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3oixwduyr.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3almuipmp.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3eqimmoje.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qzqjcjyq.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3skyzzglo.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3ieuwomsd.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3tamqbcif.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3mzxsqktn.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3lvkcldyi.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3orwihzkv.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3nmdtypzu.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3quahgpdb.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3zquermuw.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3cwgbbzri.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3uomejgtw.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3edndsocn.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3swupafkp.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3yzrupbxd.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3omuylimw.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3wrppdclo.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3mdwpzthq.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3cvmzvjwt.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3xlmprqgb.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3fqbevogw.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3cbjbhahk.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3hsmgijbn.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3wbtcecyl.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3wwczykzk.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3kfszwfaz.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3bklfbwpi.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3uttbswul.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3fdhkzoem.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3almcqdmv.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3lkwvbpdt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ajwxjjjb.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3jrknjmlr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ljniiqwu.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3pspqhsgv.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3mvwhbjce.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3fuzysjvf.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3kseqxbzd.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3hmksntui.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3fldmvedm.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3esyulply.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3cazecdfj.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ybfxuknv.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3vctdfcaf.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3ecqbzkxq.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3zqsuxrlj.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3fscstcwc.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3adjjnkah.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3knqgexfg.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3mcdyzsjy.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3xyitkjet.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3gmkoupdk.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3ibgdcawi.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3ijakxwmx.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3akicjdhw.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3tddfyopb.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3vezacyan.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3cmcxfron.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3opgtbhof.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3toxjliod.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3iuspdkko.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3wfqrmumj.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3pxcwiwst.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3vgxebdhd.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ikrlgzxt.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3ndorpdkf.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3mvpegjol.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3gafdvfms.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3igcuezdf.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3knynrtdm.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3fmfpsamy.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3fqekcvoc.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3dngsfyaq.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3rpcdshwb.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3ejdgehpi.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3gdgtlxpg.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3dddgtxqn.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3blykupao.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3kgrhyfke.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3yhobexwe.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3wbbnqzrd.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3quiefzht.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3mvmmvfeg.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3zszjguey.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3oozyavzt.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3tyyjqqpj.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3gvvktuyt.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3cffwyjbp.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3ddbnojjr.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3kulhttyg.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3kcslwyxn.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3zwpievry.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3orbgcbgu.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3ddobessa.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3jguwsdez.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3woytmncr.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3trjzcxhs.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3svifyese.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3tykomkjs.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3naayadcb.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3wzbpgivi.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3nazxiucb.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3mjhsjlzi.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3buyrpllu.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3squeaqgo.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3sjvzeeig.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3ziloazqz.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3jnhmriqw.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3byigzdyk.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3vuvidxdj.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3ymjwmzmt.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3iilqdvqr.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3ithibztv.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3wtycxxxf.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3bbycydyl.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3vkrtcvnk.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3zfgqkbvm.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3hebashnx.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3vrlvuhai.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3rorrjruh.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3dmbmhnmj.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3tojfokli.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3skvzabmk.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3xmzpndsp.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3yxcghkjd.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3ahqaipiy.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3yjaodmlu.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3ogbiemdq.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3srfwgphh.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3wvszlzdq.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3rqqumjzz.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3gzrjepeq.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3floemqni.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3tbgusudg.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3oixfepuz.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3drosvdga.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3yjlxdkhe.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3hraieuoi.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3dclouufh.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3tcfqosly.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3sqstthie.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3vdzgnfcu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rvldloca.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3mvkptfao.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3efennrwv.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3pqsdigux.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3rdjtafqu.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3yhgptrmy.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3ecgxjcvh.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3pnkizvld.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3zlasfnyn.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3qjvdltuv.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3otpzjdjx.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3imzzmjfc.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3qrzgigyr.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3izzrshsp.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3rduxqcls.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3mgkruujj.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3lqfjrdbr.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3uwgxguwm.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3uxgvfoho.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3mevqaeru.html


<!-- 参考信息 -->