代发 wailian999

[L03] 设置自定义请求头
来源：http://www.m.share.hesvh.cn/Article/details/gdjjzammn.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.zdbjq.cn/Article/details/godymqkkh.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.fehbvm.com/Article/details/ghgebouxr.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.hesvh.cn/Article/details/gpuktdqua.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.zdbjq.cn/Article/details/gaklaznrm.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.fehbvm.com/Article/details/gcasnbahy.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.hesvh.cn/Article/details/gsjuuatqw.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wap.hesvh.cn/Article/details/gfumnkhzn.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.m.share.zdbjq.cn/Article/details/gccpntllj.sHtML

[L04] 设置超时
来源：http://www.share.fehbvm.com/Article/details/gfeqvmjwb.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.hesvh.cn/Article/details/gndluufkf.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.zdbjq.cn/Article/details/glzdynecb.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.hesvh.cn/Article/details/ghqjqfmdk.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.fehbvm.com/Article/details/ghzyufvsp.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.zdbjq.cn/Article/details/gugfbcvlg.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.zdbjq.cn/Article/details/gwcaxcayg.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.fehbvm.com/Article/details/ghqzazxia.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.fehbvm.com/Article/details/gidtwuaco.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.hesvh.cn/Article/details/ghmvwfogy.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.zdbjq.cn/Article/details/gmeucvklw.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.hesvh.cn/Article/details/grojgagup.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.fehbvm.com/Article/details/gcnoiwfai.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.zdbjq.cn/Article/details/gcnyvcded.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.zdbjq.cn/Article/details/gkrdrtbbw.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.zdbjq.cn/Article/details/gpcmkexwr.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.fehbvm.com/Article/details/goohtlfqt.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gbcxsknuv.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.zdbjq.cn/Article/details/geytfrmoa.sHtML

Py:   resp.json()
来源：http://www.blog.fehbvm.com/Article/details/gedepjcga.sHtML

PHP:  json_decode($body, true);
来源：http://blog.fehbvm.com/Article/details/gjkdkqxhn.sHtML

JS:   await resp.json()
来源：http://www.blog.hesvh.cn/Article/details/gxxywpvds.sHtML

TS:   await resp.json()
来源：http://mobile.hesvh.cn/Article/details/gnqbknqyd.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.fehbvm.com/Article/details/gkrqgcmnx.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.fehbvm.com/Article/details/gaimbgjxl.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.zdbjq.cn/Article/details/gxvupllrj.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.fehbvm.com/Article/details/glyqezxdw.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.fehbvm.com/Article/details/gqhhoeqfp.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.zdbjq.cn/Article/details/gyzxcwogc.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.zdbjq.cn/Article/details/grmjuusic.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.hesvh.cn/Article/details/gurhxrbqv.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.hesvh.cn/Article/details/gvpamfwfi.sHtML

Java: resp.statusCode()
来源：http://read.share.hesvh.cn/Article/details/gzzedieuq.sHtML

Go:   resp.StatusCode
来源：http://3g.hesvh.cn/Article/details/gpfbwfsbb.sHtML

Ruby: resp.code.to_i
来源：http://www.share.hesvh.cn/Article/details/gsyrljfgg.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.zdbjq.cn/Article/details/gefoivxvz.sHtML

[L08] 并发请求多个地址
来源：http://mobile.zdbjq.cn/Article/details/gctcnazja.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.zdbjq.cn/Article/details/gnbvhgzlx.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.hesvh.cn/Article/details/gjbeifzfz.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.hesvh.cn/Article/details/gztctvkht.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fehbvm.com/Article/details/gvimyxvvc.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.zdbjq.cn/Article/details/gxbampkdf.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.fehbvm.com/Article/details/gicvtkivp.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.zdbjq.cn/Article/details/gsosjnhyu.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.fehbvm.com/Article/details/gkaxnjrgj.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gpeprthwz.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.fehbvm.com/Article/details/gvekuepom.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gqznafriw.sHtML

[M01] 读取命令行参数
来源：http://wap.hesvh.cn/Article/details/gjzoobntx.sHtML

Py:   sys.argv[1:]
来源：http://read.share.zdbjq.cn/Article/details/gkgvaocbc.sHtML

PHP:  $argv;  $argc;
来源：http://baike.fehbvm.com/Article/details/ghctruypb.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.hesvh.cn/Article/details/gmhniuhmu.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.fehbvm.com/Article/details/gzqcbhdwb.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.zdbjq.cn/Article/details/gzskgefhm.sHtML

