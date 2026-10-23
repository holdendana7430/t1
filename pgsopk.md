代发 wailian999

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3crqzicoc.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3ottodkpe.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3daxnhwqj.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3hwtiqzmq.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3fflwqdud.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3jkjjfthw.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3mdzbezls.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3xvpwiceb.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3seyjxrac.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3olefmarj.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3xqwphbnc.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3swhnzhdn.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3embohgaf.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3whxklgpj.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3dchxkqdk.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3njlpgyfq.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3oasamhmb.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3cddzgofw.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3iggscztr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lpescsmz.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3khwmpgij.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vqbmjxho.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3njqsnwma.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3nltsmslc.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3qieihygk.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3gandidsf.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3zkxtuizy.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3ltubjdvr.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3hdfrytza.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3ngxazypw.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3roapfwia.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3eaoakikl.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3mibkvvll.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3pythukpy.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3dkqodasn.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3xwxocggu.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3mvkpjjwi.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3yxbelqzp.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3dvbhfsce.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3mkogqwma.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3ewvkfess.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3tynumkxj.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3rksfxgja.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3nrhmzjvl.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3mhqirmuw.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3bqgffrmz.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3cthmibjq.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3vdbtvjwp.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3lrhatlqa.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3iqqwmltr.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3hxvpdqvv.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3lvfoivoa.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3hjbaqiug.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3dncphqmp.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3urjmxkyx.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3tpmgsrme.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3uwbfbmiq.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3vbzughgo.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3uawydrwz.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3jtjmctcf.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3ojgzmyma.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3ukxzjxwo.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3ojzyplbs.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3xqddrwak.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3kfclvsxq.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3wggrnzbt.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3fganjcyo.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3xktyaxis.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3xmjmciig.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3thxggrct.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3wjiippqn.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3tecnvcuj.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3xfvmegwb.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3yxvkcwzo.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3gyaupobe.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3fqtgwokv.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3fcxghhpa.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3sgwdssrh.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3uogkzhhh.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3gzywjbkb.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3fhzohuaq.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3gibpuksy.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3iwfysqdp.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3mvogmlrg.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3vllftggf.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3wvrvkkyu.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3eiihgkam.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3vbnmmdhc.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3zhjrvgac.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3xsgjuhzi.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3bkrbrtez.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3hvefbjzu.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3ljfbzimu.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3duomsdft.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dgxrjhsd.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3uhvulndr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gxpkwdss.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3jvtotywa.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3mlshaxlh.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3rtzjlnwz.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3zoiwjdsw.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3xmpkufdp.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3pklbdbyf.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3ybziwfjq.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3thlrvquk.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3hnpqepft.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3xwoguvmw.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3wzyujiqu.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3wzchokxc.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3jovakngf.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3mhpdedon.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3yurccniw.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3htpkykme.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3zkgcwozq.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3fxuhvane.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3lchvphko.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3sdrswybf.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3rlmiygcv.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3znghnugc.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3agewldwi.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3mixihthi.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3jxfdpzeu.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3mpdoijst.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3utvhpvjm.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3vamjoark.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3rorgekjf.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3zejfgsdu.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3igjistxa.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3covcqnbl.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3xxwkaxgw.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3jdaiehyo.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3jrjxwwyk.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3pcqhykda.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3wpooiljj.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3qqeinhsf.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3mdhzweui.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3syvlbsmc.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3tsipxcho.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ysgoyyvr.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3cncholfu.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3rpasxznf.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3wgfaducf.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3tmllxcab.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3rcngqysa.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3bprjcyvt.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3tloibxft.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3uhaaptbq.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ylxxbbij.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3fchilwsu.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3wqdoqgnw.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3xznhjwsr.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3qkywpwep.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3qnrbhben.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3txamocwx.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3dhjjbzng.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3rpaerqqq.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3bzqvxirx.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3lguhvlhw.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3uglrsfjl.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3deivnpgi.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3ynuhldss.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3tdsjdbqw.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3tgjsdtse.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3yrwwgmbf.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3pkfepbxp.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3owcnwnsf.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3blauxocy.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3vqfxinhz.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3shcmxgkp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ivtbxpru.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3otwnrtuz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wwkqzcyc.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3svmfanqh.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3hyuilibf.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3wjhnhtxo.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3wjmmamfj.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3dkdzbtho.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3twdqsike.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3pgqvqsed.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3hngdjbwb.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3rjhrgqki.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3midubwjs.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3ikbnezve.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3opbooumy.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3bizlrfup.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3ijkglcya.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3izdizgew.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hrwkcsww.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3oxanjeoa.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3khngkgxl.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3vwrctibd.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3vsuwuxwx.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3rrgrvmsp.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3gjkvfvcu.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3yefwjilw.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3nzaruukt.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3suvnvpkp.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3nohapkvo.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3qouzanzt.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3nljxeddb.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xxalldvz.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3fkqdqzsp.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3icorodyi.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3qslhsnqe.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3tfotpnan.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3fwiwrjmx.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3ufjngdjb.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3gdpqjwif.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3fbfaxqgn.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3bczblhnb.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3akmeivpo.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3raozjhjj.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3xrwnttel.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3zvzpyenh.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3xxccgujg.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3jcxoofta.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3mybimnxh.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zyysdhzi.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3mvdwcrgf.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3mwdsodbm.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3vikdopfj.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3qygetvxp.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3zgwgiqlh.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3snyguhfi.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3loqsdogd.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3eouvnpnw.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3twcuqari.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3otvftlje.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3hmbvotqh.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3caotsmgk.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3krxmfnxn.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3gnzjtywk.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3loieptna.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3zpjmqyzp.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3zipvsode.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3ljpifmtk.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3txovvgkt.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3zpzavjmo.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3sijvsutx.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3prnckryd.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3yglaqall.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3zicdjeiy.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3gickzuhs.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3nvnlfcap.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3mkvkesej.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3octnutem.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3okqdzdcn.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3nlytlipv.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3jyiagbba.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3xdkbbazk.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3hoqfdihn.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3sxjnmurt.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3brxfjjcj.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3dllduuev.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3ppthgdsk.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3sllaezjg.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3eodksxlt.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3lbqvgncz.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3wrlmxmrj.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3qoypgucg.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3mhpdmely.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3tqcsdxmy.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3pkevpycd.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3hofyafni.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3kzbdoxvk.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3dfyixgkg.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3wsdbqagr.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3qdhusqch.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3awhowlas.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3gmjzvjia.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3cznpeohg.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3umgrrptg.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3aomljuri.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3lnolqjoz.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3zgiytwyi.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3fuseyumk.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3cgctyqpe.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3hnlycnvy.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3jictggvc.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3formdqmc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iqxyvvqn.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3rbrmyoyi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bnupitbg.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3cmaqseun.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3buqqvqub.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3rztkduuh.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3zonhphed.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3uoobirtg.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3luzhqvdk.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3srxjkbrw.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3kckebjgn.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3tulifhnn.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3tmlmzgzr.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3zwwgpzwu.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3tvkfzfmo.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3ivtpxcme.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3ytzkswbb.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3wmwidpbq.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3nvjgdusy.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3oraklzep.html


<!-- 参考信息 -->