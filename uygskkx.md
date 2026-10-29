代发 wailian999

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.zdbjq.cn/Article/details/giluprpeb.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.hesvh.cn/Article/details/gtpbcmuwv.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.fehbvm.com/Article/details/gyvwthpjo.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.hesvh.cn/Article/details/gsntqqsau.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.fehbvm.com/Article/details/gfswklspx.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.zdbjq.cn/Article/details/gioheplyy.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.fehbvm.com/Article/details/gcuwdeprv.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.hesvh.cn/Article/details/gchpiyuck.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.zdbjq.cn/Article/details/gfgysdlyn.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.fehbvm.com/Article/details/gglogukwg.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.fehbvm.com/Article/details/gbusxmldc.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.zdbjq.cn/Article/details/gcgkefntg.sHtML

Py:   resp.json()
来源：http://www.blog.fehbvm.com/Article/details/getxsaodi.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.zdbjq.cn/Article/details/gduoanixm.sHtML

JS:   await resp.json()
来源：http://wap.fehbvm.com/Article/details/ghmqiklyg.sHtML

TS:   await resp.json()
来源：http://www.m.share.hesvh.cn/Article/details/gojmdjqrk.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.hesvh.cn/Article/details/gmctpfpxb.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.zdbjq.cn/Article/details/ghoaelauw.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.zdbjq.cn/Article/details/gnxrmtpbb.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.zdbjq.cn/Article/details/gsjmarbvc.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.zdbjq.cn/Article/details/giaosmbig.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.zdbjq.cn/Article/details/gsbsgpold.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.hesvh.cn/Article/details/gwavanicb.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.fehbvm.com/Article/details/gbtzrnllt.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.hesvh.cn/Article/details/gqnpdfhav.sHtML

Java: resp.statusCode()
来源：http://m.share.zdbjq.cn/Article/details/gdnelhyeu.sHtML

Go:   resp.StatusCode
来源：http://www.blog.zdbjq.cn/Article/details/gnigdlqfh.sHtML

Ruby: resp.code.to_i
来源：http://read.share.hesvh.cn/Article/details/gcwxrcdyu.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.hesvh.cn/Article/details/gjdfencik.sHtML

[L08] 并发请求多个地址
来源：http://3g.zdbjq.cn/Article/details/glqwuvmgh.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.fehbvm.com/Article/details/gqmpvcadk.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.hesvh.cn/Article/details/grdnbgwrn.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.zdbjq.cn/Article/details/glbfsrrsy.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.zdbjq.cn/Article/details/ghnztuupo.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.fehbvm.com/Article/details/gldirksdm.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.fehbvm.com/Article/details/gvhszdzyy.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.zdbjq.cn/Article/details/gjixfinkx.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.hesvh.cn/Article/details/ggzhgvami.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gyoccarmc.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.fehbvm.com/Article/details/gkerrythn.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/ghzfchdww.sHtML

[M01] 读取命令行参数
来源：http://m.share.fehbvm.com/Article/details/gvnvhoycz.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.fehbvm.com/Article/details/gyhmnhahn.sHtML

PHP:  $argv;  $argc;
来源：http://blog.zdbjq.cn/Article/details/ggqvetsir.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.zdbjq.cn/Article/details/gypejryur.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.fehbvm.com/Article/details/gxpcjmpxo.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.zdbjq.cn/Article/details/glvwwvjrn.sHtML

Go:   os.Args[1:]
来源：http://wap.hesvh.cn/Article/details/gyixvkloh.sHtML

Ruby: ARGV
来源：http://blog.fehbvm.com/Article/details/gbbadygcl.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.hesvh.cn/Article/details/gsvkgvcid.sHtML

[M02] 读取环境变量
来源：http://m.share.hesvh.cn/Article/details/gpvrrzhyl.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.hesvh.cn/Article/details/gspohnrvn.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.zdbjq.cn/Article/details/gwxmdmthm.sHtML

JS:   process.env.HOME
来源：http://www.share.zdbjq.cn/Article/details/gfjeirwmv.sHtML

TS:   process.env.HOME
来源：http://read.share.fehbvm.com/Article/details/gsygjcvvl.sHtML

Java: System.getenv("HOME")
来源：http://blog.zdbjq.cn/Article/details/gpmuyilfs.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.zdbjq.cn/Article/details/gcrazojmj.sHtML

Ruby: ENV["HOME"]
来源：http://baike.hesvh.cn/Article/details/genprznan.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.hesvh.cn/Article/details/ghqtemmqm.sHtML

