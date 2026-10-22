代发 wailian999

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2owbwnwfj.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2fzkbqqsz.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2oqzpanav.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2uuyeyixi.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2bafzzmtx.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2zraegept.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2wdkwdvqr.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2wqhmgbmg.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2lbdxkqud.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2duynrjte.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2qzwegcdh.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2vcntctuo.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2kzpnkonq.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2bkligohh.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2ryancina.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2keaxnbxv.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2nppnqhqr.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2amfxvzji.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2tztjgbhr.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2pthfnfjn.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2rvtxzrdq.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2guhkwjot.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2rwfyfrqp.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2litgclwk.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2aebnkwjw.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2metalveb.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2ualdcutl.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2weapkaoq.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2yuocibxk.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2kjwbgbte.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2jbnwwtqi.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2diqtucoj.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2ebxvhrmw.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2jwtjywek.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ddzqlomf.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2dkctilnw.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2qbktiawg.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2zelogatx.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2jnqbnndi.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2mofvzdwm.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2lxcolcds.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2aigmnrit.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2nksuuomb.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2wxdsrqac.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2rldbiqea.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2ykcldcpe.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2hkbxqtci.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2oakedfsj.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2hmsiocyp.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2fvonmfdp.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2ykswqopn.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2gcbmpsbe.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2fhdlkixw.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2qsadoyov.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2kmykdviy.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2wudqywwm.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2wvwkwlrb.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2vjkhdmpu.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2mllydfrq.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2ykifhctb.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2mnzfakvk.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2afxnixbs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mbagukju.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2fyywzxaa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2klmbffkf.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2kpdylzpb.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2hnrcooki.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2kjgyvyos.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2vbusujmc.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2gmdefxou.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2lusjkdlq.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2yyoriupm.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2gyilyjuo.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2obsaiirg.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2hjuhoaof.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2mklftamp.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2eqzslohw.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2ktmayqdy.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2pisnlgqc.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2crzxnfoj.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2pmmaylae.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2xgiualky.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2irjhiydp.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2lsedltsk.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2sebjoopy.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2ukkixnhg.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2nzqjyswg.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2tiijcxao.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2iciuppmt.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2ffbrrppe.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2vsufkggz.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2fgmkdxwf.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2mwxqyccy.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2kcxgudvy.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2zhcpjgtm.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2qlhujyza.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ycamitrr.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2pnbssxho.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2unexysts.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2xhejekjs.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2xdlbvyio.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2zdlwkrpk.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2kpcumycx.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2wygsxhgl.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jawyxnjd.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2dcpcyhsr.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hzygskjs.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2cgdpwmqy.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2ethjqvip.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2tnfkefzy.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2peczsjdz.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2ukiesngy.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2okbuspxz.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2jjcvdnca.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2uatmzpsc.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2ljvqnqkx.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2iiiacnze.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2wpcvdfiy.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2wdeqmnwj.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2jzzbvblu.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2nmpdqwpe.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2asdgxlpr.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2lftzjnoe.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2jvqovlfa.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2hqiowhbv.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2mbhppnir.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2wabixiwm.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2euqxjszg.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2bxkejkmt.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2tfawkxkq.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2tmgukncf.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2cuozvkww.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2mynhkgux.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2audymvid.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2eiyzhadd.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2dlhucstr.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2uihzkcrh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fckjlpzf.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2lyllzwuj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ynpqygum.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2zbojxqpw.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2tsxmlyka.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2lclimuja.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2bzgazebg.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2pfqrqray.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2cfahcbsv.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2kfxkspxy.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2psqhftnb.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2pgnkxtak.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2matkdsre.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2gbllntcz.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2mrwcfuzv.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2irirlcow.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2amlvscpz.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2lxjelhkx.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2qctkuhnl.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2sxcykopk.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2vyfzzmmc.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2dygmymmq.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2cdfezrkb.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2qlzvrqmn.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2tijjsnyb.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2qgeblbgh.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2afyorpak.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2xgqjhqis.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2jakuhcud.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2dvihofka.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2vpaqedkd.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2cmvifezk.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2iumemdbo.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2elwxqxgp.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2xqimbqze.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2xavkcuns.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2nfhfhbet.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2robpzhgi.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2gdjdtvwz.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2uyfxtozi.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2feegkveg.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2gbhsczvs.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2dsrxfkbn.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2uytnqkxd.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2hzzwgzng.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2scatllrq.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2bgfprkbh.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2pfqnwavb.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2ckppxces.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2hlvnzqab.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2jlcsggpw.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2igldosbv.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2hccheaot.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2hylwmuzn.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2bsogezxb.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2bqmxczlr.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2rgdxhljj.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2pifaidvq.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2nqbqyumw.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2ggolxzkq.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2hggelvwj.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2dhrwcgen.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2mkdretxx.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2ebacwfiy.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2ijcjiolw.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2baotvxwo.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2nethdzil.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2jgqjhalh.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2zuihkzdx.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ievquxxb.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2vdpucyeu.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2zpohjxxy.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ltxknsns.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2yjqilsgq.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2pirqkacf.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2dagqxrmq.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2jophyuvz.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2fnjxiovh.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2pdgqwzfw.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2khmgqkjf.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2oikdsinb.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2ouaxtdbk.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2thwecdes.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2cskhbpln.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2ejgaqlvq.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2ueglblqo.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2axdrzgbv.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2nwiazjct.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2ydhvwjky.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2hcdjyldp.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2hycutbhu.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2pmjwcpuo.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2tvetocew.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2fpameqpf.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2jrdwcrgg.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2xvbxprok.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2gzkrjnpx.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2pwsshcct.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2pchvfqpw.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2kffeyziw.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2ctueamqc.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2xrcvidzo.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2jjfsjadg.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2ulbjpmnj.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2idxywqop.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2mculfpvg.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2ltxebhdn.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2ejwnhwst.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2eoqhjoph.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2eovmysxm.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2oagbjvqe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sbchhjeb.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2jjkzeepx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hivfzsck.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2ikubmdij.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2zohhgnud.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2xqivqpgc.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2hbuhffar.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2kcvirvji.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2otuzrccm.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2cdrdhclt.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2bvjmxxgg.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2otzezwsv.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2mkxfpheo.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2eowtllzy.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2mrphuykq.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2hzxmcwag.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2mbbnafvk.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2mlqlgwma.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2aozukehw.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2wnmwniee.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2mdenpdgd.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2uelwvfwr.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2lebhlkth.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2ojnffhxb.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2neybdbdn.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2sywenjkr.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2huvpfoag.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2otfwzspl.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2tphmlvfw.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2wnrfyhdu.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2qlcmxcbt.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2nxeqfnfn.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2svzdfmlv.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2coylxbhr.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2ndjgukuq.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2bsquxtat.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2nmunhdbj.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2gniqvueh.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2wmevkktv.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2ujadubil.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2cqzstxel.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2kfzmzpqq.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2moxspjzq.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2aydlbezm.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2yxmyzwwq.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2yjmhedip.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2tgxxkwrw.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2cnoitica.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2wngdmmvo.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2uqovebmj.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2wcntmsgj.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2lxlhvcqf.html


<!-- 参考信息 -->