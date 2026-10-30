代发 wailian999

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.fanxiaobao.xyz/Article/details/gtvxbkoto.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjujhlpuw.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyvlstmby.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.fanxiaobao.xyz/Article/details/gpmmjgits.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.fanxiaobao.xyz/Article/details/gcvdqnefx.sHtML

[L04] 设置超时
来源：http://3g.fanxiaobao.xyz/Article/details/gitwvzdwi.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.fanxiaobao.xyz/Article/details/ghkgbdasd.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gymtvpyui.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.fanxiaobao.xyz/Article/details/gsvfaxrde.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwszwpxsu.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.fanxiaobao.xyz/Article/details/gnykojcuv.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.fanxiaobao.xyz/Article/details/gtdrxrotm.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.fanxiaobao.xyz/Article/details/glbqtspal.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.fanxiaobao.xyz/Article/details/gbmyqthiv.sHtML

[L05] 上传文件（multipart）
来源：http://baike.fanxiaobao.xyz/Article/details/ggowlyasf.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.fanxiaobao.xyz/Article/details/gegmupjll.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gifjaxvnq.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqhbvrzsn.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.fanxiaobao.xyz/Article/details/gctgatowt.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.fanxiaobao.xyz/Article/details/gnxuvekxq.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gkygvenxw.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.fanxiaobao.xyz/Article/details/gknfwskox.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.fanxiaobao.xyz/Article/details/ggqntftiv.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.fanxiaobao.xyz/Article/details/gcabdgbgy.sHtML

Py:   resp.json()
来源：http://3g.fanxiaobao.xyz/Article/details/gbaqnnfaj.sHtML

PHP:  json_decode($body, true);
来源：http://blog.fanxiaobao.xyz/Article/details/gabqtgfyb.sHtML

JS:   await resp.json()
来源：http://m.share.fanxiaobao.xyz/Article/details/guqtgxarm.sHtML

TS:   await resp.json()
来源：http://read.share.fanxiaobao.xyz/Article/details/gcowpmyuy.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.fanxiaobao.xyz/Article/details/gzfwwhhjp.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpzajxbya.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.fanxiaobao.xyz/Article/details/gprezeeps.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.fanxiaobao.xyz/Article/details/giprtarqb.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfqnzrbua.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.fanxiaobao.xyz/Article/details/giygmjdsr.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxozjyzbj.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.fanxiaobao.xyz/Article/details/gzeneapvn.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.fanxiaobao.xyz/Article/details/gaxxufoxg.sHtML

Java: resp.statusCode()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqkerjfxj.sHtML

Go:   resp.StatusCode
来源：http://www.blog.fanxiaobao.xyz/Article/details/gllsdxmbn.sHtML

Ruby: resp.code.to_i
来源：http://wap.fanxiaobao.xyz/Article/details/gpciyijdr.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.fanxiaobao.xyz/Article/details/gplgthnqf.sHtML

[L08] 并发请求多个地址
来源：http://3g.fanxiaobao.xyz/Article/details/gkufzcclc.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.fanxiaobao.xyz/Article/details/gbjundkry.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.fanxiaobao.xyz/Article/details/gqrtnhqux.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fanxiaobao.xyz/Article/details/gedjfaiwl.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fanxiaobao.xyz/Article/details/grnfowmxh.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.fanxiaobao.xyz/Article/details/gvhtfdvjc.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.fanxiaobao.xyz/Article/details/gzjrqkyoq.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.fanxiaobao.xyz/Article/details/gbchjwqqm.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvcgrxcmg.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gznufeors.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfykysxsz.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwzlrpsjh.sHtML

[M01] 读取命令行参数
来源：http://blog.fanxiaobao.xyz/Article/details/gltqeavne.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmqczzajr.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.fanxiaobao.xyz/Article/details/gkqavwjqy.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvjwvqxdz.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grcxgiguz.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.fanxiaobao.xyz/Article/details/gizyhctxx.sHtML

Go:   os.Args[1:]
来源：http://www.share.fanxiaobao.xyz/Article/details/gtmaavwky.sHtML

Ruby: ARGV
来源：http://mobile.fanxiaobao.xyz/Article/details/gaholggop.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.fanxiaobao.xyz/Article/details/gjjakphdt.sHtML

