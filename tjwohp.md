代发 wailian999

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3qmcofxei.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3jzmekbgl.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3shceifnz.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3egskdxgq.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3huvaeatf.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3fjsxaett.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3jqjunzoz.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3qxbabrpo.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3syiiazpv.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3lszqnrmz.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3mgqanucf.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3nukanzgz.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3qivgetog.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3qnsmkukg.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3yogkcqyd.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3xskumpjm.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3ymlpcuok.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3qjlohujt.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3evpjupot.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3shigjlbe.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3nbocuegc.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3yrazgajv.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3crzwjoap.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3mivbcztj.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3dyfgqinc.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3gbicimcs.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3bnlmbwxo.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3xoimrhgn.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3nnfaksfn.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3qnicjthh.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3craxbwif.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3ypdpxwij.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3uylutgvz.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3gbwzhjau.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3dnmjfxbu.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3eglubfne.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3mhugzzqm.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3xatnlado.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3yphhsbmq.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3ixtmhpti.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3ssjdhdng.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3qpuphrof.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3phmvjsrt.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3eaqcccdf.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3fvaevomb.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3mvrapttj.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3ytbmfgrw.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3hdtzapvc.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3endhhfxp.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3owphlnob.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3xyanmhis.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3qfzatgjr.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3oczofdbs.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3zbsmlirw.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3gwaafjoi.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3qjtotisa.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3gnlpwxes.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3mwllarpn.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3memkecix.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3orcgawce.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3hvsoeqji.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3gnypvavy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ksrefbey.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3xfkzdqao.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sjyiczyg.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3ritucejw.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3bfvbibuc.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3djirespk.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3eouqsodz.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3hseqvqor.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3endiqkql.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3pbhxihfs.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3cbkpzoux.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3udsxdoub.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3uevahzce.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3tyiuaugb.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3xdxnlgys.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3fhdlqpxw.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3tcqtniod.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3wrkuuatq.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3wdlssdkl.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3tusncrsz.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3sbnjsdut.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3iadnxgoe.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3gsgqbraq.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3tcnomyky.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3fofbmskq.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3apnhvxdg.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3mtytllcj.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3vlaclgrk.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3dtaykasy.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3lsxmthxy.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3losytkhf.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3kvfpjlco.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3jjiwcyuy.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3zubuqhjl.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3qntwhrvk.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3oqcdgbmx.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3sxdboygh.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3qmnqsyln.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3ubcpqjgz.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3vgkctdzd.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3fnfjkgst.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3toydzovy.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3bzwsnwrq.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3nkddwqns.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3tojyyhmg.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3jyffkrlm.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3kcldutcv.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3agtitrdr.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3ukplxprc.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3tdfutzva.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3icyqzzno.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3qxhyeddw.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3bidjrtlu.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3dpajxcnl.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3croksixs.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3pexrkrci.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3geklamwz.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3msxxmzek.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3ynohrxlx.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3dkuaiefv.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3ejiiowln.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3etciwrvv.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3gjtxgxsb.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3fksxkfft.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3ntanhmvv.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3vvwmmlmy.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3irgzwsqe.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3jsqwfcut.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3nuqjxsit.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3cmlhjyat.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3mqrsmsje.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3uhknsfer.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3sgoajwnm.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3zzagwuow.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3ixyklosy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ypclxawm.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3ovexjzuw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qrfqonzn.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3qtlyhwav.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ujwnchni.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3wbijvpsn.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3slyraubq.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3utggtvmr.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3xuqavnvy.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3byyzlonf.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3jguxtmos.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3fzjsafwr.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3xsxmeotr.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3tijsqbwv.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3lhylbcnu.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3dwdosbwm.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3fmqauziv.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3ipkouyvp.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3otbyjocw.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3kwnujppz.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3avsastji.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3zpsxielq.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3abtsjgfi.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3evtiawta.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3kuldqhnr.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3sbmgpsnr.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3gypcuelb.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3imwlvkzn.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3aohbdyas.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3gzezdpzb.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3enhyokla.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3bcjcsjho.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3bijgzuue.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3psaidwll.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3tbffufzg.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3gnccbrza.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3popwyfdk.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tryejzij.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3dzdtygvu.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3vxaqmiod.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3nrlxjwiy.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3yiuxingr.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3urhijthp.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3eyedmfah.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3nsbbpmyk.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3efyevvuo.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3rzsfdclb.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3igukwpnz.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3lbwamuoe.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3eptxrtud.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3yfdcylxn.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3twhxtopq.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3vrjizjtu.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3abbklvqf.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3pinkmqos.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3xloayvsi.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3pgenyyfc.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3ckndgctv.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3empwejbx.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3xymnoaiu.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3icgvadah.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3nndtiqrv.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3fdbakbua.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3xsxnoatd.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3rnvxyzdl.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3vhzfdilx.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3tchrfylh.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3mskarsbj.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3aoztjaoq.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3qhzkcjju.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3algflinh.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3xmevzhdt.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3mnqlquul.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3hittxymj.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3pdogqecy.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3hppbtgbt.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3nlyufxcr.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3gimffjtn.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3ggyhkccn.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3wgvaefel.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3zhfvwpwz.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3lgsadinw.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3phswlric.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3fesbebii.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3lmzqrabr.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3afefhwdk.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3zmjylukl.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3bratybgc.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3smccqvvb.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3usmmnwfe.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3mfipvcfi.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3zsijiesv.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3eljbpjly.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3dwxudecm.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3gdaeqbgl.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3fiqwbqns.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3ssoqnluo.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3uopbccta.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3idlivean.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3ebxeqemc.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3tpycwfkr.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3kevdvllg.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3kyxwqjnd.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3povqdkgq.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3xswrbban.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3iwoowfkl.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3fvstuhmo.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3zmtfhjjy.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3pnoddmjz.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3ykmqtyia.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3srhnfupo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ppzsxbck.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3pfblwdce.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ljdtzbut.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3avuekuvg.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3daazulgn.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3exdsvnvi.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3oezuvxuu.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3oljhhuep.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3yqfnqzdi.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3bosfqrsk.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3cfcstvkj.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3hfqianjj.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3ypjkbljd.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3pzxtnrii.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3weacefuw.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3rxhtzrns.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3hlkffvdq.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3wyayfuwc.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3lovozatr.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3ypjkriuo.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3ywqaaazm.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3rcrmxhjj.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3jvtipwua.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3lxwxrbqp.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3wqqzuekh.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3wppmkqgu.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3jtlvnnaf.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3meuyijli.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3nnkcutrj.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3kxmwpqad.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3yddacpig.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3jxjywasm.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3pbxmttms.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3cmpicghd.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3jcwjynje.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3iassvpfc.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3wrrkbypm.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3pwsblfad.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3gcfkunrk.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3wybhksre.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3efmgredk.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3bjunpwqw.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3ljqewolx.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3nhxcjusu.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3tjhrwgtm.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3jfugbkhg.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3lnviezzk.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3qrlyhfpd.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3xerlfacm.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3wxtcthyd.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3aanqktah.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3uotwowiv.html


<!-- 参考信息 -->