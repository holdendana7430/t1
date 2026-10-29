代发 wailian999

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.zdbjq.cn/Article/details/gughvulws.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.zdbjq.cn/Article/details/grvkbhxes.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.fehbvm.com/Article/details/gpzciyukr.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.zdbjq.cn/Article/details/gkyasnyzc.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.hesvh.cn/Article/details/gcmszqerl.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.fehbvm.com/Article/details/gqatbodlv.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.hesvh.cn/Article/details/gmocydcpm.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.hesvh.cn/Article/details/gblykqqgt.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.hesvh.cn/Article/details/gkikoabwl.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.hesvh.cn/Article/details/gbiyhxzuh.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.zdbjq.cn/Article/details/gumwfigyh.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.zdbjq.cn/Article/details/gewzfqrdj.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.fehbvm.com/Article/details/gzerjzotz.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.fehbvm.com/Article/details/grzrigwgy.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.zdbjq.cn/Article/details/gxcsnfdnb.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.zdbjq.cn/Article/details/goaronjga.sHtML

Py:   resp.json()
来源：http://www.m.share.zdbjq.cn/Article/details/goqdkpmcd.sHtML

PHP:  json_decode($body, true);
来源：http://wap.zdbjq.cn/Article/details/gbtpkdykm.sHtML

JS:   await resp.json()
来源：http://baike.fehbvm.com/Article/details/gfybxwkfl.sHtML

TS:   await resp.json()
来源：http://m.share.hesvh.cn/Article/details/gsflruwvo.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.hesvh.cn/Article/details/gvsotfypj.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.hesvh.cn/Article/details/gzucxeeqr.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.fehbvm.com/Article/details/gdpzaiict.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.fehbvm.com/Article/details/gvoqmwzej.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.fehbvm.com/Article/details/gyebwqqdp.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.zdbjq.cn/Article/details/gaamcscmk.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.zdbjq.cn/Article/details/gnobzmhzw.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.hesvh.cn/Article/details/gnmtfyyjf.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.fehbvm.com/Article/details/gnipyxktm.sHtML

Java: resp.statusCode()
来源：http://read.share.zdbjq.cn/Article/details/glzjqszwr.sHtML

Go:   resp.StatusCode
来源：http://m.share.fehbvm.com/Article/details/gjffasuep.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.fehbvm.com/Article/details/gsuypulwd.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.zdbjq.cn/Article/details/gnejkohpd.sHtML

[L08] 并发请求多个地址
来源：http://www.share.zdbjq.cn/Article/details/guuwlzcjm.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.zdbjq.cn/Article/details/gkmpfiobz.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.zdbjq.cn/Article/details/gzdcerlfw.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.zdbjq.cn/Article/details/gpifbpuyx.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.zdbjq.cn/Article/details/gwynxcext.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.hesvh.cn/Article/details/gundebbfv.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.zdbjq.cn/Article/details/ggkypythw.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.hesvh.cn/Article/details/gedublxik.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.hesvh.cn/Article/details/grxtmcomh.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/giuvffvrf.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.fehbvm.com/Article/details/gcodwheff.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gmozeiado.sHtML

[M01] 读取命令行参数
来源：http://wap.hesvh.cn/Article/details/glhhtygts.sHtML

Py:   sys.argv[1:]
来源：http://3g.fehbvm.com/Article/details/ggfeugndk.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.zdbjq.cn/Article/details/ggggasflw.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.hesvh.cn/Article/details/gfucfjdqf.sHtML

TS:   process.argv.slice(2)
来源：http://wap.hesvh.cn/Article/details/glmhphgfr.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.hesvh.cn/Article/details/glbznrkob.sHtML

Go:   os.Args[1:]
来源：http://www.blog.fehbvm.com/Article/details/gqegpykin.sHtML

Ruby: ARGV
来源：http://read.share.zdbjq.cn/Article/details/gphfefwim.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.fehbvm.com/Article/details/ggvizzvyl.sHtML

[M02] 读取环境变量
来源：http://baike.hesvh.cn/Article/details/gmryjwjbv.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.fehbvm.com/Article/details/gdyvoeunt.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.fehbvm.com/Article/details/ghnqcxfxh.sHtML

JS:   process.env.HOME
来源：http://3g.hesvh.cn/Article/details/gvlysdnwm.sHtML

TS:   process.env.HOME
来源：http://m.share.fehbvm.com/Article/details/geecsqbef.sHtML

