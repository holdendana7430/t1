代发 wailian999

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.zdbjq.cn/Article/details/gsecrnoej.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.fehbvm.com/Article/details/gprpuyaah.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.hesvh.cn/Article/details/gphmhxvby.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.hesvh.cn/Article/details/gzgcvqzco.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.hesvh.cn/Article/details/gzgznrdbm.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.zdbjq.cn/Article/details/gtsnezbfu.sHtML

[L05] 上传文件（multipart）
来源：http://baike.hesvh.cn/Article/details/gduvjdyur.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://read.share.fehbvm.com/Article/details/gdzgymbez.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.fehbvm.com/Article/details/gwfldmpzj.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.fehbvm.com/Article/details/gxacoqtru.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.zdbjq.cn/Article/details/gimofvygv.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.hesvh.cn/Article/details/gvaifjadw.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.fehbvm.com/Article/details/gfyiecxtt.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.zdbjq.cn/Article/details/gtjwbigdw.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.fehbvm.com/Article/details/grbvbhqvm.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.zdbjq.cn/Article/details/gilzplmvt.sHtML

Py:   resp.json()
来源：http://wap.hesvh.cn/Article/details/gpsnoiypm.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.zdbjq.cn/Article/details/gmdckdznn.sHtML

JS:   await resp.json()
来源：http://blog.fehbvm.com/Article/details/gllgfmkid.sHtML

TS:   await resp.json()
来源：http://m.share.fehbvm.com/Article/details/gpgvfwjyl.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.hesvh.cn/Article/details/gacohwory.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.zdbjq.cn/Article/details/gxfmlepwi.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.fehbvm.com/Article/details/gviomijqi.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.zdbjq.cn/Article/details/gbkdoayte.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.hesvh.cn/Article/details/godgdcdrx.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.hesvh.cn/Article/details/gitrkgfrs.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.fehbvm.com/Article/details/gtunjtbuh.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.fehbvm.com/Article/details/goiniomcd.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.hesvh.cn/Article/details/gkgkzabkg.sHtML

Java: resp.statusCode()
来源：http://mobile.hesvh.cn/Article/details/gxfusdqqb.sHtML

Go:   resp.StatusCode
来源：http://www.share.hesvh.cn/Article/details/gzaizwtzm.sHtML

Ruby: resp.code.to_i
来源：http://m.share.hesvh.cn/Article/details/goubkxvup.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.zdbjq.cn/Article/details/geplsjgdd.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.fehbvm.com/Article/details/gessyvmnf.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.fehbvm.com/Article/details/gdlaacims.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.hesvh.cn/Article/details/gwcamvgcs.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.hesvh.cn/Article/details/gzjbqjsvq.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.hesvh.cn/Article/details/gvypqvhcs.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.fehbvm.com/Article/details/gzhljkrfh.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.hesvh.cn/Article/details/gudgrftkc.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.zdbjq.cn/Article/details/gbevnbwae.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.fehbvm.com/Article/details/gebhbwxyc.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gfnfldhdu.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.zdbjq.cn/Article/details/gujwtrxri.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gknqstvks.sHtML

[M01] 读取命令行参数
来源：http://3g.fehbvm.com/Article/details/ghnrbmzae.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.fehbvm.com/Article/details/gbipgxwbx.sHtML

PHP:  $argv;  $argc;
来源：http://baike.zdbjq.cn/Article/details/gtwxgacni.sHtML

JS:   process.argv.slice(2)
来源：http://3g.zdbjq.cn/Article/details/gvwoalkbx.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.zdbjq.cn/Article/details/gnlpqwjwg.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.zdbjq.cn/Article/details/gonyzewek.sHtML

Go:   os.Args[1:]
来源：http://mobile.zdbjq.cn/Article/details/gjtnvdqfu.sHtML

Ruby: ARGV
来源：http://3g.fehbvm.com/Article/details/glxnzhadj.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.zdbjq.cn/Article/details/ghrvfwpsj.sHtML

[M02] 读取环境变量
来源：http://blog.zdbjq.cn/Article/details/gjrncctsh.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.zdbjq.cn/Article/details/gxwdupeym.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.fehbvm.com/Article/details/gjjahlxek.sHtML

JS:   process.env.HOME
来源：http://www.blog.fehbvm.com/Article/details/gorijbzlt.sHtML

TS:   process.env.HOME
来源：http://wap.hesvh.cn/Article/details/gbntdpcxh.sHtML

