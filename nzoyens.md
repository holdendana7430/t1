代发 wailian999

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.zdbjq.cn/Article/details/gxvfmibui.sHtML

[L04] 设置超时
来源：http://mobile.hesvh.cn/Article/details/gdejszlhc.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.zdbjq.cn/Article/details/gcfzbdafs.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://read.share.fehbvm.com/Article/details/gxeiyydic.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.zdbjq.cn/Article/details/ggcuiuxnq.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.zdbjq.cn/Article/details/ggkwrkkei.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.hesvh.cn/Article/details/ghmvhiqrt.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.fehbvm.com/Article/details/gbxoovehy.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.zdbjq.cn/Article/details/glplaagzf.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.zdbjq.cn/Article/details/gdpgjjjqe.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.zdbjq.cn/Article/details/gknlssisg.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.hesvh.cn/Article/details/gkmdgzyux.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.hesvh.cn/Article/details/ganxzszdp.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.hesvh.cn/Article/details/gryndbuqd.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.hesvh.cn/Article/details/gtgywiebl.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.zdbjq.cn/Article/details/gpxeslups.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.fehbvm.com/Article/details/gfaxbbbbh.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.fehbvm.com/Article/details/gwgctnvoz.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gektvxmyw.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.fehbvm.com/Article/details/gyiilytkr.sHtML

Py:   resp.json()
来源：http://read.share.fehbvm.com/Article/details/gglfawaye.sHtML

PHP:  json_decode($body, true);
来源：http://3g.zdbjq.cn/Article/details/gxucknajs.sHtML

JS:   await resp.json()
来源：http://3g.zdbjq.cn/Article/details/gddhyvept.sHtML

TS:   await resp.json()
来源：http://baike.fehbvm.com/Article/details/gsnofqwzw.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.hesvh.cn/Article/details/gzrufuyaw.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.hesvh.cn/Article/details/gmguaxadn.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.fehbvm.com/Article/details/gkmujyovf.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.hesvh.cn/Article/details/gquqdfthg.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.fehbvm.com/Article/details/grsecwwwu.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.fehbvm.com/Article/details/gdlpmvwjn.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.hesvh.cn/Article/details/gjtfoyiyq.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.zdbjq.cn/Article/details/gqkwmojig.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.zdbjq.cn/Article/details/glhajasyz.sHtML

Java: resp.statusCode()
来源：http://read.share.fehbvm.com/Article/details/gigekrluw.sHtML

Go:   resp.StatusCode
来源：http://www.blog.hesvh.cn/Article/details/gdavpofvi.sHtML

Ruby: resp.code.to_i
来源：http://baike.zdbjq.cn/Article/details/gmihmjjvw.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.fehbvm.com/Article/details/guvcnzudf.sHtML

[L08] 并发请求多个地址
来源：http://3g.zdbjq.cn/Article/details/gjiuadhdn.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.hesvh.cn/Article/details/gfdyyajln.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.zdbjq.cn/Article/details/gwauwnaqk.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fehbvm.com/Article/details/gsdnudquu.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.zdbjq.cn/Article/details/gcleavbln.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.zdbjq.cn/Article/details/gljnajjxb.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.zdbjq.cn/Article/details/gkinhpiqi.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.fehbvm.com/Article/details/gvdrofrbj.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.hesvh.cn/Article/details/gvwapoiml.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gmjismuav.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.zdbjq.cn/Article/details/gmfmknuza.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gbkjygosn.sHtML

[M01] 读取命令行参数
来源：http://3g.fehbvm.com/Article/details/gxoefzunb.sHtML

Py:   sys.argv[1:]
来源：http://baike.hesvh.cn/Article/details/gckuxmwcp.sHtML

PHP:  $argv;  $argc;
来源：http://blog.hesvh.cn/Article/details/gefychnnf.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.zdbjq.cn/Article/details/gxarmeido.sHtML

TS:   process.argv.slice(2)
来源：http://wap.fehbvm.com/Article/details/gqkzkqedo.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.hesvh.cn/Article/details/gzwsfyzmc.sHtML

Go:   os.Args[1:]
来源：http://baike.hesvh.cn/Article/details/gyzbmkndj.sHtML

Ruby: ARGV
来源：http://read.share.hesvh.cn/Article/details/gyrdjriwi.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.hesvh.cn/Article/details/gvvoquqvk.sHtML

