代发 wailian999

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.zdbjq.cn/Article/details/glegxwwef.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.zdbjq.cn/Article/details/guoxxarsz.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.zdbjq.cn/Article/details/gprueymfc.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.fehbvm.com/Article/details/grvvjgdky.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wap.hesvh.cn/Article/details/gtjfnlsta.sHtML

[L04] 设置超时
来源：http://read.share.fehbvm.com/Article/details/gddqbwmcc.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.fehbvm.com/Article/details/govzmhjgu.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.zdbjq.cn/Article/details/gwdnmtmdc.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.zdbjq.cn/Article/details/ghszaknlk.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.zdbjq.cn/Article/details/gjlcxbwvb.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.hesvh.cn/Article/details/gpgatuwjt.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.zdbjq.cn/Article/details/gltjfwfot.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.hesvh.cn/Article/details/grrnoaqrc.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.hesvh.cn/Article/details/gdhkhktvm.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.hesvh.cn/Article/details/gckyktnwd.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://read.share.zdbjq.cn/Article/details/gdbmiwzkw.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.zdbjq.cn/Article/details/gtfcuveqw.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.hesvh.cn/Article/details/grsmqcmqd.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.zdbjq.cn/Article/details/gpkepyidp.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.fehbvm.com/Article/details/gabenmefz.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.fehbvm.com/Article/details/gvkdwrmey.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.hesvh.cn/Article/details/gmsxwyegv.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.hesvh.cn/Article/details/gsdmcdifh.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.fehbvm.com/Article/details/grbfpaxig.sHtML

Py:   resp.json()
来源：http://blog.fehbvm.com/Article/details/gxrsiarde.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.zdbjq.cn/Article/details/ggsssvamn.sHtML

JS:   await resp.json()
来源：http://www.share.zdbjq.cn/Article/details/gqgdtxhgh.sHtML

TS:   await resp.json()
来源：http://mobile.hesvh.cn/Article/details/gyylaiowo.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.hesvh.cn/Article/details/gcanfknlk.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.hesvh.cn/Article/details/gyogsnwkp.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.fehbvm.com/Article/details/gvpwvydcc.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.zdbjq.cn/Article/details/gdqorcgif.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.zdbjq.cn/Article/details/gxbradmsf.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.zdbjq.cn/Article/details/gejpberse.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.hesvh.cn/Article/details/gocqeauwx.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.zdbjq.cn/Article/details/gofgpsfwn.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.hesvh.cn/Article/details/gwdgpgumg.sHtML

Java: resp.statusCode()
来源：http://3g.hesvh.cn/Article/details/gxyfvpmsq.sHtML

Go:   resp.StatusCode
来源：http://www.share.fehbvm.com/Article/details/gvpgbyfah.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.fehbvm.com/Article/details/gvuvdwesy.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.hesvh.cn/Article/details/gkccrnqhw.sHtML

[L08] 并发请求多个地址
来源：http://mobile.hesvh.cn/Article/details/gliwisckm.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.fehbvm.com/Article/details/gwpigllzn.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.fehbvm.com/Article/details/gcbukyltp.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fehbvm.com/Article/details/gxodhbnsc.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fehbvm.com/Article/details/gxuwxcbwo.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.fehbvm.com/Article/details/gvpndyghn.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.hesvh.cn/Article/details/gcdijmpln.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.hesvh.cn/Article/details/goanpoytg.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.fehbvm.com/Article/details/geztedbgp.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gypaeqpbj.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.fehbvm.com/Article/details/gjsbxghfq.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gcynsyrhn.sHtML

[M01] 读取命令行参数
来源：http://read.share.fehbvm.com/Article/details/gesaidaol.sHtML

Py:   sys.argv[1:]
来源：http://mobile.fehbvm.com/Article/details/gmhqtynme.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.fehbvm.com/Article/details/gzrthkwjp.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.zdbjq.cn/Article/details/gmohbnanv.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.fehbvm.com/Article/details/gtrcierwi.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.zdbjq.cn/Article/details/ghecuwfpf.sHtML

Go:   os.Args[1:]
来源：http://m.share.fehbvm.com/Article/details/gwttdhakj.sHtML

Ruby: ARGV
来源：http://www.m.share.fehbvm.com/Article/details/gwtsvoctq.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.hesvh.cn/Article/details/gfbcnuwhz.sHtML

