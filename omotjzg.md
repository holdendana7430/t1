代发 wailian999

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.hesvh.cn/Article/details/gbgjqpole.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.fehbvm.com/Article/details/gnuopaimb.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.hesvh.cn/Article/details/gsoejguoo.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.zdbjq.cn/Article/details/gpovmadkf.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.hesvh.cn/Article/details/guvdcfllh.sHtML

[L04] 设置超时
来源：http://blog.hesvh.cn/Article/details/gkknwcxca.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.fehbvm.com/Article/details/guycrzrjk.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.zdbjq.cn/Article/details/grmjkhkvv.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.hesvh.cn/Article/details/glarsrxyf.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.hesvh.cn/Article/details/gqckibpxs.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.hesvh.cn/Article/details/gzijucvof.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.fehbvm.com/Article/details/gysdslsvc.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.hesvh.cn/Article/details/gemmmnqlh.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.zdbjq.cn/Article/details/gwsewcvbp.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.fehbvm.com/Article/details/glqfruufa.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.hesvh.cn/Article/details/giniieynh.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.zdbjq.cn/Article/details/gfysewrrl.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blog.fehbvm.com/Article/details/gtyjwypcq.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.fehbvm.com/Article/details/gglzqedrc.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.hesvh.cn/Article/details/grmllqfvl.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.fehbvm.com/Article/details/gbfmdiwne.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.fehbvm.com/Article/details/gdaqrfabw.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.zdbjq.cn/Article/details/gtjgubetw.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.hesvh.cn/Article/details/gqgioekvd.sHtML

Py:   resp.json()
来源：http://www.share.zdbjq.cn/Article/details/gkeeymkwx.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.fehbvm.com/Article/details/gbatpmocw.sHtML

JS:   await resp.json()
来源：http://mobile.fehbvm.com/Article/details/gnuhwyjjl.sHtML

TS:   await resp.json()
来源：http://www.blog.zdbjq.cn/Article/details/gpwbmalmi.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.fehbvm.com/Article/details/gouulpfmr.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.fehbvm.com/Article/details/giwposxkr.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.hesvh.cn/Article/details/gowbyjcfu.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.zdbjq.cn/Article/details/garvtckmm.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.hesvh.cn/Article/details/gohztuxve.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.fehbvm.com/Article/details/gdbblwttq.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.hesvh.cn/Article/details/glpfhqfii.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.zdbjq.cn/Article/details/gwikpnaoy.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.hesvh.cn/Article/details/ginyjwkib.sHtML

Java: resp.statusCode()
来源：http://wap.zdbjq.cn/Article/details/gkjzrcghn.sHtML

Go:   resp.StatusCode
来源：http://www.blog.hesvh.cn/Article/details/gmwigvpqj.sHtML

Ruby: resp.code.to_i
来源：http://mobile.hesvh.cn/Article/details/gylgixyby.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.hesvh.cn/Article/details/gwnsmthka.sHtML

[L08] 并发请求多个地址
来源：http://www.share.fehbvm.com/Article/details/gmqhltlor.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.fehbvm.com/Article/details/gqavlrczt.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.zdbjq.cn/Article/details/gsbpopzdn.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.zdbjq.cn/Article/details/gebnfyncc.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fehbvm.com/Article/details/gpcgesyxv.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.fehbvm.com/Article/details/gfkftasod.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.hesvh.cn/Article/details/gazlxofeg.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.hesvh.cn/Article/details/gsyppjwcx.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.fehbvm.com/Article/details/ggqouskph.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gxnnrxzxs.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.hesvh.cn/Article/details/gxzivmpym.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/goapgnoan.sHtML

[M01] 读取命令行参数
来源：http://mobile.zdbjq.cn/Article/details/gfupouogc.sHtML

Py:   sys.argv[1:]
来源：http://m.share.hesvh.cn/Article/details/gfhiwbtit.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.fehbvm.com/Article/details/gsdrslofp.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.zdbjq.cn/Article/details/gszkchgke.sHtML

TS:   process.argv.slice(2)
来源：http://wap.fehbvm.com/Article/details/gibwomfmf.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.fehbvm.com/Article/details/glymtbndz.sHtML

Go:   os.Args[1:]
来源：http://www.share.hesvh.cn/Article/details/gfnxqmope.sHtML

