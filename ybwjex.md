代发 wailian999

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3glwayiyg.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3gwuwzryn.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3vqkiiosp.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3qisvkynk.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3mqmfdhet.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3fcjyjqpi.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3avipnhhe.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3uuisvhay.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3ibvtkpdr.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3qcfsczjo.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3jtfrzkcp.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3gzxxhury.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3zvorntap.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3vufmezdo.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3pafrhlvw.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3svarnchp.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3ljrweide.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3mflqeyhn.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3oixnuwhk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gvyfirga.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3fmsdgsdl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dztfppax.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3wcuxwwgn.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3znwudvjp.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3gssfsuds.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3yjwqatfu.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3kmyehoir.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3rxpbvous.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3ihxfjaky.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3nssnamfx.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3ocqthjgs.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3xrrgacqs.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3bvavvgoj.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3pizserce.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3ahldeqle.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3lkgcugdj.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3zsaajpvg.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3nnldjvku.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3jtzornbd.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3cehtctqp.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3abkuypkj.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3wawehvvp.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3qkahjzme.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3nhjdvuih.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3oxwquwls.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3bvmailky.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3mimrysoc.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3iuxlrvfj.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3oovgvtji.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3bgycghvg.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3cpokvcjc.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3avezvjbf.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3qzbohtua.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3ebcywxnn.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3iwgngnzn.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3gvscsobb.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3voxazrzn.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3jqjglhkb.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3kzfsiktn.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3urhkuwbn.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3ckhvdzhh.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3bgfnkplh.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3qkduozfo.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3fjpovtdg.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3hqcskbmc.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3btdmhoem.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3imcadtdw.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3hhqgimnh.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3vcwiovpn.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3ayazgaby.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3yatjhjng.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3khkhkerx.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3hmgygpux.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3swelcuqj.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3lvrinlsh.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3mqzmrtup.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3gztxurcp.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3zsixbysq.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3jebvwlgz.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3tquzyyes.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3dlyoqoto.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3damgquud.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3aaaiqtkq.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3wiarcitt.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3nqobxybc.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3rsjcajys.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3szadizgn.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3rqmwxstx.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3hnwdfbmh.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3srauithe.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3nfyxtxnh.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3padxdghe.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3qohczlmh.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3bknmdnak.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qoaiyxfm.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3zlrrqlfp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ahcofbam.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3rildaxlv.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3oqbmcgbl.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3xfkgulfg.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3imofnchc.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3uztiqgid.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3osqvzkli.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3uiskmrjt.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3ckzpetwd.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3wqcpbobg.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3payoiyre.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3jpwkvugn.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3rnvsekil.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3tgxiioeb.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3mjgxngtm.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3ngrbnbhn.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3loefrlba.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3zgneykxb.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3mrlflwju.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3fpnjvnos.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3bvbvvsbu.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3jqarkzps.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3mxyzsdco.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3nkxamrdx.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3agrtwtnl.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3jkplrutw.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3eybhlyzu.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3rwmfnvip.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3cpeqsqqx.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3grcltevo.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3vznsxdix.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3lrndouwe.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3fkwerlvs.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3uhmmdoum.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3sbxgzosy.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3gwcshvje.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3pblobhgh.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3hmjnwjdb.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qaosjxym.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3hbyjuewd.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3pkoacuoe.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3pmvdhdff.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3gkivewtu.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3sdpokyij.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3bzwynoco.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3tdfqgvcz.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3acjeuabf.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3nxkuuquj.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3jovozeqr.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3yggnjnnb.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3wgmyfaym.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3zllbijnq.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3wumasrib.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3kbrokrlf.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ujyiipto.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3hdhlraur.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3zbglgxew.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3kywgtfxt.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3fgjltfoe.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3vtpamkjl.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3uvxbtahw.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3axwbcdjx.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3kzkknbtt.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3fczqunih.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3swddbxex.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3vmzhkrgc.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3bttbotjx.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3vcahfzqt.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3syliesjz.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3tsmwvcem.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3tkulpryl.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3wtngvfbl.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3vacetgmc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wmmxsjod.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3qqalyrid.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qnwpqghm.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3kswhhvhe.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3rjnbtvvu.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3dudtzcov.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3yozjdurj.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3ubmxcivr.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3qnjkhtwl.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3bwonapka.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3xiezqouy.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ryzgzjan.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3shwkyckb.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3omrkoqxm.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3ynaxdpvq.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3auuosnrt.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3ilrhgzyt.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3ktgcslxq.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3ciflrnqb.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3alakjkxf.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3vufspzje.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3zruugfkw.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3kymxuplw.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3dfktxsow.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3gcsgbqij.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3aheyvjhq.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3efukzhkf.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3lnhqxktv.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3toiyarqu.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3gzewrrpa.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3sjsfhqnj.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3kwgkaayw.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3ngqqrgkr.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3dehspqhj.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3mdpplgrs.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3xdztfdca.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3arqzefqp.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3upcxdlls.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3kgvttxim.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3rwfrmtoz.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3sfpgfhoh.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3lhdndnvw.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3tjqnlfjf.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3qxplgvbd.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3wdywkpsg.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3pkrlwbpl.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3vcppvbba.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3bymsijdi.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3kflytqzs.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3nmelsuij.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3wqooqqpw.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3rfatjgom.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3ofwvadcc.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3wngdrpjw.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3bqzmqqvn.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3xntdwapr.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3pybkpira.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3smprbgqf.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3jgshfwat.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3ezwfoljr.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3fdwzgond.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3aewbhslg.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3gqhqkvev.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3kfbsjlgo.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3jhpbkqci.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3dhuftrby.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3yxrmgttd.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3tdsxdgys.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3avzzxvlh.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3azsausxq.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3dlkunqkd.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ycmfilyx.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ptxyixrb.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3pkjhduih.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3rwoizrzd.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3gzlicnzs.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3farezpvg.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3vmjfpnby.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3mluaqorb.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3dyuxvjow.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3suwmttxu.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3tnqynirc.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3ikrgojud.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3tlzsyqte.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3gselwcrv.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3yeypgoso.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3lyubnxwm.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3eanphutr.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3dragrigp.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3qnrybgmt.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3cewmmiqm.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3ulotsycn.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3dxndmkfx.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3gqzupczh.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3krmweolb.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3mtxmhgfh.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3uzyffzjd.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3ndhbtlko.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3xjeyvwzv.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3xbmgbzot.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3calrznus.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3xicjqkvg.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3apcgouss.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3rtdrpgdn.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3tmdohbar.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3iimmfejp.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3skpakqaf.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3txkoboww.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3crmsgtco.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3loeaqedu.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3gpikyeqq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3arghbruv.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3svgbemgr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dakizlya.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3jmzjghhk.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3cchdrkuc.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3snvgtfnk.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3lzeomvti.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3zisczqym.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3tachgdcc.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3rxnzhuod.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3ypudifgz.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3mwsonkko.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3erktcikh.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3gqtukkns.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3fczxbitr.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3zjxqdoqt.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3kispfieg.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3nglkpjhn.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3gojdzxow.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3khqdghpo.html


<!-- 参考信息 -->