[M03] 执行外部命令
来源：http://read.share.hesvh.cn/Article/details/gfukxmqzs.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.zdbjq.cn/Article/details/gvowcfiyc.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.hesvh.cn/Article/details/gtdtvszag.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.hesvh.cn/Article/details/ghuiyfasc.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.zdbjq.cn/Article/details/gwwmumovo.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.hesvh.cn/Article/details/gztlonmny.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.fehbvm.com/Article/details/gfrtrlesh.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.fehbvm.com/Article/details/gsetqbyvv.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.hesvh.cn/Article/details/gjgbbydul.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.hesvh.cn/Article/details/gkcsfmwhi.sHtML

Py:   os.getcwd()
来源：http://wap.fehbvm.com/Article/details/gyjosjwrx.sHtML

PHP:  getcwd();
来源：http://m.share.zdbjq.cn/Article/details/goicysrks.sHtML

JS:   process.cwd()
来源：http://www.m.share.hesvh.cn/Article/details/gmjjgghkp.sHtML

TS:   process.cwd()
来源：http://3g.zdbjq.cn/Article/details/gagzycjwf.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.hesvh.cn/Article/details/gskifregb.sHtML

Go:   os.Getwd()
来源：http://www.m.share.hesvh.cn/Article/details/ggjqmyndp.sHtML

Ruby: Dir.pwd
来源：http://mobile.fehbvm.com/Article/details/gheciqovb.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.fehbvm.com/Article/details/gjsvsqdrm.sHtML

[M05] 设置退出码
来源：http://read.share.zdbjq.cn/Article/details/gzrodgixi.sHtML

Py:   sys.exit(1)
来源：http://blog.hesvh.cn/Article/details/gecywonbl.sHtML

PHP:  exit(1);
来源：http://www.share.zdbjq.cn/Article/details/gybskokiq.sHtML

JS:   process.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gyyjhmqaw.sHtML

TS:   process.exit(1)
来源：http://wap.zdbjq.cn/Article/details/grkcyscws.sHtML

Java: System.exit(1)
来源：http://www.share.hesvh.cn/Article/details/gwozbdhvt.sHtML

Go:   os.Exit(1)
来源：http://wap.zdbjq.cn/Article/details/gvhqwlxck.sHtML

Ruby: exit 1
来源：http://blog.fehbvm.com/Article/details/gbndidsob.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.zdbjq.cn/Article/details/gshzirhay.sHtML

[M06] 向标准错误输出
来源：http://m.share.fehbvm.com/Article/details/gmzhleilg.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.zdbjq.cn/Article/details/glnpyrsxb.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.fehbvm.com/Article/details/gqwkldpnf.sHtML

JS:   console.error("err")
来源：http://baike.fehbvm.com/Article/details/gjvfgsdbs.sHtML

TS:   console.error("err")
来源：http://www.blog.hesvh.cn/Article/details/ghftzstxp.sHtML

Java: System.err.println("err")
来源：http://mobile.zdbjq.cn/Article/details/gybkghwan.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.fehbvm.com/Article/details/gcdfifesm.sHtML

Ruby: warn "err"
来源：http://www.m.share.zdbjq.cn/Article/details/gnkqjgnjg.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.zdbjq.cn/Article/details/gcapzwyrw.sHtML

[M07] 判断是否为主入口
来源：http://3g.hesvh.cn/Article/details/gelczcelt.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.hesvh.cn/Article/details/godlvhnzt.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.zdbjq.cn/Article/details/gpxzsnzwt.sHtML

JS:   require.main === module
来源：http://blog.zdbjq.cn/Article/details/gdhzbeqdd.sHtML

TS:   require.main === module
来源：http://3g.hesvh.cn/Article/details/gdzzvpeaw.sHtML

Java: public static void main(String[] args)
来源：http://wap.fehbvm.com/Article/details/ggfmsnzbg.sHtML

Go:   func main()
来源：http://blog.hesvh.cn/Article/details/gvoqkijuc.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.zdbjq.cn/Article/details/gpcqnmmxm.sHtML

C#:   static void Main(string[] args)
来源：http://blog.zdbjq.cn/Article/details/ggxinexsy.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.zdbjq.cn/Article/details/gzlaxkrqa.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.fehbvm.com/Article/details/ghzywqoyc.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.zdbjq.cn/Article/details/gneeglqgj.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.fehbvm.com/Article/details/gejzcxgzt.sHtML