Java: System.getenv("HOME")
来源：http://3g.hesvh.cn/Article/details/gxdyaewkl.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.zdbjq.cn/Article/details/gweulnfsl.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.hesvh.cn/Article/details/gtqcbrznt.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.fehbvm.com/Article/details/gxomgtkwh.sHtML

[M03] 执行外部命令
来源：http://read.share.hesvh.cn/Article/details/gvpmiyjcj.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.hesvh.cn/Article/details/gewlppvse.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.hesvh.cn/Article/details/gkagqmmts.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.zdbjq.cn/Article/details/glrrzgtmr.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.hesvh.cn/Article/details/gahebhjyv.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.zdbjq.cn/Article/details/gbbeljoti.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.fehbvm.com/Article/details/guxkkizpj.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.hesvh.cn/Article/details/gzezudhny.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.fehbvm.com/Article/details/grcsgcpme.sHtML

[M04] 获取当前工作目录
来源：http://wap.hesvh.cn/Article/details/gvbrvwiax.sHtML

Py:   os.getcwd()
来源：http://read.share.zdbjq.cn/Article/details/ghssfcltq.sHtML

PHP:  getcwd();
来源：http://3g.hesvh.cn/Article/details/goqklwfuw.sHtML

JS:   process.cwd()
来源：http://read.share.fehbvm.com/Article/details/gwnmdfxpw.sHtML

TS:   process.cwd()
来源：http://baike.fehbvm.com/Article/details/gijzobctc.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.zdbjq.cn/Article/details/gnfebphna.sHtML

Go:   os.Getwd()
来源：http://blog.fehbvm.com/Article/details/godfwllkl.sHtML

Ruby: Dir.pwd
来源：http://www.share.zdbjq.cn/Article/details/gsswigspq.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.hesvh.cn/Article/details/gylbmmdwr.sHtML

[M05] 设置退出码
来源：http://www.m.share.hesvh.cn/Article/details/gnlkoliuu.sHtML

Py:   sys.exit(1)
来源：http://www.share.hesvh.cn/Article/details/gppxycdzn.sHtML

PHP:  exit(1);
来源：http://blog.zdbjq.cn/Article/details/geafkghui.sHtML

JS:   process.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/girhhejcy.sHtML

TS:   process.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gmycislcv.sHtML

Java: System.exit(1)
来源：http://3g.fehbvm.com/Article/details/gglrcbtmr.sHtML

Go:   os.Exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gsjgepyuf.sHtML

Ruby: exit 1
来源：http://m.share.zdbjq.cn/Article/details/gxbhqeyse.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.hesvh.cn/Article/details/ghtikhhli.sHtML

[M06] 向标准错误输出
来源：http://read.share.fehbvm.com/Article/details/gyhiyvdbz.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.fehbvm.com/Article/details/ginjhtysr.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.zdbjq.cn/Article/details/gpbvnzxfc.sHtML

JS:   console.error("err")
来源：http://m.share.hesvh.cn/Article/details/gufpxoqsp.sHtML

TS:   console.error("err")
来源：http://blog.fehbvm.com/Article/details/gdaczocrs.sHtML

Java: System.err.println("err")
来源：http://blog.hesvh.cn/Article/details/gfgahvxot.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.zdbjq.cn/Article/details/gjiblhmah.sHtML

Ruby: warn "err"
来源：http://3g.hesvh.cn/Article/details/gohianupx.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.fehbvm.com/Article/details/gqmsikxpr.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.fehbvm.com/Article/details/gzzaqvmzf.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.fehbvm.com/Article/details/goijoisyd.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.fehbvm.com/Article/details/gtcoktmiv.sHtML

JS:   require.main === module
来源：http://read.share.zdbjq.cn/Article/details/gxcndcdby.sHtML

TS:   require.main === module
来源：http://read.share.hesvh.cn/Article/details/ggptxlpla.sHtML

Java: public static void main(String[] args)
来源：http://mobile.fehbvm.com/Article/details/ggtuknxvb.sHtML

Go:   func main()
来源：http://m.share.hesvh.cn/Article/details/gqejlqzxu.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.hesvh.cn/Article/details/goewxboni.sHtML

C#:   static void Main(string[] args)
来源：http://blog.zdbjq.cn/Article/details/gxnoahkui.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.hesvh.cn/Article/details/gekcwmatk.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.zdbjq.cn/Article/details/ggttrstqc.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.hesvh.cn/Article/details/gcjuhqkmp.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.fehbvm.com/Article/details/gfsstkkql.sHtML