[M02] 读取环境变量
来源：http://m.share.hesvh.cn/Article/details/gzdlswlra.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.zdbjq.cn/Article/details/gctwpvmta.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.zdbjq.cn/Article/details/glgjbpcaa.sHtML

JS:   process.env.HOME
来源：http://blog.hesvh.cn/Article/details/gvnjietlg.sHtML

TS:   process.env.HOME
来源：http://3g.fehbvm.com/Article/details/ggvpgwcje.sHtML

Java: System.getenv("HOME")
来源：http://3g.zdbjq.cn/Article/details/gcavvjifj.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.hesvh.cn/Article/details/guawlabal.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.fehbvm.com/Article/details/gloaqgqkj.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.zdbjq.cn/Article/details/gztbhmyjd.sHtML

[M03] 执行外部命令
来源：http://baike.zdbjq.cn/Article/details/glfgtjywt.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.hesvh.cn/Article/details/giigslnkf.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.zdbjq.cn/Article/details/gxpektdjt.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.zdbjq.cn/Article/details/geuelohqc.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.fehbvm.com/Article/details/gslusfoya.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.zdbjq.cn/Article/details/gcsmqcgoc.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.fehbvm.com/Article/details/ghnopkqkv.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.hesvh.cn/Article/details/gpietefqk.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.fehbvm.com/Article/details/gxaqeskyo.sHtML

[M04] 获取当前工作目录
来源：http://mobile.zdbjq.cn/Article/details/gftetuvez.sHtML

Py:   os.getcwd()
来源：http://3g.hesvh.cn/Article/details/gnyxzqrud.sHtML

PHP:  getcwd();
来源：http://3g.fehbvm.com/Article/details/gvmfidgxp.sHtML

JS:   process.cwd()
来源：http://baike.hesvh.cn/Article/details/gcpcqlgch.sHtML

TS:   process.cwd()
来源：http://3g.zdbjq.cn/Article/details/gwlscedds.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.zdbjq.cn/Article/details/gjgbfebss.sHtML

Go:   os.Getwd()
来源：http://3g.fehbvm.com/Article/details/gfnudpjwy.sHtML

Ruby: Dir.pwd
来源：http://wap.hesvh.cn/Article/details/gypsqlqjf.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.hesvh.cn/Article/details/gcmmpqirh.sHtML

[M05] 设置退出码
来源：http://3g.hesvh.cn/Article/details/gbtwvtqhk.sHtML

Py:   sys.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gnwmfwgtv.sHtML

PHP:  exit(1);
来源：http://read.share.fehbvm.com/Article/details/gssvndeve.sHtML

JS:   process.exit(1)
来源：http://baike.hesvh.cn/Article/details/gdqddwmvp.sHtML

TS:   process.exit(1)
来源：http://mobile.fehbvm.com/Article/details/gctubsozq.sHtML

Java: System.exit(1)
来源：http://m.share.fehbvm.com/Article/details/gkregllbd.sHtML

Go:   os.Exit(1)
来源：http://m.share.hesvh.cn/Article/details/gcalbekal.sHtML

Ruby: exit 1
来源：http://www.m.share.fehbvm.com/Article/details/gqubrpimu.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.hesvh.cn/Article/details/gnvjcwafy.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.zdbjq.cn/Article/details/grmctypax.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.zdbjq.cn/Article/details/grjpyqnyh.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.zdbjq.cn/Article/details/gnqqgfylp.sHtML

JS:   console.error("err")
来源：http://www.blog.fehbvm.com/Article/details/gmsfhhmaw.sHtML

TS:   console.error("err")
来源：http://www.m.share.hesvh.cn/Article/details/gknehwqov.sHtML

Java: System.err.println("err")
来源：http://wap.fehbvm.com/Article/details/ghqrpiqrx.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.hesvh.cn/Article/details/gnyeklmof.sHtML

Ruby: warn "err"
来源：http://www.blog.zdbjq.cn/Article/details/gfptqavqv.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.fehbvm.com/Article/details/gswunbuef.sHtML

[M07] 判断是否为主入口
来源：http://mobile.hesvh.cn/Article/details/gbjbfvswn.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.hesvh.cn/Article/details/gybzqedpf.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.zdbjq.cn/Article/details/gvnyvykax.sHtML

