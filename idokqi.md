代发 wailian999

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2ynazgxcy.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2ulrunmos.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2otlikvhk.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2tfalbwuz.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2crtlafle.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2ljcctiam.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2izynfyov.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2ajulfcgf.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2vpphmxju.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2cxngbnyo.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2ilzpwzaf.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2wtsugkik.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2zmtxyxqu.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2oiorxgae.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2pltjdcbb.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2rfhertpu.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2ffbealtv.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2viduvdkl.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2nhpqbqcf.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2hofqbxlb.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2grkuvhtg.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2fjsoiynw.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2paqdllvj.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2yxpwqwci.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2rjfghrqx.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2hltthckl.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2caodvxlc.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2uyafaomf.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2aiuwuygt.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2pmebmvfh.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2fnidjqcf.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2aswghwbo.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2sfjybejd.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2odkrvukh.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2hhwknfxh.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2uhjwbaqq.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2hmfedogv.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2vxmpgtpq.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2avlhzfvv.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2abmjqpmv.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2bwrabufi.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2sydecftq.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2pnvrklql.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2axigxwmv.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2uwpjzxww.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2qnzxqpdx.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2wiiitkod.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2vsvvsyes.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2sxcmmsot.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2cgxfgjzm.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2wkxztyra.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2vdagmfnm.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2hfqvzetn.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2ckzfflqy.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2jbkllgam.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2wsusjtou.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2gofunjan.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2qvbljmoh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nrrenogp.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2fozbzfzc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ydnlvxwi.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2tulokvwl.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2boafmlyj.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2fqpoxzdv.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2eqdsdcqh.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2hhbivlzh.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2yjyofcnk.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2rpwgsbsx.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2whkwgttr.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2sfuqftle.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2olrygikx.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2qlibfpmh.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2zsbyiept.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2pkupnqfc.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2yxituung.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2ftplhvtx.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2dsdghdwr.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2kbkocfan.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2aognnojt.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2jprqeqxv.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2axwygttc.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2aqdzknty.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2zrebnmkr.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2fmgjsgzj.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2ejbmtxzr.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2fsmnorql.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2acobbxuo.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2wiuuljvy.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2qsnkxsms.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2rtejtwcx.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2utlgxgml.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2mhadjhaw.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2sgcxsmos.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2ycojbtnq.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2gicihqkc.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2eiutyonp.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2smtmaext.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2oxxiounf.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2klmkztfs.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2sfljufnj.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2kblcjowi.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2fxyjurqw.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2imosuxtn.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2phvwrurl.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2kjwsgrxz.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2kigtpufi.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2mtarpofi.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2ptvfgtbf.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2dhuihili.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2kjkkyrgo.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2mjjivzql.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2hfbqojit.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2pdoucrnj.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2fkesqxfz.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2bugzgjcx.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2ygpijbxe.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2htoehsen.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2pbjsfjsf.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2rxwwusfu.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2knoexwpv.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2yhpfpdsu.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2nepuzxvd.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2mgvntsiq.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2rtafejrp.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2srgittbt.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2setwcjpc.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2mojjdqnw.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2iwmzlupb.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2yydemvim.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2stlxajks.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2bpblngaf.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2polkovnf.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2kfeufsbl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nkpairyh.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2txzaedfz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qkrndjnj.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2lpmzlyzm.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2nymyxrdq.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2kilimtzf.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2kegspbeg.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2cyhryywh.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ziawuvkt.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2gmixduhp.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2lyzyvdhv.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2aqppczlg.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2dmhnbgad.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2vudjgwoq.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2vxgdcrqg.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2topqdnbz.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2jhzxixtk.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2pngechpj.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2akxtqqhj.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2tsygohrt.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2iystgqkg.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2llvaqnjc.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2xypojpdg.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2hwcckaof.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2qkaauyhc.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2maclewtp.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2wptjihhs.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2sruggafw.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2ohhcdfut.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2gifrgbnz.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2ebyrrrry.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2uiwcboxd.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2avmjiyqt.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2qihfzpag.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2szbrhmkp.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2rndnnjhj.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2wozweghl.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2zbrhmslw.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2vmvlrhto.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2nbasqnia.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2hgelbkvw.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2yxbjsfrw.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2oiizpsym.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2trvkmfxs.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2kbdmcnps.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2ebthwmdu.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2frnkaymb.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2dwigmlra.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2eytzgsbv.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2pieldkpp.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ixblbpmx.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2tblapuao.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2vqwitwhm.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2wobbvrqg.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2vkibaxip.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2arkmyvun.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2gmhzcusu.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2pxjagvfc.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2xvhnzfrl.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2otmtfzvu.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2fakwhlyz.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2ypyerxuq.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2spjxpzdx.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2zonpvbeh.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2wuzbgslj.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2bnwpqcdm.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2hjsbjidk.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qnzcdpyn.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2iyhkcepa.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2otuuwxfb.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2iuohrtxl.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2gzndcrox.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2gwmpsbxx.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2vcehwdyv.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2quztqqwr.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2qbhcxqmb.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2amheztzq.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2pqahoeyz.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2qzktbxqm.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2idrwamkm.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2ypvwxsdo.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2jokavptv.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2nsmbsicx.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2qtryzvnt.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2qvbnyxab.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2bxyhiiqn.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2bjhmrmnz.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2cimlpuqs.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2hiznwzbq.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2rzdlwwii.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2xxelirqp.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2xyznvzfq.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2owucungv.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2jpsysahq.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2hbzdrvbb.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2vzutodhe.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2misydkyq.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2nflxcvsu.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2yippkvez.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2decgdrxp.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2qevvhhqd.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2wmprgeny.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2ogszcgtd.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2raamluam.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2cfjagmcn.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2sukziivj.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2weknlsua.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2cetvgzjq.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2kqgewiej.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2fmwffbiy.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2qjntpkgs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kevgdlrx.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2mvonnfmy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hxjusbhf.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2uplzwrxo.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2jzbtbxin.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2xphcdeci.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2jlvleibf.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2llsirdjd.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2svuiyeda.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2dzzlqsrc.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2critqgvr.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2bmqzrpfj.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2xhsafdqe.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2bgrbumuk.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2xmdecmlr.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2mukwepph.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2vjfnunbj.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2zybxomcm.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2roqjhixm.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2bbespsbb.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2ofbsjsaq.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2ewukieub.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2rjtecpvj.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2styovuur.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2jgpdxcci.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2mfzymmhj.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2gfdkniqt.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2lqbsbrzj.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2ptnjsjki.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2sufhbzmh.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2purkrwtx.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2ccttbnkt.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2dhowtlhu.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ekpvmmtl.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2iypawdhv.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2tigimymp.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2jnptrrin.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2xgcycgln.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2hqnqcgtl.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2ltkqyodj.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2dhmmepla.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2qsphfffr.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2yoqfdhst.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2gfoghzdm.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2oheghiac.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2idxudlrk.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2kzzeldyr.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2glqpiiqy.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2aflogplc.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2izsdkthw.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2itawwwby.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2qzjjebax.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2zbyczjdm.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2wcndbitg.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2tqphpoey.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2xmggxzfq.html


<!-- 参考信息 -->