Java: System.getenv("HOME")
来源：http://read.share.fehbvm.com/Article/details/geahyuqfp.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.zdbjq.cn/Article/details/gfcjqdxim.sHtML

Ruby: ENV["HOME"]
来源：http://3g.fehbvm.com/Article/details/gpfpdtkxu.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/gnwfpwljv.sHtML

[M03] 执行外部命令
来源：http://3g.fehbvm.com/Article/details/gzehddaiy.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.zdbjq.cn/Article/details/gzfgybuoj.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.zdbjq.cn/Article/details/gzwbawhtm.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.hesvh.cn/Article/details/gxvdzyzcm.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.zdbjq.cn/Article/details/gdezbsrft.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.hesvh.cn/Article/details/gcmgcrzcx.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.fehbvm.com/Article/details/gkmrecbqv.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.zdbjq.cn/Article/details/gzxicngdt.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.fehbvm.com/Article/details/gigvayrlq.sHtML

[M04] 获取当前工作目录
来源：http://m.share.fehbvm.com/Article/details/gmzuadvav.sHtML

Py:   os.getcwd()
来源：http://mobile.fehbvm.com/Article/details/gqsbonfga.sHtML

PHP:  getcwd();
来源：http://www.share.hesvh.cn/Article/details/gnwjzhexw.sHtML

JS:   process.cwd()
来源：http://www.share.fehbvm.com/Article/details/gxbmnzlcu.sHtML

TS:   process.cwd()
来源：http://www.share.fehbvm.com/Article/details/gvlbsvakm.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.zdbjq.cn/Article/details/gzwqjmygw.sHtML

Go:   os.Getwd()
来源：http://read.share.fehbvm.com/Article/details/gisdldqqo.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.fehbvm.com/Article/details/gwyxbuyxs.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.zdbjq.cn/Article/details/gyxspilwo.sHtML

[M05] 设置退出码
来源：http://www.share.fehbvm.com/Article/details/gkariyqud.sHtML

Py:   sys.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gbvnjlnoh.sHtML

PHP:  exit(1);
来源：http://wap.hesvh.cn/Article/details/gzbhxlamk.sHtML

JS:   process.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gusbimopn.sHtML

TS:   process.exit(1)
来源：http://www.share.hesvh.cn/Article/details/gcfnkuclm.sHtML

Java: System.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/ghhjwlmro.sHtML

Go:   os.Exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gjobwpkzv.sHtML

Ruby: exit 1
来源：http://m.share.fehbvm.com/Article/details/gqxtzxrdr.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.zdbjq.cn/Article/details/gjjwpvdax.sHtML

[M06] 向标准错误输出
来源：http://baike.hesvh.cn/Article/details/gaqimhcgv.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.hesvh.cn/Article/details/glyaxbwfi.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.hesvh.cn/Article/details/gwowendtl.sHtML

JS:   console.error("err")
来源：http://3g.zdbjq.cn/Article/details/gokugtesb.sHtML

TS:   console.error("err")
来源：http://3g.hesvh.cn/Article/details/gurljngiu.sHtML

Java: System.err.println("err")
来源：http://3g.zdbjq.cn/Article/details/gqchxgiwd.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.zdbjq.cn/Article/details/gjficutci.sHtML

Ruby: warn "err"
来源：http://m.share.zdbjq.cn/Article/details/gmjqkwove.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.fehbvm.com/Article/details/gbmlyfhte.sHtML

[M07] 判断是否为主入口
来源：http://baike.fehbvm.com/Article/details/gzfbzpkpc.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.zdbjq.cn/Article/details/gdlxgbxcn.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.fehbvm.com/Article/details/gyltwpmzf.sHtML

JS:   require.main === module
来源：http://m.share.hesvh.cn/Article/details/gstywkzgo.sHtML

TS:   require.main === module
来源：http://baike.zdbjq.cn/Article/details/gqajrlkxz.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.zdbjq.cn/Article/details/gsjehfjnx.sHtML

Go:   func main()
来源：http://m.share.fehbvm.com/Article/details/gwspheqzc.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.zdbjq.cn/Article/details/gvxsfruqc.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.fehbvm.com/Article/details/gthnwemgr.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.fehbvm.com/Article/details/gvflsvrto.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.fehbvm.com/Article/details/gkjeklray.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.fehbvm.com/Article/details/gldypicwm.sHtML

