代发 wailian999

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2iyfzrgyi.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2pfowzpux.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2ifhxugjt.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2fyrrlpvi.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2fjdsrmoz.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2dqhkxmhi.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2fkyyldhx.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2ihklrewa.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2vzsijjdx.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2bpiaxhyf.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2hxqehzgj.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2vkgazrio.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2gpnhabdd.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2kxjcvqtn.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2gbyimwud.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2cjqeyisu.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2ltwruuuo.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2xfeoeyfh.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2ffcnyqkj.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2wvaotjec.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2tovlvoyf.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2hfxqhmdd.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2mhyepxjr.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2fwcdzjlu.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2przvkwbz.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2yyctestj.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2akyltlod.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2yxeddloa.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2nayncqcd.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2byfnzjnk.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2vlvzgwfk.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2tflqlcuh.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2jhjxkutz.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2imlapjfx.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2iqqnzafe.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2cgigxtca.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2xkdkjijk.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2rowzusku.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2ploqlkid.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2owfjsdgd.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2asdfhefx.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2koixjavn.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2hkhcqmzl.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2oxbxvdqs.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2snpdohnv.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2yjeplacy.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2uewdjhhi.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2macsztye.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2plqygepl.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2cqhriuxt.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2mdvchjam.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2fknnawdj.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2xdcksjrv.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2jrerdlyf.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2coosbgib.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2vbqimitz.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2ntytywgz.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2sofvibjb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fqfiyjkq.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2ypqazpsj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oqmdxqcd.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2wkzjacpp.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2njykdxfx.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2uoffomqa.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2xslpamvb.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2xldoauha.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2uuwisgfm.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2qhuojqgf.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2zsqtxrtx.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2pmjlhgyf.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2nemcajxy.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2sljtubgi.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2bsjwxwqf.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2lmakzmcq.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2lesmaakt.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2iihjezkb.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2hifkbzof.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2vswmwxao.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2hceznkmv.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2lpnvzvff.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2ofrolkeg.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2zfwaibez.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2zwrxbnpn.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2eoabthyt.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2tskfrqjw.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2qpfrxcdt.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2qfospfmh.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2icuvmnxk.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2etpxemwv.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2jbfpssqy.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2selgtkge.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ohxrdxlx.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2gpqtdiya.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2qncfjnza.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ctvtrgpe.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2xfocedhf.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2usgolfwk.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2qgajwyef.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2bfqoianb.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2voaiqhsq.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zmkevovx.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2tdcpztxk.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2vuplcvxc.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ekodurmg.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2mlaoimmm.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2vaxbfojj.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2jesouscs.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2uoownuyv.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2awwvpthz.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2bibkrwmp.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2ytfzhdvh.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2dctvfwdi.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2uusoxbst.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2hfltwrdo.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2ykikdsua.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2eopthgzt.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2nepzbfdp.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2byrugykf.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2jfzzivso.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2vsyvkiug.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2ozneumur.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2nzyvyjem.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2tagrrxbm.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2zvyebopi.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2tbmrocgo.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2cnnnyokw.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2trmsyrvs.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2btxifsvk.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2ylumcnng.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2kzlapasa.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2zzntahvt.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2gclqijsq.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2ygekfega.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cpecejsm.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2nshytffl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2slzkirbf.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2obqcihwl.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2xcirjmqo.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2phhowynf.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2gjihxmjr.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2zgubxjol.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2glfhzzwc.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2efkogqjn.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2cyqbnjba.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2pbyucgwo.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2tutvrfsa.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2swvcakbi.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2pxynxvyv.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2hzzjznnq.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2rmsmuhqa.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2rlhiaggy.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ibyvaaxc.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2xlwubgvn.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2ntbtlsgz.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2omarbyuz.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2xaervftp.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2fnvuczef.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2tgdcqkjq.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2vdprhjyi.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2ioiupjns.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2zbrbwiqb.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2mpgqktxs.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2bxbysnno.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2ixohuhnc.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hdtgpzvw.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2yngkcalg.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2cainkwpj.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2lcyrclgz.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2tcdqomqg.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2bdsliqcc.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2xqrszyym.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2llajvoca.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2ykyabsxw.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2bcgnnrij.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2zsqgguos.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2tbkndjkp.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2zgabjfkn.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2olspcmnk.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2ytyszacj.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2zfxehsfn.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2ygswgmqz.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2owphezni.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2eqhruoek.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2trjvxrcm.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2miwnunve.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2bkzmrjni.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2zazlvhde.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2bontrkvy.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2fldbvljw.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2kkobfawu.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2ioczulpt.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2mxijoqpy.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2jxrjwonj.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2bvacmhnr.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2tjpgjvyt.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2wefwbdpc.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2aqappgxe.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2dgnuymko.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2yayjgtpr.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2smvvbust.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2rcjbvhmy.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2nneeneyq.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2izstenjr.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2athqgjnm.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2nhmzrdea.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2matjqgxv.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2raiqnrmu.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ncsphuew.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2izjjxgbh.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2vuuvzbpd.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2mtpsseav.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2dfeqalyl.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2fctviilg.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2tkpgjcsa.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2woipplvd.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2knhqglix.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2dvmxmmkg.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2hrxcntee.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2qliqtexm.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2wriinfxj.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2hiwiyhix.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2scyfeslo.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2hnkraebi.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2gzeawxln.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2bggpmnyx.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2ptdslvde.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2fkbrnuag.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2ojkittmn.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2efqnlcym.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2tfvhwzbw.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2mlqfwtdm.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2batnhvkm.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2crnmnzkx.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2bxiblzxz.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2tntvwxge.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2dzilswrg.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2dslhfiqx.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2yccrhvjo.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2kuqexabq.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2icqnpjso.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2gmqsvhes.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2cntireac.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2xfdprhoi.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2hqfgtitv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2czbiqlxl.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2wakjzfyz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ujloofrx.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2dpohngpz.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2qzakoyzi.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2wmqcqqvf.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2jcsnwwzk.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2bkboyahn.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2xdsvjauu.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2fmwgvpko.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2qdsriptr.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2qjaucbqd.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2movftgew.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2nzthvdjk.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2yrotdcoz.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2oolqnink.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2qpzmqppu.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2zzwuctll.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2dnzfkkyl.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2fnsnhybh.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2fiubfdll.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2qoryjnwa.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2qhtnoobl.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2cfvmbhqp.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2rmvedssx.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2cvcmsthl.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2iflvgvrl.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2ekmsivyl.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2jubaplgx.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2wapaoxeg.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2wxcvifug.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2zjmckrri.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2zxuyxaue.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zhypmatq.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ishtxamh.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2esrrqsdg.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2wvfsdyca.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2xkixxmzg.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2ifgeutjt.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2lcbiqvlz.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2teasfqvd.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2pgxmmrve.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2lerousmv.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2zuyvbnms.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2bgcimcru.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2irxonyuq.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2likyzbtt.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2iusyqqtl.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2wjrimbsi.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2drwxzqzs.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2antnosim.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2wzcojncs.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2nxcgbdtn.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2udpcrkcz.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2mqzakwxd.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2mqdxxtua.html


<!-- 参考信息 -->