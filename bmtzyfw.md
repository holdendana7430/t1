代发 wailian999

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.hesvh.cn/Article/details/gskljrqfh.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.hesvh.cn/Article/details/gdwyctgld.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.hesvh.cn/Article/details/gctqovfkx.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.hesvh.cn/Article/details/guzvnebqb.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.hesvh.cn/Article/details/gizlvouat.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.zdbjq.cn/Article/details/gbfejmrgh.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.zdbjq.cn/Article/details/gvivbmmxp.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.zdbjq.cn/Article/details/gllgqvwiw.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.zdbjq.cn/Article/details/ghgpletkt.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.fehbvm.com/Article/details/gfeotkisj.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.hesvh.cn/Article/details/gsiyhaoos.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.fehbvm.com/Article/details/ggqxuxbmz.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.zdbjq.cn/Article/details/gvgmdnnzz.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.zdbjq.cn/Article/details/gtbwxfkye.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.fehbvm.com/Article/details/gvonpnrqx.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.zdbjq.cn/Article/details/gezdutpxp.sHtML

Py:   resp.json()
来源：http://baike.fehbvm.com/Article/details/gcihfpgfd.sHtML

PHP:  json_decode($body, true);
来源：http://baike.zdbjq.cn/Article/details/gvqwovupo.sHtML

JS:   await resp.json()
来源：http://mobile.fehbvm.com/Article/details/gclnebiey.sHtML

TS:   await resp.json()
来源：http://www.m.share.hesvh.cn/Article/details/glydttebu.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.hesvh.cn/Article/details/gqbzfdtuf.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.fehbvm.com/Article/details/gfawemils.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.fehbvm.com/Article/details/gpwojuese.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.fehbvm.com/Article/details/geugixxik.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.fehbvm.com/Article/details/gnskbfpay.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.fehbvm.com/Article/details/gddlfvsqd.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.fehbvm.com/Article/details/gusxesqtz.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.fehbvm.com/Article/details/gucwjrwda.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.fehbvm.com/Article/details/gromjewgc.sHtML

Java: resp.statusCode()
来源：http://3g.fehbvm.com/Article/details/gkmuauqkq.sHtML

Go:   resp.StatusCode
来源：http://www.share.zdbjq.cn/Article/details/gnyyzojmd.sHtML

Ruby: resp.code.to_i
来源：http://baike.fehbvm.com/Article/details/gzdxbgftv.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.zdbjq.cn/Article/details/grmviwjnr.sHtML

[L08] 并发请求多个地址
来源：http://wap.hesvh.cn/Article/details/gnnkcwdwk.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.zdbjq.cn/Article/details/ggicbdmyv.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.zdbjq.cn/Article/details/gvzskgvag.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.zdbjq.cn/Article/details/gbhxcqevz.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fehbvm.com/Article/details/gzzlvysac.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.hesvh.cn/Article/details/gbvtwpndq.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.zdbjq.cn/Article/details/giizhbzcm.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.zdbjq.cn/Article/details/gimcnpbmd.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.hesvh.cn/Article/details/guxduwgrl.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/ggeljdmry.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.hesvh.cn/Article/details/gzawqflsv.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/giitolmzk.sHtML

[M01] 读取命令行参数
来源：http://mobile.fehbvm.com/Article/details/genmqlloi.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.fehbvm.com/Article/details/gkljppcyf.sHtML

PHP:  $argv;  $argc;
来源：http://wap.zdbjq.cn/Article/details/gjlngykiu.sHtML

JS:   process.argv.slice(2)
来源：http://baike.hesvh.cn/Article/details/gsulkxuev.sHtML

TS:   process.argv.slice(2)
来源：http://baike.fehbvm.com/Article/details/glhkmcevr.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.fehbvm.com/Article/details/gglrdshns.sHtML

Go:   os.Args[1:]
来源：http://www.share.hesvh.cn/Article/details/grnfuqiat.sHtML

Ruby: ARGV
来源：http://wap.fehbvm.com/Article/details/gdjzmlhli.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.zdbjq.cn/Article/details/geazqjoub.sHtML

[M02] 读取环境变量
来源：http://www.share.fehbvm.com/Article/details/gorkscgqx.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.hesvh.cn/Article/details/giyimkpoi.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.hesvh.cn/Article/details/gowuzenln.sHtML

JS:   process.env.HOME
来源：http://m.share.zdbjq.cn/Article/details/gpgaeglmq.sHtML