[M02] 读取环境变量
来源：http://mobile.zdbjq.cn/Article/details/gzxjqpjta.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.zdbjq.cn/Article/details/glenkhdev.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.fehbvm.com/Article/details/gsyqwyclr.sHtML

JS:   process.env.HOME
来源：http://m.share.zdbjq.cn/Article/details/gyaqgiepn.sHtML

TS:   process.env.HOME
来源：http://read.share.fehbvm.com/Article/details/gojqufjup.sHtML

Java: System.getenv("HOME")
来源：http://www.share.hesvh.cn/Article/details/gusntttpt.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.hesvh.cn/Article/details/gxqhyiznx.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.fehbvm.com/Article/details/guvwuvcex.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.fehbvm.com/Article/details/gsdtolekd.sHtML

[M03] 执行外部命令
来源：http://mobile.zdbjq.cn/Article/details/gerenrsdm.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.zdbjq.cn/Article/details/guvglmzfk.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.zdbjq.cn/Article/details/gbmvcuptp.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.fehbvm.com/Article/details/gddtgreaw.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.zdbjq.cn/Article/details/giydavwah.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.zdbjq.cn/Article/details/gpgnxlyhr.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.zdbjq.cn/Article/details/gxfwojrid.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.fehbvm.com/Article/details/ghqpttdmw.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.hesvh.cn/Article/details/gizwvqqsn.sHtML

[M04] 获取当前工作目录
来源：http://read.share.zdbjq.cn/Article/details/glcunfxql.sHtML

Py:   os.getcwd()
来源：http://www.share.zdbjq.cn/Article/details/gpzzdaflw.sHtML

PHP:  getcwd();
来源：http://www.blog.zdbjq.cn/Article/details/gpqdguwje.sHtML

JS:   process.cwd()
来源：http://blog.fehbvm.com/Article/details/gbakmnunn.sHtML

TS:   process.cwd()
来源：http://mobile.fehbvm.com/Article/details/gyldxjqtj.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.fehbvm.com/Article/details/gdldiyuxy.sHtML

Go:   os.Getwd()
来源：http://www.blog.zdbjq.cn/Article/details/gdnhxzeox.sHtML

Ruby: Dir.pwd
来源：http://mobile.fehbvm.com/Article/details/gpjlxntvy.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.hesvh.cn/Article/details/gjaoubrrq.sHtML

[M05] 设置退出码
来源：http://baike.fehbvm.com/Article/details/gqupnwzrm.sHtML

Py:   sys.exit(1)
来源：http://m.share.fehbvm.com/Article/details/gupiiryfr.sHtML

PHP:  exit(1);
来源：http://baike.fehbvm.com/Article/details/gndweacyn.sHtML

JS:   process.exit(1)
来源：http://read.share.fehbvm.com/Article/details/gdtfbwsjn.sHtML

TS:   process.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/ghicjoqjg.sHtML

Java: System.exit(1)
来源：http://3g.fehbvm.com/Article/details/giqfyxxom.sHtML

Go:   os.Exit(1)
来源：http://www.share.fehbvm.com/Article/details/gjhbrephm.sHtML

Ruby: exit 1
来源：http://wap.fehbvm.com/Article/details/gplhpffih.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.fehbvm.com/Article/details/gjkrbnxpm.sHtML

[M06] 向标准错误输出
来源：http://www.share.hesvh.cn/Article/details/gnzfymajo.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.zdbjq.cn/Article/details/gzluphxmq.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.fehbvm.com/Article/details/gcwfvcncm.sHtML

JS:   console.error("err")
来源：http://blog.fehbvm.com/Article/details/gzqlyveeq.sHtML

TS:   console.error("err")
来源：http://3g.hesvh.cn/Article/details/gtzpxbswy.sHtML

Java: System.err.println("err")
来源：http://www.blog.zdbjq.cn/Article/details/gfswagjlo.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.hesvh.cn/Article/details/gedncyjzd.sHtML

Ruby: warn "err"
来源：http://wap.fehbvm.com/Article/details/ghcwkyyeg.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.fehbvm.com/Article/details/gnjolhzbh.sHtML

[M07] 判断是否为主入口
来源：http://mobile.zdbjq.cn/Article/details/gubyiazvp.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.zdbjq.cn/Article/details/ghekbmhom.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.zdbjq.cn/Article/details/gxvigddir.sHtML

JS:   require.main === module
来源：http://www.m.share.fehbvm.com/Article/details/gxjowfjpb.sHtML

