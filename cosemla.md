代发 wailian999

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.zdbjq.cn/Article/details/gtsfrfrlg.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.fehbvm.com/Article/details/ggtlmfhzn.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.hesvh.cn/Article/details/gphtobran.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.hesvh.cn/Article/details/gtkbuenmf.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.hesvh.cn/Article/details/gofbdnryf.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.blog.hesvh.cn/Article/details/gporthjyt.sHtML

[L05] 上传文件（multipart）
来源：http://wap.zdbjq.cn/Article/details/giuktlvpw.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.hesvh.cn/Article/details/gjgcmwksg.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.fehbvm.com/Article/details/gpvjjkbko.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.zdbjq.cn/Article/details/gkjxipymd.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.fehbvm.com/Article/details/gyyecpeqo.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.fehbvm.com/Article/details/gprbukxbs.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.fehbvm.com/Article/details/gxnknevnf.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.hesvh.cn/Article/details/gmevgpizn.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.fehbvm.com/Article/details/gqvwogvds.sHtML

[L06] 解析响应为 JSON
来源：http://wap.zdbjq.cn/Article/details/ghffwzgpv.sHtML

Py:   resp.json()
来源：http://www.blog.fehbvm.com/Article/details/gerkfkjdb.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.fehbvm.com/Article/details/gjircbwch.sHtML

JS:   await resp.json()
来源：http://3g.hesvh.cn/Article/details/gqbvncfgn.sHtML

TS:   await resp.json()
来源：http://mobile.fehbvm.com/Article/details/goicfpawb.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.hesvh.cn/Article/details/gfzgummal.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.fehbvm.com/Article/details/gqdwddjks.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.zdbjq.cn/Article/details/gcbnppamy.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.fehbvm.com/Article/details/gxycdvspd.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.zdbjq.cn/Article/details/gafnrlvma.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.zdbjq.cn/Article/details/gogbzdgyx.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.hesvh.cn/Article/details/gonlolzvl.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.fehbvm.com/Article/details/gcetuuyxf.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.fehbvm.com/Article/details/gvqnkeqzo.sHtML

Java: resp.statusCode()
来源：http://www.blog.hesvh.cn/Article/details/giqbgchmp.sHtML

Go:   resp.StatusCode
来源：http://www.share.fehbvm.com/Article/details/gekiadkms.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.hesvh.cn/Article/details/gjlnelhns.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.zdbjq.cn/Article/details/gmnppguhd.sHtML

[L08] 并发请求多个地址
来源：http://blog.fehbvm.com/Article/details/gwqepziwo.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.hesvh.cn/Article/details/greprkewr.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.zdbjq.cn/Article/details/gsdbxuirw.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.hesvh.cn/Article/details/gprixpiwi.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fehbvm.com/Article/details/gunkiudhz.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.hesvh.cn/Article/details/gxzihtdwn.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.fehbvm.com/Article/details/gbrxsgeoo.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.zdbjq.cn/Article/details/gpqxtwcrc.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.fehbvm.com/Article/details/gavxbdouy.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gmlnzhpsi.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.zdbjq.cn/Article/details/ggufzsout.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gobxdxlqk.sHtML

[M01] 读取命令行参数
来源：http://blog.zdbjq.cn/Article/details/ghmovuzqo.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.zdbjq.cn/Article/details/gefyinljb.sHtML

PHP:  $argv;  $argc;
来源：http://3g.fehbvm.com/Article/details/gicmnprup.sHtML

JS:   process.argv.slice(2)
来源：http://blog.zdbjq.cn/Article/details/grfxrkojc.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.zdbjq.cn/Article/details/grvqaddff.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.hesvh.cn/Article/details/gswbiqwvr.sHtML

Go:   os.Args[1:]
来源：http://m.share.zdbjq.cn/Article/details/guqplkvtq.sHtML

Ruby: ARGV
来源：http://blog.zdbjq.cn/Article/details/gughgxatl.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.fehbvm.com/Article/details/gpfhxtzqu.sHtML

[M02] 读取环境变量
来源：http://read.share.hesvh.cn/Article/details/gevvtgerj.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.hesvh.cn/Article/details/ghmfgiorw.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.fehbvm.com/Article/details/gfuelzhab.sHtML

JS:   process.env.HOME
来源：http://www.blog.fehbvm.com/Article/details/gotuceymj.sHtML