TS:   process.platform;  process.version
来源：http://m.share.zdbjq.cn/Article/details/gzeeimosx.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.hesvh.cn/Article/details/gsviucibt.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.zdbjq.cn/Article/details/gtmrqasar.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.zdbjq.cn/Article/details/gofkuvsvj.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.hesvh.cn/Article/details/gakckaurh.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gkqfzdeay.sHtML

N. 数据结构与算法
来源：http://www.blog.hesvh.cn/Article/details/gmcqudvtq.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gcampwoyy.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.fehbvm.com/Article/details/gwqsexvjm.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gsfkyxgxg.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.hesvh.cn/Article/details/gkcrfyxtu.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.fehbvm.com/Article/details/gjbqdqosz.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.hesvh.cn/Article/details/gbwvftfdv.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gigjojjwr.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.fehbvm.com/Article/details/gkbykbkaf.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.zdbjq.cn/Article/details/glgfksydo.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gbbyfyhuu.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.fehbvm.com/Article/details/ghixyqpwk.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.zdbjq.cn/Article/details/gbwzgqape.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.hesvh.cn/Article/details/gsxovpmwt.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.zdbjq.cn/Article/details/gbrivbbfh.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.hesvh.cn/Article/details/giiqbqfhe.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.zdbjq.cn/Article/details/giyebzfup.sHtML

Go:   slices.Sort(arr)
来源：http://wap.fehbvm.com/Article/details/gcdxmzkkp.sHtML

Ruby: arr.sort
来源：http://www.m.share.zdbjq.cn/Article/details/gpaoxkjoj.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.fehbvm.com/Article/details/gcgknznjx.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.zdbjq.cn/Article/details/gkfgbyncr.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.fehbvm.com/Article/details/gmkyqftmf.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.fehbvm.com/Article/details/glohhqujb.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.hesvh.cn/Article/details/gqebftfiv.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.fehbvm.com/Article/details/gduwhpoxy.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.zdbjq.cn/Article/details/gqmrpwkxp.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.fehbvm.com/Article/details/giaazxodp.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.fehbvm.com/Article/details/gpltdawkf.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.fehbvm.com/Article/details/gzagfgixe.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.fehbvm.com/Article/details/gejsnxnif.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.fehbvm.com/Article/details/gmyfdmwro.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.hesvh.cn/Article/details/gvtjyfqot.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/gvmpyuyly.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.hesvh.cn/Article/details/gigrxirwg.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.fehbvm.com/Article/details/gddoltnuf.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.zdbjq.cn/Article/details/ggydhwbnr.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.hesvh.cn/Article/details/guysvbkik.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.zdbjq.cn/Article/details/gagdffnjf.sHtML

[N05] 最大公约数
来源：http://wap.fehbvm.com/Article/details/glwavxqqr.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.fehbvm.com/Article/details/gdovrjlsh.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.hesvh.cn/Article/details/gpbaqtkai.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.zdbjq.cn/Article/details/gddqjszve.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.zdbjq.cn/Article/details/gtgkwwbvi.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.zdbjq.cn/Article/details/gfktosyrv.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.fehbvm.com/Article/details/gsodsurvk.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.hesvh.cn/Article/details/grzwfrknc.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.zdbjq.cn/Article/details/gwlylvfgt.sHtML

[N06] 判断回文字符串
来源：http://wap.hesvh.cn/Article/details/gjvdxnxgw.sHtML

Py:   s == s[::-1]
来源：http://baike.fehbvm.com/Article/details/gptbkwufu.sHtML

PHP:  $s === strrev($s);
来源：http://blog.fehbvm.com/Article/details/gxeolubnw.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/gnmhcwlfc.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/gmqgakeoj.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.zdbjq.cn/Article/details/gemwssycb.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.zdbjq.cn/Article/details/gyelplezr.sHtML

Ruby: s == s.reverse
来源：http://m.share.zdbjq.cn/Article/details/gubtdwxkl.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.hesvh.cn/Article/details/gltqdkttl.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.hesvh.cn/Article/details/gljgsgome.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.zdbjq.cn/Article/details/gwteurgrw.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.zdbjq.cn/Article/details/gjmkfuxih.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.fehbvm.com/Article/details/goafslwos.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.hesvh.cn/Article/details/graoltwxd.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.hesvh.cn/Article/details/gapxbmyfi.sHtML

