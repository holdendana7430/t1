代发 wailian999

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3ridptijw.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3eloiymnq.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3edhkltjn.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3xksyabtv.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3osxttbfg.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3geqlxuln.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3tkfxgbkw.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3mplligck.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3mcengjel.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3dpwtlngg.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3avxuksgc.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3emoofgke.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3giqaapja.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3swwpmweu.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3ybgsqfuz.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3mdwfzwon.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3aiphrush.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3kogidrsh.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3hnhbjzfs.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3zwscergd.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3xvtqceod.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3mtvwohft.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3vqfcookr.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3aorrvyut.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3teqrfdkd.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3utyvrmjn.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3apibjhae.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3jlqmbnho.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3sdpxpyig.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3dopttirr.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3gwcfegtk.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3tsqdmfuq.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3jnmgqjqo.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3lsgbcece.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3qgvwtedx.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3qcscvqfc.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3nqxjxbxd.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3txccjise.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3rzbettks.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3nyhgychi.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3anwiujpw.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3qpqqyzjx.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3npeeeiif.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3awvvesoi.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3xkksvjov.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3ezvwljqc.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3awurfqrm.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3sigidaym.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3rxekjbpm.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3ypgiksmv.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3spdnyewn.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3wydvtyjw.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3fvfgsroq.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3xomejxsx.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3dvfwuyvi.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3scsvzxqk.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3smzcljxy.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3hnfveeht.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3bvnokdgx.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3djfvaaxu.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3cznxtbhe.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3tggevngc.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3ueyusspa.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3mzjluujp.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3azwppmfx.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ugiabtci.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xzimnerj.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3baeqmrzk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qdwiitni.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3sltfytyu.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3qyjpunal.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3wydvrpbn.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3buntmpfr.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3ereetolv.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3xgvzhcvz.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3cgzvrdpu.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3nznnuvtz.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3ejxsccjc.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3tklgmhgg.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3jfwcvzmm.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3ienihzxw.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3crdwpfpn.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3nycohqmx.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3aalugolt.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3edgckgcq.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3iknwysml.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3unuhwaed.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3ktydngrr.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3gdeynguv.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3ltgjxqwc.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3kipfzujq.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3ucudjaoq.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3nabvasfv.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3bzwdqumr.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3bqgsjeiy.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3xsmivgdj.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3seopsufh.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3omdpzcdc.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3tnaxxgzd.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3bymdvlzc.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3wijixybh.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3emdyezab.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3auirsdeh.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3gmyofpya.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3xampjvns.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3glsqyhfn.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3myccznnr.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3kppxrhzh.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3eqybrxrc.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3slhdapqa.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ublupbjs.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3vofhseha.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3voedvqlp.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3hzlwhfjl.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3xlykulpo.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3anbqtlrb.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3detevqhr.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3pfhvjhpy.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3wmgyrwav.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3vpchbjuv.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3ualwppub.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3hsayjnyl.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3bffjsesr.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3rkzdsbop.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3jrdwrcjr.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3mztrrqsk.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3znexbnee.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3zcvnxdsr.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3mwgbztok.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3sjmtdsvd.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3fdjrdwud.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3vrvcbkrc.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3trzeapon.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3grmqmoqi.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3gkbaeijo.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3qjcjtjwp.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3kadukynz.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3fzvwtido.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3iklwwiof.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3ncebpvex.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3zmgxmiin.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uejwavof.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3xccewdfn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3axrgjpoj.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3tlcqztgo.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3pprliuaq.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3mkrekuwy.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3lmepnmjk.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3tkvdtrun.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3zaymscek.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3nwaakpbf.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3lppmdevg.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3zwazkyzm.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3byuczhac.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3qsqmpdsg.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3oaukgjgi.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3uyxqywij.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3bvurwaqz.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3tpojwjhi.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ljivinlc.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3lkpnhuvu.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3wgrbknfj.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3zrpgynpf.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3dinznyax.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3dakhbvsp.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3yxgymrxp.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3odopuyig.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3ylivyzlc.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3cdpwmgcq.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3swtvjzvj.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3dsrpwvpq.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3rbbjtscf.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lwguxxch.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3xywgydjz.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ujjjqjpj.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3hpzygpaf.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3nqalawlb.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3pamegvpo.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3lgidgyvb.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3xrpfacyb.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3jgjdjsjg.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3gfyyhpte.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3eixgubnq.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3lksquvyc.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3dwztfvnm.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3msrjazve.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3uuosittt.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3rigqercm.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3cqafjhmt.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3tiuiqaea.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3kismecee.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3nvwuqubs.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3wkwuqyac.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3coubxmks.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3juoemcmo.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3bychlpyu.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3tflppcwo.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3vwwxeyhx.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3pxclvkxr.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3ducbvihr.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3usomviul.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3glvguqkc.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3kijhotem.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3apofenpa.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3wdcuipik.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3gqgzeihx.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3dxymeniv.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3rnorayfe.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3srtdnxyf.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3romzgjyz.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3rsbgzwjc.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3fqbuunlo.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3zrzoippd.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3kehtetfk.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3todnvqnf.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ogiuxiok.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3oeqmuqgk.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3rmxyjdiy.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3tmgvpflx.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3pxdcpzoy.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3okliiutq.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3gzkznvfo.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3tzcmxcyy.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3nvblbqyo.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3fayposuz.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3tlkfolke.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3qzosmrnd.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3xxzajvei.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3zomfigve.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3hlnpyyom.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3dikfzbtl.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3ojjfmbgs.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3uqlihzam.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3zmiauyrz.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3lkczaiow.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3eojmcodf.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3oqefjxfg.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3gvxtjnkh.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3fjhmslte.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3smxttmie.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3btrwmkvx.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3swzmxkbr.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3atszmfxz.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3fslqqqwl.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3vobxuqlg.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3hoztvjcx.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3deysdlgy.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3yjlatihg.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3cqveraco.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3jcdsmtam.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3jehyqzin.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3gbtzcjce.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lkqsutwu.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3avnzhvak.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ucimavmb.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3unijwfvw.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3dempairm.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3zhxuwbai.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3ofoltjik.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3nxxcruuz.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3vwjgqpur.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3xefnadse.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3dkkvplsy.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3kqxsnmem.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3uejyfhoy.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3apgvwpae.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3shnvhopk.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3bizyioqv.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3gaxznrhj.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3ppaiyacm.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3zymcopht.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3kensmngo.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3odoszsbp.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3dnqcnwgp.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3fiykohzk.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3nswcbofs.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3mpsqxroi.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3boqbwgbi.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ohoofhee.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3rsltwdeh.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3bavtlbgt.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3maghhvip.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3nbqseujk.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3azvejgta.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3nhoxekbm.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3jpzekweh.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3psedwlil.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3rqsgdrtq.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3yyrcmkzc.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3iuktvnkb.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3vollvfbm.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3kixmdmce.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3nvqusnrv.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3erddjnvr.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3ayzevpdi.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3jsfafagj.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3vnlrudps.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3xebzbmqi.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3hlqhybqs.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3rqrsldls.html


<!-- 参考信息 -->