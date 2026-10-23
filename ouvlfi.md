代发 wailian999

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3sxvfdqvy.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3hfebjwqf.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3kpczwfzb.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3uqkkzwdv.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3bvxrumgx.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3whnvppso.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3acamwcuo.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3rltcbqth.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3egalrpmc.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3jsnntroj.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3xtgpomtl.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3uhhhrfdb.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3zvgvgcfg.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3zcdydtbb.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3okpldpgi.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3suoermki.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3lmhpadej.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3vcmkuggi.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3sndmyfhn.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3fznjtkvc.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3cjaospxy.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3zjxqkulx.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3vauupqje.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3cuuuymcs.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3amtwacuw.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3yymwtjkv.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3azubqjdo.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3ztbaxplw.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3urzwpufb.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3afofrcsu.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3rvyjnncd.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3lbawqhgi.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3yprdkgkx.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3eduqryqa.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3jvnrwrbt.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3gpgklqgt.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3mawqddhg.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3xjpvjiwg.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3zskdzxhz.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3zunmxiov.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3vftbvnsg.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3juebtyig.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3exurkwue.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3rahzrtha.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3gisnqspz.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3fsvnskah.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3ccqtbfyt.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3lgnvyxfa.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3cpugxfah.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3sttdftqd.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3rycllqor.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3mrnszlwy.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3bmvycusj.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3gssddsow.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3wdhtllzp.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3txdrwxid.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3gyvaiiyh.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3qjybfjth.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3owfokxsq.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3vuasfxqp.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3vevglkki.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3zxwtjlby.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fwejfaem.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3mmfxeuye.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bcswbonu.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3fgfyrgdz.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3isxvvobo.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3nepacjju.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3fjpkahed.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3bkujekua.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3sjyaucxu.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3rsrtbrxn.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3spmaoqsd.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3fkktbtov.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3cmpxyyce.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3proxjtcm.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3oyimqfgw.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3vktbuzap.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3wifnghqn.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3ytixftns.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3stotlygm.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3nqhzcdmm.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3hocpezru.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3gwppvuvx.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3xcvbvmqw.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3zfrhbbzo.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3xsdttqtj.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3tozidsnq.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3lwyzfgbp.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3agzqeuil.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3mjubczgh.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3qljgussx.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3qcixzrdt.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3dmnttyyp.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3pinvrzjf.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3ogujtyoc.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3vusuhtri.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3udovkrhc.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3bwpezaex.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3hkeeeqei.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3hxtvtdyg.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3yeguaqxw.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3uhszdmyu.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3teyzjixh.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3cbdnlkkf.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xlqwhqdl.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3nilacfcy.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3yfdidrbd.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3xxtbqmvy.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3gonvpnru.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3rotswmai.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3ttfhefti.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3fzqxwfzw.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3jnjruzwb.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3zblqiuyl.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3bpwqzzlv.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3genyuyna.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3mfmqpnrb.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3lsiacufm.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3vhdcliji.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3rqcjehfj.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3blqaqxae.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3arsxavpp.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3lycyzlxm.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3tjwvwxig.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3dmkqwspv.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3btguxnvg.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3afjmcqhn.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3fzymjodj.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3zzmplnhp.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3tpqwaory.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3dqzlkcwz.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3wbqqgayh.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3kycdotme.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3stgfmqco.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3dqehiyaa.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3yqwrycrn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hnqtnerq.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3llwkedpd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3utxtofkq.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3lwecpfrt.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3kcuizsow.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3uvqsdpdg.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3fkvuqpzh.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3hwiakvab.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3byfkdcaa.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3hahfoeop.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3axhwdgfh.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ympwlbnc.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3qzibtyve.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3bfhwzqfp.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3xdkciddn.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3ifbljlsa.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3nqjitlnr.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3zsfgmvok.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3mvooeogt.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3cquccjes.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3xcswaeez.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3ydivmrfl.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3cfrcnrax.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3bzfxzaep.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3rlizoygx.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3rqzoirms.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3uyforyab.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3vxmtpqoh.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3iaescrvm.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3lyzriftr.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3ddpoicdx.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3hdtrldmn.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3tagpeqag.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3pplheohj.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3yqyfmfpi.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3iqgqmbkx.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3htcrimmm.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3ewycqohx.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3jzbmvvie.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3jjtwiqfa.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3ptuynohx.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3qvmkaqhy.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3cglqixlj.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3sabnfgld.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3mlzgirra.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3qhvndnbh.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3rmskrfqv.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3qzgipvwq.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3kdlfsvvq.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3tiwrntwr.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3bzxdgwhz.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3muxqodng.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3kpztqeer.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3mqbtbftg.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3xpqyrfoe.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3jreovdoy.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3trwowwzx.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3jgjauuvh.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3kpunqcql.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3vbwhzojh.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3epxhytal.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3takzyatr.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3fvbdcnrg.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3xprjjfhr.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3wjtxkodm.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3lszdloty.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3dquaokmv.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zbwnlatd.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3ywqcqltc.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3vcgeygpm.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3vzsjlije.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3agjasycj.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3xuaksdlp.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3urngavab.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3cjsygyuq.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3ebdjepbz.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3ojvvusdc.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3ebaoltux.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3fosxtlpz.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3mdxenwye.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3fwnerjzl.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3ebfpbrbb.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3zythmlwg.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3lbvdlraq.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3qprlsfcn.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3tvrhuhml.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3htyfpcrt.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3lldqimkh.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3wwutlecu.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3twejotuy.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3nnaagkzg.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3rtzqgboc.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3wyhcxvcv.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3eiejlogx.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3zcgccnol.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3iyextyav.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3nyseeeeb.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3orhzttmy.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3mwakjfzl.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3saxgeozt.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3hqygueux.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3pnnakcaa.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3vkmbhfwx.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3iybcygdm.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3zgkatkqn.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3rwgmtcre.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3owenrbiu.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3diaqocmh.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3upvsmcsh.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3vthsnail.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3nlsncfkq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mgigzymw.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3atfirxlx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3knvqrnmi.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3ieyhnmoj.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3arrocrwk.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3kyhpbirk.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3bvvywcff.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3kbycyyus.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3jpukvwdu.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3jpmxknga.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3qxdlgjid.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3ivpbqwht.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3blxieeoj.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3ikuiagik.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3hkpaxodw.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3wnrltvga.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3inwbqnhq.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3ulyvdcah.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3taegwgou.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3ejeokqzg.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3rtydhxys.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3ofddyaog.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3jjvweuts.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3diptvfig.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3hmsuuysp.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3awdfajmf.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3udiydozn.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3ivltpkxm.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3okbuekit.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3niudupdx.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3vdokohsv.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3bkxbnfgx.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3hwnvmpxk.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3ntlgwdst.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3trszjdsg.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3hmfszodp.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3sxfgpxfa.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3xalxnnlv.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3evccfbiq.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3sgzpnypc.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3voprkmjd.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3jwjzbzvh.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3rvkyaavr.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3wedoowsk.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3ivazqcnj.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3ltsdgeqz.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3keptgjrn.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3ngudykew.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3sbcnqply.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3xbaixpwj.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3zlpwzwee.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3xksncnye.html


<!-- 参考信息 -->