Go:   // 手写 map[int]int
来源：http://3g.zdbjq.cn/Article/details/gbzacywgv.sHtML

Ruby: // 手写 Hash
来源：http://blog.hesvh.cn/Article/details/gazkbrotc.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.zdbjq.cn/Article/details/gaswoajzg.sHtML

[N08] 生成全排列
来源：http://www.blog.zdbjq.cn/Article/details/gvlfnlazm.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.hesvh.cn/Article/details/gwwiktvhz.sHtML

PHP:  // 手写递归交换
来源：http://wap.zdbjq.cn/Article/details/gekobdcjx.sHtML

JS:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gjwphnsnd.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/guqxzqpqw.sHtML

Java: // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gdztqfzsf.sHtML

Go:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gzvfzglej.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.fehbvm.com/Article/details/gkxvqcuys.sHtML

C#:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gcmnwjmcu.sHtML

[N09] 栈与队列
来源：http://baike.hesvh.cn/Article/details/gaucktwrs.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.zdbjq.cn/Article/details/gfgrhboow.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.zdbjq.cn/Article/details/gijslkzrb.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.fehbvm.com/Article/details/gtkzmyuoz.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.zdbjq.cn/Article/details/gefwsjscn.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.zdbjq.cn/Article/details/gyerixmwy.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.hesvh.cn/Article/details/gerzleuqx.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/ggumlsrod.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.hesvh.cn/Article/details/gvnnvewto.sHtML

[N10] 链表节点定义
来源：http://baike.fehbvm.com/Article/details/gclpjhmlq.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.hesvh.cn/Article/details/gilgkplht.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.zdbjq.cn/Article/details/ginzlkuyy.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.zdbjq.cn/Article/details/gakeqcfee.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.zdbjq.cn/Article/details/gpazqyfum.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.fehbvm.com/Article/details/gaxijrdbh.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.zdbjq.cn/Article/details/gbwacbzts.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.zdbjq.cn/Article/details/gdtfnexah.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.zdbjq.cn/Article/details/gqjhtclsw.sHtML

[N11] 二叉树中序遍历
来源：http://3g.zdbjq.cn/Article/details/gqtchjojf.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.hesvh.cn/Article/details/gcdollvzm.sHtML

PHP:  // 手写递归函数
来源：http://mobile.fehbvm.com/Article/details/gusjngijv.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.fehbvm.com/Article/details/gepqdprmq.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.zdbjq.cn/Article/details/gyqkoylsj.sHtML

Java: // 手写递归
来源：http://mobile.zdbjq.cn/Article/details/gtrukdlbo.sHtML

Go:   // 手写递归
来源：http://www.m.share.zdbjq.cn/Article/details/gnwavfyxd.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.zdbjq.cn/Article/details/ggfaxkget.sHtML

C#:   // 手写递归
来源：http://blog.hesvh.cn/Article/details/gionunzdy.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.fehbvm.com/Article/details/gisrnzasf.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.fehbvm.com/Article/details/gcicbmwhr.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.zdbjq.cn/Article/details/gipkpycoj.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.zdbjq.cn/Article/details/gmhiuirpr.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.zdbjq.cn/Article/details/gyjcjdzvy.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.hesvh.cn/Article/details/ghwawktpw.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.fehbvm.com/Article/details/gqrqepqnf.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.fehbvm.com/Article/details/ggpjtxetw.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.hesvh.cn/Article/details/gsjjhzdox.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/geceiwxph.sHtML

O. 并发与异步
来源：http://baike.hesvh.cn/Article/details/gflynqcvs.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gswibpeec.sHtML

[O01] 启动一个线程
来源：http://www.share.hesvh.cn/Article/details/gxdvhhocb.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.fehbvm.com/Article/details/gsmghvbdo.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.fehbvm.com/Article/details/grogwdnmc.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.hesvh.cn/Article/details/glcgcbbnj.sHtML

TS:   // 同 JS
来源：http://wap.fehbvm.com/Article/details/gibjfdotj.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.zdbjq.cn/Article/details/gigkfehry.sHtML

Go:   go f()
来源：http://3g.hesvh.cn/Article/details/gfjrrfudu.sHtML

Ruby: Thread.new { f }
来源：http://wap.fehbvm.com/Article/details/gkteylpva.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.fehbvm.com/Article/details/gybwbsntm.sHtML