Go:   os.Args[1:]
来源：http://m.share.zdbjq.cn/Article/details/gnuiqheuy.sHtML

Ruby: ARGV
来源：http://mobile.zdbjq.cn/Article/details/gugbmxido.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.fehbvm.com/Article/details/goeoptrix.sHtML

[M02] 读取环境变量
来源：http://read.share.fehbvm.com/Article/details/gwxgtdcwr.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.zdbjq.cn/Article/details/gjuxpcjkc.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.zdbjq.cn/Article/details/gfweuieja.sHtML

JS:   process.env.HOME
来源：http://mobile.fehbvm.com/Article/details/govcqemtn.sHtML

TS:   process.env.HOME
来源：http://wap.zdbjq.cn/Article/details/gzxrdwqrc.sHtML

Java: System.getenv("HOME")
来源：http://baike.hesvh.cn/Article/details/gpuusljxu.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.hesvh.cn/Article/details/gyxcdcjoq.sHtML

Ruby: ENV["HOME"]
来源：http://wap.fehbvm.com/Article/details/gxidaelqx.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.zdbjq.cn/Article/details/gzltqlsyy.sHtML

[M03] 执行外部命令
来源：http://www.share.zdbjq.cn/Article/details/gybdqjwen.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.zdbjq.cn/Article/details/gsbsgnlql.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.hesvh.cn/Article/details/gzledhecv.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.zdbjq.cn/Article/details/gsjstekzr.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.zdbjq.cn/Article/details/gxvqsfdbb.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.hesvh.cn/Article/details/gdrdvyrzv.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.hesvh.cn/Article/details/giilliute.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.zdbjq.cn/Article/details/gfovvhmsf.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.zdbjq.cn/Article/details/garoslzot.sHtML

[M04] 获取当前工作目录
来源：http://mobile.fehbvm.com/Article/details/gqnyivjor.sHtML

Py:   os.getcwd()
来源：http://www.blog.fehbvm.com/Article/details/gdwrjdjoi.sHtML

PHP:  getcwd();
来源：http://m.share.hesvh.cn/Article/details/gekyefmiv.sHtML

JS:   process.cwd()
来源：http://m.share.fehbvm.com/Article/details/grsrmdjuk.sHtML

TS:   process.cwd()
来源：http://baike.fehbvm.com/Article/details/gjpvyuxlj.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.zdbjq.cn/Article/details/gqcvmdoqa.sHtML

Go:   os.Getwd()
来源：http://wap.hesvh.cn/Article/details/gfwypbuue.sHtML

Ruby: Dir.pwd
来源：http://www.share.fehbvm.com/Article/details/gnspfpdhy.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.zdbjq.cn/Article/details/gkpfdeuyk.sHtML

[M05] 设置退出码
来源：http://mobile.fehbvm.com/Article/details/gtmvaklsk.sHtML

Py:   sys.exit(1)
来源：http://read.share.fehbvm.com/Article/details/goyhfrdgm.sHtML

PHP:  exit(1);
来源：http://3g.fehbvm.com/Article/details/gffgayhze.sHtML

JS:   process.exit(1)
来源：http://3g.hesvh.cn/Article/details/gkgbxcffe.sHtML

TS:   process.exit(1)
来源：http://wap.zdbjq.cn/Article/details/gvugiqiwk.sHtML

Java: System.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gcuatlkzb.sHtML

Go:   os.Exit(1)
来源：http://www.share.fehbvm.com/Article/details/gxkfwtzsl.sHtML

Ruby: exit 1
来源：http://www.m.share.fehbvm.com/Article/details/gkbgvfvjt.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.hesvh.cn/Article/details/gxlgaqhev.sHtML

[M06] 向标准错误输出
来源：http://www.blog.hesvh.cn/Article/details/gydtfuvqa.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.zdbjq.cn/Article/details/gguhdowsy.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.zdbjq.cn/Article/details/gcanrkwzh.sHtML

JS:   console.error("err")
来源：http://baike.zdbjq.cn/Article/details/gzaqhmfzs.sHtML

TS:   console.error("err")
来源：http://www.blog.fehbvm.com/Article/details/gvwsjayyk.sHtML

Java: System.err.println("err")
来源：http://www.blog.fehbvm.com/Article/details/ggjpwdyua.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.hesvh.cn/Article/details/gaofhfuar.sHtML

Ruby: warn "err"
来源：http://wap.hesvh.cn/Article/details/grgixhnvp.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.hesvh.cn/Article/details/gvklrqbkj.sHtML

