代发 wailian999

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.fehbvm.com/Article/details/gzwmyvbnj.sHtML

[L04] 设置超时
来源：http://www.blog.zdbjq.cn/Article/details/gztjryone.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.fehbvm.com/Article/details/glveippbs.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.zdbjq.cn/Article/details/gpwdtyahg.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.hesvh.cn/Article/details/gevawlvkz.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.zdbjq.cn/Article/details/gbpfqtlyv.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.hesvh.cn/Article/details/gdygwrndv.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.fehbvm.com/Article/details/gdgzavpkm.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.hesvh.cn/Article/details/gdwhkouya.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.zdbjq.cn/Article/details/gbhxfortk.sHtML

[L05] 上传文件（multipart）
来源：http://baike.zdbjq.cn/Article/details/gwmfekobn.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.hesvh.cn/Article/details/gzjipleig.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.hesvh.cn/Article/details/gczdcanad.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blog.fehbvm.com/Article/details/gcvbquyti.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.zdbjq.cn/Article/details/gesuteudv.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.zdbjq.cn/Article/details/geocytvcq.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.hesvh.cn/Article/details/glyusttrv.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.zdbjq.cn/Article/details/gybmeuluv.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gunpfwutx.sHtML

[L06] 解析响应为 JSON
来源：http://3g.hesvh.cn/Article/details/gbwnuaxsv.sHtML

Py:   resp.json()
来源：http://www.blog.fehbvm.com/Article/details/gexdhiguf.sHtML

PHP:  json_decode($body, true);
来源：http://3g.fehbvm.com/Article/details/gbhccdhht.sHtML

JS:   await resp.json()
来源：http://www.blog.fehbvm.com/Article/details/gzjjjcznr.sHtML

TS:   await resp.json()
来源：http://blog.hesvh.cn/Article/details/gyyljdrpb.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.zdbjq.cn/Article/details/gtackuqwx.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.zdbjq.cn/Article/details/guwabjeax.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.zdbjq.cn/Article/details/gpnbwtljz.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.zdbjq.cn/Article/details/gnicqdktk.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.zdbjq.cn/Article/details/gnpwgubzw.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.hesvh.cn/Article/details/gwfaiulha.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.hesvh.cn/Article/details/ghqixstpo.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.hesvh.cn/Article/details/gjjwxdnnz.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.zdbjq.cn/Article/details/gbxhybwga.sHtML

Java: resp.statusCode()
来源：http://wap.hesvh.cn/Article/details/ggqdofzex.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.zdbjq.cn/Article/details/gfdkzdywi.sHtML

Ruby: resp.code.to_i
来源：http://3g.fehbvm.com/Article/details/gdnkluvqq.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.zdbjq.cn/Article/details/ghzorvdbg.sHtML

[L08] 并发请求多个地址
来源：http://blog.fehbvm.com/Article/details/grnqqgrgo.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.zdbjq.cn/Article/details/gefhuievu.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.hesvh.cn/Article/details/gpdimjltt.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.zdbjq.cn/Article/details/gvwpwdhzj.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.zdbjq.cn/Article/details/gujszsrvl.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.zdbjq.cn/Article/details/gfxfdspai.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.zdbjq.cn/Article/details/gdhvpptxv.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.zdbjq.cn/Article/details/gyhoccehs.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.fehbvm.com/Article/details/guhdepcka.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gerpmggss.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.zdbjq.cn/Article/details/gjydmqdtk.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gwjeqvfwi.sHtML

[M01] 读取命令行参数
来源：http://m.share.hesvh.cn/Article/details/gfnuutlal.sHtML

Py:   sys.argv[1:]
来源：http://3g.hesvh.cn/Article/details/gphnboflv.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.zdbjq.cn/Article/details/gfqeblatt.sHtML

JS:   process.argv.slice(2)
来源：http://wap.zdbjq.cn/Article/details/gixlnmyxp.sHtML

TS:   process.argv.slice(2)
来源：http://3g.fehbvm.com/Article/details/gbomiidkf.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.hesvh.cn/Article/details/guccgwydq.sHtML

Go:   os.Args[1:]
来源：http://www.blog.zdbjq.cn/Article/details/gajhnodgt.sHtML

Ruby: ARGV
来源：http://m.share.hesvh.cn/Article/details/gcbpmpxuq.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.fehbvm.com/Article/details/gelaujmjq.sHtML