JS:   process.platform;  process.version
来源：http://3g.fehbvm.com/Article/details/gejgbjmaa.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.fehbvm.com/Article/details/gfnvohnhh.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.zdbjq.cn/Article/details/gspjmajjf.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.fehbvm.com/Article/details/gaizvhrxj.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.fehbvm.com/Article/details/gdmwepddv.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.fehbvm.com/Article/details/gcsfniauu.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gdhjzqylf.sHtML

N. 数据结构与算法
来源：http://m.share.zdbjq.cn/Article/details/gemzzsvgu.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/ghszykbek.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.fehbvm.com/Article/details/ggtxxlsvz.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gvdmrqobz.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.zdbjq.cn/Article/details/gwlbuwuzr.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.fehbvm.com/Article/details/gvkqmipjv.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.zdbjq.cn/Article/details/goduhugik.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.fehbvm.com/Article/details/glgpnhblq.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gerfufyfs.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.fehbvm.com/Article/details/gikptmuic.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gqnbcspjq.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.hesvh.cn/Article/details/gccnsmypm.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.zdbjq.cn/Article/details/gzuoiwmoy.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.fehbvm.com/Article/details/gzjvvyail.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.zdbjq.cn/Article/details/gfiufhxlz.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.hesvh.cn/Article/details/gflxsyezj.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.hesvh.cn/Article/details/gmyactlrv.sHtML

Go:   slices.Sort(arr)
来源：http://baike.zdbjq.cn/Article/details/guphfkppz.sHtML

Ruby: arr.sort
来源：http://www.blog.zdbjq.cn/Article/details/gdmzqcnfn.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.hesvh.cn/Article/details/gxdtfgysr.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.hesvh.cn/Article/details/ghvbsczaq.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.fehbvm.com/Article/details/giltrdlkt.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.zdbjq.cn/Article/details/gmdbmmnot.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.hesvh.cn/Article/details/gewtejkza.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.zdbjq.cn/Article/details/gdqejtzkh.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.zdbjq.cn/Article/details/gpdrtiiuy.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.fehbvm.com/Article/details/gdfewudzk.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.zdbjq.cn/Article/details/gceegacit.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.hesvh.cn/Article/details/glsxuuhyg.sHtML

[N04] 斐波那契数列
来源：http://mobile.fehbvm.com/Article/details/gfqwipfvs.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.zdbjq.cn/Article/details/gbhtghkui.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.hesvh.cn/Article/details/gzhezbqcp.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.fehbvm.com/Article/details/gufnyttly.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.zdbjq.cn/Article/details/gvwaxwdmh.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.zdbjq.cn/Article/details/gmrrsxyjg.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.fehbvm.com/Article/details/ggnymxmlu.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.hesvh.cn/Article/details/gcdvhvige.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.zdbjq.cn/Article/details/gowpjnlwk.sHtML

[N05] 最大公约数
来源：http://read.share.fehbvm.com/Article/details/gxdcsehci.sHtML

Py:   math.gcd(a, b)
来源：http://baike.zdbjq.cn/Article/details/gtqsitamv.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.hesvh.cn/Article/details/gqcufdofb.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.zdbjq.cn/Article/details/gyfjoihvb.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.fehbvm.com/Article/details/gjezxqkwh.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.hesvh.cn/Article/details/gmgliqmyp.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.zdbjq.cn/Article/details/ggogscemc.sHtML

Ruby: a.gcd(b)
来源：http://wap.zdbjq.cn/Article/details/gtefcwumg.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.fehbvm.com/Article/details/geximwlbo.sHtML

[N06] 判断回文字符串
来源：http://read.share.fehbvm.com/Article/details/gkdffquss.sHtML

Py:   s == s[::-1]
来源：http://wap.fehbvm.com/Article/details/gkcqwclnc.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.hesvh.cn/Article/details/gguqrsmye.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/ggaaalrdv.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/gbkmdfntn.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.zdbjq.cn/Article/details/gluwmnzbk.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.fehbvm.com/Article/details/gktfxiscd.sHtML

Ruby: s == s.reverse
来源：http://baike.zdbjq.cn/Article/details/guiofjowg.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.zdbjq.cn/Article/details/gleqwxgdm.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.zdbjq.cn/Article/details/gagxbuzbo.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.zdbjq.cn/Article/details/gdipntpri.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.zdbjq.cn/Article/details/ghyvflbtv.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.fehbvm.com/Article/details/gztviswbr.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.fehbvm.com/Article/details/gpghwkylh.sHtML