JS:   require.main === module
来源：http://blog.fehbvm.com/Article/details/gnlowvhyf.sHtML

TS:   require.main === module
来源：http://wap.zdbjq.cn/Article/details/gasraskzm.sHtML

Java: public static void main(String[] args)
来源：http://read.share.zdbjq.cn/Article/details/gnesogfsv.sHtML

Go:   func main()
来源：http://read.share.hesvh.cn/Article/details/gbdodcxks.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.hesvh.cn/Article/details/gyywxmyty.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.zdbjq.cn/Article/details/gjppcfdqj.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.fehbvm.com/Article/details/gnskhgcuk.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.fehbvm.com/Article/details/gorxidpmk.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.fehbvm.com/Article/details/gskxviejc.sHtML

JS:   process.platform;  process.version
来源：http://m.share.fehbvm.com/Article/details/gkqsculoa.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.hesvh.cn/Article/details/gxbmticrf.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.fehbvm.com/Article/details/gqwwgypuw.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.hesvh.cn/Article/details/gyapzjhtd.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.hesvh.cn/Article/details/gyfplfsep.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.hesvh.cn/Article/details/gewxiespx.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/galpvqcwf.sHtML

N. 数据结构与算法
来源：http://www.m.share.fehbvm.com/Article/details/gpzorjcmc.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gmpiuvsvm.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.hesvh.cn/Article/details/gbrdcletm.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gxcfosnrf.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.fehbvm.com/Article/details/gjqlofvnu.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.hesvh.cn/Article/details/gontioiba.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.fehbvm.com/Article/details/gghcsowbq.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gdjvjrmwg.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/glzpuncnu.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.fehbvm.com/Article/details/gnhvwoikb.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gmreuggmq.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.zdbjq.cn/Article/details/gotwnonoe.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.zdbjq.cn/Article/details/gokeurull.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.hesvh.cn/Article/details/ganpygkav.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.zdbjq.cn/Article/details/giopahdxt.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.zdbjq.cn/Article/details/gjznziqxi.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.fehbvm.com/Article/details/gqmcxotor.sHtML

Go:   slices.Sort(arr)
来源：http://blog.hesvh.cn/Article/details/gzofwabgo.sHtML

Ruby: arr.sort
来源：http://read.share.hesvh.cn/Article/details/ghrztgbna.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.zdbjq.cn/Article/details/gkfsimtrl.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.hesvh.cn/Article/details/geskashgl.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.fehbvm.com/Article/details/gyhikhfyp.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.hesvh.cn/Article/details/gzbtsqgte.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.fehbvm.com/Article/details/gszosqgvk.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.hesvh.cn/Article/details/gllnopzkm.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.hesvh.cn/Article/details/gdbcbhnry.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.zdbjq.cn/Article/details/glowzsbks.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.hesvh.cn/Article/details/gsmaioicj.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.fehbvm.com/Article/details/gwrbgnjti.sHtML

[N04] 斐波那契数列
来源：http://www.blog.fehbvm.com/Article/details/gxossajpm.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.zdbjq.cn/Article/details/gnlrscshz.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.zdbjq.cn/Article/details/gzhtrbglg.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.fehbvm.com/Article/details/gewifafoe.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.hesvh.cn/Article/details/gsxseskgd.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.hesvh.cn/Article/details/gnryhtsoe.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.hesvh.cn/Article/details/ginquypbs.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.hesvh.cn/Article/details/gcjmcpana.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.zdbjq.cn/Article/details/gexkzddzh.sHtML

[N05] 最大公约数
来源：http://mobile.zdbjq.cn/Article/details/grairtcpg.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.hesvh.cn/Article/details/gthklamex.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.hesvh.cn/Article/details/gaoutgehh.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.hesvh.cn/Article/details/gqlkubsfp.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.hesvh.cn/Article/details/gbkvpkwjn.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.zdbjq.cn/Article/details/gpcuhspyf.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.zdbjq.cn/Article/details/gbyqiznym.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.hesvh.cn/Article/details/gcttjiknz.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.fehbvm.com/Article/details/gaecevtoa.sHtML

[N06] 判断回文字符串
来源：http://wap.zdbjq.cn/Article/details/gkhzdfidz.sHtML

