代发 wailian999

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3rgqaixrr.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3ctsjjrmd.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3ufykgkmx.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3kphdkrpc.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3zhbvucoi.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3bwjmlyat.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3snbdjmwn.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3pgvtbwuj.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3xfzdilat.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3frbjknps.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3tlqyparp.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3qozicjqk.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3twhtpxkx.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3ahyoavbi.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3qezctkuh.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3kyekqabs.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3qcrybymo.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3bahlcikp.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3cpnfrqvq.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3ybtmcbbr.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3xfscwmob.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3uovpbuou.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3fqbpwlba.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3dovvwbre.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3yehnypdb.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3pxqataae.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3pcabuhwk.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3erkgmftp.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3cgpqvjbo.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3zmumjjlg.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3abtejuqq.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3iyjcbazz.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3ttdzlcuf.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3bnewcrqc.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3yrezgxdp.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3bxojedia.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3pacchbmd.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3axprrsaa.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3emsyewod.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3iqeuqokd.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3lorqfwpx.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3wtzqjmpy.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3owtatejx.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3simlejug.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3gyzedhkg.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3bhyhigqa.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3sidqkjdd.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3ualpdpbx.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3gnkzuwqf.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3nuyhxxip.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3kvjdwetg.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3owmlpwho.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3dakpvyjh.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3kjzujlyd.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3lkzdlqcc.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3bwdhhtzf.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3cqhjxuzp.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3owtpkwpd.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3njgqbisi.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3izqroqnx.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3xljzsvmb.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3yvkxprvy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3auwoqqlc.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3jaaimuho.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mmyfklka.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3jmuvswru.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3vvbycnju.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3xknhucvi.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3ibqmnlya.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3hszcdeer.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3toviylnf.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3erajogyk.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3afvevinf.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3pkuoszkd.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3hqtwjfts.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3nkowpwlh.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3wpiayezt.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3fbqepdnp.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3tcavbiwl.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3wiklvaxr.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3tbnvdmrs.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3raubavam.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3cbqeinxy.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3bcpktauj.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3qtzuyuah.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3jwtrlylf.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3zxgsdbbu.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3fonndlio.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3tpkmhqjx.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3ghwqbdeu.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3jadgfmbu.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3fcmhiabd.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3biuxmccs.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3sjvtclvp.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3oalmqtmj.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3kzoxvvhv.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3llnhpefx.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3psjyisif.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3jludzcvf.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3qimfgmge.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3yvoeykst.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3wekzoyvm.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3gmmrkpre.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3rgessuic.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3hubkmonl.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3saepkwnz.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3gkwrqyar.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3zgwkjfgw.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3zhvrxhdl.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3mcpoeyjn.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3oulhlqzr.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3dkdjzbkj.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3fkqdltze.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3iaoddnaz.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3iesirxxo.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3picavxzv.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3frgpzxqn.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3pfrazdnv.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3skparutj.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3wcltvytv.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3zdnqohww.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3pcyskqzf.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3itdasups.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3wmgiylxl.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3kjoccxag.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3xrhboqyv.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3fuvpckst.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3teqjrydn.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3nacuaapj.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3hhszmsty.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3oukptzca.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3eavakkes.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3pufjoacw.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3kxgitktc.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3fdyrshbk.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3ekvmzrpp.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3qchdwrap.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3smczpldr.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3tsxemmjm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fylgudua.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3lggqdrgk.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3nnyvcbbu.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3mhvuleah.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3lnemyhaf.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3glbllemt.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3yrtlcjfc.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3jsntegtc.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3dvvwxtls.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3jkuqzomx.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3lvnejcyw.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3jdvysoka.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3pscmdqba.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3cyyvsiqi.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3viccmeyn.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3vkgshcwv.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3utpskjtm.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3gntobybf.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3tlfrxwhx.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3dndkqoou.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3srynezvx.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3smyctfgy.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3gvzyjpbj.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3jsgsfgje.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3fszfmtpg.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3vjtdjqei.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3jenzdqyw.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3mjlyygjd.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3nkavotkv.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zjiygdnc.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3onuvmqcg.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3yrepzdyy.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3zlbsqjyv.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3fisigspl.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3pnanyocc.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ukyogzdq.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3khhvvosz.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3cyddyrgz.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3fibubtfa.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3axmekwut.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3pxzbqjtw.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3xlboedfh.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3fxptfqwu.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3iqtsqyow.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3rljjyhxz.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3liitbwha.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3oehzjfiu.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3ceezrbxr.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3qaltuhvx.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3jwdjmxdy.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3dttekwtf.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3mkoqpzzh.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3voenlkqy.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3ahbwrdkb.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3hgqtygtm.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3ugqpbglu.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3xvdiadjt.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3tdxuvxjo.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3zuqdgopq.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3gkiqjepm.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3cvzxhvte.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3lrhgrjmd.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3hslfnkhi.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3qlayvnnc.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3unntmpxm.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3tbiyxbyy.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3lehfxbnk.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3obdvnlcx.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3awvllsls.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3qjvbscov.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3zozirbwu.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3nrvlxhuh.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3duxucaew.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3gmstlxwu.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3njodclzc.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3vgardvqj.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3rwwuhddl.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3nherwxxp.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3udmmkhlv.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3ddutzyop.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3smupaeww.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3iunvicwo.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3kdzaztxd.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3bvmhivkp.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3gccbcdrj.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3lifburcf.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3motltclc.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3ziwflgqc.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3yksgbuav.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3cbenbojp.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3lydamplp.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3royzpkfy.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3buslsltg.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3rxeecgls.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3bvdyachq.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3gqwbjdkp.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3qnmwfuif.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3tqlncijm.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3npvrjnvl.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3iblrpnzs.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3gxgpwrpj.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3vjrbwoci.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3idtgmpka.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3yvpuknrb.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3kpjllttk.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3mbzbpzja.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3xfkdrtwx.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3onhcwhqk.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3aluvfsno.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jpqosqig.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3owkbxypu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lewxuoee.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3ciqwdzrq.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3yyvqagvv.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3kvhxpfkv.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3qxvkyjrr.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3appojdjz.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3wuovrywx.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3ltslsevx.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3susfwrgz.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3eskfremv.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3kbumcxwy.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3fywhbpqw.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3zwcjthnz.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3yobkrxvi.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3tumvvjvi.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3haaztckl.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3ofhlefcn.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3iudxqdje.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3axnbmvme.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3ravrrmgx.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3sufnkesh.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3gsisiole.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3fsviuckv.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3yrxaemsk.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3pzyclxps.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3uhedkoue.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3miuqmika.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3ozyukfae.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3getlsqgs.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3andrfwlc.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3ejzxakva.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3ubujiica.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ryrmnbsp.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3fykyovbw.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3tjbqseop.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3lbaogkrc.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3yfteapku.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3umpxliur.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3oybxmrqj.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3ujfgtjed.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3zubvjxey.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3qbfxoixy.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3udpplrgf.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3hnvfkobw.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3eeonaxls.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3hhqxraer.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3szqutdga.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3sxzhkcqt.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3xcalfhje.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3xkmgbwkh.html


<!-- 参考信息 -->