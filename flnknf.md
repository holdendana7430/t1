代发 wailian999

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2vacfcchd.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2erjqprfv.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2jwioomln.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2jpgbqmtn.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2xyjvykpl.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2ezbiqxqc.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2fnigdmat.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2xjglgncz.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2vxrtswfi.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2xlpkwoim.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2cpudqsef.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2xjkghwgm.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2emvvvmqo.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2xaidvyyp.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2kjybdxsd.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2zyyvlqoh.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2gybafhvr.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2jmvqsnga.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2rlmzecki.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ydzqhyqw.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2ylqjfovl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wpgzofbu.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2pplnwzqv.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2jbkfcfwv.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2bqperbyg.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2krlbzpks.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2tcifxjud.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2cvrdofmj.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2hvdznwzb.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2ppzpxakq.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2spbcqpcc.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2dwnrlhsm.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2btdxxyqw.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2eutjceoz.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2qywodcax.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2itrpznlc.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2shcjkcaq.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2laricshc.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2ywypzhyb.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2uirtwdtf.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2jyaelyab.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2mpmavqcr.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2zzdqctci.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2ywifilsd.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2piyjligq.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2tmskhvif.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2bdmkiczg.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2uettskgh.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2lilxuqdx.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2dxyzhkbr.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2nkemfckr.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2sotsdvxo.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2rkkqadya.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2nmgzucpx.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2pbwaydjc.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2oscxfzla.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2kwrojnpf.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2gnvjescc.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2ixwclhud.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2ciqulkyn.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2jwyrobbc.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2ekarlrmz.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2usrskupd.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2twuazfru.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2ahasceja.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2zcpcujid.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2lneyckdv.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2hdwkciyx.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2dxnpnira.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2xbgkltom.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2vpdpbtui.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2bheabmne.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2bnwgehla.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2amlpyzqg.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2whnbrpbm.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2wdkaeqba.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2omwqtmrl.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2wipsnbbn.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2fxurerrw.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2bdahwftk.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2vrozxebk.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2amqkbfka.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2quwcnesh.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2ertolzju.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2pxpvqhrl.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2fwoutthn.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2sxqnxijx.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2pbjgdlba.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2eeeszfqi.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2hclxwsng.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2cawpbzwd.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2xzydrulv.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2yhlxsfze.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2egzxgesa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cgjziflt.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2qfcftxvd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2frwsnhgw.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2tgqmceuj.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2mvsviqyl.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2skbkufoj.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2ejocqqlo.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2pcuuaxrb.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2bhvivauk.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2cbtmfrzx.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2fqgbjhth.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2lxendyil.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2waxjsraw.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2ivfgrogf.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2xocfpzvy.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2sgdmugvt.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2qctvweqi.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2tfawrnjn.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2yyriyuiu.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2ylkifupt.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2mcrlrnxi.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2xxueagqj.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2aipxdpkw.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2vwmkgeal.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2lkdyvjdn.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2hkhrkgbx.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2vggpstoz.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2hmzwlmyx.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2bamkskqk.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2niruwshi.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2vbokuqmi.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ytwtnaix.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2xubgrxqp.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2jldqmbqj.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2xehrqkfr.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2izsnkvlm.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2opwvditd.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2qkgzrhfy.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2fykordkc.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2beyfysee.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ynukbyfj.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2okmovuyn.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2evnhnlwf.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2bbktawfz.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2njaglbno.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hcqydwbi.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2ikkozkhv.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2mabhhsmx.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2pbkvbjqo.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2fopzavct.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2vyzblzxv.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2uojcbcgm.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2xwwmcxdx.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2lrphrqkm.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2trimompm.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2khsmokxa.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2gpvqivkg.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2wxikzmos.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2nucjekmn.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2yqnzhjcj.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2konzyirb.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2wqbxpqma.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2kledlijv.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2ztertjdz.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2qqwseybs.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2mejlpler.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2jsoasjvf.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2etyteoyl.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2tynjhvft.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2nttgwpnx.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2vjxtamvm.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2vqtedszv.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2ewqsqrya.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2yljmlwsv.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2iwtnddmw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bybjgkyo.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2mcpgasku.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mevyzooc.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2yyjydlpz.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ironlkjw.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2rkaegnpu.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2murnihhb.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2xykdrsqv.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2zzjcwlug.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ayoegrhk.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2ubcvrnvg.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2xtomppoq.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2afirjxyw.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2dgiwgdlk.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2qaqecesf.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2zmrzrajw.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2bukzqfsj.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2ejxhoedd.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2bvpluprc.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2cdqbbyrq.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2osqmlqoe.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2bbbbujem.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2jhfhzmux.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2enqrrnxr.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2aaoxuqzw.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2qskvqlnk.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2oreufzxw.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2jvzsqksw.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2obyyaxhw.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2kamzzqqd.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2sszpukhd.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2uczodvom.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2jlohkrlo.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2nvnksokl.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2vuzwvpwm.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2rqrkaylg.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2veabkpkv.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2vmivsssw.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ffbjgqwo.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2ighzurhf.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2xwkvgaft.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2ncjybwvt.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2nvxuykqi.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2wjttagcu.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2phutziyc.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2aokxxdab.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ekqfeqyx.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2ibtdtlkx.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2bhgovuzb.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2wnhfemrp.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2bdzvehpp.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2enacpmhf.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2ckybjmbr.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2enmkyvis.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2oqvmmwbe.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2vxyckgkq.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2ddxflcyt.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2lqyijdwz.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2raiekinw.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2ofwljlbk.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2fsxpjwxm.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2mbtvhdoe.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2ujqtluaf.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2bzyaeshk.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2zvxfhsqn.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2dzexwitg.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2bgmcwpoa.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fmugiahf.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2wkxawbrg.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2jvwegmlv.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2yzwnuizt.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2qityitwu.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2dwfsgssj.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2youlryuv.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2yhhacial.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2brrljduu.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2jbhyzgby.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2xvmvgkmb.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2favrzjzc.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2wvjapfro.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2rbtgysgh.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2hwpciukv.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2tsksimwl.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2ktfaczrc.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2vgacewuy.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2ukjbfscf.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2mnyxxdou.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2youxdtqa.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2ntmyofhi.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2oywdvyak.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2iyifzflh.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2ifuypmhn.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2sbztfoxe.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2bnvxrfhl.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2uyuobshv.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2nwwykebh.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2eyfckxod.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2jplrmpqf.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2trslfqdf.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2ydmfbuob.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2teqnmguw.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2efvsjtxy.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2dczgozwz.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2powdpnlt.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2esfphnfq.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2auysuccs.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2tevnubli.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2fogbxsgq.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2mcanpocl.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2yaapkamw.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2vgmfqpqk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mnhmecgx.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2pcmrykbl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pcystkxy.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2hlbithae.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2tzspbtue.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2orblnajt.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2ilyxjlqc.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2aaeevpqx.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2vfzqstxo.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2ybhzfshk.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2ttzbriip.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2rvnfcpsg.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2ppfnrdev.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2zugkvcga.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2xrlpuhtd.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2nurluovj.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2zfuoqfxp.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2fkohvord.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2jkxmpikb.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2lbwuljxc.html


<!-- 参考信息 -->