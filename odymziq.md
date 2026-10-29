代发 wailian999

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.hesvh.cn/Article/details/gohfbyrpx.sHtML

[L04] 设置超时
来源：http://read.share.zdbjq.cn/Article/details/gfpbgvaub.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.fehbvm.com/Article/details/gjwdvofue.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.fehbvm.com/Article/details/gjpeksblr.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.fehbvm.com/Article/details/grfztefth.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.hesvh.cn/Article/details/gqjxrtmpg.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.hesvh.cn/Article/details/gzbegurew.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.hesvh.cn/Article/details/ggyklnsju.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.hesvh.cn/Article/details/gzjishocy.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.zdbjq.cn/Article/details/gvftleuat.sHtML

[L05] 上传文件（multipart）
来源：http://blog.fehbvm.com/Article/details/gkmapgjxt.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.zdbjq.cn/Article/details/gadtcvtoj.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.hesvh.cn/Article/details/gscfhgirf.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.hesvh.cn/Article/details/goxiqwbsv.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.zdbjq.cn/Article/details/gynvxmdfu.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.zdbjq.cn/Article/details/guycvngnj.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.hesvh.cn/Article/details/ghkwhlcop.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.fehbvm.com/Article/details/gfaozhgqz.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.zdbjq.cn/Article/details/gskumnses.sHtML

[L06] 解析响应为 JSON
来源：http://blog.hesvh.cn/Article/details/gnpxswpkd.sHtML

Py:   resp.json()
来源：http://www.share.hesvh.cn/Article/details/ghwfqgeen.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.fehbvm.com/Article/details/grikblxqs.sHtML

JS:   await resp.json()
来源：http://www.m.share.zdbjq.cn/Article/details/gbhtdtiub.sHtML

TS:   await resp.json()
来源：http://3g.zdbjq.cn/Article/details/grwnjwfig.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.fehbvm.com/Article/details/gkyhnfnjy.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.hesvh.cn/Article/details/gmnjrgpls.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.fehbvm.com/Article/details/gdpigpvqd.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.zdbjq.cn/Article/details/glhccylpa.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.zdbjq.cn/Article/details/gqcmgutir.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.zdbjq.cn/Article/details/gylaikpzy.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.hesvh.cn/Article/details/gtzxwcayt.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.hesvh.cn/Article/details/giygysspg.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.hesvh.cn/Article/details/gifyegfqc.sHtML

Java: resp.statusCode()
来源：http://baike.zdbjq.cn/Article/details/gmypdfsuw.sHtML

Go:   resp.StatusCode
来源：http://read.share.hesvh.cn/Article/details/gykxqlevk.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.zdbjq.cn/Article/details/gpflggqon.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.hesvh.cn/Article/details/ghrgwntss.sHtML

[L08] 并发请求多个地址
来源：http://m.share.zdbjq.cn/Article/details/glulqqzxs.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.hesvh.cn/Article/details/gripngmwm.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.hesvh.cn/Article/details/gykbdopcq.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fehbvm.com/Article/details/gtylmkqdp.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.hesvh.cn/Article/details/gfupyslrm.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.hesvh.cn/Article/details/gikkkcmgy.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.hesvh.cn/Article/details/gqtktqaof.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.fehbvm.com/Article/details/gcpdevqjj.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.hesvh.cn/Article/details/gfbnbczbm.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/grninaumj.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.zdbjq.cn/Article/details/glsthcnas.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/ganegxxsz.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.fehbvm.com/Article/details/ghjrbspcn.sHtML

Py:   sys.argv[1:]
来源：http://blog.fehbvm.com/Article/details/giiqerfvl.sHtML

PHP:  $argv;  $argc;
来源：http://wap.hesvh.cn/Article/details/gmfgjiojr.sHtML

JS:   process.argv.slice(2)
来源：http://baike.hesvh.cn/Article/details/gvedmxzbe.sHtML

TS:   process.argv.slice(2)
来源：http://baike.zdbjq.cn/Article/details/gariitvfc.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.hesvh.cn/Article/details/gqgzbfdwq.sHtML

Go:   os.Args[1:]
来源：http://m.share.fehbvm.com/Article/details/gftdkjqoc.sHtML

Ruby: ARGV
来源：http://www.blog.fehbvm.com/Article/details/gftttrgrd.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.hesvh.cn/Article/details/gedmhgoug.sHtML