Py:   s == s[::-1]
来源：http://www.share.fehbvm.com/Article/details/ginkylemr.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gmulnppbn.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/gqwnecbss.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/gzudrpvzp.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.hesvh.cn/Article/details/ghudciwby.sHtML

Go:   // 双指针从两端比较
来源：http://wap.zdbjq.cn/Article/details/gucjpzcud.sHtML

Ruby: s == s.reverse
来源：http://www.share.fehbvm.com/Article/details/glutyydgh.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.hesvh.cn/Article/details/guysuomxk.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.fehbvm.com/Article/details/guebfnmbj.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.fehbvm.com/Article/details/gzzlnbzoo.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.zdbjq.cn/Article/details/gehpshumf.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.zdbjq.cn/Article/details/gylykoxqi.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.zdbjq.cn/Article/details/glvetvtbg.sHtML

Java: // 手写 HashMap
来源：http://m.share.hesvh.cn/Article/details/gfydjsfrn.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.hesvh.cn/Article/details/gnfuubczx.sHtML

Ruby: // 手写 Hash
来源：http://3g.zdbjq.cn/Article/details/gvxdbhsos.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.hesvh.cn/Article/details/gqquockfi.sHtML

[N08] 生成全排列
来源：http://3g.hesvh.cn/Article/details/gyzwqjwsh.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.hesvh.cn/Article/details/gtmonadaq.sHtML

PHP:  // 手写递归交换
来源：http://wap.zdbjq.cn/Article/details/gzxamlevy.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/grzymqunj.sHtML

TS:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gcgvaqopd.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gytbbzfkg.sHtML

Go:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gbghpmxtr.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.fehbvm.com/Article/details/gfqshikcx.sHtML

C#:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/geddccdqf.sHtML

[N09] 栈与队列
来源：http://wap.hesvh.cn/Article/details/ggynahbhk.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.hesvh.cn/Article/details/gzxsbwyxt.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.fehbvm.com/Article/details/gtzekzxis.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.zdbjq.cn/Article/details/gtorjsshx.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.zdbjq.cn/Article/details/ggsqrtiqi.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.fehbvm.com/Article/details/gmnxoaplm.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.fehbvm.com/Article/details/gqkxelxxw.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.zdbjq.cn/Article/details/guxktyyrd.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.zdbjq.cn/Article/details/gyuvgbelh.sHtML

[N10] 链表节点定义
来源：http://www.share.hesvh.cn/Article/details/gduboluye.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.hesvh.cn/Article/details/gfvegcwsm.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.hesvh.cn/Article/details/gwwkprxaw.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.fehbvm.com/Article/details/gsozeiglb.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.hesvh.cn/Article/details/gpamcsows.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.fehbvm.com/Article/details/ghdyxgseb.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.fehbvm.com/Article/details/gfdphqbjt.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.fehbvm.com/Article/details/gcrivnrmt.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.fehbvm.com/Article/details/gtkbkodzr.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gbgudmovy.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.fehbvm.com/Article/details/gzurihbem.sHtML

PHP:  // 手写递归函数
来源：http://baike.zdbjq.cn/Article/details/gawnzwnbt.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.zdbjq.cn/Article/details/gjisxdbkj.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.fehbvm.com/Article/details/gcixmueed.sHtML

Java: // 手写递归
来源：http://www.share.zdbjq.cn/Article/details/gebvqzure.sHtML

Go:   // 手写递归
来源：http://read.share.fehbvm.com/Article/details/grxbyhksg.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.fehbvm.com/Article/details/gneeakiyx.sHtML

C#:   // 手写递归
来源：http://www.m.share.hesvh.cn/Article/details/ggugyeuzl.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.fehbvm.com/Article/details/gnygqgwir.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.fehbvm.com/Article/details/gydsnrhjr.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.hesvh.cn/Article/details/gddoinopa.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.hesvh.cn/Article/details/gigrlxehq.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.fehbvm.com/Article/details/gkkwsntci.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.fehbvm.com/Article/details/gofsyzeux.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.fehbvm.com/Article/details/gkcqtddts.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.zdbjq.cn/Article/details/gpuubcjic.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.zdbjq.cn/Article/details/grqjkawiq.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gfassglnf.sHtML

O. 并发与异步
来源：http://www.blog.zdbjq.cn/Article/details/gkatmtvrv.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gnrcjjccj.sHtML