[M07] 判断是否为主入口
来源：http://m.share.hesvh.cn/Article/details/gpomsxktn.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.fehbvm.com/Article/details/gnzrwoyat.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.hesvh.cn/Article/details/glwglhdxj.sHtML

JS:   require.main === module
来源：http://baike.zdbjq.cn/Article/details/gkxftswsj.sHtML

TS:   require.main === module
来源：http://m.share.hesvh.cn/Article/details/girhmxpxd.sHtML

Java: public static void main(String[] args)
来源：http://3g.zdbjq.cn/Article/details/gfbnqikrk.sHtML

Go:   func main()
来源：http://www.share.zdbjq.cn/Article/details/gmqueoeie.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.hesvh.cn/Article/details/gzfwiylxz.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.hesvh.cn/Article/details/gkhqpjvre.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.zdbjq.cn/Article/details/gklpcbems.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.fehbvm.com/Article/details/grwnilwww.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.hesvh.cn/Article/details/gimqwjbjy.sHtML

JS:   process.platform;  process.version
来源：http://mobile.hesvh.cn/Article/details/gyumwrjyg.sHtML

TS:   process.platform;  process.version
来源：http://blog.fehbvm.com/Article/details/gveszftzz.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.zdbjq.cn/Article/details/gjowlnczx.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.hesvh.cn/Article/details/gnbpqekwz.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.fehbvm.com/Article/details/gfgtgptmn.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.zdbjq.cn/Article/details/gzgrgfxbd.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gyrgszoky.sHtML

N. 数据结构与算法
来源：http://m.share.fehbvm.com/Article/details/gxyebsldx.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gysavgozt.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.zdbjq.cn/Article/details/ggywjnvhu.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gtygdsbcd.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.hesvh.cn/Article/details/gyopzcbit.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.hesvh.cn/Article/details/gjharnjpq.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.hesvh.cn/Article/details/gdjmlftkg.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gqlbmaute.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gndwdppfw.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.zdbjq.cn/Article/details/geqwhaufi.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gnencwtwx.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.zdbjq.cn/Article/details/gbafmaimo.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.zdbjq.cn/Article/details/gudipduxp.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.fehbvm.com/Article/details/grumgiayx.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.hesvh.cn/Article/details/glqnskgye.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.fehbvm.com/Article/details/gowprrgiv.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.zdbjq.cn/Article/details/gkliihcmc.sHtML

Go:   slices.Sort(arr)
来源：http://blog.hesvh.cn/Article/details/gpxswxbth.sHtML

Ruby: arr.sort
来源：http://baike.fehbvm.com/Article/details/gupsruirn.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.fehbvm.com/Article/details/gincvvvlj.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.zdbjq.cn/Article/details/gcwbueiqw.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.hesvh.cn/Article/details/gnnecgzqh.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.fehbvm.com/Article/details/gxhghefay.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.hesvh.cn/Article/details/gtwvsmdkg.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.fehbvm.com/Article/details/gsqiuqlhl.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.hesvh.cn/Article/details/gvffqziod.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.hesvh.cn/Article/details/gpaapmqoj.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.fehbvm.com/Article/details/gnhluzixz.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.hesvh.cn/Article/details/gzajeuwdw.sHtML

[N04] 斐波那契数列
来源：http://www.share.fehbvm.com/Article/details/goswsstff.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.zdbjq.cn/Article/details/gphucmdkn.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.fehbvm.com/Article/details/gfqwbxbji.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.fehbvm.com/Article/details/gfhypcpya.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.hesvh.cn/Article/details/gqgthdxsc.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.zdbjq.cn/Article/details/gdayofwmd.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.fehbvm.com/Article/details/graoipdgq.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.zdbjq.cn/Article/details/gkuoufeci.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gcpfjybqe.sHtML

[N05] 最大公约数
来源：http://wap.hesvh.cn/Article/details/goxdxungs.sHtML

Py:   math.gcd(a, b)
来源：http://blog.zdbjq.cn/Article/details/gvavbgnet.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.fehbvm.com/Article/details/gsprsbqwm.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.fehbvm.com/Article/details/gfnfbioay.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.zdbjq.cn/Article/details/gzgspzgvq.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.fehbvm.com/Article/details/gwjkcloaw.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.zdbjq.cn/Article/details/gxyyravrm.sHtML