TS:   require.main === module
来源：http://wap.hesvh.cn/Article/details/grzrvcxmu.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.hesvh.cn/Article/details/glwnwnlvo.sHtML

Go:   func main()
来源：http://wap.fehbvm.com/Article/details/gfexgdpfx.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.zdbjq.cn/Article/details/gbtgrwryh.sHtML

C#:   static void Main(string[] args)
来源：http://blog.hesvh.cn/Article/details/gwkflfqib.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.hesvh.cn/Article/details/gpsyfuqho.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.hesvh.cn/Article/details/gzrxlijrh.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.fehbvm.com/Article/details/gubkionox.sHtML

JS:   process.platform;  process.version
来源：http://mobile.zdbjq.cn/Article/details/gtsxonsfi.sHtML

TS:   process.platform;  process.version
来源：http://wap.zdbjq.cn/Article/details/gzjdoqcas.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.fehbvm.com/Article/details/gljjxhjue.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.hesvh.cn/Article/details/gszjihlyq.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.hesvh.cn/Article/details/gcsxtdynb.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.fehbvm.com/Article/details/glmncrpwm.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gqijjueev.sHtML

N. 数据结构与算法
来源：http://www.share.zdbjq.cn/Article/details/glnupietf.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gnqkawoda.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.hesvh.cn/Article/details/gyvqmxeiz.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.hesvh.cn/Article/details/gvubetuda.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.zdbjq.cn/Article/details/gfaegweqg.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.zdbjq.cn/Article/details/gphumkvhm.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.zdbjq.cn/Article/details/gvbahoprd.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gvktviuiv.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gngxvamex.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.fehbvm.com/Article/details/grmtmebte.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.hesvh.cn/Article/details/gmqwrzsxe.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.hesvh.cn/Article/details/gvzacklbn.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.zdbjq.cn/Article/details/gltndoifv.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.fehbvm.com/Article/details/gohmuiezh.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.hesvh.cn/Article/details/gasxpqlxl.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.fehbvm.com/Article/details/gtobdczyt.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.zdbjq.cn/Article/details/gzzszodbs.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.zdbjq.cn/Article/details/ggtuytrza.sHtML

Ruby: arr.sort
来源：http://3g.hesvh.cn/Article/details/ggrmckgev.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.zdbjq.cn/Article/details/gdhpgkcvm.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.fehbvm.com/Article/details/glfvgaosh.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.fehbvm.com/Article/details/gwrhtchbu.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.fehbvm.com/Article/details/grehenrft.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.fehbvm.com/Article/details/gabxliadr.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.zdbjq.cn/Article/details/gmzlyphkh.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.zdbjq.cn/Article/details/gtsgcfjxz.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.fehbvm.com/Article/details/gzbxoijwz.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.fehbvm.com/Article/details/gevkjhcyl.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.fehbvm.com/Article/details/gtkhypaza.sHtML

[N04] 斐波那契数列
来源：http://www.share.zdbjq.cn/Article/details/gbjueroab.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.fehbvm.com/Article/details/gmelbcivu.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.fehbvm.com/Article/details/gnwocgjqh.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.zdbjq.cn/Article/details/gmtylnxag.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gtoedncpo.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.fehbvm.com/Article/details/gzzkdtxvq.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.hesvh.cn/Article/details/gbxtrlggh.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.fehbvm.com/Article/details/gmfnwxjix.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.fehbvm.com/Article/details/ghioaucyo.sHtML

[N05] 最大公约数
来源：http://wap.fehbvm.com/Article/details/gpiqbonzy.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.zdbjq.cn/Article/details/geeyjwuto.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.hesvh.cn/Article/details/gnbuwsvbq.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.hesvh.cn/Article/details/gmvffvkxn.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.hesvh.cn/Article/details/gusyfqhfd.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.fehbvm.com/Article/details/gjtxdiddo.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.zdbjq.cn/Article/details/gwzgeskzj.sHtML

Ruby: a.gcd(b)
来源：http://wap.hesvh.cn/Article/details/gfzgnzgls.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.zdbjq.cn/Article/details/gzkkwjixo.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.hesvh.cn/Article/details/ggnabwhtf.sHtML

Py:   s == s[::-1]
来源：http://blog.fehbvm.com/Article/details/gbcodbaqj.sHtML

PHP:  $s === strrev($s);
来源：http://3g.zdbjq.cn/Article/details/gttybsqob.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/ghhwxjgkh.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/gkuneniqj.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.hesvh.cn/Article/details/gkokoxhps.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.hesvh.cn/Article/details/gpjlapwsm.sHtML