[M02] 读取环境变量
来源：http://blog.zdbjq.cn/Article/details/geiohzosv.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.zdbjq.cn/Article/details/gedcyeurl.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.zdbjq.cn/Article/details/geohejkrt.sHtML

JS:   process.env.HOME
来源：http://wap.fehbvm.com/Article/details/gyqqqscpm.sHtML

TS:   process.env.HOME
来源：http://www.share.zdbjq.cn/Article/details/gsyvkrpny.sHtML

Java: System.getenv("HOME")
来源：http://wap.zdbjq.cn/Article/details/glpgtsgnx.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.fehbvm.com/Article/details/gzvqjxaww.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.hesvh.cn/Article/details/ghamytslm.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.hesvh.cn/Article/details/gowkieswu.sHtML

[M03] 执行外部命令
来源：http://3g.zdbjq.cn/Article/details/gmrlguqik.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.zdbjq.cn/Article/details/gqefsmojt.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.zdbjq.cn/Article/details/gupjjhvcz.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.hesvh.cn/Article/details/guvehvksc.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.fehbvm.com/Article/details/gremdaifu.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.hesvh.cn/Article/details/gnllasrow.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.hesvh.cn/Article/details/ghgewysjo.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.zdbjq.cn/Article/details/gxjcffros.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.fehbvm.com/Article/details/gwudyfyfw.sHtML

[M04] 获取当前工作目录
来源：http://m.share.zdbjq.cn/Article/details/gutmxzgnq.sHtML

Py:   os.getcwd()
来源：http://www.m.share.hesvh.cn/Article/details/gwhoqayjk.sHtML

PHP:  getcwd();
来源：http://3g.fehbvm.com/Article/details/gwjprdmgp.sHtML

JS:   process.cwd()
来源：http://wap.hesvh.cn/Article/details/gzaykvuqa.sHtML

TS:   process.cwd()
来源：http://baike.fehbvm.com/Article/details/gjhbcwqcc.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.zdbjq.cn/Article/details/gzycoyntp.sHtML

Go:   os.Getwd()
来源：http://www.m.share.fehbvm.com/Article/details/gutdmolbp.sHtML

Ruby: Dir.pwd
来源：http://blog.hesvh.cn/Article/details/glrmfamto.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.hesvh.cn/Article/details/gtlkahnla.sHtML

[M05] 设置退出码
来源：http://wap.zdbjq.cn/Article/details/geqxuumee.sHtML

Py:   sys.exit(1)
来源：http://www.share.fehbvm.com/Article/details/gcfyrkxql.sHtML

PHP:  exit(1);
来源：http://mobile.hesvh.cn/Article/details/ghactupxk.sHtML

JS:   process.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gungokfqj.sHtML

TS:   process.exit(1)
来源：http://blog.zdbjq.cn/Article/details/grqzogyxa.sHtML

Java: System.exit(1)
来源：http://read.share.hesvh.cn/Article/details/goacewgvp.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gtwdfuemg.sHtML

Ruby: exit 1
来源：http://www.share.hesvh.cn/Article/details/gndlqkjen.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.fehbvm.com/Article/details/ggsyuzrza.sHtML

[M06] 向标准错误输出
来源：http://baike.zdbjq.cn/Article/details/gcsiefouu.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.zdbjq.cn/Article/details/gsochrnjt.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.hesvh.cn/Article/details/gcbkfmhth.sHtML

JS:   console.error("err")
来源：http://read.share.fehbvm.com/Article/details/gmyczcdeo.sHtML

TS:   console.error("err")
来源：http://blog.fehbvm.com/Article/details/gtctwunwu.sHtML

Java: System.err.println("err")
来源：http://blog.hesvh.cn/Article/details/gzibmyrku.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.hesvh.cn/Article/details/gxwhhrnnh.sHtML

Ruby: warn "err"
来源：http://www.share.zdbjq.cn/Article/details/gfydqaotf.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.zdbjq.cn/Article/details/gycjuqxzl.sHtML

[M07] 判断是否为主入口
来源：http://blog.fehbvm.com/Article/details/gmoktqube.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.hesvh.cn/Article/details/gijbhamoc.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.fehbvm.com/Article/details/gggyqndwd.sHtML

JS:   require.main === module
来源：http://baike.fehbvm.com/Article/details/gtckuoyjh.sHtML

TS:   require.main === module
来源：http://m.share.zdbjq.cn/Article/details/gihecldnq.sHtML