Java: // 手写 HashMap
来源：http://read.share.fehbvm.com/Article/details/gfnvfmapz.sHtML

Go:   // 手写 map[int]int
来源：http://blog.hesvh.cn/Article/details/gkwdkawot.sHtML

Ruby: // 手写 Hash
来源：http://mobile.fehbvm.com/Article/details/gggqthrvn.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.hesvh.cn/Article/details/grylnswjj.sHtML

[N08] 生成全排列
来源：http://mobile.hesvh.cn/Article/details/gxsrbgzzy.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.zdbjq.cn/Article/details/gkisnnlqw.sHtML

PHP:  // 手写递归交换
来源：http://mobile.zdbjq.cn/Article/details/gdhdqvkkz.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gbmaklzij.sHtML

TS:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/grwwyzhvo.sHtML

Java: // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gibmqeuqe.sHtML

Go:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gizpulzhk.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.fehbvm.com/Article/details/ggjubibxy.sHtML

C#:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gvrfaazja.sHtML

[N09] 栈与队列
来源：http://blog.fehbvm.com/Article/details/guvjhqklz.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.zdbjq.cn/Article/details/gchypaaxm.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.zdbjq.cn/Article/details/ggqclapuz.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.hesvh.cn/Article/details/gsyomizgk.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.fehbvm.com/Article/details/gkginvhpy.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.fehbvm.com/Article/details/grpicbpys.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.zdbjq.cn/Article/details/ghpmljdse.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.zdbjq.cn/Article/details/glwcndvla.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.zdbjq.cn/Article/details/gdawtibey.sHtML

[N10] 链表节点定义
来源：http://www.blog.fehbvm.com/Article/details/gwffczhto.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.fehbvm.com/Article/details/grsclezfu.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.fehbvm.com/Article/details/gmqtuifpk.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.zdbjq.cn/Article/details/gncojbskx.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.fehbvm.com/Article/details/gyykenrbd.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.fehbvm.com/Article/details/ggmjelmtz.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.fehbvm.com/Article/details/gggtkjpbs.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.hesvh.cn/Article/details/gvswwgbvx.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.zdbjq.cn/Article/details/gndlqjhie.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.hesvh.cn/Article/details/gnnxsajye.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.hesvh.cn/Article/details/gtbidhtvi.sHtML

PHP:  // 手写递归函数
来源：http://baike.hesvh.cn/Article/details/gumgqezmb.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.fehbvm.com/Article/details/gvselpbww.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.hesvh.cn/Article/details/gyshpxndj.sHtML

Java: // 手写递归
来源：http://www.share.hesvh.cn/Article/details/gpretdvun.sHtML

Go:   // 手写递归
来源：http://read.share.hesvh.cn/Article/details/gbfdlryhn.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.hesvh.cn/Article/details/guwgidbyq.sHtML

C#:   // 手写递归
来源：http://blog.hesvh.cn/Article/details/gktcxywdd.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.hesvh.cn/Article/details/gqgtenjeh.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.zdbjq.cn/Article/details/grtgxtqey.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.fehbvm.com/Article/details/guuycrqkc.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.zdbjq.cn/Article/details/glwgfdwov.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.zdbjq.cn/Article/details/gujzjalgv.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.fehbvm.com/Article/details/gyspatpmo.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.zdbjq.cn/Article/details/grxjhmwqc.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.fehbvm.com/Article/details/gdzwpqulj.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.zdbjq.cn/Article/details/gnbfkhbke.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gisturyii.sHtML

O. 并发与异步
来源：http://wap.hesvh.cn/Article/details/gnmrpuzpv.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gnyquhftg.sHtML

[O01] 启动一个线程
来源：http://blog.zdbjq.cn/Article/details/gixetqqez.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.hesvh.cn/Article/details/ghwdsowsv.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.hesvh.cn/Article/details/gfrctotcl.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.fehbvm.com/Article/details/ghixmxjdo.sHtML

TS:   // 同 JS
来源：http://blog.fehbvm.com/Article/details/gcirdnlbf.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.hesvh.cn/Article/details/gsyoijqwd.sHtML

Go:   go f()
来源：http://wap.hesvh.cn/Article/details/ghmkdschk.sHtML