TS:   process.env.HOME
来源：http://www.blog.zdbjq.cn/Article/details/gixmcaemz.sHtML

Java: System.getenv("HOME")
来源：http://mobile.hesvh.cn/Article/details/gvgseiwdu.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.zdbjq.cn/Article/details/gpfeibfvi.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.hesvh.cn/Article/details/grvsquami.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.zdbjq.cn/Article/details/gyhqahdsx.sHtML

[M03] 执行外部命令
来源：http://3g.hesvh.cn/Article/details/gtauvkiue.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.zdbjq.cn/Article/details/gpzeqzgyl.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.fehbvm.com/Article/details/ghyetdxnc.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.zdbjq.cn/Article/details/ghbpzduki.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.fehbvm.com/Article/details/gvsxjfnta.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.fehbvm.com/Article/details/gjoklmpjl.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.hesvh.cn/Article/details/gonansjar.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.fehbvm.com/Article/details/gosqoaptt.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.zdbjq.cn/Article/details/ghkpbmmbd.sHtML

[M04] 获取当前工作目录
来源：http://www.share.fehbvm.com/Article/details/gqrdgjfqc.sHtML

Py:   os.getcwd()
来源：http://blog.hesvh.cn/Article/details/gaekgcfri.sHtML

PHP:  getcwd();
来源：http://blog.hesvh.cn/Article/details/ggzszlwrx.sHtML

JS:   process.cwd()
来源：http://3g.zdbjq.cn/Article/details/gsxxsxymy.sHtML

TS:   process.cwd()
来源：http://3g.fehbvm.com/Article/details/gllugyqna.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.fehbvm.com/Article/details/gwqcemhar.sHtML

Go:   os.Getwd()
来源：http://m.share.hesvh.cn/Article/details/gnoomxbuh.sHtML

Ruby: Dir.pwd
来源：http://m.share.hesvh.cn/Article/details/ggmsdxocb.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.zdbjq.cn/Article/details/gknndttvm.sHtML

[M05] 设置退出码
来源：http://www.blog.hesvh.cn/Article/details/gtdbophrj.sHtML

Py:   sys.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gopecyqci.sHtML

PHP:  exit(1);
来源：http://www.blog.zdbjq.cn/Article/details/gpdgvcpew.sHtML

JS:   process.exit(1)
来源：http://baike.hesvh.cn/Article/details/gujkagutn.sHtML

TS:   process.exit(1)
来源：http://read.share.hesvh.cn/Article/details/ggjawizva.sHtML

Java: System.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gltexoall.sHtML

Go:   os.Exit(1)
来源：http://m.share.hesvh.cn/Article/details/gvwejifag.sHtML

Ruby: exit 1
来源：http://www.share.hesvh.cn/Article/details/gbgwwmvag.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.zdbjq.cn/Article/details/gaaifvtjt.sHtML

[M06] 向标准错误输出
来源：http://read.share.fehbvm.com/Article/details/ghiiidfwz.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.hesvh.cn/Article/details/gnwoazbtr.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.zdbjq.cn/Article/details/guocttumr.sHtML

JS:   console.error("err")
来源：http://blog.zdbjq.cn/Article/details/gtdulsojq.sHtML

TS:   console.error("err")
来源：http://read.share.hesvh.cn/Article/details/gsqkztecl.sHtML

Java: System.err.println("err")
来源：http://blog.hesvh.cn/Article/details/gsalawhvb.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.fehbvm.com/Article/details/grvgpgwdr.sHtML

Ruby: warn "err"
来源：http://m.share.zdbjq.cn/Article/details/gmcbxtkjr.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.zdbjq.cn/Article/details/gdwbbbbgp.sHtML

[M07] 判断是否为主入口
来源：http://www.share.zdbjq.cn/Article/details/gbudroncy.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.fehbvm.com/Article/details/glhlxtfds.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.hesvh.cn/Article/details/gbqcfetiy.sHtML

JS:   require.main === module
来源：http://baike.fehbvm.com/Article/details/gfrbciyji.sHtML

TS:   require.main === module
来源：http://www.m.share.fehbvm.com/Article/details/gmrripxlf.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.zdbjq.cn/Article/details/grllhrwhi.sHtML

Go:   func main()
来源：http://m.share.fehbvm.com/Article/details/gwiriapay.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.zdbjq.cn/Article/details/gvugfhtya.sHtML

