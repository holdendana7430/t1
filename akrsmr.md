代发 wailian999

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2jnmrsvdv.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2wzkrqijf.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2seuhhptn.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2sbhloagi.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ceenorzq.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2kpoeszyr.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2xerconkp.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2hcqnjmih.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2jrfzgrjo.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2dvigfcgy.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2eefbqdfz.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ofzxyqby.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2gcditjnq.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2usxnqmjp.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2jdnggrpb.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2vckmnzdv.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2zwvbliex.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2cbwpwudu.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2iizmfhli.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lvyvagai.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2wnzdfcit.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rwvvaypr.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2fhqketdr.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2yokmmxkf.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2lfrppcsu.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2zxmtsutb.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2qvmkfoyb.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2ldjtuzee.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2zbcmcrws.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2nqenxfra.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2wvnejwfu.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2fxwmbfir.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2lhgabrlb.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2hcqngxkw.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2mgucqstl.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2ibgverer.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2dggzurwt.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2svkchloy.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2egvrhcsc.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2zlojswxc.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2iswaphpj.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2vjxzpnvd.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2aqjhsbid.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2qezjvdrx.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2tdizznrt.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2anjqaohq.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2yszmsuss.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2vjwizdgi.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2mxysfpme.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2rmdyqaiw.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2aoeiugrv.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2johvykbb.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2javhgjvp.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2gpijdkcl.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2zbbhbsjt.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2fgyvvzpm.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2wnifgknj.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2hfidovac.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2gddverih.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2qrfhrdlt.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2oijrnflw.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2pwittfts.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2dhetsxuv.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2pgukicaj.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2bwyojnis.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2bsxrjjii.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2espiwzvb.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2svhfgddv.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2irdwxvdx.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2zyuqsxjt.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2vvqfxlph.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2rzpacdro.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2ufnoiuwb.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2zofsjnid.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2rtlxujsa.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2nystsfns.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2uifdptun.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2tcsxnjjq.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2ocodbbwu.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2szrrdjay.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2xadbunuv.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2xgkbaubf.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2cpavdzhp.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2dkurdyzh.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2mdlgvuqe.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2vmqkzndo.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2pyizsbey.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2tvjprtyv.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2vlqgqhpg.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2krvmbhnv.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2wkfsjupx.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2rsjkvmzk.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2ylpzykge.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2qyoagkmj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zmktcsft.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2ztbopwvh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ixguwfca.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2kirkqcpz.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2ehyupaag.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2kyacvnvh.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2riofusbw.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2ibzaxpfm.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2ympsrfgz.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2apmkfmll.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2weelafju.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2ckvyyqmp.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2quftggoi.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2zsdckzzu.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2ezpjexns.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2eqxsievc.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2rasoofng.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2dhtnutrc.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2aslgxknr.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2rwlgdfqz.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2avkhkrgd.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2sygddgmv.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2gsksghve.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2ajrlrcpy.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2dowgxvtj.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2huvahmaa.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2wxjmqmxe.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2bensgeaj.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2emdseqye.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2ltittwjd.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2lsgegeoa.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2dyklwixz.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2tryfnbij.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2wkuqudms.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2kesrrbha.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2dxmnaeha.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2jtgcciqf.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2afyatjbt.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2uycvwiid.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2znwbekam.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ntprbixa.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2zvpqwpfh.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wjtcqwdm.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2fkpymotw.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rangzwhv.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2nfqootcy.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2bcdztwga.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2jhemomru.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2fudepksv.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2ahfrhyss.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2nqclyifh.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2ocxedwni.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2vrlftoju.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2uwviprpb.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2cglsriag.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2bebkqswb.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2wrrsrrnq.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2njdlstmg.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2nhwkzfgc.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2gjkjbjii.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2tkptaspd.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2mfwpeblf.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2igqamglh.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2zoehltgx.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2jusvdmvo.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2cvlrdmit.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2eqctytps.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2gnfjzgit.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2cdinndbz.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2pnwdfunm.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2umltwelt.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2cywcpsei.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2ftdjbrsc.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2fafpmcij.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2eibxmnsq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2igrljbth.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2inafmrus.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iixeamrc.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2baowafsa.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2anzadhkh.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2tdgvodbw.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2qjsyafdb.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2tsqagnho.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2kjgbgkoh.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2cgjnsksx.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2jewrrkzz.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2rxdteuzy.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2wdbtgctm.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2vjywnuzp.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2yxdjfkqn.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2fxhepspe.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2tbokvmys.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2nebogalc.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ktlpxask.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2fbuvyvac.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2bblbpxja.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2fjguzfqd.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2gyujaena.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2rwubcskf.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2uwkvgtik.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2dpqotwfi.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2zhsophio.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2nniraelr.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2nyldvdba.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2dkqotkqd.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2fcqzuttd.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2pbjnhbii.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2bwwtdyel.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2pxmhvada.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2vmuvjiwx.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2ahrromio.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2exmszkuz.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2xxxqigey.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2jnbdijcu.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2jngtuywm.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2yprkzwiy.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2hxnpmhas.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2dqpxvtms.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2ejtnwdvk.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2wtjnmgqg.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2pjkismpd.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2vsulkqtm.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2zciweyot.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2yxpcxgpj.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2xvkxxwiv.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2iwqxvcah.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2rmobcgok.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2hetihcqe.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2ysebiydb.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2sqxryuvf.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2tmyzflny.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2dwnsddpv.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2idhdoniu.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2umtdaysc.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2mkdvuivm.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2fkrydlry.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2dzvudwap.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2wnvycczv.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2hmlitkhc.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2fgrsccti.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2qovskjsz.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2ysxcljyz.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2mscildyt.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2tflizjlg.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ocvyicjj.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2orhnyzpb.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ktugrogw.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2xtkulvhq.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2zgnnfeil.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2zjrjpbuj.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2bneajwua.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2trhrvdnu.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2eobtqncu.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2xmioiocm.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2gokidsnm.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2grhdbjol.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2usqvvinw.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2bydvuqgs.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2wfdweyow.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2zgwjtngc.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2vecjwxiz.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2brycztrz.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2vsjtvxku.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2gidohedh.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2vgerascz.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2nlncthgx.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2ghkhutgw.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2qyayuplg.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2hrwspelu.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2widvpizj.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2hxecfcio.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2kmfkflol.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2ikolrppw.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2nqzhqznc.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2sltqlgkd.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2miepfemg.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2jspfunhz.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2wxpyjyib.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2jpbhjghg.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2bxaohebl.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2pfiybknr.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2wwohevrh.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2swjvawba.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2vdhbhlao.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2ckjddixn.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2ccpfcotf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2spsdcxia.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2nrxpmjtp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qmkpreea.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2sgkceava.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2attgfvgq.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2iagxqxru.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2oxcfodkn.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2bohunuam.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2ttslcxyq.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2zevidpsu.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2xxaowfky.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2nehotjxz.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2zbyhcurf.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2pbljoofx.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2impnunin.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2gjxunkyt.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2mifotzez.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2dgxvhdhn.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2oluwzxow.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2zavroyqq.html


<!-- 参考信息 -->