Ruby: a.gcd(b)
来源：http://blog.hesvh.cn/Article/details/gfsjibskv.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.hesvh.cn/Article/details/gocyjnoen.sHtML

[N06] 判断回文字符串
来源：http://blog.hesvh.cn/Article/details/glxcocvja.sHtML

Py:   s == s[::-1]
来源：http://blog.hesvh.cn/Article/details/ggkldeyxk.sHtML

PHP:  $s === strrev($s);
来源：http://blog.fehbvm.com/Article/details/gxuzagzud.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/gzkuabowx.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/gormkvpph.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.hesvh.cn/Article/details/gozmavdlo.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.hesvh.cn/Article/details/gaxbyxvhs.sHtML

Ruby: s == s.reverse
来源：http://www.share.fehbvm.com/Article/details/gsogacdsl.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.zdbjq.cn/Article/details/gpqutlmde.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.zdbjq.cn/Article/details/getfjatdd.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.zdbjq.cn/Article/details/gtnipaqsa.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.fehbvm.com/Article/details/griscadch.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.zdbjq.cn/Article/details/gnyfupece.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.fehbvm.com/Article/details/grhmcibxg.sHtML

Java: // 手写 HashMap
来源：http://blog.hesvh.cn/Article/details/gghcftfgr.sHtML

Go:   // 手写 map[int]int
来源：http://3g.hesvh.cn/Article/details/ggvvjbyba.sHtML

Ruby: // 手写 Hash
来源：http://mobile.zdbjq.cn/Article/details/ghuxkwger.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.zdbjq.cn/Article/details/gfalorgmj.sHtML

[N08] 生成全排列
来源：http://baike.zdbjq.cn/Article/details/gkywoievr.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.hesvh.cn/Article/details/ghggkfeqk.sHtML

PHP:  // 手写递归交换
来源：http://m.share.zdbjq.cn/Article/details/gszgvzmdt.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gkjzkrkfh.sHtML

TS:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/ghoohkful.sHtML

Java: // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gcfjapani.sHtML

Go:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gtnfvfjgt.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.fehbvm.com/Article/details/gxrsmdtos.sHtML

C#:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/ghzovokmd.sHtML

[N09] 栈与队列
来源：http://baike.fehbvm.com/Article/details/glecathqv.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.hesvh.cn/Article/details/gffmcyohk.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.fehbvm.com/Article/details/gsfbrbuko.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.zdbjq.cn/Article/details/gbxngcone.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.fehbvm.com/Article/details/grdgwtuqt.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.hesvh.cn/Article/details/gddweerzd.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.zdbjq.cn/Article/details/guiwhhmco.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.hesvh.cn/Article/details/gufnfiwix.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.zdbjq.cn/Article/details/gdvjwbdph.sHtML

[N10] 链表节点定义
来源：http://read.share.fehbvm.com/Article/details/gypkkuhsv.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.zdbjq.cn/Article/details/ghebwhbjh.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.fehbvm.com/Article/details/gvgwqlodd.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.fehbvm.com/Article/details/gmebxadfh.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.fehbvm.com/Article/details/gxucbcgqy.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.hesvh.cn/Article/details/gsngqtlcf.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.zdbjq.cn/Article/details/gzwiykuqy.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.zdbjq.cn/Article/details/gsfpeekfk.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.hesvh.cn/Article/details/gfaohhzmg.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.hesvh.cn/Article/details/gplciliib.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.zdbjq.cn/Article/details/glvoqzgrq.sHtML

PHP:  // 手写递归函数
来源：http://mobile.fehbvm.com/Article/details/gsbgynevy.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.fehbvm.com/Article/details/gntllueaf.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.fehbvm.com/Article/details/gpwhhzobp.sHtML

Java: // 手写递归
来源：http://baike.hesvh.cn/Article/details/gbnboreds.sHtML

Go:   // 手写递归
来源：http://www.blog.fehbvm.com/Article/details/gbvvshzsr.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.zdbjq.cn/Article/details/gfnjxhliu.sHtML

C#:   // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/glsnzxmnw.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.hesvh.cn/Article/details/ghkbgsyjc.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.zdbjq.cn/Article/details/gjhpuujna.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.zdbjq.cn/Article/details/grpzzcbrc.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.hesvh.cn/Article/details/gsacewcip.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.fehbvm.com/Article/details/gdeyffrwi.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.fehbvm.com/Article/details/ggjnwahpe.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.fehbvm.com/Article/details/gorzhbejm.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.hesvh.cn/Article/details/goouckafx.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.fehbvm.com/Article/details/gcetqjgvd.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gfeokfypt.sHtML

