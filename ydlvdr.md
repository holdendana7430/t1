代发 wailian999

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2eypuioko.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2nnodcrkk.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2xfxbruit.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2vdqrckdo.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2yoiawfqn.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2wpxayvky.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2ukhtvean.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2cctcmjhi.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2kswviabe.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2paazppac.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2arpezzfw.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2vchexrtb.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2kihimjah.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2nqpwjroi.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2encioivl.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2nrtkruhn.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2xgrkllyg.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2zfdebakv.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2puqijgrq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wnvebglg.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2igolqqnt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2odqmtron.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2odidande.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2xwtvhxyv.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2jheiceds.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2xqjrptup.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2sqngzobq.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2knzfwydk.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2uqifowad.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2wpwpjtjz.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2nxrmkzur.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2jdaiwraw.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2qrpjzdaa.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2inyvhpgh.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2dhrtlbhy.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2ioyxmjmg.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2xgahfhtv.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2tleufmdz.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2dlwpqqkh.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2stdlidmm.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2pncmehpf.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2dupmhoiz.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2opcmbhrq.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2szckqpfj.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2vmshdkkj.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2zzhpqoku.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2uezawrum.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2uzxwurcn.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2tbvrpzgj.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2ijjgvbst.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2fbnisdpv.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2vfnihwqp.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2axxupiks.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2zrafldrs.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2ugvcvewj.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2vafbmxsi.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2mifnxnab.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2ojrcivfy.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2tafkndql.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2cumfplhd.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2eqnthayi.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2qlktpimn.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2xgrigepw.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2giijzjfg.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2fvjduiag.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2ejgupazm.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2kjnrfohw.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2wumoiida.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2asitokvs.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2lildhpmj.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2weyntpiv.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2jlmtvpgb.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2zrttgodt.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2thsxrsxs.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2ilgwyxyy.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2mesakyud.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2bcyylzhl.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2dsiriuee.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2qegulpkl.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2wqbztkkx.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2xzphnswo.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2xomvqgrk.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2neglkeur.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2oziavzwo.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2uenuqyyw.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2rxmiuojb.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2rqlsblgs.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2fjgqxyok.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2pnzqvofc.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2zkknxgaw.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2pfxiiinv.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2jneawsjt.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2yzkfheml.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2iibpnegd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wehogtob.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2vxuihkwm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pvudlash.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2zksaopje.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2rocraxeg.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2vmbwsovf.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2eigbuthx.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2zozhsrhz.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2yjyglhnx.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2rvygavcz.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2zzynbqej.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2mhjraznv.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2cnbzvzlk.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ammdyhju.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2nbvbeyvb.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2rslmeapw.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2zgnsyrxr.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2qroicxgt.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2rstxjmzf.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2gehzffkr.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2eveunsbb.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2dbhupqri.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2ttrgaoax.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2urzhoslu.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2pjuvvuxv.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2nwyaiozn.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2xnjzozbz.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2vqxsantg.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2shltdxvz.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2yogzhpci.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2mvcdfzjv.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2kuitchuv.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2uoytenqb.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2gbuihzdb.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2bokypyzq.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2jtihdild.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2gufauaoq.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2tdtavvby.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2lrwneqcx.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2wmabgxkj.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2frhghcvn.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2pouxrjnn.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2wggaahps.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ibbwsxpt.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ngcnwqyr.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hcsvdpvy.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2udekanlu.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2xdhgcork.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2wzsncmzn.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2tgraoetr.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2cgqwjdxp.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2jbukhaot.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2cincwsgt.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2vokrqmzj.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2dcuzjktx.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2oirpfkpe.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2rswjyirh.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2rvduygpa.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2jykwstrd.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2gfcgmujv.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2ntdbkjwx.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2qrczhyom.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2qhgagbwg.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2zaqrxnhu.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2oobwhwhv.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2lfgjgtok.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2hsyoudsc.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2kjsokkbj.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2kbnbiune.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2watxhwxj.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2yqhoiiqy.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2zzprgsje.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2scdxtgtx.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2jkbovlyu.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2arksopvf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2corgyahl.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2nrhznlpi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ubthgvww.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2trdwhwsk.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2tkrggbom.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2wjbpohtq.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2xrhgwtye.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2hotfhtmf.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2gltitskx.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2znorgtvf.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2mnyqtdox.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2xnadejlb.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2bppodgvv.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2vijahxub.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2qvkwyznw.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2aasnvznf.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2ubhxocby.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2ldpgqeuu.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2tqjhgvgd.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2pwyxyzoh.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2zgigihvz.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2uaykvalr.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2ytfjewei.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2rufdcydo.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2dsbmneos.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2ayylwobf.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2eybqhyaq.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2xqenyfgb.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2mattoloz.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2vtaedrjv.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2rgfefgwh.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mocuxzqo.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2nfmodico.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2wnlntusv.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2yzbtstcp.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2njujpjrs.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2jnibmlxk.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2bjqtdtii.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2pslfefuo.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2yqcsfisk.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2vygdijcy.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2qxacyocx.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2znplcoco.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2kxrytoep.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2krxptivj.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2bwnmapbr.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2zybncnxg.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2fscdnijd.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2nqojbpwe.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2mvaffaiv.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2esnwrcco.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2oizuante.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2pqbshyda.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2rgpllyvm.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2cqychszg.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2bbedzujp.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2odmhjcde.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2cilauqux.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2ijiwhcht.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2pzqnhutm.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2hiuryqne.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2tvpdgnpr.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2zexdvawq.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2zolnqmms.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2fqneugyo.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2dofhwatu.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2lmcsxkgj.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2nfawnivy.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2mcwlwjhl.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ptrrtioa.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2yzlpoxgr.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2wjgstzen.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2wdjzrtpt.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2zzzsxzmq.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2btaeawdk.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2mktqothh.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2vnwptswb.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2cjkvhpmn.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2vgaipdsh.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2vwrgxzlp.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2jxmupbwb.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2hwqaqpft.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2aqnmvxam.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2qosdktjj.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2dglmihye.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2ooavsgmn.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2bhpwewco.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2jedlopum.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2aatkxbfk.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2qjgnxvjf.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2zjlipwkw.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2kqfsaudm.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2xtoeiqaz.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2iynrxbww.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2mebxpjmr.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2anmvoons.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2xtfpyiph.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2xqaexcrw.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2lfcagpic.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2tnmypgos.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2dgnrpsam.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2yyhhtqfz.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2jodmrtmv.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2tgdcrouf.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2zmigitty.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2vfmstsgj.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2orblgkqo.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2ihfzmpkm.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2cmkjrwvm.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2jqgipqpz.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2addknayk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2arnlfiyw.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2dlldqyhq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xcgqxbdv.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2regcemmj.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2tvvynzej.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2ahsnylow.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2zjyefucp.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2fwjftavb.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2swwwxmof.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2gdbwigjc.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2geltqhtw.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2xaqxaqil.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2wedfzbea.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2ugipupmq.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2ghjohume.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2isvdhyzp.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2xrlidiuw.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2qmqdfaap.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2nwiertxi.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2uremuyif.html


<!-- 参考信息 -->