TS:   process.env.HOME
来源：http://m.share.fehbvm.com/Article/details/gyaiapnmc.sHtML

Java: System.getenv("HOME")
来源：http://3g.hesvh.cn/Article/details/govnmqiqs.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.fehbvm.com/Article/details/gnkmmowfw.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.zdbjq.cn/Article/details/ghpuszcol.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.fehbvm.com/Article/details/ggbbvswzf.sHtML

[M03] 执行外部命令
来源：http://mobile.hesvh.cn/Article/details/gwafkvyct.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.zdbjq.cn/Article/details/gizpslrne.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.zdbjq.cn/Article/details/gkiqusnlh.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.hesvh.cn/Article/details/gqeqliqxk.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.fehbvm.com/Article/details/gapsfgaao.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.fehbvm.com/Article/details/gzwymdpgf.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.hesvh.cn/Article/details/gumvoucmy.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.hesvh.cn/Article/details/ghxnvxfju.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.fehbvm.com/Article/details/ghxsagucm.sHtML

[M04] 获取当前工作目录
来源：http://m.share.zdbjq.cn/Article/details/gottpnbia.sHtML

Py:   os.getcwd()
来源：http://blog.fehbvm.com/Article/details/ghqbigaqr.sHtML

PHP:  getcwd();
来源：http://m.share.hesvh.cn/Article/details/gkpzabaex.sHtML

JS:   process.cwd()
来源：http://www.blog.fehbvm.com/Article/details/gwaewecaz.sHtML

TS:   process.cwd()
来源：http://www.share.fehbvm.com/Article/details/gssmfcntj.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.fehbvm.com/Article/details/gddssvzda.sHtML

Go:   os.Getwd()
来源：http://www.blog.hesvh.cn/Article/details/gcldujqba.sHtML

Ruby: Dir.pwd
来源：http://wap.zdbjq.cn/Article/details/gptbequrk.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.fehbvm.com/Article/details/gjwuafvkz.sHtML

[M05] 设置退出码
来源：http://www.blog.hesvh.cn/Article/details/gchpnguwb.sHtML

Py:   sys.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gsdkhdzxl.sHtML

PHP:  exit(1);
来源：http://www.m.share.zdbjq.cn/Article/details/gmsvgvwge.sHtML

JS:   process.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gagyzqnpx.sHtML

TS:   process.exit(1)
来源：http://3g.hesvh.cn/Article/details/gupeskpon.sHtML

Java: System.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gktbinhvr.sHtML

Go:   os.Exit(1)
来源：http://3g.hesvh.cn/Article/details/gzrzqlzoj.sHtML

Ruby: exit 1
来源：http://baike.zdbjq.cn/Article/details/gxvkzkdhi.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.hesvh.cn/Article/details/gettfdisx.sHtML

[M06] 向标准错误输出
来源：http://www.blog.fehbvm.com/Article/details/gfwcynder.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.fehbvm.com/Article/details/gmrixmosa.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.fehbvm.com/Article/details/gmtoxbett.sHtML

JS:   console.error("err")
来源：http://wap.hesvh.cn/Article/details/geatwjfoe.sHtML

TS:   console.error("err")
来源：http://wap.zdbjq.cn/Article/details/gijmmqljr.sHtML

Java: System.err.println("err")
来源：http://www.share.hesvh.cn/Article/details/gzqmivbgz.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.zdbjq.cn/Article/details/gmssfjmeo.sHtML

Ruby: warn "err"
来源：http://www.share.hesvh.cn/Article/details/gbwcsmjox.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.fehbvm.com/Article/details/gnmndxbxi.sHtML

[M07] 判断是否为主入口
来源：http://baike.fehbvm.com/Article/details/gsrkczkiq.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.hesvh.cn/Article/details/gnymhxhzp.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.zdbjq.cn/Article/details/gjmgqikvw.sHtML

JS:   require.main === module
来源：http://blog.fehbvm.com/Article/details/gmgkyanrz.sHtML

TS:   require.main === module
来源：http://www.blog.zdbjq.cn/Article/details/gvtigvfhn.sHtML

Java: public static void main(String[] args)
来源：http://mobile.fehbvm.com/Article/details/gzppgrvcb.sHtML

Go:   func main()
来源：http://read.share.hesvh.cn/Article/details/ghjaftbcv.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.fehbvm.com/Article/details/gsixddrxt.sHtML