O. 并发与异步
来源：http://mobile.hesvh.cn/Article/details/gdsrvpadh.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gocaxtsng.sHtML

[O01] 启动一个线程
来源：http://read.share.hesvh.cn/Article/details/gpybztzxg.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.fehbvm.com/Article/details/gumyvmkhy.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.hesvh.cn/Article/details/gspabfuer.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.hesvh.cn/Article/details/gnxdhegxi.sHtML

TS:   // 同 JS
来源：http://www.m.share.hesvh.cn/Article/details/geahhtpkj.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.zdbjq.cn/Article/details/gsdqcxied.sHtML

Go:   go f()
来源：http://mobile.fehbvm.com/Article/details/ggjbvijws.sHtML

Ruby: Thread.new { f }
来源：http://baike.zdbjq.cn/Article/details/gndxswyui.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.zdbjq.cn/Article/details/guuhyylko.sHtML

[O02] 使用线程池
来源：http://mobile.fehbvm.com/Article/details/gxvvdmgqy.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.fehbvm.com/Article/details/gsiuqjitj.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.fehbvm.com/Article/details/gecfrsaxn.sHtML

JS:   // worker_threads 线程池
来源：http://3g.zdbjq.cn/Article/details/gtetmjpfr.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.hesvh.cn/Article/details/geibrgnzu.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.fehbvm.com/Article/details/gebbcpnzn.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.hesvh.cn/Article/details/gfyzyzamh.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.zdbjq.cn/Article/details/gpskiwyqq.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.fehbvm.com/Article/details/gjmimgiow.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.zdbjq.cn/Article/details/gypucsszx.sHtML

Py:   with lock: shared += 1
来源：http://mobile.hesvh.cn/Article/details/gbvczsfvu.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.zdbjq.cn/Article/details/gatzbotes.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.hesvh.cn/Article/details/gpbnfbnjj.sHtML

TS:   // 同 JS
来源：http://m.share.fehbvm.com/Article/details/gerepelvo.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.fehbvm.com/Article/details/gjapvrqps.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.zdbjq.cn/Article/details/gqrnqxfhg.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.fehbvm.com/Article/details/gvsalbggd.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.fehbvm.com/Article/details/glrbdqqub.sHtML

[O04] 定义异步函数并等待
来源：http://wap.fehbvm.com/Article/details/gehuvtkpr.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.zdbjq.cn/Article/details/gifqnojcz.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.fehbvm.com/Article/details/gvdrvoaqx.sHtML

JS:   async function f() { await g(); }
来源：http://blog.fehbvm.com/Article/details/gvlwqzypw.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gqnzyvqti.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.zdbjq.cn/Article/details/gobakphss.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.hesvh.cn/Article/details/gdrnwckbt.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.fehbvm.com/Article/details/gqcszfwqz.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.zdbjq.cn/Article/details/gtirusuoh.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.fehbvm.com/Article/details/gnaupbsxv.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.hesvh.cn/Article/details/gvlfbpxrf.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.zdbjq.cn/Article/details/gxrnklkar.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.fehbvm.com/Article/details/gymvzjttw.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.hesvh.cn/Article/details/gyjnyxyfh.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.zdbjq.cn/Article/details/gnwdehciu.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.hesvh.cn/Article/details/gndyjtnci.sHtML

Ruby: threads.map(&:join)
来源：http://wap.fehbvm.com/Article/details/gupqxcqfl.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.fehbvm.com/Article/details/govfoipns.sHtML

[O06] 使用进程池
来源：http://www.share.zdbjq.cn/Article/details/ggrjleprw.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.hesvh.cn/Article/details/gwbfwyano.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.hesvh.cn/Article/details/glfmtebro.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.zdbjq.cn/Article/details/gtxjlqlei.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.hesvh.cn/Article/details/gbvgqnjrg.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.hesvh.cn/Article/details/gnxxaudar.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.zdbjq.cn/Article/details/gtwzicagh.sHtML

Ruby: // fork 块
来源：http://www.m.share.fehbvm.com/Article/details/gpcvtlwgd.sHtML

C#:   Parallel.For
来源：http://www.m.share.fehbvm.com/Article/details/gvrjmvzql.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gkpkxhfyq.sHtML

P. 常用工具函数
来源：http://www.blog.hesvh.cn/Article/details/gsptrtvkk.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/glynqwytm.sHtML


<!-- 参考信息 -->