[M02] 读取环境变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gamuggrnq.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.fanxiaobao.xyz/Article/details/gjoquiqwf.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.fanxiaobao.xyz/Article/details/gwrvdzcpw.sHtML

JS:   process.env.HOME
来源：http://www.share.fanxiaobao.xyz/Article/details/gretbfhwv.sHtML

TS:   process.env.HOME
来源：http://3g.fanxiaobao.xyz/Article/details/gtzglolbd.sHtML

Java: System.getenv("HOME")
来源：http://www.share.fanxiaobao.xyz/Article/details/gfaybyimy.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.fanxiaobao.xyz/Article/details/gxjadpscw.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gknpsqcdz.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.fanxiaobao.xyz/Article/details/gpehkufwu.sHtML

[M03] 执行外部命令
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfdnsumue.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtemifkno.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.fanxiaobao.xyz/Article/details/gnjvjvnbs.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjfqednwg.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.fanxiaobao.xyz/Article/details/gysqcivgj.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.fanxiaobao.xyz/Article/details/gdjxzrhko.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.fanxiaobao.xyz/Article/details/gllmzhkqc.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.fanxiaobao.xyz/Article/details/gqfkttgme.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.fanxiaobao.xyz/Article/details/gyecpfoua.sHtML

[M04] 获取当前工作目录
来源：http://baike.fanxiaobao.xyz/Article/details/gxqprbght.sHtML

Py:   os.getcwd()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvwmbblal.sHtML

PHP:  getcwd();
来源：http://baike.fanxiaobao.xyz/Article/details/gaegunqjw.sHtML

JS:   process.cwd()
来源：http://www.share.fanxiaobao.xyz/Article/details/gwdksnjzj.sHtML

TS:   process.cwd()
来源：http://mobile.fanxiaobao.xyz/Article/details/gsnkxlfkb.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.fanxiaobao.xyz/Article/details/ghgprtjrr.sHtML

Go:   os.Getwd()
来源：http://m.share.fanxiaobao.xyz/Article/details/gjdoerypn.sHtML

Ruby: Dir.pwd
来源：http://wap.fanxiaobao.xyz/Article/details/gxezoctng.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmnmddgwv.sHtML

[M05] 设置退出码
来源：http://blog.fanxiaobao.xyz/Article/details/gwjrutwov.sHtML