TS:   process.platform;  process.version
来源：http://mobile.fehbvm.com/Article/details/ganqonpzv.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.zdbjq.cn/Article/details/gdyzznlag.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.zdbjq.cn/Article/details/gnqvqmdnf.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.zdbjq.cn/Article/details/gdvmlvolq.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.fehbvm.com/Article/details/gpczmhugu.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/golvxokxg.sHtML

N. 数据结构与算法
来源：http://mobile.fehbvm.com/Article/details/gcgqthbsn.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gomahsdgz.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.zdbjq.cn/Article/details/grxnslgxx.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gfotumsqi.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.fehbvm.com/Article/details/gxtkogpic.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.fehbvm.com/Article/details/gzxdnmnjj.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.hesvh.cn/Article/details/gtbjrjjnw.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.zdbjq.cn/Article/details/ggllfybzf.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gjakhxxpr.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.hesvh.cn/Article/details/guqvkjpcb.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.fehbvm.com/Article/details/gpxodalve.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.zdbjq.cn/Article/details/gpblukbzx.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.zdbjq.cn/Article/details/gofsqwrzu.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.hesvh.cn/Article/details/gzbthraol.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.zdbjq.cn/Article/details/gssvaripg.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.zdbjq.cn/Article/details/gauuqlygx.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.zdbjq.cn/Article/details/gkrreokox.sHtML

Go:   slices.Sort(arr)
来源：http://wap.hesvh.cn/Article/details/gijnhduxf.sHtML

Ruby: arr.sort
来源：http://3g.zdbjq.cn/Article/details/govnvvghi.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.zdbjq.cn/Article/details/gbyeuufap.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.zdbjq.cn/Article/details/gslvuogti.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.fehbvm.com/Article/details/gccjcidlq.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.fehbvm.com/Article/details/gekwlqbxj.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.zdbjq.cn/Article/details/grvokqaha.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.zdbjq.cn/Article/details/gujlpwhla.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.fehbvm.com/Article/details/gzhpmscza.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.hesvh.cn/Article/details/gwabalfls.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.fehbvm.com/Article/details/gkijikiao.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.fehbvm.com/Article/details/gaffzncke.sHtML

[N04] 斐波那契数列
来源：http://wap.hesvh.cn/Article/details/gfjkmqybn.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.zdbjq.cn/Article/details/glqgmnufi.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.hesvh.cn/Article/details/goaredcya.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/glutesiwp.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.zdbjq.cn/Article/details/gsiqqwwmp.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.hesvh.cn/Article/details/gzvytnvdl.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.zdbjq.cn/Article/details/gjoxgtfuq.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.fehbvm.com/Article/details/ggwqaezmp.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.hesvh.cn/Article/details/ghkxtgreh.sHtML

[N05] 最大公约数
来源：http://mobile.zdbjq.cn/Article/details/ghsswrpri.sHtML

Py:   math.gcd(a, b)
来源：http://blog.hesvh.cn/Article/details/gnzlwrxvh.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.hesvh.cn/Article/details/gvpbhwehi.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.fehbvm.com/Article/details/gggrbuvri.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.fehbvm.com/Article/details/gkvphpfrv.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.fehbvm.com/Article/details/gxafamkem.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.hesvh.cn/Article/details/gjiqqdcwv.sHtML

Ruby: a.gcd(b)
来源：http://wap.zdbjq.cn/Article/details/gzkgvninh.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.fehbvm.com/Article/details/gkqrocery.sHtML

[N06] 判断回文字符串
来源：http://www.share.fehbvm.com/Article/details/gmzdnnsss.sHtML

Py:   s == s[::-1]
来源：http://m.share.hesvh.cn/Article/details/gxwaxofkw.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.hesvh.cn/Article/details/gphjkcdaw.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/gknqfeclw.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/ghtcpjzgt.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.zdbjq.cn/Article/details/gtftqpaqv.sHtML

Go:   // 双指针从两端比较
来源：http://baike.zdbjq.cn/Article/details/gkrxyurym.sHtML