[M02] 读取环境变量
来源：http://www.m.share.zdbjq.cn/Article/details/gbcuohjkh.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.fehbvm.com/Article/details/gyiixkdvo.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.fehbvm.com/Article/details/gontbweex.sHtML

JS:   process.env.HOME
来源：http://3g.zdbjq.cn/Article/details/gkucirgnh.sHtML

TS:   process.env.HOME
来源：http://baike.zdbjq.cn/Article/details/grtyjbhus.sHtML

Java: System.getenv("HOME")
来源：http://read.share.zdbjq.cn/Article/details/genhxltaf.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.zdbjq.cn/Article/details/gpfcjgyaa.sHtML

Ruby: ENV["HOME"]
来源：http://baike.fehbvm.com/Article/details/grkeazhtq.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.zdbjq.cn/Article/details/gzsngtuwt.sHtML

[M03] 执行外部命令
来源：http://www.m.share.fehbvm.com/Article/details/gutxaqavs.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.zdbjq.cn/Article/details/gaxotyikb.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.hesvh.cn/Article/details/gjiccpncc.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.fehbvm.com/Article/details/gebvmtecd.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.fehbvm.com/Article/details/gawyuwxhm.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.zdbjq.cn/Article/details/gviwdqyma.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.zdbjq.cn/Article/details/gmebbzwpm.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.hesvh.cn/Article/details/gbkjyktwh.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.fehbvm.com/Article/details/grqaznawf.sHtML

[M04] 获取当前工作目录
来源：http://mobile.hesvh.cn/Article/details/grsjcebnv.sHtML

Py:   os.getcwd()
来源：http://www.blog.zdbjq.cn/Article/details/gvbqzadov.sHtML

PHP:  getcwd();
来源：http://baike.hesvh.cn/Article/details/gptgwmxzz.sHtML

JS:   process.cwd()
来源：http://m.share.fehbvm.com/Article/details/geudtbuno.sHtML

TS:   process.cwd()
来源：http://mobile.fehbvm.com/Article/details/gvyoguysx.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.zdbjq.cn/Article/details/goytstjps.sHtML

Go:   os.Getwd()
来源：http://read.share.fehbvm.com/Article/details/gbhbjeexo.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.fehbvm.com/Article/details/gtrkmlmex.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.fehbvm.com/Article/details/gqgqvzuof.sHtML

[M05] 设置退出码
来源：http://wap.zdbjq.cn/Article/details/gnzlkyvqd.sHtML

Py:   sys.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gnwnlhszn.sHtML

PHP:  exit(1);
来源：http://www.share.zdbjq.cn/Article/details/gihfpotib.sHtML

JS:   process.exit(1)
来源：http://baike.fehbvm.com/Article/details/gzskeaihe.sHtML

TS:   process.exit(1)
来源：http://3g.hesvh.cn/Article/details/ghtspoujk.sHtML

Java: System.exit(1)
来源：http://www.share.fehbvm.com/Article/details/gpxwcjmsy.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/guaxiyyke.sHtML

Ruby: exit 1
来源：http://blog.hesvh.cn/Article/details/gpqqdueyl.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.zdbjq.cn/Article/details/gxiicqhtk.sHtML

[M06] 向标准错误输出
来源：http://read.share.fehbvm.com/Article/details/gpeoostfk.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.zdbjq.cn/Article/details/ghyomgdit.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.hesvh.cn/Article/details/glvehbjsg.sHtML

JS:   console.error("err")
来源：http://www.blog.hesvh.cn/Article/details/gwwuuaqqb.sHtML

TS:   console.error("err")
来源：http://m.share.fehbvm.com/Article/details/gumveolci.sHtML

Java: System.err.println("err")
来源：http://wap.fehbvm.com/Article/details/ghewauuap.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.zdbjq.cn/Article/details/gscwtyttx.sHtML

Ruby: warn "err"
来源：http://mobile.fehbvm.com/Article/details/gobfzeumg.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.fehbvm.com/Article/details/gncdpvgny.sHtML

[M07] 判断是否为主入口
来源：http://blog.fehbvm.com/Article/details/grxpmancm.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.hesvh.cn/Article/details/gwbhurhby.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.hesvh.cn/Article/details/gghgizfvk.sHtML

JS:   require.main === module
来源：http://baike.fehbvm.com/Article/details/gretefitd.sHtML

TS:   require.main === module
来源：http://wap.fehbvm.com/Article/details/gjuxptbzr.sHtML