C#:   static void Main(string[] args)
来源：http://3g.zdbjq.cn/Article/details/gyawxfbfg.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.hesvh.cn/Article/details/gxoyxalez.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.fehbvm.com/Article/details/ghooggnao.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.hesvh.cn/Article/details/givnznizb.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.hesvh.cn/Article/details/gizylhjzl.sHtML

TS:   process.platform;  process.version
来源：http://blog.fehbvm.com/Article/details/griqudvra.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.fehbvm.com/Article/details/grlumogpb.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.fehbvm.com/Article/details/gphyvpjvy.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.zdbjq.cn/Article/details/gimhmwyjz.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.zdbjq.cn/Article/details/gklmqxras.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gsrkdgetv.sHtML

N. 数据结构与算法
来源：http://www.blog.fehbvm.com/Article/details/gdsdrftkf.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/ggceinqix.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.fehbvm.com/Article/details/grdzbrwgy.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gdptglfpc.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.fehbvm.com/Article/details/gezpinmbu.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.hesvh.cn/Article/details/gusysptcz.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.zdbjq.cn/Article/details/grxfjyjxq.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.fehbvm.com/Article/details/gwxssytmt.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.fehbvm.com/Article/details/gjlsljdpg.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.fehbvm.com/Article/details/gsnmowhrm.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gvsoyreef.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.zdbjq.cn/Article/details/gbgmrdrrg.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.zdbjq.cn/Article/details/gbdjvtddg.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.hesvh.cn/Article/details/gkqytnnul.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.fehbvm.com/Article/details/gvoiqyjpj.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.fehbvm.com/Article/details/gqjffkfkk.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.fehbvm.com/Article/details/gmfwreudu.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.hesvh.cn/Article/details/gkiwirbgz.sHtML

Ruby: arr.sort
来源：http://blog.hesvh.cn/Article/details/gmgotjwfo.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.hesvh.cn/Article/details/ggxjtzbze.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.zdbjq.cn/Article/details/grxgpkdrk.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.fehbvm.com/Article/details/gghzxmzuo.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.fehbvm.com/Article/details/gwzaxaflu.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.fehbvm.com/Article/details/gllsnvuec.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.zdbjq.cn/Article/details/grcikvquv.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.fehbvm.com/Article/details/gvszayrle.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.fehbvm.com/Article/details/gkriwqmxp.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.hesvh.cn/Article/details/gyjqbqgpn.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.fehbvm.com/Article/details/gnqhfefwt.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.hesvh.cn/Article/details/gabqncdkk.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.hesvh.cn/Article/details/gnxcgnihj.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.fehbvm.com/Article/details/gsqfmhdmi.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/gccpklloj.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.fehbvm.com/Article/details/gorshabyb.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.hesvh.cn/Article/details/gcrwdjuwi.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.zdbjq.cn/Article/details/gfzuiegmo.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.fehbvm.com/Article/details/gwplchbgh.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.zdbjq.cn/Article/details/gbtoumaej.sHtML

[N05] 最大公约数
来源：http://www.m.share.zdbjq.cn/Article/details/gscxgjxdd.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.fehbvm.com/Article/details/gcahqvxlr.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.zdbjq.cn/Article/details/ghnvoyqpb.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.hesvh.cn/Article/details/ghwqlgezn.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.fehbvm.com/Article/details/gydeihntc.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.fehbvm.com/Article/details/gvqwercsm.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.zdbjq.cn/Article/details/ghxysogcw.sHtML

Ruby: a.gcd(b)
来源：http://read.share.fehbvm.com/Article/details/ggxsmtxga.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.zdbjq.cn/Article/details/gncqlqrmz.sHtML

[N06] 判断回文字符串
来源：http://mobile.fehbvm.com/Article/details/gtlvztiil.sHtML

Py:   s == s[::-1]
来源：http://wap.hesvh.cn/Article/details/gcdjuhpkf.sHtML

PHP:  $s === strrev($s);
来源：http://baike.fehbvm.com/Article/details/gjlytpcnk.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/gwddgyvqh.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/gnusyzesm.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.fehbvm.com/Article/details/gjpwxnrvn.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.zdbjq.cn/Article/details/gnxbqavjx.sHtML

