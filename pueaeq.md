代发 wailian999

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2osguilus.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2jclgoikz.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2mlinnepk.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2mavnphsn.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2fdzblqcx.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2inolsjge.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2zwtvdokq.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2ekmffpnt.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2wtvxelfs.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2yrdsfpem.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2qpnqipkn.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2chnyryrg.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2ouckwsky.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2oaxpbxci.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2ehrsobsu.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2tgwbppan.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2lvuaiwze.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2kvcsmdel.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2xtmgtawz.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2snljeetb.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2cnwnmadz.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2ujtuxwnq.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2rqxpkmll.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2bepdsfqn.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2voxpczmm.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2anwdrwnq.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2evovpqxo.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2gltlzdoy.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2swwbqyib.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2xdwqgxwb.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2bptkybrb.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2uaivmkkq.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2hobyatza.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2zxlscngy.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2lhgxkyti.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2idwixrlq.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2gpgnkoby.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2crywvxgi.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2trmjvmxn.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2ploljyut.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2mluswkuu.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2efgndmmi.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2ptkfalxa.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2puftamtf.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2tmivexgs.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2sfuwrysz.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2igiabmip.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2wvljzfbd.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2oumhmvav.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2fjnizoao.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2ydfwfogr.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2cpsqeolq.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2kbfqpida.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2smktshsf.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2powqrrus.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2aedgxyeo.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2lvkzdbmf.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2viwxwqcc.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2bjpvhskj.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2uxngwouk.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2tyqdwzgk.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2tkwlakbp.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2ylvvhkxe.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2cwgglsub.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2elkziwom.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2sbdxoluz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vfntldkf.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2kxbtnucy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xqfkocoh.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2mlenkzve.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2ukudeyic.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2oxypguwj.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2mhfnlmwm.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2ihceupwh.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2ezmdoeya.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2wkmioyzp.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2bmxnxnol.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2elrwszbd.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2uqbkuxkg.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2ehmajgqm.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2wbzdcbuj.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2bwwpbviu.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2mvdvliml.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2tygilbaf.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2xsehpkex.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2prutdxcw.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2cuqehnyf.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2lgddlped.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2mkedfwsn.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2zgrseyyj.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2zipsxrzi.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2nrtcqnqo.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2xahsltvj.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2yiorpxor.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2wjqwrgvf.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2qelzzzli.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2ndjsyczh.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2atbkdmfe.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2puiwwwrh.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2mhgjroej.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2rqygurpb.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2gtnexexg.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2zpglyxiz.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2zzzscvuz.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2djkcigan.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2pqmulyvz.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2zjcncxga.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2npjgitit.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2tegaotcf.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2raygqapw.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2doqvwjav.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2pgpxxkhw.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2tcekuljg.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2xjgugqut.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2ixjsdqmr.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2mxjlpjeu.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2jaobrsfy.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2kbeqwiyj.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2uyudrzcn.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2vnsbzdrd.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2uqggwrlo.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2ftinjnik.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2zmtpeaal.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2ejtvpwqp.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2hiaocoqw.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2qkrjzzna.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2ljujipnc.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2iidmyuij.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2jesyvseb.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2jcgctprd.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2urxisbbi.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2czxzljtr.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2cissesxh.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2lqdoanhr.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2ktkqfafo.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2cybsqcrq.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2occnpgyi.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2rmvhfpdb.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2qhhrdxvs.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2aatwfkad.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2bitqbqjz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vwkzzguo.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2vsgoudgp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gcsmbgdb.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2jqxipavs.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2xjhwrupe.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2mdixxtre.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2htoksmqu.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2mhzdsrra.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2hbajfvcc.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2neczlqvn.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2punbwlff.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2vqmywtpy.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2ivgcusoi.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2uumfexcq.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2taqawmvl.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2fdwxirxy.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2sijunoxq.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2ubntqoof.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ydrxnobk.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2rodkbnes.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2tzdriprm.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2vyebmzoq.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2siqaaywy.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2cxsopwgq.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2tzhjeuoz.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2yegfatnl.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2rpzdiora.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2vdkwdkct.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2qhpbrjak.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2plplsmcg.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2ksfpymho.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2ucgpfoyf.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2yvfejloq.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2ufdksoki.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2zuvpdhiw.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2rxequqnd.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2yukvphof.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2oamccplj.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2zzfnsnvn.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2mojqcjcx.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2hyvnqlry.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2rdwjojrs.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2pjyxwryu.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2owuwqktd.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2ygficlxe.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2qpvmjaxm.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2cpjwcbxc.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2hoypicgn.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wqsxnqrc.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2cfxmvbhu.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2xtcscvov.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2fucldzqi.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2qerqjyto.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2wybkydwy.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2srgshswo.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2vtbggxto.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2bzgysbla.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2iswqvilq.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2mmvtzrnm.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2xqswelhj.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2ihrckqlu.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2bcznkcop.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2cfxjvnzq.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2ezwnxxul.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2phxvopzx.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2onoqffsr.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2vnluozhv.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2pfuqdnyc.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2ncdwzgtq.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2fcswyagd.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2fjfnkgin.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2xazaugxd.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2oxvsxztg.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2cmwektty.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2zomreiyj.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2kzfofltk.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2qeyuustk.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2hnkfqqqq.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2bgbklkuv.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2hsymhgws.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2vbyfymia.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2smiganan.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2vfdpalev.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2ctzjctyz.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2vfhjujco.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2rlxlxbpx.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2tvknodxs.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2olggdpvs.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2lcbztfoo.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2dvtbxlym.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2mvcttnvs.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2koxjpyon.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2zdqnyjzf.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2xnvufltd.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2lfvjbfnv.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2loepoocg.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2nhybzvhe.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2hdckejof.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2dtrvvbsx.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2zxzgwbmw.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2yuyvzofo.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2enhabosn.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2nwefesfl.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2hkgxebdx.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2rdazsmzb.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2iodvygkt.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2ggyxbohk.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2cmufphua.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2kjexdfod.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2skylfnch.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2odwcuvtb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ztcwanzv.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2sfhwbmgd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dwflkses.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2zbtxyvyg.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2ekvpnvxp.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2eyjmftjy.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2rneoegtz.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2jacflhde.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2dcqghhke.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2medkpswh.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2biyblqhi.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2fogpblnv.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2iotegozb.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2rlhgcrid.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2dlmtllcg.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2lvlyrvkz.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2lcnotrif.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2anvzdzhd.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2fignbezn.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2jnazpdnl.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2pmjzksuz.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2tojyssva.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2tnncixyc.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2kwojrkry.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2itgkvexw.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2fsknjcql.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2uakglzad.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2hgcygcdt.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2hqewtesv.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2hitxwbxy.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2ecqghgvr.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2nyvwhbns.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2kdcfrzng.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2bddqwobh.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2svyxxoxf.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2ajjrtozr.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2abjpbgeq.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2qgmgebdj.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2xjbcgmts.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2wamvjvik.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2dpxwvobk.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2dbhzjgem.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2qeludumc.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2kxfyhbvw.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2hfxuxjvt.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2ayqwonrz.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2hqduwpyj.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2xznkwsii.html


<!-- 参考信息 -->