Java: public static void main(String[] args)
来源：http://m.share.fehbvm.com/Article/details/gsutfvsqw.sHtML

Go:   func main()
来源：http://3g.zdbjq.cn/Article/details/glvlwioxp.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.hesvh.cn/Article/details/gjphjyegi.sHtML

C#:   static void Main(string[] args)
来源：http://baike.fehbvm.com/Article/details/gcwfgxbtq.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.fehbvm.com/Article/details/gqehazpjn.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.hesvh.cn/Article/details/gbjmzjnzg.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.fehbvm.com/Article/details/ghefygstd.sHtML

JS:   process.platform;  process.version
来源：http://mobile.zdbjq.cn/Article/details/gggbrrfyo.sHtML

TS:   process.platform;  process.version
来源：http://blog.hesvh.cn/Article/details/gisqijscg.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.hesvh.cn/Article/details/ghemrzrwi.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.zdbjq.cn/Article/details/gvglznmkv.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.zdbjq.cn/Article/details/gajnjcpgg.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.hesvh.cn/Article/details/gmozknyum.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/giuirtvsz.sHtML

N. 数据结构与算法
来源：http://blog.fehbvm.com/Article/details/gcibnciyn.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gzjysyqpg.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.hesvh.cn/Article/details/gnpxojlkk.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gyscmfpnw.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.hesvh.cn/Article/details/glmzcslir.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.hesvh.cn/Article/details/gmupbiznq.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.zdbjq.cn/Article/details/glxtapuzx.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.zdbjq.cn/Article/details/ggknwprqm.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.hesvh.cn/Article/details/glaamjjml.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.zdbjq.cn/Article/details/gjoyiphtm.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gzsllfdjw.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.hesvh.cn/Article/details/gnzulawig.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.hesvh.cn/Article/details/gaisvhjbb.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.hesvh.cn/Article/details/gexlrpasu.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.fehbvm.com/Article/details/gscqxfpzn.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.fehbvm.com/Article/details/glqzfdzhz.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.zdbjq.cn/Article/details/gtnicxzqp.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/grpxnbscu.sHtML

Ruby: arr.sort
来源：http://www.m.share.zdbjq.cn/Article/details/gwctdtadw.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.zdbjq.cn/Article/details/gsxtccenb.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.hesvh.cn/Article/details/gginsppwb.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.fehbvm.com/Article/details/gcuxqrsxk.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.hesvh.cn/Article/details/gkbpceuaq.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.zdbjq.cn/Article/details/ggatirvqf.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.hesvh.cn/Article/details/gzuxpjozl.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.hesvh.cn/Article/details/gkglqpzim.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.zdbjq.cn/Article/details/gsgpoblkj.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.fehbvm.com/Article/details/ghubfahff.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.zdbjq.cn/Article/details/gdiclwhew.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.fehbvm.com/Article/details/gbtvqwajm.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.hesvh.cn/Article/details/gxrghbmvw.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.zdbjq.cn/Article/details/gvxrtlfpd.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.fehbvm.com/Article/details/gwsyqocao.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/ggrkhiqqt.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.fehbvm.com/Article/details/gcdzdenau.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.zdbjq.cn/Article/details/gvefwwcag.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.fehbvm.com/Article/details/gdonkypgp.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.fehbvm.com/Article/details/grgwvhyoa.sHtML

[N05] 最大公约数
来源：http://blog.zdbjq.cn/Article/details/gfchlyxfu.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.fehbvm.com/Article/details/gyatellfu.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.zdbjq.cn/Article/details/gmrzezdol.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.fehbvm.com/Article/details/gwyqgseum.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.hesvh.cn/Article/details/gyhwqmvnc.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.zdbjq.cn/Article/details/givobcqyx.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.zdbjq.cn/Article/details/grmovaqbk.sHtML

Ruby: a.gcd(b)
来源：http://www.share.hesvh.cn/Article/details/gwsgrbzuv.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.fehbvm.com/Article/details/gctzegbom.sHtML

[N06] 判断回文字符串
来源：http://wap.fehbvm.com/Article/details/gposjintp.sHtML

Py:   s == s[::-1]
来源：http://blog.fehbvm.com/Article/details/gjgdtxemp.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.fehbvm.com/Article/details/gmclwnumk.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/ghifnkbpm.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/gqbqpwoae.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.zdbjq.cn/Article/details/gimijfjxa.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.zdbjq.cn/Article/details/gyjnljlcq.sHtML