C#:   static void Main(string[] args)
来源：http://baike.zdbjq.cn/Article/details/goyshygwc.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.zdbjq.cn/Article/details/gjubzlauv.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.fehbvm.com/Article/details/gnwygljcz.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.hesvh.cn/Article/details/gygooklsv.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.zdbjq.cn/Article/details/ggzujblzc.sHtML

TS:   process.platform;  process.version
来源：http://m.share.zdbjq.cn/Article/details/gjtoekjdy.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.hesvh.cn/Article/details/gjhzkckgn.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.fehbvm.com/Article/details/gupfgnlou.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.fehbvm.com/Article/details/ghwkyennm.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.zdbjq.cn/Article/details/ghkmngkme.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gwvomnflm.sHtML

N. 数据结构与算法
来源：http://m.share.hesvh.cn/Article/details/gffjjbxgm.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gpwumqefo.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.zdbjq.cn/Article/details/gklugegws.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.hesvh.cn/Article/details/gcymwrvfz.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.hesvh.cn/Article/details/gldvyooob.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.fehbvm.com/Article/details/gsyrbtkrs.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.zdbjq.cn/Article/details/gedjupqdk.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gekyfgajg.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.hesvh.cn/Article/details/gecivxwoc.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.fehbvm.com/Article/details/gyrodibjp.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.hesvh.cn/Article/details/gsgpenpuf.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.zdbjq.cn/Article/details/gifwmksuj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.zdbjq.cn/Article/details/glvklgcqa.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.fehbvm.com/Article/details/glteccava.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.hesvh.cn/Article/details/gszntawhs.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.zdbjq.cn/Article/details/gucbytgkf.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.fehbvm.com/Article/details/gdbjeumuy.sHtML

Go:   slices.Sort(arr)
来源：http://baike.fehbvm.com/Article/details/geldqupgw.sHtML

Ruby: arr.sort
来源：http://www.blog.hesvh.cn/Article/details/giavyzgga.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.hesvh.cn/Article/details/gkfcdrcui.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.fehbvm.com/Article/details/gcuapvtzg.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.fehbvm.com/Article/details/gxixzvsyl.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.hesvh.cn/Article/details/gfmasonzr.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.hesvh.cn/Article/details/gbtcnmttc.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.zdbjq.cn/Article/details/gshykvlrs.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.hesvh.cn/Article/details/gyewuivyo.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.zdbjq.cn/Article/details/guuxxkzwa.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.fehbvm.com/Article/details/gxtawfceh.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.hesvh.cn/Article/details/gbsuvwmjs.sHtML

[N04] 斐波那契数列
来源：http://www.share.hesvh.cn/Article/details/glvicpzki.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.zdbjq.cn/Article/details/glcohjhik.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.fehbvm.com/Article/details/guajbycgn.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.hesvh.cn/Article/details/gfzwecvao.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.zdbjq.cn/Article/details/ggagnazul.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.hesvh.cn/Article/details/ggaypuswt.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.fehbvm.com/Article/details/gpjvezzbv.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.hesvh.cn/Article/details/gozslpbbn.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.zdbjq.cn/Article/details/gwakdoggl.sHtML

[N05] 最大公约数
来源：http://baike.zdbjq.cn/Article/details/gsvpqohqj.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.hesvh.cn/Article/details/gwpefoftq.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.hesvh.cn/Article/details/graepugnw.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.zdbjq.cn/Article/details/gmfnhqolx.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.hesvh.cn/Article/details/gglhukxrw.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.fehbvm.com/Article/details/gjqhqlgev.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.hesvh.cn/Article/details/gsopiiyrx.sHtML

Ruby: a.gcd(b)
来源：http://m.share.zdbjq.cn/Article/details/goouhfqyw.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.hesvh.cn/Article/details/gwawhhngx.sHtML

[N06] 判断回文字符串
来源：http://baike.fehbvm.com/Article/details/gbbanriey.sHtML

Py:   s == s[::-1]
来源：http://www.share.hesvh.cn/Article/details/gwrthbusc.sHtML

PHP:  $s === strrev($s);
来源：http://baike.hesvh.cn/Article/details/ggbbtrlnz.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/gsniwbedu.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/gqknrkwug.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.fehbvm.com/Article/details/gimgmykru.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.zdbjq.cn/Article/details/grsibszyk.sHtML