Java: public static void main(String[] args)
来源：http://baike.fehbvm.com/Article/details/gbvhwqmaz.sHtML

Go:   func main()
来源：http://mobile.fehbvm.com/Article/details/gkyptaypc.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.fehbvm.com/Article/details/gsqjanfew.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.fehbvm.com/Article/details/gfoyzwjxn.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.fehbvm.com/Article/details/gedjxsqwm.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.hesvh.cn/Article/details/guwypksew.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.hesvh.cn/Article/details/gjpneblqh.sHtML

JS:   process.platform;  process.version
来源：http://baike.fehbvm.com/Article/details/gwcnniyqs.sHtML

TS:   process.platform;  process.version
来源：http://read.share.fehbvm.com/Article/details/gruanqjpg.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.zdbjq.cn/Article/details/gjlrrtgfo.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.fehbvm.com/Article/details/guelurpjd.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.zdbjq.cn/Article/details/gqnjwepbh.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.fehbvm.com/Article/details/ghnrgwqbf.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gfadyomcu.sHtML

N. 数据结构与算法
来源：http://baike.hesvh.cn/Article/details/gjiiiezgn.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gaivcdfns.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.fehbvm.com/Article/details/gjoqzopyb.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.hesvh.cn/Article/details/gmyilmzww.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.zdbjq.cn/Article/details/gqjrgnbdl.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.fehbvm.com/Article/details/greqnnbqu.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.zdbjq.cn/Article/details/gkpzajxod.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gyjrepdwf.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/goiourhwl.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.hesvh.cn/Article/details/gtqvbfwmn.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.hesvh.cn/Article/details/geabpuuyg.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.hesvh.cn/Article/details/gcrlbuvez.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.fehbvm.com/Article/details/gpmyrryik.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.fehbvm.com/Article/details/gdbefaanl.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.hesvh.cn/Article/details/gajnvyruc.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.hesvh.cn/Article/details/gaeyrtsep.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.fehbvm.com/Article/details/guxywmver.sHtML

Go:   slices.Sort(arr)
来源：http://blog.fehbvm.com/Article/details/gjzmtopyf.sHtML

Ruby: arr.sort
来源：http://3g.hesvh.cn/Article/details/gqlmpocae.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.hesvh.cn/Article/details/gzpwufwgt.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.zdbjq.cn/Article/details/gqdqmehcz.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.hesvh.cn/Article/details/gxmmzccza.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.fehbvm.com/Article/details/gdrdbbkwr.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.hesvh.cn/Article/details/gfgbzzage.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.hesvh.cn/Article/details/gjscqpvgo.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.zdbjq.cn/Article/details/gphooseup.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.fehbvm.com/Article/details/glvfotxsz.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.zdbjq.cn/Article/details/gmnwazobg.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.hesvh.cn/Article/details/gphptfhra.sHtML

[N04] 斐波那契数列
来源：http://3g.zdbjq.cn/Article/details/gheahidbd.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.zdbjq.cn/Article/details/gzgvgrpra.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.fehbvm.com/Article/details/glxnebpmf.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.zdbjq.cn/Article/details/gmdugdetm.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/gqtewlbpt.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.hesvh.cn/Article/details/govpolxyy.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.hesvh.cn/Article/details/ginnctgzx.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.hesvh.cn/Article/details/gxmobyjck.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.zdbjq.cn/Article/details/gdddwrzvn.sHtML

[N05] 最大公约数
来源：http://mobile.fehbvm.com/Article/details/gsbmvrjia.sHtML

Py:   math.gcd(a, b)
来源：http://3g.hesvh.cn/Article/details/gfgkgizvi.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.fehbvm.com/Article/details/gqvldvmmc.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.zdbjq.cn/Article/details/gufjgmlkt.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.zdbjq.cn/Article/details/gvyjgscya.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.zdbjq.cn/Article/details/ggvygpixy.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.hesvh.cn/Article/details/gtkyqwcyy.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.hesvh.cn/Article/details/gqglfhxoc.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.fehbvm.com/Article/details/guomcncld.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.fehbvm.com/Article/details/gljcztqaq.sHtML

Py:   s == s[::-1]
来源：http://www.blog.zdbjq.cn/Article/details/ghvlhbhze.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.hesvh.cn/Article/details/ghphlcdgj.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/gdkjtjpcf.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/gkmmnoptt.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.fehbvm.com/Article/details/giousnyia.sHtML

Go:   // 双指针从两端比较
来源：http://baike.fehbvm.com/Article/details/gvbzjjkil.sHtML