Ruby: s == s.reverse
来源：http://mobile.fehbvm.com/Article/details/gdwfukcaj.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.hesvh.cn/Article/details/gbiipugrw.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.fehbvm.com/Article/details/gydeppvlu.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.fehbvm.com/Article/details/gaoojvtnt.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.zdbjq.cn/Article/details/gennkestr.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.zdbjq.cn/Article/details/gcxgzicvp.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.zdbjq.cn/Article/details/gwglgbmny.sHtML

Java: // 手写 HashMap
来源：http://wap.hesvh.cn/Article/details/gzdwbleup.sHtML

Go:   // 手写 map[int]int
来源：http://wap.hesvh.cn/Article/details/glkasvzoc.sHtML

Ruby: // 手写 Hash
来源：http://3g.fehbvm.com/Article/details/gkepirgiq.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.zdbjq.cn/Article/details/gubvviypp.sHtML

[N08] 生成全排列
来源：http://www.m.share.zdbjq.cn/Article/details/gtryosime.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.zdbjq.cn/Article/details/gqqynmaam.sHtML

PHP:  // 手写递归交换
来源：http://baike.hesvh.cn/Article/details/gxbsvdorn.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/grzpmccmq.sHtML

TS:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gdbsrzzsm.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gqumhywsm.sHtML

Go:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gokftdsds.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.zdbjq.cn/Article/details/ghybmrdcw.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/ghqjxgapx.sHtML

[N09] 栈与队列
来源：http://baike.zdbjq.cn/Article/details/gnpceiufr.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.fehbvm.com/Article/details/gmbpegyki.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.fehbvm.com/Article/details/gzqwznzfa.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.zdbjq.cn/Article/details/gugmtsios.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.zdbjq.cn/Article/details/gfftzbevi.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.hesvh.cn/Article/details/gzqzteess.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.fehbvm.com/Article/details/goaunkdrx.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.hesvh.cn/Article/details/gtzlwqsgk.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.zdbjq.cn/Article/details/glmxfonkp.sHtML

[N10] 链表节点定义
来源：http://wap.hesvh.cn/Article/details/gvyhsdmnn.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.fehbvm.com/Article/details/gtedudpvu.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.fehbvm.com/Article/details/gubxmgead.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.hesvh.cn/Article/details/ggzqagisr.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.zdbjq.cn/Article/details/gxjavnycy.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.zdbjq.cn/Article/details/gnoihjktt.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.hesvh.cn/Article/details/gmpxbfqcj.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.hesvh.cn/Article/details/gyeojcnqz.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.hesvh.cn/Article/details/gnoixeubg.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.hesvh.cn/Article/details/gpqhvlsnp.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.fehbvm.com/Article/details/glnwlmkmq.sHtML

PHP:  // 手写递归函数
来源：http://baike.zdbjq.cn/Article/details/gugkgmgmo.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.zdbjq.cn/Article/details/ggqkculcc.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.hesvh.cn/Article/details/gmpnvjpam.sHtML

Java: // 手写递归
来源：http://www.share.zdbjq.cn/Article/details/gqewhmyab.sHtML

Go:   // 手写递归
来源：http://www.m.share.hesvh.cn/Article/details/gmopmeazs.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.hesvh.cn/Article/details/gnmkdtckk.sHtML

C#:   // 手写递归
来源：http://www.m.share.hesvh.cn/Article/details/glmwvqgim.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.hesvh.cn/Article/details/gsbrhrynp.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.fehbvm.com/Article/details/gfhyouoft.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.fehbvm.com/Article/details/gutarnies.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.fehbvm.com/Article/details/gmnwmxlab.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.zdbjq.cn/Article/details/gdthqzovu.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.fehbvm.com/Article/details/gmfpuoixi.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.fehbvm.com/Article/details/gohfnwisq.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.fehbvm.com/Article/details/gmzrsxaty.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.hesvh.cn/Article/details/gaptiwlpz.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gccglmrnh.sHtML

O. 并发与异步
来源：http://wap.hesvh.cn/Article/details/gcsgglmiy.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/geioynoqy.sHtML

[O01] 启动一个线程
来源：http://www.m.share.zdbjq.cn/Article/details/gmdpelcul.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.fehbvm.com/Article/details/gyvpulksw.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.fehbvm.com/Article/details/gfgohdhvb.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.hesvh.cn/Article/details/gorgdlwjm.sHtML

TS:   // 同 JS
来源：http://www.m.share.zdbjq.cn/Article/details/gpuitoymk.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.hesvh.cn/Article/details/gjvdciodo.sHtML

