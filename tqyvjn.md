代发 wailian999

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2hiijoifg.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2zbouaajf.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2fbhatcqu.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2jzcoljdi.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2gzfqeldy.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2unrlsytn.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2zyfypfxi.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2ugovjhor.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2wjhycgfz.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2mefnikeo.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2onykmepv.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2cyvhuels.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2wafxlkkl.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2rinfttne.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2xzuitafg.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2xuvuaige.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2nwsoekev.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2wvfnwggs.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2gniraios.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2yzulddjl.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2rqmmkszo.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2ooayjnxs.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2nsfdxeux.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2bhriuewt.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2imxobkwv.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2weclkron.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2jvfmihzg.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2cusngtmb.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2iiryhsrg.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2vqdqkvev.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2wnkxlmtx.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2xzzvvvep.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2wgwucmkn.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2lzgwhjvo.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2cndjgcyv.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2nnqtxhls.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2olfawpbe.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2czpjdixy.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2atwylsox.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2ygpxfqvh.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2vfeopkrd.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2vdbwaljy.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2zelfitvk.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2sefrrbsu.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2rbkxqnuc.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2rfpygqty.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2jyazvozp.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2ycirrrca.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2fujvqqlj.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2bunyzggl.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2ughdeape.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2awegjcld.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2lgxqlkwm.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2yxcsptoy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qehrqnzr.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2vyxajpxh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zvkwrbma.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2jrzcqfpi.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2avrnqzyd.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2pwhcyhxw.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2uryothvy.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2ybipnlcu.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2ksjwiruy.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2havqxtxs.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2usolpmhx.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2ifnhblna.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2izqjpiuy.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2rnutaqna.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2lzloknei.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2arctotke.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2urerwgkf.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ssxdmazr.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2ofyiycjp.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2rysmzefv.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2heziyqdi.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2hggtpkvr.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2xwsnxuxk.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2crapennb.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2sxhaqjcc.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2dxetouim.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2ueqrpjod.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2dpsedvpi.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2ztojltlq.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2ojajtwlj.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2lvlhxbqv.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ehxvhnpy.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2bodwlrtu.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2pgkurubt.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ssdvaewl.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2awnksdhy.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2jfyaxlus.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2vyfnywpm.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2jdmkcrbv.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2cmifvsdz.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zigfwfpu.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2ixjdhtsq.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2tveelizd.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qehmyniy.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2fspfcqkm.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2htdoolbg.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2icaxgvoh.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2rkcjlvnh.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2khxpqznv.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2fbgeevpx.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2wblegfil.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2jrwbolmt.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2crmqybcy.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2hllaouhl.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2tegvwpve.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2vrmcacsu.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2vneciiba.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2ppmpmkat.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2dduqqswv.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2zztpiljz.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2quyexocv.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2kaudvlqd.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2godftyrt.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2cndgdqcg.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2sgrvghtw.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2qothxvys.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2edtcbqpr.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2hkgprrhg.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2gumjrwlr.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2oqdniidx.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2lspnqyif.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2hoilzacp.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2sykewruc.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2fzxptyzf.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2ghaorbvh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tchdxcll.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2qfkwmvgd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tllromji.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2amanhkgv.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2hlpgglfv.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2utgjtnar.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2kwplmscp.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2juxuwbqu.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ldzbdddr.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2kklzwukh.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2xlaezwvk.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2snxoxlsy.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2xwvnrpmb.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2fgsnzwip.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2nfvuxnzl.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2zofjyfyz.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2wlxxizch.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2stymgvms.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2khvbxipb.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2tvptwidg.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2lkdmmhtd.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2rxghqaht.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2ricmdoii.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2fizrlbaq.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2dsqgvunk.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2ohjqmsvv.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2bputuhwc.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2wskxwswu.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2tzsgtkpk.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2xgmnlmpw.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2vvxxwlis.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2innfgjnn.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2nbmxspwl.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2wzubzzec.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2vjyuctzl.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2ojurvhhr.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2gsbyskkq.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2bgwlgjxh.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2mhndsdiu.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2bkbgndgd.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2pcoxwmyf.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2chvryefp.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2menqizee.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2eqwgaoga.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2vcrlrdrb.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2ndcymxfm.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2taoocmad.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2xhxmyfbr.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2bbwhxeau.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2zokhdjqp.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2fgsrrwde.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2jgmztdfp.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2rxgqfzkn.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2tptrcyhw.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2usjspxnd.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2jpsaxpsn.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2ofeetbvd.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2zoardvzt.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2eypytosn.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2tdgtdbcb.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2tzoiwgcj.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2gvfmveoq.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2kvzmpnii.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2nrdfsqox.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2qrckwbsd.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2gtalxtmd.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2qigdpwkv.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2oxjsprtw.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2zhuieqfc.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2pavcttdg.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2gmiirefr.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2qrpkfgsh.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2hqobyagq.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2cnplljew.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2boazltak.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2dsswzdbq.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2lqiqaxrh.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2ipjnafdq.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2gdxtqiuf.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2kcpncaeu.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2dxxboosf.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2kzsfuyep.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2dilechvd.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2pcojxcpy.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2lpvxxovx.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2gmohvlqh.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2dnulgpny.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2xosoanpu.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2ytnwsuhx.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2bmrdskos.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2uovucosz.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2ixqpxdsi.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2enktwmvy.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2wgkgxzwq.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2ohlddrmi.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2pshozuem.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2qxbmkwbq.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2vadbvszp.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2aqlddwlj.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2ukciofbz.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2vqbcqtue.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2wgpjizmd.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2nojoqxpf.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2tgdillol.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2qzdbhahj.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2fxruclcv.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2xmvxzggc.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2pnuvsozj.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2spybfgvi.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2rtzirnnk.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2rabuqsix.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cmqvkfqn.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2ejsdqfax.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xdvjvtcj.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2jubxyrqy.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2dxjmfwmx.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2gcjbmccn.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2aqdqssff.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2jlpuvolm.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2wnslcydl.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2dczvcjmz.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2sfioipdx.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2anyzdgzh.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2fahrkpcu.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2bjvvrjxm.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2nmjnfpon.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2mlacxrvv.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2jkrqoywu.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2gimfankt.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2nitmbokk.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2nhmojgxh.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2sjeacser.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2czhqgymz.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2hxeeedzr.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2qvhzudeu.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2hvktxmne.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2bvsassgg.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ecjbahoa.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2eczhnlaw.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2syhrvxkc.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2gydjeadn.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2pfhhdakg.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2efkycnnh.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2ovybhmsx.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2yjrgjedw.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2tjjshwyb.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2oviogskl.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2wrskbbqx.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2veowkgyn.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2sjnwkxij.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2delhfdzi.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2pwazajay.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2swyktkda.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2ddbbsurd.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2rkoyboxt.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2jewqnlzp.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2nofkbknt.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2ozififeo.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2icgjbdlb.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2mslcgzwz.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2ibwqofoa.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2hebhzgwm.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2fuuixpmy.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2nmwtuolw.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2uoblelaf.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2gbvzjlht.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2mvalilay.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2zyphdlcg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mfboievg.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2cvleosez.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cuxppojm.html


<!-- 参考信息 -->