Ruby: s == s.reverse
来源：http://www.share.fehbvm.com/Article/details/gojncyovm.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.zdbjq.cn/Article/details/geivcbbrf.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.zdbjq.cn/Article/details/gilnetaux.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.hesvh.cn/Article/details/gszvwrtpy.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.hesvh.cn/Article/details/gnfwpfskn.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.zdbjq.cn/Article/details/gqisqdbdj.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.zdbjq.cn/Article/details/grfeednej.sHtML

Java: // 手写 HashMap
来源：http://mobile.zdbjq.cn/Article/details/gaypzeelc.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.hesvh.cn/Article/details/gyzhfcgoz.sHtML

Ruby: // 手写 Hash
来源：http://m.share.hesvh.cn/Article/details/glddxntul.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.fehbvm.com/Article/details/ggwnmgnjf.sHtML

[N08] 生成全排列
来源：http://3g.fehbvm.com/Article/details/guyqltxsh.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.fehbvm.com/Article/details/gageofjai.sHtML

PHP:  // 手写递归交换
来源：http://blog.zdbjq.cn/Article/details/gypeappfw.sHtML

JS:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gaxjxosst.sHtML

TS:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gipkmapso.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gqyxxdheq.sHtML

Go:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gunsuvait.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.zdbjq.cn/Article/details/gpdzxwjvy.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gnjlegiuc.sHtML

[N09] 栈与队列
来源：http://mobile.fehbvm.com/Article/details/guwzjtvha.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.fehbvm.com/Article/details/gijlwmepu.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.hesvh.cn/Article/details/glfevfrad.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.zdbjq.cn/Article/details/gundvfqxz.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.hesvh.cn/Article/details/gpirxwhqo.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.zdbjq.cn/Article/details/grwoohqmk.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.zdbjq.cn/Article/details/gsigwsrek.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.fehbvm.com/Article/details/gdwuqixdv.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.fehbvm.com/Article/details/grqooipsw.sHtML

[N10] 链表节点定义
来源：http://mobile.hesvh.cn/Article/details/ghptbccft.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.fehbvm.com/Article/details/ghezvglmv.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.fehbvm.com/Article/details/godhnaybd.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.zdbjq.cn/Article/details/gjrlpjzto.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.hesvh.cn/Article/details/gqthoydax.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.hesvh.cn/Article/details/gwndddcen.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.fehbvm.com/Article/details/gckpvcant.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.zdbjq.cn/Article/details/gvpkvvqxg.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.hesvh.cn/Article/details/gebhylqmw.sHtML

[N11] 二叉树中序遍历
来源：http://wap.hesvh.cn/Article/details/gbzepxbfu.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.hesvh.cn/Article/details/guvvjimyu.sHtML

PHP:  // 手写递归函数
来源：http://mobile.zdbjq.cn/Article/details/gigaiwgpu.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.hesvh.cn/Article/details/gmthlswfv.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.zdbjq.cn/Article/details/gbzbjbmkz.sHtML

Java: // 手写递归
来源：http://www.share.hesvh.cn/Article/details/gpknvaiyx.sHtML

Go:   // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/gskmqpezl.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.fehbvm.com/Article/details/gacsnylve.sHtML

C#:   // 手写递归
来源：http://3g.zdbjq.cn/Article/details/gseyoevwv.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.zdbjq.cn/Article/details/giypbzybx.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.fehbvm.com/Article/details/gbvojqyob.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.zdbjq.cn/Article/details/gcqcldqms.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.fehbvm.com/Article/details/gibjmacgx.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.hesvh.cn/Article/details/ggvngqoun.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.fehbvm.com/Article/details/gxpxdmxsp.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.zdbjq.cn/Article/details/gzmmddgqz.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.hesvh.cn/Article/details/gusrzorsu.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.hesvh.cn/Article/details/gdelamntu.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gnbgabvzo.sHtML

O. 并发与异步
来源：http://mobile.hesvh.cn/Article/details/gxynkbpga.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gwaspagrg.sHtML

[O01] 启动一个线程
来源：http://read.share.zdbjq.cn/Article/details/gtyqfnpgs.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.fehbvm.com/Article/details/gtmzsdkum.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.fehbvm.com/Article/details/gfbqjishd.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.zdbjq.cn/Article/details/gcjzbwzbc.sHtML

TS:   // 同 JS
来源：http://3g.hesvh.cn/Article/details/grmsbuejs.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.hesvh.cn/Article/details/gkprlzqve.sHtML