Ruby: ARGV
来源：http://3g.fehbvm.com/Article/details/gbsionyid.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.hesvh.cn/Article/details/gyuyaiasl.sHtML

[M02] 读取环境变量
来源：http://baike.hesvh.cn/Article/details/gjzamdyxw.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.zdbjq.cn/Article/details/gdusnzfrv.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.zdbjq.cn/Article/details/geowuvomy.sHtML

JS:   process.env.HOME
来源：http://wap.hesvh.cn/Article/details/gfoxgygkj.sHtML

TS:   process.env.HOME
来源：http://www.share.hesvh.cn/Article/details/gezvjtjxa.sHtML

Java: System.getenv("HOME")
来源：http://baike.fehbvm.com/Article/details/gkxuyejic.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.hesvh.cn/Article/details/gywaffjxq.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.fehbvm.com/Article/details/gcdurzpmz.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.hesvh.cn/Article/details/gseszhgnk.sHtML

[M03] 执行外部命令
来源：http://m.share.zdbjq.cn/Article/details/girxygrvk.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.fehbvm.com/Article/details/gfnutsonm.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.fehbvm.com/Article/details/geawmbrfc.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.fehbvm.com/Article/details/gnrodutcj.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.zdbjq.cn/Article/details/gjfnntwpb.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.zdbjq.cn/Article/details/gssraifea.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.fehbvm.com/Article/details/gvkfygwbk.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.zdbjq.cn/Article/details/gcawmhxzk.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.zdbjq.cn/Article/details/gwbqdnmma.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.hesvh.cn/Article/details/gccpwhbyv.sHtML

Py:   os.getcwd()
来源：http://mobile.zdbjq.cn/Article/details/gwwfoagoi.sHtML

PHP:  getcwd();
来源：http://wap.hesvh.cn/Article/details/gnlxrguie.sHtML

JS:   process.cwd()
来源：http://baike.zdbjq.cn/Article/details/glchfaiqc.sHtML

TS:   process.cwd()
来源：http://blog.hesvh.cn/Article/details/glzipeldn.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.fehbvm.com/Article/details/gvgrasfvb.sHtML

Go:   os.Getwd()
来源：http://baike.zdbjq.cn/Article/details/gynygfdyw.sHtML

Ruby: Dir.pwd
来源：http://mobile.hesvh.cn/Article/details/gembsjahv.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.zdbjq.cn/Article/details/gcnjziftt.sHtML

[M05] 设置退出码
来源：http://mobile.zdbjq.cn/Article/details/grhwzifxm.sHtML

Py:   sys.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gogqnblib.sHtML

PHP:  exit(1);
来源：http://3g.hesvh.cn/Article/details/gcgdyaeea.sHtML

JS:   process.exit(1)
来源：http://read.share.hesvh.cn/Article/details/gmhtivycl.sHtML

TS:   process.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gqleabdlu.sHtML

Java: System.exit(1)
来源：http://m.share.hesvh.cn/Article/details/gfsneqcxb.sHtML

Go:   os.Exit(1)
来源：http://read.share.hesvh.cn/Article/details/gzgfplimo.sHtML

Ruby: exit 1
来源：http://3g.fehbvm.com/Article/details/gbvbbczya.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.fehbvm.com/Article/details/grlmhfenc.sHtML

[M06] 向标准错误输出
来源：http://blog.zdbjq.cn/Article/details/gyrnvalqi.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.zdbjq.cn/Article/details/gaadauzxv.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.zdbjq.cn/Article/details/gjifduupm.sHtML

JS:   console.error("err")
来源：http://wap.fehbvm.com/Article/details/gqzbdqqgn.sHtML

TS:   console.error("err")
来源：http://www.blog.zdbjq.cn/Article/details/gswxlqhdi.sHtML

Java: System.err.println("err")
来源：http://www.m.share.hesvh.cn/Article/details/gvcmsgrfr.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.zdbjq.cn/Article/details/gkadiljkb.sHtML

Ruby: warn "err"
来源：http://3g.hesvh.cn/Article/details/gyaxxxygj.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.hesvh.cn/Article/details/gycbmwfyp.sHtML

[M07] 判断是否为主入口
来源：http://mobile.zdbjq.cn/Article/details/geehhpqbo.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.fehbvm.com/Article/details/ghwmspinc.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.fehbvm.com/Article/details/gabhxnwfi.sHtML

JS:   require.main === module
来源：http://wap.zdbjq.cn/Article/details/groszlazy.sHtML

