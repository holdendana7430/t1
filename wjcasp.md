代发 wailian999

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2tatgemuu.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2vzawzjlj.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2lwgeyurf.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2jcpixgjd.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2ijiarjwr.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2jiibxzrq.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2rxynowfq.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2btmvflrn.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2mcrbcdml.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2fefzvsmg.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2uylpunxk.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2kumyzknl.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2cdqvjqny.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2tivxkecu.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2jxbeguzo.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2tipixfeo.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2egvhdlaf.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2ggkdzgjk.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2luxtkkpq.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2hapnkjhd.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2bcsbjyip.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2ohfsfouy.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2dlsgnvcp.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2hpblvnrs.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2ynaojevo.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2ckwxbxqk.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2dvtvdjfd.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2ydnyskmm.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2wcfhsgkj.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2sepnqxec.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2xywxyhxb.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2wutduedw.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2jwvocpmb.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2njabjvxk.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2rgpymnvo.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2ktzvjzcm.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2akagokfn.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2cemilael.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ijmzdctb.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2hxrdcxjp.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2nzgevfjd.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2eyoxwsgn.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2jcmouanw.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2kgsffqvj.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2taittyvq.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2alsoasjy.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2ltthpyei.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2pipmmlzc.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2jonobrwg.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2nbwrhhvh.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2wvjtaxbt.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2zcndaxpz.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2iucyzyrw.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2gcbrilfl.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2wqhqeour.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2pqgtwvmg.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2brgajkjy.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2sflthime.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2nqmetgng.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2sglngdih.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2pzyusqck.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2judvncrt.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2zdtebgkf.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2onzpbsqr.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2hhuunbzs.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2ednyccbq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2deatkbdq.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2eibrhtov.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nieyzkqy.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2kmyzwztq.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2yasnlmfg.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2tbupnlxz.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2cuzrksfj.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2ptjvfvwc.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2xvdllvvs.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2gdffuoyh.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2ovzcgkbc.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2pdkqchsz.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2kphfmqbe.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2llnyizpz.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2wxkljmlw.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2drohlakq.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2ycscfjwa.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2ujqixuwk.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2tpkapmrk.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2whtnfpkb.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2cgmtjnpm.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2kzgfhinj.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2niugwgnn.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2ogusorwi.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2hdjdmtnt.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2phagajkw.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2xpmrubib.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2vpbgsfoy.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2dqbwrqam.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2gbhrojoo.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2oeouivlk.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2hvnpniwu.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2zydhlyjc.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2bnykreqf.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2lmjnosww.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2pvnvdqix.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2jyovbjan.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2khrtxytd.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2lkisjcqx.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2iamsgpoo.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2audfmttx.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2ystwxsjm.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2rczmbybr.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2bajvugdb.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2gvfdtsdn.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qisamuqt.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2lyysezfh.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2jjrhvcda.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2eoxzexkp.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2ldnuopno.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2kqoctblf.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2dclijecc.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2rzrzkgdw.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2wegtugxf.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2aebkofsj.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2tvnqyvft.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2vtydhgtt.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2vcjekkyr.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2gfkekyxa.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2vsuagwpx.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2wioxttew.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2hxwpzetd.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2ktodxary.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2wpptisau.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2zinfgeim.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2ddttuqzf.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2cxecefrm.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2abhrfjtd.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2qdcluqkc.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2wnpsgevf.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2grsafjda.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2fmhbzbxz.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2worwpwlt.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2ztmsdmzd.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2aysmvlza.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uvodbygu.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2gpntrsit.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fcipsgjo.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2wkcvgrfl.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2hcqxnuaq.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2ivkrlfit.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2ansaxuiv.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2nukplnqp.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2atewxbuc.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2yaogdybz.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2frmddyad.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2otyxvfsy.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2liatxtek.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2mptafdhy.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2wirtkurx.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2ueuszgpo.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2nnbbolpz.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2xykiqvro.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2uvockoiq.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2nxkapksr.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2uvqirbbl.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2tcdifswx.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2snefrszr.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2sdbprtvw.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2dpcnlrfr.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2zobawwrm.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2izfxrtbp.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2pzenrjut.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2ckgtaznc.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2cupzaeeu.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2poiubqwu.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2mixuusuc.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2anpcubbw.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2jtebrgcu.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2acojvvev.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2wzjhqgwj.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2kqtoncvg.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2oqcegyst.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2pakqgikq.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2edxwogef.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2lckfyovm.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2unjfmhec.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2lehhzryh.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2akxpligk.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2gdlicvsb.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2ukklspuv.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2jtomtwfx.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2olfstafq.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ioeamkah.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2xwixelfr.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2eogrdvmb.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2lcrhmbfk.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2beeamexy.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2krhtkxui.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2uqgchmlf.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2jbhippsb.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2utsrbqrr.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2sztizzob.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2khwkgvhw.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2zooiwyhl.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2fyndraty.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2prqvptku.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2gyauwfta.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2vtevtfje.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2fyedylwn.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2dfdhfgqc.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2dlimsgqp.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2tqysvzzz.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2wsvaxtwo.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2qhkgluel.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ntoshytc.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2uxhbcjbf.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2wtgugeym.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2rxaggrph.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2vjubdlap.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2dzpnsiai.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2xcwtlvaf.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2dbamduxo.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2vxpyqspq.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2vuwfvkcb.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2ixishepu.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2syxqjkad.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2kmbzjwge.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2ugearqqj.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2wslpscrx.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2nkcnkrem.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2yumfxfdj.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2wwpxjaoa.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2eljbtanx.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2bpbvjocv.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2vbfkpygi.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2krimkqhs.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2kgzlvzjd.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2hfwaibvq.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2cuvgqxvu.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2tzfsqsns.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2swdbwauv.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2piurmpkc.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2vixviaxd.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2eteacakz.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2dxuacavf.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2itlmotxp.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2nhiiuesq.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2nbrhylok.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2gvdzzgih.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2kzltjjpp.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2nclciykt.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2lhujwesw.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2uqdlnxut.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2tzahhdqr.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2vvvcezfx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ewlcewpp.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2cboucess.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jcdxwftl.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2udchffir.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2bqosggxm.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2awnbnezw.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2ivfcvawl.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2pustdzev.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2ugfrjvbk.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2qhdprkud.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2myfrekaj.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2wjzdeobp.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2bzmkovmd.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2zeeebwcj.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2urddlipk.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2cmpvwtbh.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2bdopvaaq.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2frrnffvn.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2wajprfzq.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2dvrutgio.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2dpkywwbw.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2phbngtom.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2oaisduvx.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2lsistxba.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2gmpgvgps.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2jtdlybng.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ajdtvbkg.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2tluuaogp.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2wszafjwz.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2fcifdzgu.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2qufgzetf.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2pldzdwkd.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2xtoueqfx.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2tnyqthxj.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2crpucwij.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2rtzlxpog.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2xevngkhc.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2ioroybcl.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2dqiivzvm.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2ybblviry.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2itdbgiqb.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2jjpogevs.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2ptzhmito.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2lquphoxs.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2pyzkijrk.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2ixoaqpmc.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2rdmeuvfh.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2ncgnquwu.html


<!-- 参考信息 -->