Go:   go f()
来源：http://mobile.hesvh.cn/Article/details/gadqnspdo.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.fehbvm.com/Article/details/gggusvucl.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.fehbvm.com/Article/details/gxspmzmbj.sHtML

[O02] 使用线程池
来源：http://wap.zdbjq.cn/Article/details/gzmcetbiw.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.zdbjq.cn/Article/details/gjpniuzhd.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.zdbjq.cn/Article/details/gzdlxkqnr.sHtML

JS:   // worker_threads 线程池
来源：http://baike.zdbjq.cn/Article/details/gqfvuzdop.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.fehbvm.com/Article/details/gwvxklvdu.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.zdbjq.cn/Article/details/gtsjuddud.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.hesvh.cn/Article/details/gpabswtxk.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.fehbvm.com/Article/details/gazafmzwp.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.zdbjq.cn/Article/details/gfyqaziou.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.zdbjq.cn/Article/details/gksuxhvle.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.hesvh.cn/Article/details/gudcyvdrf.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.fehbvm.com/Article/details/gsupneyjb.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.fehbvm.com/Article/details/gmtydayfl.sHtML

TS:   // 同 JS
来源：http://www.share.hesvh.cn/Article/details/ghgorylyt.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.fehbvm.com/Article/details/gtkgbdmdc.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.hesvh.cn/Article/details/gswpicude.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.fehbvm.com/Article/details/gvzuzvuxm.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.zdbjq.cn/Article/details/georptdor.sHtML

[O04] 定义异步函数并等待
来源：http://wap.fehbvm.com/Article/details/gxiuysojb.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.hesvh.cn/Article/details/generaemx.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.zdbjq.cn/Article/details/gpoqjqkhx.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.hesvh.cn/Article/details/guuzgytko.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.zdbjq.cn/Article/details/gzvuhjpky.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.hesvh.cn/Article/details/gosvrejpg.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.zdbjq.cn/Article/details/gqmqlcvml.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.fehbvm.com/Article/details/gcxxyvevy.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.fehbvm.com/Article/details/grshbnyiv.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.hesvh.cn/Article/details/gqinnpaum.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.zdbjq.cn/Article/details/gfmeivbhq.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.hesvh.cn/Article/details/gskeqwebk.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.zdbjq.cn/Article/details/gsgngagrj.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.fehbvm.com/Article/details/gvzvdgwbm.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.hesvh.cn/Article/details/ghtjhpnbk.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.hesvh.cn/Article/details/gmeavixtm.sHtML

Ruby: threads.map(&:join)
来源：http://wap.hesvh.cn/Article/details/ggzxzxjeo.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.hesvh.cn/Article/details/gwagkozyr.sHtML

[O06] 使用进程池
来源：http://m.share.fehbvm.com/Article/details/gpfrnmtlq.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.fehbvm.com/Article/details/gkjchambf.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.zdbjq.cn/Article/details/gmhbjkphm.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.zdbjq.cn/Article/details/grkmxgzeu.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.fehbvm.com/Article/details/gtrcgmoms.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.fehbvm.com/Article/details/gadpjnwcp.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.hesvh.cn/Article/details/guytuncoc.sHtML

Ruby: // fork 块
来源：http://www.blog.fehbvm.com/Article/details/gbgrbyywr.sHtML

C#:   Parallel.For
来源：http://www.m.share.zdbjq.cn/Article/details/gaqsvdwfm.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gfzppvsfd.sHtML

P. 常用工具函数
来源：http://baike.hesvh.cn/Article/details/gxlavakny.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gqctnmrku.sHtML

[P01] 生成 UUID
来源：http://www.m.share.hesvh.cn/Article/details/gcqizfabs.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.hesvh.cn/Article/details/graquvagd.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.hesvh.cn/Article/details/gtfnjvuvf.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.fehbvm.com/Article/details/gspyramvl.sHtML

TS:   crypto.randomUUID()
来源：http://wap.zdbjq.cn/Article/details/gymtdpcjl.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.zdbjq.cn/Article/details/guvmrpbmx.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.zdbjq.cn/Article/details/gagapkwsy.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.fehbvm.com/Article/details/gxupvdbae.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.hesvh.cn/Article/details/gcfpdjudp.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.hesvh.cn/Article/details/gpililvil.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.hesvh.cn/Article/details/gpypnizzu.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.zdbjq.cn/Article/details/gyxzllfgx.sHtML


<!-- 参考信息 -->