TS:   require.main === module
来源：http://baike.zdbjq.cn/Article/details/grlvametw.sHtML

Java: public static void main(String[] args)
来源：http://www.share.zdbjq.cn/Article/details/gafuszrnf.sHtML

Go:   func main()
来源：http://3g.fehbvm.com/Article/details/goynvqotc.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.zdbjq.cn/Article/details/gnebdnxaz.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.hesvh.cn/Article/details/gjzzqykpz.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.fehbvm.com/Article/details/gquegpybj.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.hesvh.cn/Article/details/giwkkydnt.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.hesvh.cn/Article/details/gjanwzkvx.sHtML

JS:   process.platform;  process.version
来源：http://www.share.hesvh.cn/Article/details/gynczqycy.sHtML

TS:   process.platform;  process.version
来源：http://mobile.fehbvm.com/Article/details/gutnrunlf.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.hesvh.cn/Article/details/gfucwnfhl.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.zdbjq.cn/Article/details/guwgmawey.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.hesvh.cn/Article/details/gybqlizld.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.fehbvm.com/Article/details/gdjaueldr.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gajvpladi.sHtML

N. 数据结构与算法
来源：http://wap.zdbjq.cn/Article/details/gmsncskbg.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/grsmelwzz.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.zdbjq.cn/Article/details/gwqrieilj.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gbiicohxt.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.hesvh.cn/Article/details/grwkdvodb.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.fehbvm.com/Article/details/gtlpzqble.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.fehbvm.com/Article/details/gnryqwgrl.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gjmizfedw.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gjqgsgfgs.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.hesvh.cn/Article/details/gnifbwxbd.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gmchzlevz.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.fehbvm.com/Article/details/grewqectb.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.hesvh.cn/Article/details/gjbbwaosk.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.fehbvm.com/Article/details/glttppvnc.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.zdbjq.cn/Article/details/ghnopjnzp.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.hesvh.cn/Article/details/gkjehzyuq.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.zdbjq.cn/Article/details/godcppjlg.sHtML

Go:   slices.Sort(arr)
来源：http://blog.zdbjq.cn/Article/details/ganxpdsed.sHtML

Ruby: arr.sort
来源：http://mobile.fehbvm.com/Article/details/glzgqjxot.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.hesvh.cn/Article/details/gobxfcqry.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.zdbjq.cn/Article/details/gnyyrojum.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.fehbvm.com/Article/details/gecdvrmgp.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.zdbjq.cn/Article/details/gfnjgnbxa.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.fehbvm.com/Article/details/grfjlduqe.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.zdbjq.cn/Article/details/gaieawfkj.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.fehbvm.com/Article/details/gggpktabe.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.zdbjq.cn/Article/details/gyxxulzhs.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.fehbvm.com/Article/details/ggqphfpfh.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.zdbjq.cn/Article/details/groqhbybg.sHtML

[N04] 斐波那契数列
来源：http://wap.zdbjq.cn/Article/details/goaxywkei.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.fehbvm.com/Article/details/gbwrvqgnt.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.fehbvm.com/Article/details/gffcbtmww.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.fehbvm.com/Article/details/glzcajtrf.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.zdbjq.cn/Article/details/gwncvjhhj.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.hesvh.cn/Article/details/gjbqhsxrz.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.hesvh.cn/Article/details/gwvujazxj.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.fehbvm.com/Article/details/gkyojlblg.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.hesvh.cn/Article/details/gjeqmsdyq.sHtML

[N05] 最大公约数
来源：http://baike.fehbvm.com/Article/details/ganlqtqlk.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.hesvh.cn/Article/details/gvfjexkfc.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.hesvh.cn/Article/details/gaajtycxz.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.zdbjq.cn/Article/details/gnpctxqfu.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.hesvh.cn/Article/details/gvtfialom.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.zdbjq.cn/Article/details/goxfzkxyb.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.hesvh.cn/Article/details/gdjxavffb.sHtML

Ruby: a.gcd(b)
来源：http://baike.fehbvm.com/Article/details/gbhnmlmvh.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.fehbvm.com/Article/details/ghascbcsy.sHtML

[N06] 判断回文字符串
来源：http://www.blog.zdbjq.cn/Article/details/ghvqjglqr.sHtML

Py:   s == s[::-1]
来源：http://www.share.fehbvm.com/Article/details/gidwtjhoj.sHtML