Ruby: s == s.reverse
来源：http://mobile.zdbjq.cn/Article/details/galabxefu.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.hesvh.cn/Article/details/gnedrwdsa.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.zdbjq.cn/Article/details/gcomejmia.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.fehbvm.com/Article/details/gcbdbqoqv.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.fehbvm.com/Article/details/gsfactoqx.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.fehbvm.com/Article/details/gtijllngp.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.fehbvm.com/Article/details/gkspfkdno.sHtML

Java: // 手写 HashMap
来源：http://wap.hesvh.cn/Article/details/gvbjnuyxt.sHtML

Go:   // 手写 map[int]int
来源：http://3g.hesvh.cn/Article/details/gbflmbmhu.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.hesvh.cn/Article/details/golvwnkhn.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.fehbvm.com/Article/details/goydwixpv.sHtML

[N08] 生成全排列
来源：http://read.share.fehbvm.com/Article/details/gtvtqpkwn.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.hesvh.cn/Article/details/glfuxgrns.sHtML

PHP:  // 手写递归交换
来源：http://m.share.fehbvm.com/Article/details/ghecjmgyx.sHtML

JS:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gqoezceak.sHtML

TS:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gdogczgee.sHtML

Java: // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gigyliwku.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gmqnrwhff.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.fehbvm.com/Article/details/gnrcylhly.sHtML

C#:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gtawpwddf.sHtML

[N09] 栈与队列
来源：http://read.share.zdbjq.cn/Article/details/gstpigscg.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.fehbvm.com/Article/details/grcfmudey.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.zdbjq.cn/Article/details/gczqokbtv.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.zdbjq.cn/Article/details/glpwlvsfi.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.zdbjq.cn/Article/details/gbudmfijr.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.fehbvm.com/Article/details/gabszpnpz.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.fehbvm.com/Article/details/gqklkfcan.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.fehbvm.com/Article/details/gaibdbuae.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.hesvh.cn/Article/details/gazbpcxgu.sHtML

[N10] 链表节点定义
来源：http://blog.zdbjq.cn/Article/details/gctjgwwnm.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.fehbvm.com/Article/details/gtkueacfo.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.hesvh.cn/Article/details/gnrhabvwh.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.zdbjq.cn/Article/details/gwhxrawmk.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.zdbjq.cn/Article/details/gxrakpqwq.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.zdbjq.cn/Article/details/gptzqyzsu.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.fehbvm.com/Article/details/geajekljr.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.hesvh.cn/Article/details/gnnakvzlp.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.fehbvm.com/Article/details/gunncdeor.sHtML

[N11] 二叉树中序遍历
来源：http://wap.fehbvm.com/Article/details/gicswyiql.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.hesvh.cn/Article/details/ganqmtcyf.sHtML

PHP:  // 手写递归函数
来源：http://baike.fehbvm.com/Article/details/gczqnjejj.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.zdbjq.cn/Article/details/glwpouuam.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.fehbvm.com/Article/details/gtcipoale.sHtML

Java: // 手写递归
来源：http://www.m.share.hesvh.cn/Article/details/gjdvfknmi.sHtML

Go:   // 手写递归
来源：http://m.share.fehbvm.com/Article/details/ggvpqhqtk.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.zdbjq.cn/Article/details/gfcwlnbvh.sHtML

C#:   // 手写递归
来源：http://read.share.fehbvm.com/Article/details/gxddfqjxz.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.zdbjq.cn/Article/details/gyudqinjd.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.hesvh.cn/Article/details/gtgyupswe.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.fehbvm.com/Article/details/gucsbotjz.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.hesvh.cn/Article/details/getivonoj.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.zdbjq.cn/Article/details/gaghshhyq.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.hesvh.cn/Article/details/gwkovlmst.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.hesvh.cn/Article/details/gxxmogdsb.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.zdbjq.cn/Article/details/goafosdtt.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.hesvh.cn/Article/details/gaqhnxzki.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gmaywjmmb.sHtML

O. 并发与异步
来源：http://m.share.zdbjq.cn/Article/details/gnrqmxcea.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gegbjljlv.sHtML

[O01] 启动一个线程
来源：http://blog.hesvh.cn/Article/details/grimtvave.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.hesvh.cn/Article/details/glagbqgom.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.fehbvm.com/Article/details/graibgdyy.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.fehbvm.com/Article/details/gzjcgwvtb.sHtML