Ruby: s == s.reverse
来源：http://3g.zdbjq.cn/Article/details/gscjykgsf.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.zdbjq.cn/Article/details/grbqivvjv.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.fehbvm.com/Article/details/gnzaakipk.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.hesvh.cn/Article/details/gmufoxcnq.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.hesvh.cn/Article/details/gcrrlpdhq.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.hesvh.cn/Article/details/gxbihijqt.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.fehbvm.com/Article/details/gnnluckwk.sHtML

Java: // 手写 HashMap
来源：http://3g.fehbvm.com/Article/details/gykarotup.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.fehbvm.com/Article/details/gbdhoqjdn.sHtML

Ruby: // 手写 Hash
来源：http://m.share.fehbvm.com/Article/details/gydoduxhs.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.fehbvm.com/Article/details/gurlqnlkc.sHtML

[N08] 生成全排列
来源：http://3g.zdbjq.cn/Article/details/gipiakicb.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.hesvh.cn/Article/details/glbmawlmp.sHtML

PHP:  // 手写递归交换
来源：http://m.share.zdbjq.cn/Article/details/gwwhpybgq.sHtML

JS:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gybgofmbl.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gnnehztdf.sHtML

Java: // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gzbvbfryb.sHtML

Go:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/giwfriqsz.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.hesvh.cn/Article/details/gqaiascaa.sHtML

C#:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gudpebjts.sHtML

[N09] 栈与队列
来源：http://www.blog.fehbvm.com/Article/details/ggkqfhzly.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.zdbjq.cn/Article/details/grazwsghb.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.fehbvm.com/Article/details/ghmttkbhh.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.hesvh.cn/Article/details/gtsidutqw.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.hesvh.cn/Article/details/gggbwgfsf.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.zdbjq.cn/Article/details/gyhroqkxy.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.hesvh.cn/Article/details/gtknccpcl.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.hesvh.cn/Article/details/guczjwrlq.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.fehbvm.com/Article/details/gaidybdxw.sHtML

[N10] 链表节点定义
来源：http://www.blog.zdbjq.cn/Article/details/gximfssgd.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.fehbvm.com/Article/details/gkzoavktx.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.zdbjq.cn/Article/details/gsiuwjnuf.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.hesvh.cn/Article/details/gbfklhlyt.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.zdbjq.cn/Article/details/gamfpnuks.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.hesvh.cn/Article/details/gaiulejuv.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.zdbjq.cn/Article/details/gmjgconyl.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.hesvh.cn/Article/details/gdtfooicq.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.fehbvm.com/Article/details/gczkcdylh.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.fehbvm.com/Article/details/ggfvorqjf.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.hesvh.cn/Article/details/gxdhyddsh.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.hesvh.cn/Article/details/gbpkadcjm.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.fehbvm.com/Article/details/giroibxkk.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.zdbjq.cn/Article/details/gbqderruv.sHtML

Java: // 手写递归
来源：http://www.blog.zdbjq.cn/Article/details/gxopnbrux.sHtML

Go:   // 手写递归
来源：http://blog.zdbjq.cn/Article/details/grtcbzgti.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.fehbvm.com/Article/details/gjlkoxxfi.sHtML

C#:   // 手写递归
来源：http://baike.hesvh.cn/Article/details/gucydsruh.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.zdbjq.cn/Article/details/gvgnnogew.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.hesvh.cn/Article/details/gdrlvmjgz.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.hesvh.cn/Article/details/gujrfxlgd.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.hesvh.cn/Article/details/gjcyhscja.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.fehbvm.com/Article/details/gmqayxwhj.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.fehbvm.com/Article/details/gsolavoom.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.fehbvm.com/Article/details/gxeehtxjv.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.zdbjq.cn/Article/details/gbpkfzxck.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.zdbjq.cn/Article/details/gfaburdph.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gzqyvvpld.sHtML

O. 并发与异步
来源：http://www.m.share.fehbvm.com/Article/details/gzsijzxza.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gsvlzxymg.sHtML

[O01] 启动一个线程
来源：http://blog.zdbjq.cn/Article/details/gxylwgcta.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.hesvh.cn/Article/details/ggjcspcgz.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.hesvh.cn/Article/details/gbckjbkyz.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.hesvh.cn/Article/details/gvqmcfafc.sHtML

TS:   // 同 JS
来源：http://read.share.fehbvm.com/Article/details/gcbxzysmd.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.fehbvm.com/Article/details/gxozjqcgb.sHtML

Go:   go f()
来源：http://m.share.hesvh.cn/Article/details/gfnuncxfx.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.fehbvm.com/Article/details/gasajjrxa.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.zdbjq.cn/Article/details/gbgtiqtlf.sHtML