PHP:  $s === strrev($s);
来源：http://3g.zdbjq.cn/Article/details/gacqtmplg.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/glcnzzjkf.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/gjliahwnv.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.zdbjq.cn/Article/details/gwdmngrrg.sHtML

Go:   // 双指针从两端比较
来源：http://wap.hesvh.cn/Article/details/guohlgawr.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.zdbjq.cn/Article/details/gdwawqfgu.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.fehbvm.com/Article/details/gnpfdmvxg.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.hesvh.cn/Article/details/gozokoudw.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.hesvh.cn/Article/details/gbfnrgqek.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.zdbjq.cn/Article/details/gxthtltoy.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.fehbvm.com/Article/details/gzxkgftor.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.zdbjq.cn/Article/details/gmokegkxy.sHtML

Java: // 手写 HashMap
来源：http://read.share.fehbvm.com/Article/details/gvoyvtstr.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.hesvh.cn/Article/details/gejgcswxc.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.fehbvm.com/Article/details/gfwfclmlt.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.zdbjq.cn/Article/details/gqprxguza.sHtML

[N08] 生成全排列
来源：http://www.m.share.zdbjq.cn/Article/details/gcjtmlhqn.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gtwaphore.sHtML

PHP:  // 手写递归交换
来源：http://mobile.hesvh.cn/Article/details/gfkpiidfp.sHtML

JS:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/goecjhocx.sHtML

TS:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/glgjburfg.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gkunofaes.sHtML

Go:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gbhnazoyx.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.fehbvm.com/Article/details/gzlfcduji.sHtML

C#:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gibzwiivv.sHtML

[N09] 栈与队列
来源：http://baike.zdbjq.cn/Article/details/grqnadbzp.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.zdbjq.cn/Article/details/gytfqmmth.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.hesvh.cn/Article/details/gwdbcnzuh.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/gsynnpugh.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.zdbjq.cn/Article/details/gekedqscb.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.zdbjq.cn/Article/details/gepddbqxo.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.zdbjq.cn/Article/details/gucolayll.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.hesvh.cn/Article/details/grrordwmm.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.hesvh.cn/Article/details/gmdcvdzlt.sHtML

[N10] 链表节点定义
来源：http://baike.hesvh.cn/Article/details/gdviojung.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.hesvh.cn/Article/details/gpixzxqew.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.fehbvm.com/Article/details/gtqycgvxu.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.zdbjq.cn/Article/details/gtyxmwdiw.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.zdbjq.cn/Article/details/gemjhthte.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.zdbjq.cn/Article/details/gkfhozmkm.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.fehbvm.com/Article/details/govppzdpb.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.fehbvm.com/Article/details/gshdtjbfq.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.fehbvm.com/Article/details/gyeqyanqc.sHtML

[N11] 二叉树中序遍历
来源：http://wap.fehbvm.com/Article/details/gjxxwmzmn.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.zdbjq.cn/Article/details/gfcydrcyb.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.hesvh.cn/Article/details/gjelplrnj.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.hesvh.cn/Article/details/gwldolvxn.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.fehbvm.com/Article/details/ggzalrslm.sHtML

Java: // 手写递归
来源：http://www.m.share.hesvh.cn/Article/details/gffhwhcxu.sHtML

Go:   // 手写递归
来源：http://www.m.share.hesvh.cn/Article/details/gfxlkdkho.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.zdbjq.cn/Article/details/gzsojcxxm.sHtML

C#:   // 手写递归
来源：http://read.share.hesvh.cn/Article/details/gspbcrudv.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.zdbjq.cn/Article/details/gejhaauin.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.fehbvm.com/Article/details/gxqiyzhnn.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.zdbjq.cn/Article/details/gcfdfalqf.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.fehbvm.com/Article/details/gceownfrr.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.zdbjq.cn/Article/details/gxczlpbve.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.zdbjq.cn/Article/details/gjqpffwqg.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.hesvh.cn/Article/details/guecedfyu.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.zdbjq.cn/Article/details/ginoddpko.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.hesvh.cn/Article/details/gbdusklsz.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gfrsrwrnh.sHtML

O. 并发与异步
来源：http://mobile.hesvh.cn/Article/details/guvmawyzl.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gcsjeamyh.sHtML