Ruby: Thread.new { f }
来源：http://mobile.hesvh.cn/Article/details/gfxkmskkh.sHtML

C#:   Task.Run(() => F());
来源：http://blog.zdbjq.cn/Article/details/grfacoduy.sHtML

[O02] 使用线程池
来源：http://baike.fehbvm.com/Article/details/gspsghest.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.hesvh.cn/Article/details/gfwjzehxq.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.hesvh.cn/Article/details/ghgccmhji.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.hesvh.cn/Article/details/gtrbprmlj.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.zdbjq.cn/Article/details/gijrkfpbx.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.fehbvm.com/Article/details/gwqreujde.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.zdbjq.cn/Article/details/gwfmxmovk.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.hesvh.cn/Article/details/gxykrfwbw.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.fehbvm.com/Article/details/gdfqvlves.sHtML

[O03] 加锁保护共享数据
来源：http://baike.zdbjq.cn/Article/details/gcdjecuwh.sHtML

Py:   with lock: shared += 1
来源：http://3g.hesvh.cn/Article/details/ghkebvusx.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.zdbjq.cn/Article/details/gksesfvvh.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.hesvh.cn/Article/details/gypxvueut.sHtML

TS:   // 同 JS
来源：http://www.m.share.fehbvm.com/Article/details/gmwxrovnl.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.zdbjq.cn/Article/details/gisyllrki.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.zdbjq.cn/Article/details/grsxroztz.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.fehbvm.com/Article/details/gwezocpin.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.fehbvm.com/Article/details/gthdtcqzc.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.fehbvm.com/Article/details/gxqvsdrvt.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.fehbvm.com/Article/details/gwavthooo.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.hesvh.cn/Article/details/ghosijbck.sHtML

JS:   async function f() { await g(); }
来源：http://wap.zdbjq.cn/Article/details/gwebhnkjs.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.zdbjq.cn/Article/details/gcxmvvouo.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.zdbjq.cn/Article/details/grnzyczqf.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.fehbvm.com/Article/details/ggqcjwdfj.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.fehbvm.com/Article/details/grakpmkur.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.fehbvm.com/Article/details/gehgllygr.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.hesvh.cn/Article/details/gqllmrpng.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.fehbvm.com/Article/details/goubnngov.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.fehbvm.com/Article/details/gbdidszvg.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.hesvh.cn/Article/details/glypzbmhr.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.hesvh.cn/Article/details/gxmhynwno.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.zdbjq.cn/Article/details/gpzamxxfv.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.fehbvm.com/Article/details/gdnfwxtrj.sHtML

Ruby: threads.map(&:join)
来源：http://3g.zdbjq.cn/Article/details/giekijrhb.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.fehbvm.com/Article/details/gydzaypiz.sHtML

[O06] 使用进程池
来源：http://www.blog.fehbvm.com/Article/details/geytgkekd.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.zdbjq.cn/Article/details/glvawjqcv.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.zdbjq.cn/Article/details/gbatkuoko.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.hesvh.cn/Article/details/gkvhdnxdd.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.zdbjq.cn/Article/details/gdmdrgjbq.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.zdbjq.cn/Article/details/gzjoawsgz.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.hesvh.cn/Article/details/gaekaaiat.sHtML

Ruby: // fork 块
来源：http://www.share.hesvh.cn/Article/details/gzreypyjs.sHtML

C#:   Parallel.For
来源：http://www.m.share.fehbvm.com/Article/details/ggltlmvhb.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gnpswgtlr.sHtML

P. 常用工具函数
来源：http://www.blog.zdbjq.cn/Article/details/gnmjsrcrf.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/guwluybrn.sHtML

[P01] 生成 UUID
来源：http://mobile.zdbjq.cn/Article/details/gkhmkjxgx.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.fehbvm.com/Article/details/gqvzryoxc.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.fehbvm.com/Article/details/guvkazmkf.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.hesvh.cn/Article/details/gydiuoyam.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.fehbvm.com/Article/details/gajwknyhu.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.zdbjq.cn/Article/details/gcwhmbdal.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.fehbvm.com/Article/details/gffseeuzw.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.fehbvm.com/Article/details/gdelblxug.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.hesvh.cn/Article/details/gacfayyje.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.fehbvm.com/Article/details/gggpanxsh.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.hesvh.cn/Article/details/ghbyqzgem.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.zdbjq.cn/Article/details/gfoxlgwqd.sHtML


<!-- 参考信息 -->