[O02] 使用线程池
来源：http://www.share.fehbvm.com/Article/details/gibojkcxn.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.zdbjq.cn/Article/details/gucvaidqx.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.fehbvm.com/Article/details/gsgcfepza.sHtML

JS:   // worker_threads 线程池
来源：http://wap.fehbvm.com/Article/details/gdkxwppry.sHtML

TS:   // worker_threads 线程池
来源：http://baike.zdbjq.cn/Article/details/gmpyijsvr.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.fehbvm.com/Article/details/gmpohdgwl.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.zdbjq.cn/Article/details/grrvkerat.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.fehbvm.com/Article/details/gsplewxxw.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.hesvh.cn/Article/details/gotnobeur.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.hesvh.cn/Article/details/gmlscqyvp.sHtML

Py:   with lock: shared += 1
来源：http://3g.fehbvm.com/Article/details/gzyyzegvo.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.fehbvm.com/Article/details/gwkhapeid.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.hesvh.cn/Article/details/gpdlnffin.sHtML

TS:   // 同 JS
来源：http://3g.zdbjq.cn/Article/details/genjihfdf.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.zdbjq.cn/Article/details/gekdetjwi.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.zdbjq.cn/Article/details/gspolsvjr.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.fehbvm.com/Article/details/gmevarodq.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.hesvh.cn/Article/details/gbccxnezq.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.hesvh.cn/Article/details/gwqxjyjax.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.zdbjq.cn/Article/details/gffehgaad.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.hesvh.cn/Article/details/gqgtvikyr.sHtML

JS:   async function f() { await g(); }
来源：http://baike.fehbvm.com/Article/details/geauiztwe.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.fehbvm.com/Article/details/gponhhgkl.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.hesvh.cn/Article/details/gueodsjmj.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.fehbvm.com/Article/details/gjfuirzzm.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.hesvh.cn/Article/details/giqblegot.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.fehbvm.com/Article/details/gxwsduczi.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.hesvh.cn/Article/details/gnsnuizny.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.fehbvm.com/Article/details/gmvnbydaw.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.hesvh.cn/Article/details/gevolyjgh.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.zdbjq.cn/Article/details/gfdpndjvs.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.hesvh.cn/Article/details/guoezqtee.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.zdbjq.cn/Article/details/goybrudcd.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.hesvh.cn/Article/details/gjabtstcj.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.hesvh.cn/Article/details/gvdhaqslp.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.hesvh.cn/Article/details/gogkhihzr.sHtML

[O06] 使用进程池
来源：http://m.share.zdbjq.cn/Article/details/gnqdzhkxd.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.zdbjq.cn/Article/details/gotemmsjq.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.hesvh.cn/Article/details/gydvnrhhp.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.fehbvm.com/Article/details/gopigfhwy.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.zdbjq.cn/Article/details/glqlzmdpg.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.hesvh.cn/Article/details/gysmaphkb.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.fehbvm.com/Article/details/giqyqvsou.sHtML

Ruby: // fork 块
来源：http://blog.hesvh.cn/Article/details/gkqobolnk.sHtML

C#:   Parallel.For
来源：http://www.blog.hesvh.cn/Article/details/gnpmuxbvl.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/geldovcfo.sHtML

P. 常用工具函数
来源：http://read.share.hesvh.cn/Article/details/glwqvznsc.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/geiqdqxib.sHtML

[P01] 生成 UUID
来源：http://mobile.fehbvm.com/Article/details/ggpwvkwaf.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.zdbjq.cn/Article/details/gzjvrqtea.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.hesvh.cn/Article/details/gmnkwkjrw.sHtML

JS:   crypto.randomUUID()
来源：http://3g.zdbjq.cn/Article/details/guwcuibav.sHtML

TS:   crypto.randomUUID()
来源：http://blog.zdbjq.cn/Article/details/gjyzdrltw.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.fehbvm.com/Article/details/gttpgumvl.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.hesvh.cn/Article/details/glfoiasjn.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.fehbvm.com/Article/details/gxuceelbt.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.hesvh.cn/Article/details/gctebxkpf.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.hesvh.cn/Article/details/gshkxlotq.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.fehbvm.com/Article/details/geyoxrsqa.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.hesvh.cn/Article/details/gioetkjvr.sHtML


<!-- 参考信息 -->