Py:   sys.exit(1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gllrfttfa.sHtML

PHP:  exit(1);
来源：http://3g.fanxiaobao.xyz/Article/details/gwserdgue.sHtML

JS:   process.exit(1)
来源：http://www.share.fanxiaobao.xyz/Article/details/ghprpqewn.sHtML

TS:   process.exit(1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gfqptujym.sHtML

Java: System.exit(1)
来源：http://baike.fanxiaobao.xyz/Article/details/grolgcxiz.sHtML

Go:   os.Exit(1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gjgdfxfif.sHtML

Ruby: exit 1
来源：http://m.share.fanxiaobao.xyz/Article/details/gkqasjumm.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghigheqft.sHtML

[M06] 向标准错误输出
来源：http://3g.fanxiaobao.xyz/Article/details/gnrfoeuff.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.fanxiaobao.xyz/Article/details/gvonqsals.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.fanxiaobao.xyz/Article/details/ggbyjyxab.sHtML

JS:   console.error("err")
来源：http://www.share.fanxiaobao.xyz/Article/details/gnpmjamto.sHtML

TS:   console.error("err")
来源：http://read.share.fanxiaobao.xyz/Article/details/gvxetoarr.sHtML

Java: System.err.println("err")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpvfbtece.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsvecylpg.sHtML

Ruby: warn "err"
来源：http://www.blog.fanxiaobao.xyz/Article/details/glvxtxpjy.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmbdconcs.sHtML

[M07] 判断是否为主入口
来源：http://www.share.fanxiaobao.xyz/Article/details/gbfgavjbn.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.fanxiaobao.xyz/Article/details/gnrbwjdoi.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkczdmhkf.sHtML

JS:   require.main === module
来源：http://3g.fanxiaobao.xyz/Article/details/gjdfknczo.sHtML

TS:   require.main === module
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goqzlbitw.sHtML

Java: public static void main(String[] args)
来源：http://read.share.fanxiaobao.xyz/Article/details/gcfbkpbts.sHtML

Go:   func main()
来源：http://blog.fanxiaobao.xyz/Article/details/gdasgojdl.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.fanxiaobao.xyz/Article/details/ghdwhaael.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxidzgsao.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.fanxiaobao.xyz/Article/details/gzuocqstu.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.fanxiaobao.xyz/Article/details/guhmlybpo.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gammoqlwb.sHtML

JS:   process.platform;  process.version
来源：http://wap.fanxiaobao.xyz/Article/details/gazggiabw.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gosjeazik.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.fanxiaobao.xyz/Article/details/glhfhagay.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.fanxiaobao.xyz/Article/details/grcyhpdrg.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.fanxiaobao.xyz/Article/details/gsohgzonx.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.fanxiaobao.xyz/Article/details/gktcgdbef.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gkpgazjqi.sHtML

N. 数据结构与算法
来源：http://blog.fanxiaobao.xyz/Article/details/gquejlqjc.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/grrrfvijj.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.fanxiaobao.xyz/Article/details/gcyihglrs.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.fanxiaobao.xyz/Article/details/gbyeqhemk.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.fanxiaobao.xyz/Article/details/gxgmwmjim.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.fanxiaobao.xyz/Article/details/gesshrgjs.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.fanxiaobao.xyz/Article/details/griqwtwhc.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxrjobpxf.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwsxuvclp.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.fanxiaobao.xyz/Article/details/geluareya.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmlyydbdw.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghyyfpbfz.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.fanxiaobao.xyz/Article/details/gbxvlksri.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.fanxiaobao.xyz/Article/details/gaypitgty.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.fanxiaobao.xyz/Article/details/gymcciwfx.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.fanxiaobao.xyz/Article/details/gewkxuayx.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.fanxiaobao.xyz/Article/details/gvlunqngh.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.fanxiaobao.xyz/Article/details/gqydrpxfc.sHtML

Ruby: arr.sort
来源：http://www.share.fanxiaobao.xyz/Article/details/gbtvxpfit.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.fanxiaobao.xyz/Article/details/gtktjpzkz.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.fanxiaobao.xyz/Article/details/gdcxhlfkt.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.fanxiaobao.xyz/Article/details/gdwiwucrk.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.fanxiaobao.xyz/Article/details/gspjrajaj.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gguhbpzfk.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.fanxiaobao.xyz/Article/details/gigvlfhnx.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.fanxiaobao.xyz/Article/details/gvdvcbihq.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.fanxiaobao.xyz/Article/details/gbkosjmrw.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzlxljcza.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.fanxiaobao.xyz/Article/details/gkogwezbw.sHtML

[N04] 斐波那契数列
来源：http://wap.fanxiaobao.xyz/Article/details/giifkutkb.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjvuzhzmb.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gsrbhxyrb.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.fanxiaobao.xyz/Article/details/gnxkvczwn.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.fanxiaobao.xyz/Article/details/ghgseybjd.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.fanxiaobao.xyz/Article/details/ggpmwhtxo.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gnlswqdsj.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gqlovmmdg.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.fanxiaobao.xyz/Article/details/gvlvzxazi.sHtML

[N05] 最大公约数
来源：http://www.share.fanxiaobao.xyz/Article/details/gjjflfpmd.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.fanxiaobao.xyz/Article/details/gitmvibym.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.fanxiaobao.xyz/Article/details/gakgpmbzb.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gzsynrttz.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.fanxiaobao.xyz/Article/details/grrwnjnqq.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gluhwyuob.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.fanxiaobao.xyz/Article/details/gqhewxrmr.sHtML

Ruby: a.gcd(b)
来源：http://mobile.fanxiaobao.xyz/Article/details/glellmziw.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzfpsqmki.sHtML

[N06] 判断回文字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gfpyloiws.sHtML

Py:   s == s[::-1]
来源：http://m.share.fanxiaobao.xyz/Article/details/gmesnpgul.sHtML

PHP:  $s === strrev($s);
来源：http://wap.fanxiaobao.xyz/Article/details/gqjabczup.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.fanxiaobao.xyz/Article/details/gkfgstwdh.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.fanxiaobao.xyz/Article/details/geaoddgbx.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.fanxiaobao.xyz/Article/details/gochszhlv.sHtML

Go:   // 双指针从两端比较
来源：http://baike.fanxiaobao.xyz/Article/details/ghbjpeiyf.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyurvettq.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.fanxiaobao.xyz/Article/details/gfdfdsius.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.fanxiaobao.xyz/Article/details/gqqikhqpt.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvrupksfo.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.fanxiaobao.xyz/Article/details/gpfvmqqml.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsxmgpoqq.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.fanxiaobao.xyz/Article/details/gonosewhu.sHtML

Java: // 手写 HashMap
来源：http://3g.fanxiaobao.xyz/Article/details/gmwwxmkar.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.fanxiaobao.xyz/Article/details/ggimwgnld.sHtML

Ruby: // 手写 Hash
来源：http://wap.fanxiaobao.xyz/Article/details/geualdnka.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.fanxiaobao.xyz/Article/details/gqlfzhjue.sHtML

[N08] 生成全排列
来源：http://baike.fanxiaobao.xyz/Article/details/gtzfvubxf.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.fanxiaobao.xyz/Article/details/gdmghlcre.sHtML

PHP:  // 手写递归交换
来源：http://blog.fanxiaobao.xyz/Article/details/gpoaxlurf.sHtML

JS:   // 手写回溯递归
来源：http://m.share.fanxiaobao.xyz/Article/details/gttyuqomy.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.fanxiaobao.xyz/Article/details/gufihkifq.sHtML

Java: // 手写回溯递归
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxxlpubvu.sHtML

Go:   // 手写回溯递归
来源：http://3g.fanxiaobao.xyz/Article/details/gvedetgol.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.fanxiaobao.xyz/Article/details/grcztngxm.sHtML

C#:   // 手写回溯递归
来源：http://baike.fanxiaobao.xyz/Article/details/gaehhmpui.sHtML

[N09] 栈与队列
来源：http://wap.fanxiaobao.xyz/Article/details/gkzzegahm.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.fanxiaobao.xyz/Article/details/gfpohfyoe.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.fanxiaobao.xyz/Article/details/ghszglpwo.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.fanxiaobao.xyz/Article/details/gnggcqaey.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.fanxiaobao.xyz/Article/details/gvlsfqrse.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.fanxiaobao.xyz/Article/details/goqfxtcnt.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.fanxiaobao.xyz/Article/details/gabguvkyj.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.fanxiaobao.xyz/Article/details/gdwvvrkxk.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.fanxiaobao.xyz/Article/details/grdvmtpht.sHtML

[N10] 链表节点定义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmnibggqh.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.fanxiaobao.xyz/Article/details/gtalxxsmb.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gfqxvhoim.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.fanxiaobao.xyz/Article/details/galbtpzbq.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.fanxiaobao.xyz/Article/details/gxzksdbgj.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.fanxiaobao.xyz/Article/details/gszvfvjhn.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.fanxiaobao.xyz/Article/details/gzhchaklz.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.fanxiaobao.xyz/Article/details/gluvlecbb.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gakgtzwwj.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gcieltsfx.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.fanxiaobao.xyz/Article/details/guovykhle.sHtML

PHP:  // 手写递归函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gjgvdjsqu.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.fanxiaobao.xyz/Article/details/gjojbpgzo.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.fanxiaobao.xyz/Article/details/geouqphca.sHtML

Java: // 手写递归
来源：http://baike.fanxiaobao.xyz/Article/details/grnexpcfu.sHtML

Go:   // 手写递归
来源：http://www.share.fanxiaobao.xyz/Article/details/glnhiadvq.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.fanxiaobao.xyz/Article/details/gkvbdmpau.sHtML

C#:   // 手写递归
来源：http://read.share.fanxiaobao.xyz/Article/details/gpgphqslg.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.fanxiaobao.xyz/Article/details/gmftbvsvz.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.fanxiaobao.xyz/Article/details/gojrluxui.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.fanxiaobao.xyz/Article/details/gdvzdgacj.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.fanxiaobao.xyz/Article/details/gzuippedm.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.fanxiaobao.xyz/Article/details/gewdubrty.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.fanxiaobao.xyz/Article/details/gagppaogh.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.fanxiaobao.xyz/Article/details/gnicfgkbj.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.fanxiaobao.xyz/Article/details/gtrlheogc.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.fanxiaobao.xyz/Article/details/gztdxekzz.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/glhibeffd.sHtML

O. 并发与异步
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnmrkdddo.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gxbgxacrg.sHtML

[O01] 启动一个线程
来源：http://www.blog.fanxiaobao.xyz/Article/details/goxeiotmm.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.fanxiaobao.xyz/Article/details/gwjtxklza.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.fanxiaobao.xyz/Article/details/gillmeklx.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.fanxiaobao.xyz/Article/details/gwxfhyibm.sHtML

TS:   // 同 JS
来源：http://read.share.fanxiaobao.xyz/Article/details/gwxfwwqym.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.fanxiaobao.xyz/Article/details/gzfpmjkur.sHtML

Go:   go f()
来源：http://www.share.fanxiaobao.xyz/Article/details/ghgjslycw.sHtML

Ruby: Thread.new { f }
来源：http://baike.fanxiaobao.xyz/Article/details/gwjmmazrc.sHtML

C#:   Task.Run(() => F());
来源：http://blog.fanxiaobao.xyz/Article/details/gjpxghflq.sHtML

[O02] 使用线程池
来源：http://blog.fanxiaobao.xyz/Article/details/gszdhblqc.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.fanxiaobao.xyz/Article/details/gohcpchel.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.fanxiaobao.xyz/Article/details/glwiecfum.sHtML

JS:   // worker_threads 线程池
来源：http://baike.fanxiaobao.xyz/Article/details/grklfeyuo.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.fanxiaobao.xyz/Article/details/gvapzdfav.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.fanxiaobao.xyz/Article/details/gnhnmqnhn.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.fanxiaobao.xyz/Article/details/gtqycqblf.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.fanxiaobao.xyz/Article/details/gdwaeggit.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.fanxiaobao.xyz/Article/details/gfbtdsvkh.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.fanxiaobao.xyz/Article/details/gsdvfdzgs.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyhuqclyz.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkiejnvnw.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.fanxiaobao.xyz/Article/details/glxlklwgz.sHtML

TS:   // 同 JS
来源：http://3g.fanxiaobao.xyz/Article/details/gmmlokban.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gimpkpyzj.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.fanxiaobao.xyz/Article/details/gatehcequ.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.fanxiaobao.xyz/Article/details/guiyiuiov.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.fanxiaobao.xyz/Article/details/gdpfghsgv.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.fanxiaobao.xyz/Article/details/genzbykcq.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.fanxiaobao.xyz/Article/details/gtjasswtu.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghrchzlqo.sHtML

JS:   async function f() { await g(); }
来源：http://blog.fanxiaobao.xyz/Article/details/geucufked.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gqkyybhoj.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.fanxiaobao.xyz/Article/details/gikzihoaq.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.fanxiaobao.xyz/Article/details/gvugfpuii.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.fanxiaobao.xyz/Article/details/gwmdfkyio.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gszvxebdy.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxarumylk.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdiqrzmda.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.fanxiaobao.xyz/Article/details/gcypmyagj.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.fanxiaobao.xyz/Article/details/geldrogmb.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.fanxiaobao.xyz/Article/details/gvcyywomn.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.fanxiaobao.xyz/Article/details/gmqsqiupo.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjoznbjne.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.fanxiaobao.xyz/Article/details/gzkxwggoj.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gwyeusshb.sHtML

[O06] 使用进程池
来源：http://blog.fanxiaobao.xyz/Article/details/gndugspca.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.fanxiaobao.xyz/Article/details/gjtnpvfay.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.fanxiaobao.xyz/Article/details/gaodewvzr.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.fanxiaobao.xyz/Article/details/gsqiwcynz.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.fanxiaobao.xyz/Article/details/gishzaclu.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.fanxiaobao.xyz/Article/details/gghczenzv.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.fanxiaobao.xyz/Article/details/gmignlyrw.sHtML

Ruby: // fork 块
来源：http://read.share.fanxiaobao.xyz/Article/details/gngzhzymr.sHtML

C#:   Parallel.For
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvlixpxbr.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gkgqlgxws.sHtML

P. 常用工具函数
来源：http://m.share.fanxiaobao.xyz/Article/details/guerbaxgk.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwmbqsekj.sHtML

[P01] 生成 UUID
来源：http://wap.fanxiaobao.xyz/Article/details/gqfwybntd.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.fanxiaobao.xyz/Article/details/gbuxiwvnt.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.fanxiaobao.xyz/Article/details/gdbkpeqyj.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.fanxiaobao.xyz/Article/details/gcsoxfosb.sHtML


<!-- 参考信息 -->