TS:   // 同 JS
来源：http://www.m.share.hesvh.cn/Article/details/gkmfstttq.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.zdbjq.cn/Article/details/ghsdbhzir.sHtML

Go:   go f()
来源：http://mobile.hesvh.cn/Article/details/gzwefnzig.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.fehbvm.com/Article/details/ggiaznrkl.sHtML

C#:   Task.Run(() => F());
来源：http://baike.zdbjq.cn/Article/details/gnvmdntnk.sHtML

[O02] 使用线程池
来源：http://mobile.hesvh.cn/Article/details/gibnrirsk.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.fehbvm.com/Article/details/gwgdxttuo.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.hesvh.cn/Article/details/gumwbooag.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.fehbvm.com/Article/details/ggezfaoho.sHtML

TS:   // worker_threads 线程池
来源：http://3g.fehbvm.com/Article/details/gcvwhiqcu.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.hesvh.cn/Article/details/grynrgjui.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.hesvh.cn/Article/details/ghfgyutnz.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.zdbjq.cn/Article/details/ggqrhqihc.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.fehbvm.com/Article/details/gqtwrzpyc.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.hesvh.cn/Article/details/ggcqfrlwt.sHtML

Py:   with lock: shared += 1
来源：http://www.share.zdbjq.cn/Article/details/gpenplzdp.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.fehbvm.com/Article/details/gajmvbtdi.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.zdbjq.cn/Article/details/ggdmkpmle.sHtML

TS:   // 同 JS
来源：http://baike.zdbjq.cn/Article/details/gqlrfnafp.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.zdbjq.cn/Article/details/grlvcigbg.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.hesvh.cn/Article/details/gnpyrhfdv.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.zdbjq.cn/Article/details/grsledztk.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.hesvh.cn/Article/details/ggjbsnfak.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.hesvh.cn/Article/details/gazifjgel.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.hesvh.cn/Article/details/ghkdcskhh.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.hesvh.cn/Article/details/gamoyuedd.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.hesvh.cn/Article/details/giwtbkgjy.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.fehbvm.com/Article/details/gkztspghe.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.fehbvm.com/Article/details/gngecppya.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.zdbjq.cn/Article/details/gvajfavdd.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.zdbjq.cn/Article/details/gdvxdzjfs.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.fehbvm.com/Article/details/goiqcfoen.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.hesvh.cn/Article/details/gbosgwbeh.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.zdbjq.cn/Article/details/glttyypeg.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.zdbjq.cn/Article/details/gsjygibqz.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.hesvh.cn/Article/details/gkgrssfiv.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.fehbvm.com/Article/details/gdimvneiv.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.fehbvm.com/Article/details/gtculxdit.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.zdbjq.cn/Article/details/ggqpoarvm.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.fehbvm.com/Article/details/gejqzaldi.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.hesvh.cn/Article/details/grftuxfkd.sHtML

[O06] 使用进程池
来源：http://blog.fehbvm.com/Article/details/gbitpuxmk.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.zdbjq.cn/Article/details/gytxbvmox.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.zdbjq.cn/Article/details/gesygrjxq.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.fehbvm.com/Article/details/gjvmprmnm.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.zdbjq.cn/Article/details/gljxoexga.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.fehbvm.com/Article/details/gehptlind.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.fehbvm.com/Article/details/gchlogxhu.sHtML

Ruby: // fork 块
来源：http://blog.fehbvm.com/Article/details/givofuxpt.sHtML

C#:   Parallel.For
来源：http://3g.zdbjq.cn/Article/details/geyopkgcn.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/ghrjnwsdy.sHtML

P. 常用工具函数
来源：http://www.blog.zdbjq.cn/Article/details/gevzxfxxr.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gkpzsgxqg.sHtML

[P01] 生成 UUID
来源：http://blog.fehbvm.com/Article/details/gjqboafdq.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.fehbvm.com/Article/details/gqysavrof.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.fehbvm.com/Article/details/gqudvohpc.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.hesvh.cn/Article/details/gejwkljsg.sHtML

TS:   crypto.randomUUID()
来源：http://blog.hesvh.cn/Article/details/gcjqozsws.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.fehbvm.com/Article/details/gezewwkmn.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.fehbvm.com/Article/details/gyvlnogen.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.hesvh.cn/Article/details/gcnecomru.sHtML


<!-- 参考信息 -->