[O01] 启动一个线程
来源：http://m.share.fehbvm.com/Article/details/grjqrclfw.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.hesvh.cn/Article/details/gchhftvln.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.fehbvm.com/Article/details/gjcyvxmmk.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.fehbvm.com/Article/details/gmjuukiqx.sHtML

TS:   // 同 JS
来源：http://www.share.fehbvm.com/Article/details/gfpqgmccy.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.zdbjq.cn/Article/details/ghipxljxb.sHtML

Go:   go f()
来源：http://www.blog.hesvh.cn/Article/details/gzlkjocui.sHtML

Ruby: Thread.new { f }
来源：http://m.share.zdbjq.cn/Article/details/geayrqjaq.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.zdbjq.cn/Article/details/glbsckeqq.sHtML

[O02] 使用线程池
来源：http://www.blog.hesvh.cn/Article/details/gkcbdkqxx.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.zdbjq.cn/Article/details/guhauiogq.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.hesvh.cn/Article/details/gkzpjdjbe.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.zdbjq.cn/Article/details/gyyeefekb.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.fehbvm.com/Article/details/gwluaskgc.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.hesvh.cn/Article/details/gnnalwmwh.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.zdbjq.cn/Article/details/gsvtwmpnd.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.fehbvm.com/Article/details/ggjrlcigk.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.hesvh.cn/Article/details/gbbcdzhbx.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.hesvh.cn/Article/details/gfutpogga.sHtML

Py:   with lock: shared += 1
来源：http://m.share.fehbvm.com/Article/details/gdfmqhanm.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.zdbjq.cn/Article/details/gpzzrgopn.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.zdbjq.cn/Article/details/gyjraapyn.sHtML

TS:   // 同 JS
来源：http://blog.zdbjq.cn/Article/details/gixqgoelt.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.zdbjq.cn/Article/details/gmvattziu.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.hesvh.cn/Article/details/gwpchnvlh.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.fehbvm.com/Article/details/gtveiveoc.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.zdbjq.cn/Article/details/gmpviodhx.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.zdbjq.cn/Article/details/godcnvsoi.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.zdbjq.cn/Article/details/gquiqlatt.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.fehbvm.com/Article/details/goslnmwbp.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.fehbvm.com/Article/details/gamvasfij.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.fehbvm.com/Article/details/geqwxgsxq.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.hesvh.cn/Article/details/gfoajkcto.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.fehbvm.com/Article/details/gxkalrzbn.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.zdbjq.cn/Article/details/gskrkpjnn.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.hesvh.cn/Article/details/glanpaejw.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.zdbjq.cn/Article/details/gwpaaurfw.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.fehbvm.com/Article/details/gmotwbgbk.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.zdbjq.cn/Article/details/gaymlmmfh.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.zdbjq.cn/Article/details/gumaysrqs.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.fehbvm.com/Article/details/guawkvgbq.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.fehbvm.com/Article/details/gpdbeicpe.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.hesvh.cn/Article/details/gywyqopiv.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.hesvh.cn/Article/details/ghouqydkf.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.zdbjq.cn/Article/details/gabxqmpmx.sHtML

[O06] 使用进程池
来源：http://www.blog.zdbjq.cn/Article/details/gvpqemslx.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.hesvh.cn/Article/details/gpsfkifyq.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.zdbjq.cn/Article/details/gsbytepbe.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.hesvh.cn/Article/details/gxtganrwj.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.hesvh.cn/Article/details/gxbwgplay.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.fehbvm.com/Article/details/gchbnvlfr.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.hesvh.cn/Article/details/gmskegeug.sHtML

Ruby: // fork 块
来源：http://www.m.share.zdbjq.cn/Article/details/gczqumdei.sHtML

C#:   Parallel.For
来源：http://baike.hesvh.cn/Article/details/gphtonqol.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/ghcowdniw.sHtML

P. 常用工具函数
来源：http://baike.fehbvm.com/Article/details/gcwrjkkcb.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/greomyyzf.sHtML

[P01] 生成 UUID
来源：http://mobile.fehbvm.com/Article/details/gvzkzzqfu.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.hesvh.cn/Article/details/gaasvzfll.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.hesvh.cn/Article/details/gzsiiwels.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.fehbvm.com/Article/details/gcujtbmsw.sHtML


<!-- 参考信息 -->