Ruby: s == s.reverse
来源：http://baike.fehbvm.com/Article/details/gaswexvvj.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.hesvh.cn/Article/details/gnxwodged.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.hesvh.cn/Article/details/gwjolodcu.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.fehbvm.com/Article/details/ghgcspaiw.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.zdbjq.cn/Article/details/gvvspemqm.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.hesvh.cn/Article/details/grmbwmbgw.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.hesvh.cn/Article/details/gsncpuony.sHtML

Java: // 手写 HashMap
来源：http://read.share.hesvh.cn/Article/details/gwugazlvi.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.zdbjq.cn/Article/details/gsqxemcfu.sHtML

Ruby: // 手写 Hash
来源：http://3g.zdbjq.cn/Article/details/ghwdawnpv.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.hesvh.cn/Article/details/gnpvhzhqe.sHtML

[N08] 生成全排列
来源：http://wap.hesvh.cn/Article/details/gcswjyzms.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.hesvh.cn/Article/details/gfbhkqons.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.fehbvm.com/Article/details/gwrdfuwcy.sHtML

JS:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gqizzukur.sHtML

TS:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gxekovtqo.sHtML

Java: // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gigrepzpf.sHtML

Go:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gbszmksni.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.fehbvm.com/Article/details/gxhviwupw.sHtML

C#:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gakbhfkmb.sHtML

[N09] 栈与队列
来源：http://baike.zdbjq.cn/Article/details/gazgsolra.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.hesvh.cn/Article/details/gpxbrwkpj.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.fehbvm.com/Article/details/gpkzzkuop.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.fehbvm.com/Article/details/gpvenpjjp.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.fehbvm.com/Article/details/gssxiolrz.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.fehbvm.com/Article/details/gjxbnwsdd.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.hesvh.cn/Article/details/gqswadjur.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.zdbjq.cn/Article/details/gncmwjnrm.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.hesvh.cn/Article/details/grywhqjgp.sHtML

[N10] 链表节点定义
来源：http://blog.zdbjq.cn/Article/details/gnxxfueyw.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.hesvh.cn/Article/details/gbscpeczy.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.fehbvm.com/Article/details/gsbrprbsf.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.zdbjq.cn/Article/details/gfftvftgb.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.zdbjq.cn/Article/details/gwwlpycwp.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.fehbvm.com/Article/details/gqthphthz.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.fehbvm.com/Article/details/gegcyyjsi.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.fehbvm.com/Article/details/gwuraucue.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.hesvh.cn/Article/details/gvxxhtmqk.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gccwdefyr.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.fehbvm.com/Article/details/gkrandlou.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.fehbvm.com/Article/details/gyduqwuyp.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.fehbvm.com/Article/details/gunoqdzbc.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.hesvh.cn/Article/details/gxrwfwqgq.sHtML

Java: // 手写递归
来源：http://wap.hesvh.cn/Article/details/ggluhbyby.sHtML

Go:   // 手写递归
来源：http://wap.fehbvm.com/Article/details/garutxhjb.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.zdbjq.cn/Article/details/gplpmuoai.sHtML

C#:   // 手写递归
来源：http://baike.fehbvm.com/Article/details/gvpmsrrid.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.zdbjq.cn/Article/details/gekhuxgbo.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.fehbvm.com/Article/details/gmujfctqj.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.zdbjq.cn/Article/details/gxrbudsqq.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.hesvh.cn/Article/details/gokziwybj.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.zdbjq.cn/Article/details/golroopbl.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.fehbvm.com/Article/details/gsyjfpfpt.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.zdbjq.cn/Article/details/gmdcgpxdm.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.hesvh.cn/Article/details/gbhlvkxhk.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.hesvh.cn/Article/details/gafbeouvf.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/ggoahefvc.sHtML

O. 并发与异步
来源：http://3g.fehbvm.com/Article/details/giwmdqprg.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gsyyjcxjc.sHtML

[O01] 启动一个线程
来源：http://www.blog.hesvh.cn/Article/details/gubxgsigt.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.zdbjq.cn/Article/details/gcsuwcyln.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.fehbvm.com/Article/details/gysazxjal.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.zdbjq.cn/Article/details/gvcmtdoin.sHtML

TS:   // 同 JS
来源：http://blog.zdbjq.cn/Article/details/gtjsufhqu.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.zdbjq.cn/Article/details/gcuxswqjq.sHtML

Go:   go f()
来源：http://read.share.zdbjq.cn/Article/details/gntnqlyvg.sHtML