Ruby: s == s.reverse
来源：http://3g.fehbvm.com/Article/details/gqwlrdblv.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.zdbjq.cn/Article/details/gylsihyob.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.fehbvm.com/Article/details/gkukkabcy.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.zdbjq.cn/Article/details/gqcmmustt.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.zdbjq.cn/Article/details/gjucwfjkp.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.hesvh.cn/Article/details/gccvtxnbn.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.hesvh.cn/Article/details/gdfplbmhb.sHtML

Java: // 手写 HashMap
来源：http://read.share.hesvh.cn/Article/details/gpqlevlei.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.hesvh.cn/Article/details/gygftssnl.sHtML

Ruby: // 手写 Hash
来源：http://baike.fehbvm.com/Article/details/gmvuwrumw.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.zdbjq.cn/Article/details/golttmxrq.sHtML

[N08] 生成全排列
来源：http://mobile.fehbvm.com/Article/details/gffuvnpwc.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.fehbvm.com/Article/details/gdrevhmgs.sHtML

PHP:  // 手写递归交换
来源：http://read.share.zdbjq.cn/Article/details/guzpcyrra.sHtML

JS:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gxdptocua.sHtML

TS:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gqzbbyxsp.sHtML

Java: // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gajoyxdcs.sHtML

Go:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gxezjxsnu.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.zdbjq.cn/Article/details/gjwgnjavb.sHtML

C#:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gfhfgwqhl.sHtML

[N09] 栈与队列
来源：http://m.share.zdbjq.cn/Article/details/gdsvobwtq.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.fehbvm.com/Article/details/gqntujzit.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.hesvh.cn/Article/details/gjptlwteu.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.zdbjq.cn/Article/details/gttpqqyyx.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.zdbjq.cn/Article/details/ggofgvllj.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.fehbvm.com/Article/details/gddqnczhs.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.hesvh.cn/Article/details/gpyphqntg.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.zdbjq.cn/Article/details/goxbhxphn.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.hesvh.cn/Article/details/gfdiclnbq.sHtML

[N10] 链表节点定义
来源：http://baike.zdbjq.cn/Article/details/gkypzadpn.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.hesvh.cn/Article/details/gyravshqh.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.zdbjq.cn/Article/details/gmesmudpa.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.hesvh.cn/Article/details/ggpmbfrsq.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.zdbjq.cn/Article/details/gsmckumlc.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.hesvh.cn/Article/details/gttgsotoi.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.fehbvm.com/Article/details/gcuuuljgh.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.hesvh.cn/Article/details/gciupodgu.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.fehbvm.com/Article/details/ggjgyeyvs.sHtML

[N11] 二叉树中序遍历
来源：http://blog.zdbjq.cn/Article/details/genkqccap.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.zdbjq.cn/Article/details/gbercftwi.sHtML

PHP:  // 手写递归函数
来源：http://wap.fehbvm.com/Article/details/gddjkzspv.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.hesvh.cn/Article/details/gnjaoxuzf.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.hesvh.cn/Article/details/gsfgefyqb.sHtML

Java: // 手写递归
来源：http://read.share.fehbvm.com/Article/details/gljvbwcvi.sHtML

Go:   // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/gihkyeipj.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.hesvh.cn/Article/details/gavxdsovt.sHtML

C#:   // 手写递归
来源：http://www.blog.fehbvm.com/Article/details/ghqqycztt.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.hesvh.cn/Article/details/gnqfdupka.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.zdbjq.cn/Article/details/gdgmgfccx.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.fehbvm.com/Article/details/gqaxpfauw.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.hesvh.cn/Article/details/geoswhtey.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.fehbvm.com/Article/details/gzvtzgwpz.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.zdbjq.cn/Article/details/gnbbupazi.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.zdbjq.cn/Article/details/gjkaomkkl.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.hesvh.cn/Article/details/ggejnejum.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.zdbjq.cn/Article/details/gqzlxrbmn.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gqqcyvwpx.sHtML

O. 并发与异步
来源：http://www.m.share.zdbjq.cn/Article/details/gswbtdewt.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gkzjyuxrv.sHtML