Go:   go f()
来源：http://mobile.zdbjq.cn/Article/details/gsdphgwaz.sHtML

Ruby: Thread.new { f }
来源：http://m.share.fehbvm.com/Article/details/gywmttzfz.sHtML

C#:   Task.Run(() => F());
来源：http://baike.hesvh.cn/Article/details/gfepzsxqp.sHtML

[O02] 使用线程池
来源：http://mobile.zdbjq.cn/Article/details/ghaqzaueg.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.zdbjq.cn/Article/details/gcnxtbejp.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.hesvh.cn/Article/details/grcfdxish.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.hesvh.cn/Article/details/ginsrupyt.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.hesvh.cn/Article/details/grizmgppy.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.hesvh.cn/Article/details/gaedabbbs.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.zdbjq.cn/Article/details/gengqnudb.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.zdbjq.cn/Article/details/gqsmkbpwm.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.zdbjq.cn/Article/details/gyiykvnfy.sHtML

[O03] 加锁保护共享数据
来源：http://3g.fehbvm.com/Article/details/goenyowyc.sHtML

Py:   with lock: shared += 1
来源：http://mobile.hesvh.cn/Article/details/goumwemby.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.fehbvm.com/Article/details/gueslnirc.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.hesvh.cn/Article/details/grqutxfnk.sHtML

TS:   // 同 JS
来源：http://3g.zdbjq.cn/Article/details/grskavnqa.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.hesvh.cn/Article/details/gajqsxplw.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.hesvh.cn/Article/details/gyvyjbnaw.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.hesvh.cn/Article/details/glqorhqrv.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.fehbvm.com/Article/details/ghbvjakql.sHtML

[O04] 定义异步函数并等待
来源：http://wap.fehbvm.com/Article/details/ghccfktcv.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.hesvh.cn/Article/details/gzlubgbkb.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.fehbvm.com/Article/details/gujflucet.sHtML

JS:   async function f() { await g(); }
来源：http://3g.zdbjq.cn/Article/details/ggcnnwgkg.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.fehbvm.com/Article/details/gcuwagkoj.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.fehbvm.com/Article/details/gnitubamt.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.zdbjq.cn/Article/details/glwjiyrtc.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.hesvh.cn/Article/details/gvhoblnqc.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.zdbjq.cn/Article/details/gjshidgbl.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.zdbjq.cn/Article/details/gkukgwvxs.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.fehbvm.com/Article/details/gxoytxjyn.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.fehbvm.com/Article/details/gzgtvbddl.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.hesvh.cn/Article/details/gtjzjnsuu.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.zdbjq.cn/Article/details/gihueeldo.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.fehbvm.com/Article/details/gmluejndx.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.zdbjq.cn/Article/details/gqvlnqxxl.sHtML

Ruby: threads.map(&:join)
来源：http://baike.hesvh.cn/Article/details/gmpeqchcz.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.zdbjq.cn/Article/details/ghajxhtri.sHtML

[O06] 使用进程池
来源：http://blog.fehbvm.com/Article/details/gursaorwb.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.fehbvm.com/Article/details/gmifeexkf.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.zdbjq.cn/Article/details/ggkdiwnto.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.hesvh.cn/Article/details/gulejbrmp.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.hesvh.cn/Article/details/gzbnnhiph.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.hesvh.cn/Article/details/ggbvvyifm.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.hesvh.cn/Article/details/gxtrwyirn.sHtML

Ruby: // fork 块
来源：http://www.blog.fehbvm.com/Article/details/gwdkwjtjw.sHtML

C#:   Parallel.For
来源：http://www.m.share.fehbvm.com/Article/details/gyowlwjbc.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gagxfongv.sHtML

P. 常用工具函数
来源：http://baike.fehbvm.com/Article/details/gfwbuhvde.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gcwvjfbtu.sHtML

[P01] 生成 UUID
来源：http://3g.fehbvm.com/Article/details/grkviwaem.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.zdbjq.cn/Article/details/gmcydhiha.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.zdbjq.cn/Article/details/gxfpvxweg.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.fehbvm.com/Article/details/gwwgkfyvd.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.fehbvm.com/Article/details/gzijcpgvv.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.fehbvm.com/Article/details/guhqvfaqf.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.hesvh.cn/Article/details/gramyywst.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.hesvh.cn/Article/details/gurhrjlnb.sHtML


<!-- 参考信息 -->