Ruby: Thread.new { f }
来源：http://wap.zdbjq.cn/Article/details/gqjlpbumb.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.fehbvm.com/Article/details/gociovdaj.sHtML

[O02] 使用线程池
来源：http://blog.fehbvm.com/Article/details/gihqhtnot.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.zdbjq.cn/Article/details/gzaywmhyt.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.fehbvm.com/Article/details/gercvfbal.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.hesvh.cn/Article/details/gjvgwfqlv.sHtML

TS:   // worker_threads 线程池
来源：http://baike.zdbjq.cn/Article/details/gdnmqirij.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.hesvh.cn/Article/details/gblvcwynf.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.hesvh.cn/Article/details/gtrknjuyo.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.zdbjq.cn/Article/details/gkiuahwfd.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.fehbvm.com/Article/details/gzbwjvtnc.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.zdbjq.cn/Article/details/gryqlwtro.sHtML

Py:   with lock: shared += 1
来源：http://m.share.hesvh.cn/Article/details/gtwpkfsmz.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.fehbvm.com/Article/details/gdtmzlpql.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.hesvh.cn/Article/details/gqfomkwnm.sHtML

TS:   // 同 JS
来源：http://wap.zdbjq.cn/Article/details/gkfnhabdj.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.hesvh.cn/Article/details/gkfquxyvr.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.zdbjq.cn/Article/details/gsjyuvfgy.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.fehbvm.com/Article/details/gunyqqekk.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.hesvh.cn/Article/details/gytwaeyfp.sHtML

[O04] 定义异步函数并等待
来源：http://baike.hesvh.cn/Article/details/guncdrleo.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.fehbvm.com/Article/details/glfyscltl.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.zdbjq.cn/Article/details/guwgkwczw.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.fehbvm.com/Article/details/gryzvgrvs.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.fehbvm.com/Article/details/gwkabfvsj.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.zdbjq.cn/Article/details/gjepljtoa.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.zdbjq.cn/Article/details/gqygklhuh.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.zdbjq.cn/Article/details/gopusimdl.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.fehbvm.com/Article/details/gvbsnlhyl.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.zdbjq.cn/Article/details/gaylilves.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.hesvh.cn/Article/details/gwgplpnvw.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.hesvh.cn/Article/details/gxqnjcpif.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.fehbvm.com/Article/details/gdquqrtla.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.zdbjq.cn/Article/details/gwlocydre.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.fehbvm.com/Article/details/goiyeiptk.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.zdbjq.cn/Article/details/gsagvakdg.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.hesvh.cn/Article/details/geaexdfmu.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.zdbjq.cn/Article/details/gmbutjafu.sHtML

[O06] 使用进程池
来源：http://mobile.fehbvm.com/Article/details/gfltrkdmt.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.hesvh.cn/Article/details/gdtrdbasd.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.zdbjq.cn/Article/details/gakbuetwv.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.zdbjq.cn/Article/details/gjgegirmj.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.hesvh.cn/Article/details/gspbzwrxa.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.zdbjq.cn/Article/details/gcxiwuhck.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.hesvh.cn/Article/details/gdmwwikkd.sHtML

Ruby: // fork 块
来源：http://www.m.share.hesvh.cn/Article/details/gjevrsrdi.sHtML

C#:   Parallel.For
来源：http://m.share.zdbjq.cn/Article/details/golwoyhbd.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gnfchfdkx.sHtML

P. 常用工具函数
来源：http://3g.fehbvm.com/Article/details/gcvmneotb.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gyqbdatrj.sHtML

[P01] 生成 UUID
来源：http://mobile.zdbjq.cn/Article/details/gmohgsqhv.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.hesvh.cn/Article/details/gngynjzzs.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.hesvh.cn/Article/details/gtrmabggj.sHtML

JS:   crypto.randomUUID()
来源：http://baike.fehbvm.com/Article/details/glazisydb.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.fehbvm.com/Article/details/giqjuctea.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.fehbvm.com/Article/details/gpbxiijqc.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.zdbjq.cn/Article/details/ghldwnyol.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.fehbvm.com/Article/details/gfimidyqx.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.zdbjq.cn/Article/details/goxlmzdha.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.hesvh.cn/Article/details/gzhmwuvno.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.hesvh.cn/Article/details/gcbejcfrn.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.hesvh.cn/Article/details/gjcfewhlo.sHtML


<!-- 参考信息 -->