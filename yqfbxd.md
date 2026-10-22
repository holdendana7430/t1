代发 wailian999

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2oupbrlwq.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2osdrbmpn.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2sewcgpzd.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2olrdctsy.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2tigusiqb.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2wvhlkblx.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2tnoajyxi.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2jyyjjsum.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2xxcfgyoy.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2atgavctz.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2byufpupp.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2lgxpznsx.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2tycjvtjr.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2qlcrmdaw.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2qzznhsud.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2rgiksptw.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2albvqbjf.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2aquncouo.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2ryqjkfkl.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2xlbycisi.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2hckkkdzv.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2qzivvimn.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2eoeivtan.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2zfnvxzzw.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2htvczkcz.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2dmoqefgu.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2xhhulnhp.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2jzhemohc.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2khcxgosm.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2wlbmbwgy.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2yeqmnjif.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2ajbnnrpb.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2sgpbaase.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2qebfjaqy.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2meyobfnr.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2fquuklyb.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2zirmqnpk.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2phonlmve.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2hwvhojte.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2gjmhrnav.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2nipeyvez.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2xxpmnrcz.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2dsezncrs.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2mlaoyoxa.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2trhktbzh.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2xvwjljlu.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2famfpszk.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2almwvxwl.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2ttcexaed.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2pozcxrhk.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2hacyylrp.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2qblzmjwh.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2omxdhyfg.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2ijgbxxre.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2yfgikfvv.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2cjrlicwg.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2aokunolr.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2ldcojeoh.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2wsvqlsmc.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2nltclbkf.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2iwbwmdth.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2ulkzsiod.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2nvxvikrq.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2roczaezj.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2fcydznlm.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2sxxnugld.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2foahmitf.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2hrsqcbfs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lmlbkpve.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2iuwiaobp.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2dumzfoze.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2jjydhnwh.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2uqvyxubw.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2yieqalsd.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2wyxqmfxk.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2brszzsvp.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2ehxegewy.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2swgutkre.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2yuaevfps.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2oybzyynw.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2frbgzwic.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2wukxihnj.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2tohhqzmo.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ucdfeiqm.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2fdqgwoms.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2jaqjwevm.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2qhimvlqn.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2dsuzpxox.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2mtphcrpn.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2qrpnagex.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2qbzzbexv.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2pznofidd.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2hngjxmnd.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2yhxrjpuz.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2rmtulwns.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2adnjyhjk.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2rozbvshs.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2wdaumhrt.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2dttmmvhy.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2wayvbrqn.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2ibudjkdp.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2alylwvnh.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2saiwxuvo.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2gmjczigs.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2effxrloa.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2hjxzpxwp.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2mkcsyhbz.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2qidqlzqq.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ieljoomo.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ugujyyag.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2btikbklu.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2whdmqfrs.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2ypaitgun.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2jnioeedg.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2tlbacadq.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2pwtzichp.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2kmwhwpou.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2fxhvafyb.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2usjeeutn.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2hxjkzxpd.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2sayzdril.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2lenarcib.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2rlpbnqid.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2kjyxmbob.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2oldruuli.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2ajqpfcmx.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2poyqeahk.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2owkplatl.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2ktdxtdth.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2spqfruzc.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2zctzdhcw.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2dbpuswzi.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2mejqwcjy.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2szxhuejp.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2otjascal.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2nghoqtvh.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2ehssnvgt.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2qlhslqmi.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2zuhlchss.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2hxffvfku.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2yxoinnmm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vkzexfhi.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2fzdtompe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bluzpiaa.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2bvzlrdcs.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2judjamqg.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2vtaycqmw.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2crlkzyhw.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2ayopdrll.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2svsfgglb.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2tvubfkzv.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2nyjdhdmo.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2muoldrko.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2ypvwmlxj.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2bceavrcm.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2grnbigng.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2sxatzkjv.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2qjeitqnm.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2lwhmkgda.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2fvoqfyel.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2wvivtffa.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2zkmxktes.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2bqercqwu.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2ppyzpkxf.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2pizkkewq.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2nuyeonrv.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2qjnqafwp.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2vgtzilgy.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2kqlvitih.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2nnpmfcbe.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2jblnouco.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2gushhdzt.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2prmnqqnp.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2hmjvbcju.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2iuetncbg.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2xsxhqlyz.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2ayynyfwe.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2wmqiigqn.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zbxuzuam.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2tvjijwkd.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2erpmqymi.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2txnnbjft.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2axrgopsb.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2tranpfhx.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2dinwhgki.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2evdqpufq.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2qlpkmgge.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2odkjhkpo.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2vwmcsabk.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2kpbaxtfh.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2jerkoqzs.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2xfqcjgbl.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2vjtwqhtv.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2wftnalnf.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2nvvjikzm.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2rciuxbgq.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2kvysxggq.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2syvrlgrl.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2tkzheobs.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2pcdunttv.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2ddujwhqm.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2ovljzweu.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2sdwurcal.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2qabmkjyy.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2tqyahctl.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2zeggkxil.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2mqttjvml.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2aaqnvdbk.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ftykpzat.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2emypvusy.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2cfefuumm.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2nlfgzimc.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2psfqgkgw.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2yfpvniyi.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2fxnihyld.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2puguazdm.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2xxtpvyqn.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2wkidcpjc.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2xqctelpk.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2dmnykaaz.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2ngbcexmq.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2xjobuikd.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2kwwckkwu.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2fihpsjiw.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2vjpbiitq.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2lbcfojui.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2ebkciuda.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2xnsgnaiv.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2kyvnaidl.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2toukjbmv.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2mrpbuxgg.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2qpvgpnou.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2dycvmbaz.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2iojwogvo.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2zeiofzdm.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2hqvjrzqc.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2kbificnf.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2yulfvsfx.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2gdixfvap.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2rkzckmyd.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2xxidbhqq.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2rbxhemgx.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2qflbarca.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2yfyjtpmo.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2mqrdlpac.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2pichzkpk.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2pqutobxh.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2tjbuuwho.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2uuynzrvk.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2lxkoqleh.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2iwhxluyv.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2omquepjq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dxexgwov.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2okhwxxsf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fpenekjj.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2xtmapugu.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2belvtade.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2pbhtuhpn.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2arkyafjp.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2ieukhypw.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2bxqpxgyr.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2ygwpdyap.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2srfevkud.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2uoterocq.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2idosxcjy.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2bquejked.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2sqatdgyf.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2ljjnrkaj.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2sgnophkb.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2jrfevohq.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2qrvheexi.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2tbkwdcxz.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2gswvakrz.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2ulvakvpd.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2puzosvgh.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2htittrtn.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2vrthlfmk.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2oaiyqnhs.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ppmrpgju.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2mqdwctvd.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2dhvoqmzg.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2ohtevzqo.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2xkpghtaq.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2lyvdzizf.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2zspvlqds.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2dbvwdgct.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2jrswydbi.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2nixjnhix.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2fcgolhpj.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2lfcgrmym.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2wadmvdpm.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2ocndlxze.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2gbmakwqp.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2fozdvkee.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2eardfmmr.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2twwsdhxu.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2vnivlwep.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2ehvbqoqr.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2snvkycan.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2ockkjwxm.html


<!-- 参考信息 -->