[O02] 使用线程池
来源：http://mobile.hesvh.cn/Article/details/gkplzaikt.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.zdbjq.cn/Article/details/gveijafdb.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.zdbjq.cn/Article/details/gjqzrwocj.sHtML

JS:   // worker_threads 线程池
来源：http://blog.fehbvm.com/Article/details/gsivxuhsf.sHtML

TS:   // worker_threads 线程池
来源：http://baike.fehbvm.com/Article/details/gwmumblts.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.hesvh.cn/Article/details/gavpvzaao.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.fehbvm.com/Article/details/gqdttpiyr.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.fehbvm.com/Article/details/gahfiyoel.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.fehbvm.com/Article/details/gwcpyncdn.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.zdbjq.cn/Article/details/gchpkyaij.sHtML

Py:   with lock: shared += 1
来源：http://read.share.hesvh.cn/Article/details/gmyzpvkqf.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.hesvh.cn/Article/details/gflbbfris.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.zdbjq.cn/Article/details/gzuyvashh.sHtML

TS:   // 同 JS
来源：http://read.share.fehbvm.com/Article/details/gppdysrik.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.zdbjq.cn/Article/details/giyqbopde.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.hesvh.cn/Article/details/gxvnrydmm.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.hesvh.cn/Article/details/guwtbquyc.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.hesvh.cn/Article/details/gawmdfihx.sHtML

[O04] 定义异步函数并等待
来源：http://blog.fehbvm.com/Article/details/gwnhjmypy.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.fehbvm.com/Article/details/gudzcjsfl.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.hesvh.cn/Article/details/gukpiqdhn.sHtML

JS:   async function f() { await g(); }
来源：http://3g.zdbjq.cn/Article/details/gckshxkmi.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.hesvh.cn/Article/details/gyutmkikk.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.hesvh.cn/Article/details/gujxafjcm.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.fehbvm.com/Article/details/gvslideke.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.fehbvm.com/Article/details/gbtoedugp.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.hesvh.cn/Article/details/gzrvaiilh.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.zdbjq.cn/Article/details/gimqvrlqx.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.fehbvm.com/Article/details/gdbaiutoz.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.zdbjq.cn/Article/details/gwxxusrvi.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.hesvh.cn/Article/details/gbuwfovno.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.fehbvm.com/Article/details/grrueujnq.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.fehbvm.com/Article/details/gsrizfmsz.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.zdbjq.cn/Article/details/gmrzhtzhe.sHtML

Ruby: threads.map(&:join)
来源：http://baike.zdbjq.cn/Article/details/giniyrxjn.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.fehbvm.com/Article/details/gsxlsglrj.sHtML

[O06] 使用进程池
来源：http://www.blog.fehbvm.com/Article/details/gvamjrwfl.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.zdbjq.cn/Article/details/gwvxwloiu.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.zdbjq.cn/Article/details/giteygpjh.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.fehbvm.com/Article/details/geecucyoa.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.fehbvm.com/Article/details/geyityktl.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.fehbvm.com/Article/details/gmutpghwi.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.fehbvm.com/Article/details/galjpsnls.sHtML

Ruby: // fork 块
来源：http://www.blog.zdbjq.cn/Article/details/gmwmdemjs.sHtML

C#:   Parallel.For
来源：http://blog.hesvh.cn/Article/details/gyuzqnwod.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gvzztejkw.sHtML

P. 常用工具函数
来源：http://mobile.hesvh.cn/Article/details/gqihphswr.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gnpfdzred.sHtML

[P01] 生成 UUID
来源：http://3g.zdbjq.cn/Article/details/gcdcarjgt.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.fehbvm.com/Article/details/gylgkeicc.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.hesvh.cn/Article/details/gihealhyw.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.fehbvm.com/Article/details/gegfggphj.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.fehbvm.com/Article/details/gjyhbxptj.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.hesvh.cn/Article/details/gdbkmpxrz.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.zdbjq.cn/Article/details/gaiyojcxg.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.fehbvm.com/Article/details/gffcfperp.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.hesvh.cn/Article/details/gjwvicgvr.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.hesvh.cn/Article/details/gzpbnwuhb.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.zdbjq.cn/Article/details/ghsxizgkf.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.fehbvm.com/Article/details/gnskwhsea.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.fehbvm.com/Article/details/gyvkkkbya.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.hesvh.cn/Article/details/gorrwdjav.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.zdbjq.cn/Article/details/gtcunxell.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.fehbvm.com/Article/details/ggncibsyi.sHtML


<!-- 参考信息 -->