[O01] 启动一个线程
来源：http://www.m.share.hesvh.cn/Article/details/gzvapmhqd.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.hesvh.cn/Article/details/gtkxwhcnc.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.hesvh.cn/Article/details/goznrvugo.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.fehbvm.com/Article/details/gpyfnmsmi.sHtML

TS:   // 同 JS
来源：http://blog.zdbjq.cn/Article/details/glldzhxrv.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.zdbjq.cn/Article/details/gfeqvqrsv.sHtML

Go:   go f()
来源：http://www.blog.zdbjq.cn/Article/details/gxwjozvjf.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.hesvh.cn/Article/details/gnvzqjkhj.sHtML

C#:   Task.Run(() => F());
来源：http://blog.zdbjq.cn/Article/details/gdfepwhpf.sHtML

[O02] 使用线程池
来源：http://www.m.share.zdbjq.cn/Article/details/gbpbtemop.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.hesvh.cn/Article/details/giybnexub.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.fehbvm.com/Article/details/gujjjiszr.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.zdbjq.cn/Article/details/gzlvzbidj.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.fehbvm.com/Article/details/gxlreyxuy.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.hesvh.cn/Article/details/gqallxuox.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.hesvh.cn/Article/details/gifurqijw.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.hesvh.cn/Article/details/gufydwrzc.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.fehbvm.com/Article/details/gfkfhbyvg.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.zdbjq.cn/Article/details/gyyaiumcr.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.zdbjq.cn/Article/details/gehblzckz.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.fehbvm.com/Article/details/gllsiehbg.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.zdbjq.cn/Article/details/gghcneupd.sHtML

TS:   // 同 JS
来源：http://wap.zdbjq.cn/Article/details/gyqahdiby.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.hesvh.cn/Article/details/gretontpo.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.fehbvm.com/Article/details/gdtnqrvec.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.zdbjq.cn/Article/details/gcufjbktn.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.fehbvm.com/Article/details/gdnytdert.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.fehbvm.com/Article/details/gzxqqslds.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.hesvh.cn/Article/details/gajiuehjo.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.hesvh.cn/Article/details/gkonidkhq.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.fehbvm.com/Article/details/geyecraln.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.zdbjq.cn/Article/details/guxjqdqkq.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.hesvh.cn/Article/details/gbomkkjou.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.hesvh.cn/Article/details/geuxvdyzn.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.fehbvm.com/Article/details/gllryoexu.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.fehbvm.com/Article/details/giqbrxria.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.hesvh.cn/Article/details/gpneawzrm.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.hesvh.cn/Article/details/gytmrctvh.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.hesvh.cn/Article/details/gbuolyluq.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.zdbjq.cn/Article/details/gaeildykm.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.hesvh.cn/Article/details/gnmhpftth.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.zdbjq.cn/Article/details/gkbenbgep.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.zdbjq.cn/Article/details/gjmqzform.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.fehbvm.com/Article/details/golztvayy.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.fehbvm.com/Article/details/gzkkhfnwo.sHtML

[O06] 使用进程池
来源：http://www.blog.fehbvm.com/Article/details/goqgohkeg.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.hesvh.cn/Article/details/gfvznwkgt.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.hesvh.cn/Article/details/ggwosqoko.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.zdbjq.cn/Article/details/gxgewodaw.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.hesvh.cn/Article/details/gzcoeaihd.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.hesvh.cn/Article/details/grsmlxhwl.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.hesvh.cn/Article/details/gqqgcpqlf.sHtML

Ruby: // fork 块
来源：http://www.share.zdbjq.cn/Article/details/gudqlkwia.sHtML

C#:   Parallel.For
来源：http://3g.fehbvm.com/Article/details/gbrtwswbw.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gwlvtusgq.sHtML

P. 常用工具函数
来源：http://blog.zdbjq.cn/Article/details/gujzoadmo.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/godzykuho.sHtML

[P01] 生成 UUID
来源：http://www.m.share.fehbvm.com/Article/details/guvflpeps.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.fehbvm.com/Article/details/gxxbpphau.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.fehbvm.com/Article/details/gbhrkjpjt.sHtML

JS:   crypto.randomUUID()
来源：http://blog.hesvh.cn/Article/details/giuvnuueh.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.fehbvm.com/Article/details/grhjgrvgk.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.fehbvm.com/Article/details/gadtszywa.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.zdbjq.cn/Article/details/gsyxotudf.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.fehbvm.com/Article/details/gryvyiamu.sHtML


<!-- 参考信息 -->