[O01] 启动一个线程
来源：http://www.share.fehbvm.com/Article/details/ghmdkrckq.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.fehbvm.com/Article/details/gcexqxrbd.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.zdbjq.cn/Article/details/gaazdltlk.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.zdbjq.cn/Article/details/gnreoouyy.sHtML

TS:   // 同 JS
来源：http://mobile.zdbjq.cn/Article/details/gtkkexxrh.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.hesvh.cn/Article/details/gjdhbmhsc.sHtML

Go:   go f()
来源：http://m.share.hesvh.cn/Article/details/ggscngtfs.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.zdbjq.cn/Article/details/gmwevivnw.sHtML

C#:   Task.Run(() => F());
来源：http://wap.zdbjq.cn/Article/details/grjgjllbg.sHtML

[O02] 使用线程池
来源：http://www.blog.hesvh.cn/Article/details/gptasvgtt.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.zdbjq.cn/Article/details/gpxspgugp.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.zdbjq.cn/Article/details/gjzhgguid.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.fehbvm.com/Article/details/gboqonvqn.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.fehbvm.com/Article/details/gojigdufu.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.fehbvm.com/Article/details/gioqjqkaf.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.hesvh.cn/Article/details/gjxmhznmo.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.zdbjq.cn/Article/details/ghbrzeaba.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.zdbjq.cn/Article/details/ghyiwqeru.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.hesvh.cn/Article/details/gvjjlfskx.sHtML

Py:   with lock: shared += 1
来源：http://3g.hesvh.cn/Article/details/gcsuokbfq.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.zdbjq.cn/Article/details/gyraftpcg.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.fehbvm.com/Article/details/griecckgh.sHtML

TS:   // 同 JS
来源：http://3g.hesvh.cn/Article/details/gaggarabc.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.zdbjq.cn/Article/details/gkdxvdfnm.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.hesvh.cn/Article/details/grtypctql.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.fehbvm.com/Article/details/gebdhchqu.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.zdbjq.cn/Article/details/gdqsmfapb.sHtML

[O04] 定义异步函数并等待
来源：http://wap.zdbjq.cn/Article/details/gzpdtnwwb.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.hesvh.cn/Article/details/goxoqncfs.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.zdbjq.cn/Article/details/gyxnbhdbi.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.fehbvm.com/Article/details/gxzglqxct.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.zdbjq.cn/Article/details/gopqaithg.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.fehbvm.com/Article/details/gctrabgex.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.fehbvm.com/Article/details/gimozcmnk.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.zdbjq.cn/Article/details/gbndtyuzm.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.zdbjq.cn/Article/details/gwbbuixpd.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.fehbvm.com/Article/details/gxwhnxrub.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.fehbvm.com/Article/details/gxppotqjw.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.hesvh.cn/Article/details/ghekfqidu.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.fehbvm.com/Article/details/ghaurszto.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.zdbjq.cn/Article/details/gxrcuupbf.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.zdbjq.cn/Article/details/glmjqbkjp.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.fehbvm.com/Article/details/gjtsnipgm.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.hesvh.cn/Article/details/gtyjkzkwc.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.zdbjq.cn/Article/details/ghcftgwar.sHtML

[O06] 使用进程池
来源：http://read.share.hesvh.cn/Article/details/gwlavzury.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.hesvh.cn/Article/details/ggqspqgni.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.zdbjq.cn/Article/details/gxbsaynau.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.zdbjq.cn/Article/details/gjytkcciz.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.zdbjq.cn/Article/details/gwdqvggox.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.zdbjq.cn/Article/details/gapcevuds.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.hesvh.cn/Article/details/gbzcurqbq.sHtML

Ruby: // fork 块
来源：http://baike.fehbvm.com/Article/details/gxiqkrwnj.sHtML

C#:   Parallel.For
来源：http://3g.fehbvm.com/Article/details/gyfcebsme.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gnctfhsjh.sHtML

P. 常用工具函数
来源：http://wap.fehbvm.com/Article/details/gsgbnnwiu.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gjlaoflyg.sHtML

[P01] 生成 UUID
来源：http://www.m.share.zdbjq.cn/Article/details/gmtxicgnc.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.zdbjq.cn/Article/details/gcxashqkt.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.fehbvm.com/Article/details/gznwkpity.sHtML

JS:   crypto.randomUUID()
来源：http://baike.hesvh.cn/Article/details/gcaldwofp.sHtML


<!-- 参考信息 -->