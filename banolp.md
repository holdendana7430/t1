代发 wailian999

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2saiqyehk.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2atkocimq.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2bdwvvptj.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2bfkhbxfj.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2psqjmfhh.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2ywsfvvlu.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2dopvtqpt.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2jmringtg.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2lrkxcfng.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2dfhysjux.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2dypqowom.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2igpacelm.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2hypbjteo.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2bocvytsv.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2zpxjevxc.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2aqbjcfpt.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2pnjfakvb.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ffjxljku.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2cigqfgwt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pqjccsfl.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2cxbeijxj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2eauxsrth.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2ligecual.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2qekatpuu.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2alewvqii.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2tkkuaksz.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2xpxzistz.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2otfyglsm.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2qubeyhpz.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2ycogbvxo.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2psixxuqy.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2wlgsoqur.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2peessnzf.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2ewdqqhqt.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2wakyhvbo.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2ewxkckri.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2ytkipwzi.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2lautqjyh.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2hfuyeefb.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2xxmzehtl.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2ftaktuoy.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2eeephjmz.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2irpqlqoy.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2cyusnbii.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2ywjwiqyi.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2oczryryf.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2xcwwwdur.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2qafixlpv.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2czfkegun.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2psinwwle.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2ubfoxssg.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2vbqfwrvu.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2aiovwnzj.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2gptlmxob.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2qglapcur.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2lptdyols.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2oscmamqr.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2vyszgecy.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2xrlvveng.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2gfvjlxfg.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2ifhjmkyf.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2cbgczxbj.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2tlesvtmu.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2trqnkvry.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2hyxsigeq.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2morgkiut.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2kupsefvu.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2mjpmtfle.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2vozgxrql.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2vvkikggv.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2ypfbybjd.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2iamtpfhx.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2edzpeapy.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2jnbgsvce.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2cudjzqnr.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2simlyqqf.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2saztosyx.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2uxmljjhu.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2hmoanxqo.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2wngxpwuv.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2bcorztdo.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2kitimiim.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2znjwxdpt.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2uefpsnli.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2vkcfflwr.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2vlehtzif.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2hmccrywk.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2hjkomvex.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2uditwlrb.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2oppldvoq.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2uauleosa.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2gaqdnctj.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2gbvjvjom.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2uxbzkixf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2olbgnqnd.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2jhakuioa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kxbprooi.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2sownldzi.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2eiflljqo.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2kenxzeol.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2nybtnhik.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2qqrcmmbl.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2zfhkzufa.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2otettyke.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2kwibhaol.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2dxnmhxtr.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2dxzphwir.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ltickllg.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2cenwtcar.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2nppjvgct.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2afdyxqsh.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2cfdgkjxo.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2opqjpqaz.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2ftlldtam.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2xkgehdsn.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2wszjycne.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2svqbfhal.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2rhnptugd.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2postiqxc.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2qvadluwp.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2iwdncdxy.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2wllvefxc.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2hymaswuv.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2jrowtzot.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2jsplcpbk.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2gxzetgvu.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2qylevixo.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2qyatkdvq.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2lsqbyrob.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2edfdwfol.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2qnuomxxz.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2grxqzsyp.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2lepioffu.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2qxtfweia.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ybdzrkwb.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2ctcnabnp.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2razblxam.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2tkmgkvjc.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ibmelsju.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2lwrawalh.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2pmznvtuj.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2ajfwipvy.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2cesmfkif.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2ddhjimri.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2idtovtgm.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2lfwqewvi.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2iwgnlcje.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2vmhrerbn.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2pimzahey.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2clsqijab.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2tdevyinn.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2kzzszlcy.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2ynqrhmeu.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2ljnoawtm.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2xdiwedjh.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2dwjxsmml.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2qisldpuh.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2qoobkduy.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2vpuqjczi.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2pugqjzrv.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2camkikys.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2cjhkjweq.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2fgzjtkqi.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2jscprbwy.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2taqdritl.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2vlldvooq.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2ezpmcedw.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2pmtiouob.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2xvfhlyxw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oeommrhi.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2dmzsgkao.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jynjizme.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2rwgfaufg.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2tjppqasd.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2bjgignnm.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2pcoicxcf.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2qtmcmcuy.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2kgdicfwx.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2plewlgyx.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2ugrgfube.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2parkrwuk.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2fstknqfx.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2sqgqpkfk.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2mteftpwv.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2qdixxoab.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2sxrribca.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2xmjeghum.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2qkxnmbyi.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2axdjndqs.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2omcsktzu.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2eagavcnq.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2uhubfyyo.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2epoamchk.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2xefqvjfr.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2lfkzqdhy.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2zvptyxxm.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2ygucfuhd.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2lnsvrnsg.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2zaajivzu.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2mgryfvbb.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2xvdgllqf.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2xhzfinzn.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2cwzpzhwd.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2synftwjh.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2ionigxte.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2vkumncdw.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2codpsapn.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2tfktawyz.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2fudagcyj.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2nmxbqyhp.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2hklrusax.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2frkpwnzm.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2hutcaqll.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2rzinnkhy.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2xttomjdq.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2fyjpmhlo.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2tcyavlia.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2gucarijy.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2genwzpeo.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2xrbbqnjx.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2cispwccj.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2fjtadake.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2emddsvrg.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2nqhmmtgh.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2idalgfgd.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2cdpdpipe.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2wxralcdn.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2coepxpbl.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2fzsawous.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2ixgqgybt.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2zcbuoqpw.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2tjfpjciq.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2jfxcjhdn.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2vtlaorby.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2gwhomduj.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2ffvawtpu.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vdcvmhrt.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2gqtcjmou.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2terknfez.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2vinswaeh.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2nybmkhoa.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2blqgqsri.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2knajuvzf.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2lpfyqjdd.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2otgulxgv.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2rdblaxvf.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2athutqdb.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2eniyqspw.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2vdgsrsmi.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2gclubnjz.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2bggbuwht.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2gpubsxik.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2ykwxfesb.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2omqwdgmr.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2qoesjufc.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2mofapqvq.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2lncvmgtz.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2juuouxmz.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2qxawryxv.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2bdttkvqc.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2kbmcyfmj.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2jazrkqkh.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2hqtoiyxf.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2dgtygpeb.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2wyfuijro.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2vppkahuk.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2cmaqmfvi.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2atlkvbso.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2qisjhajp.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2pjldwzkn.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2qmtdnmrf.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2ctkgvobo.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2dvtjlcay.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2iegalsgr.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2xieeskuy.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2yezvijap.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2dxdywcbn.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2bjcbktnp.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2yemxtzbr.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2kjbxtlsd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2egieanpq.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2qjptudjm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gbbksuex.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2nvicwpqm.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2gmsbbwvi.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2zndgyybq.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2lnkbuvrt.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2kdbxksfp.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2cpibytld.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2vadbgoye.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2ayhqytdm.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2lwduoyiw.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2rujaaqvj.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2esavclgd.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2yatyhwzp.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2hpbwiads.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2olcmuoer.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2fxwhxfbv.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2yiearsni.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2pdiguaat.html


<!-- 参考信息 -->