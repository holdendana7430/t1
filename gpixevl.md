代发 wailian999

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.hesvh.cn/Article/details/gcrnunkcg.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.fehbvm.com/Article/details/gtouodaro.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.zdbjq.cn/Article/details/goajcbrgl.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.hesvh.cn/Article/details/ghjujnuuw.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.hesvh.cn/Article/details/gqghunbkk.sHtML

[L04] 设置超时
来源：http://m.share.zdbjq.cn/Article/details/gerkkpqfe.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.zdbjq.cn/Article/details/gfeifgita.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.zdbjq.cn/Article/details/gytphahrj.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.zdbjq.cn/Article/details/gnybapmdy.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.fehbvm.com/Article/details/gmvywrxul.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.hesvh.cn/Article/details/gplwkrfem.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.hesvh.cn/Article/details/gihqznhoa.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.zdbjq.cn/Article/details/gremuahqs.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.zdbjq.cn/Article/details/gzpmjhbsr.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.zdbjq.cn/Article/details/gbnzywjvq.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.fehbvm.com/Article/details/gmtowoajp.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.fehbvm.com/Article/details/gdrwbwuqw.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.hesvh.cn/Article/details/gxhzmheee.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.fehbvm.com/Article/details/gqgflxxwh.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.zdbjq.cn/Article/details/goskhsfxh.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.hesvh.cn/Article/details/ggvxtobkr.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.fehbvm.com/Article/details/gufhelqdf.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/ggrvwgwxx.sHtML

[L06] 解析响应为 JSON
来源：http://3g.fehbvm.com/Article/details/gevdtftec.sHtML

Py:   resp.json()
来源：http://baike.hesvh.cn/Article/details/gfvuxgqxn.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.fehbvm.com/Article/details/gbijpljwk.sHtML

JS:   await resp.json()
来源：http://baike.zdbjq.cn/Article/details/gizhcxkct.sHtML

TS:   await resp.json()
来源：http://read.share.fehbvm.com/Article/details/gkyyxqljy.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.zdbjq.cn/Article/details/gudapkkeo.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.fehbvm.com/Article/details/ggtahmtxf.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.zdbjq.cn/Article/details/gzdwpsypn.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.zdbjq.cn/Article/details/gjqogmxyt.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.fehbvm.com/Article/details/gpraotxtw.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.fehbvm.com/Article/details/gqrbdikhm.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.fehbvm.com/Article/details/gdtzmjtdi.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.zdbjq.cn/Article/details/gmcfcamok.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.zdbjq.cn/Article/details/gqcribedw.sHtML

Java: resp.statusCode()
来源：http://www.blog.zdbjq.cn/Article/details/gkqlxiaso.sHtML

Go:   resp.StatusCode
来源：http://m.share.hesvh.cn/Article/details/gszyrtgjf.sHtML

Ruby: resp.code.to_i
来源：http://3g.hesvh.cn/Article/details/gsljtyufm.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.fehbvm.com/Article/details/gulhsmdbp.sHtML

[L08] 并发请求多个地址
来源：http://www.share.zdbjq.cn/Article/details/gzckgcmdt.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.fehbvm.com/Article/details/gceplyhim.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.fehbvm.com/Article/details/gcwpfasij.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.hesvh.cn/Article/details/gvglzbmmc.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.zdbjq.cn/Article/details/gpdnhcxve.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.fehbvm.com/Article/details/gyfuhqcym.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.fehbvm.com/Article/details/gzcwuxmsl.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.zdbjq.cn/Article/details/gdhiyscac.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.zdbjq.cn/Article/details/ghoguhntm.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gacsmzvzf.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.hesvh.cn/Article/details/gkqglfkcq.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gwcjlxyrd.sHtML

[M01] 读取命令行参数
来源：http://3g.fehbvm.com/Article/details/gumvpznhr.sHtML

Py:   sys.argv[1:]
来源：http://baike.zdbjq.cn/Article/details/gttmrkgik.sHtML

PHP:  $argv;  $argc;
来源：http://blog.zdbjq.cn/Article/details/gxelacztv.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.zdbjq.cn/Article/details/gqqswlqww.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.zdbjq.cn/Article/details/grjemgxdf.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.zdbjq.cn/Article/details/ggtanusjg.sHtML

Go:   os.Args[1:]
来源：http://blog.hesvh.cn/Article/details/guvlixhgu.sHtML

Ruby: ARGV
来源：http://m.share.zdbjq.cn/Article/details/ghaufkusm.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.zdbjq.cn/Article/details/girxsdvgm.sHtML

[M02] 读取环境变量
来源：http://baike.fehbvm.com/Article/details/gmuqimcuf.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.fehbvm.com/Article/details/guekxkitf.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.hesvh.cn/Article/details/gicdjdehk.sHtML

JS:   process.env.HOME
来源：http://3g.zdbjq.cn/Article/details/gbjyljpmb.sHtML

TS:   process.env.HOME
来源：http://3g.fehbvm.com/Article/details/gzjtaeayu.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.fehbvm.com/Article/details/givbtrvmi.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.hesvh.cn/Article/details/gorldlbgk.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.hesvh.cn/Article/details/gtfemcbdq.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.hesvh.cn/Article/details/gtfsqgqrd.sHtML

[M03] 执行外部命令
来源：http://www.share.zdbjq.cn/Article/details/ghlbofkpu.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.zdbjq.cn/Article/details/gljbttgzb.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.fehbvm.com/Article/details/gfpzgtybb.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.hesvh.cn/Article/details/gcnwhutyw.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.zdbjq.cn/Article/details/glqaznzhr.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.fehbvm.com/Article/details/gejpuevrz.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.hesvh.cn/Article/details/glzeuwrzw.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.hesvh.cn/Article/details/giuxultbl.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.fehbvm.com/Article/details/gpijmbikx.sHtML

[M04] 获取当前工作目录
来源：http://wap.hesvh.cn/Article/details/griurzmxs.sHtML

Py:   os.getcwd()
来源：http://read.share.hesvh.cn/Article/details/ggvfzjbhv.sHtML

PHP:  getcwd();
来源：http://www.blog.fehbvm.com/Article/details/glvpwrnfj.sHtML

JS:   process.cwd()
来源：http://baike.zdbjq.cn/Article/details/gqqhypytw.sHtML

TS:   process.cwd()
来源：http://wap.zdbjq.cn/Article/details/gffpchizi.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.zdbjq.cn/Article/details/gmpthlmwd.sHtML

Go:   os.Getwd()
来源：http://wap.fehbvm.com/Article/details/gxjusnkat.sHtML

Ruby: Dir.pwd
来源：http://blog.zdbjq.cn/Article/details/gxncyrpzq.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.zdbjq.cn/Article/details/guwxeradp.sHtML

[M05] 设置退出码
来源：http://wap.zdbjq.cn/Article/details/gltolkana.sHtML

Py:   sys.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gppmtknxn.sHtML

PHP:  exit(1);
来源：http://wap.hesvh.cn/Article/details/ggycecpjf.sHtML

JS:   process.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/ghjtcdmbv.sHtML

TS:   process.exit(1)
来源：http://blog.zdbjq.cn/Article/details/gvenyouwq.sHtML

Java: System.exit(1)
来源：http://baike.hesvh.cn/Article/details/gdwsqcoqv.sHtML

Go:   os.Exit(1)
来源：http://www.blog.fehbvm.com/Article/details/ggyeurzbn.sHtML

Ruby: exit 1
来源：http://baike.hesvh.cn/Article/details/gbiuaxcuw.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.zdbjq.cn/Article/details/gpoxxtvjv.sHtML

[M06] 向标准错误输出
来源：http://wap.fehbvm.com/Article/details/gafekfuin.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.zdbjq.cn/Article/details/gmzrhrdmu.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.zdbjq.cn/Article/details/gdvqgalec.sHtML

JS:   console.error("err")
来源：http://www.share.zdbjq.cn/Article/details/gfyvjwykj.sHtML

TS:   console.error("err")
来源：http://baike.fehbvm.com/Article/details/gbkjxccne.sHtML

Java: System.err.println("err")
来源：http://baike.zdbjq.cn/Article/details/gucddqqgp.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.fehbvm.com/Article/details/gpnkepotu.sHtML

Ruby: warn "err"
来源：http://read.share.zdbjq.cn/Article/details/gjkniyzod.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.zdbjq.cn/Article/details/grcbetink.sHtML

[M07] 判断是否为主入口
来源：http://baike.hesvh.cn/Article/details/gxxizqfxm.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.zdbjq.cn/Article/details/gmnjemwhp.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.hesvh.cn/Article/details/gopdlihag.sHtML

JS:   require.main === module
来源：http://www.share.fehbvm.com/Article/details/gzizilcab.sHtML

TS:   require.main === module
来源：http://m.share.zdbjq.cn/Article/details/gcobfsifx.sHtML

Java: public static void main(String[] args)
来源：http://3g.hesvh.cn/Article/details/gtikexmfp.sHtML

Go:   func main()
来源：http://read.share.hesvh.cn/Article/details/gwuskoykf.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.zdbjq.cn/Article/details/gegmttamp.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.zdbjq.cn/Article/details/gxcwkctdj.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.hesvh.cn/Article/details/gmccwzadl.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.zdbjq.cn/Article/details/gutldlqsl.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.fehbvm.com/Article/details/gvolfeeau.sHtML

JS:   process.platform;  process.version
来源：http://read.share.hesvh.cn/Article/details/gyyrzlxqw.sHtML

TS:   process.platform;  process.version
来源：http://mobile.zdbjq.cn/Article/details/gcvsupnjp.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.zdbjq.cn/Article/details/gvplifnwr.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.zdbjq.cn/Article/details/gmipngqrn.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.hesvh.cn/Article/details/gyizyesur.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.fehbvm.com/Article/details/gsulccrcb.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/ghbwcuakw.sHtML

N. 数据结构与算法
来源：http://www.share.hesvh.cn/Article/details/gmebgvdfr.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gdfogkemk.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.zdbjq.cn/Article/details/gyshxrjag.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.hesvh.cn/Article/details/gfjvxibgw.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.zdbjq.cn/Article/details/gznjrzbzf.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.hesvh.cn/Article/details/guqqklvjs.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.fehbvm.com/Article/details/gdzycyehw.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gqibsaduq.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/ggksvyddx.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.zdbjq.cn/Article/details/gcpyjqmen.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gmcujvprk.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.zdbjq.cn/Article/details/gmgtvqsjx.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.zdbjq.cn/Article/details/grvdboxsm.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.zdbjq.cn/Article/details/gmrsvqzqc.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.hesvh.cn/Article/details/gshrbvagn.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.hesvh.cn/Article/details/gfqczwbnt.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.hesvh.cn/Article/details/gjngcopax.sHtML

Go:   slices.Sort(arr)
来源：http://blog.hesvh.cn/Article/details/gmqxcaupf.sHtML

Ruby: arr.sort
来源：http://wap.hesvh.cn/Article/details/gdbprcouc.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.hesvh.cn/Article/details/gaianporj.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.hesvh.cn/Article/details/gznhsgwjq.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.fehbvm.com/Article/details/ggjxdgxmq.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.zdbjq.cn/Article/details/ghwuhpoyu.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.zdbjq.cn/Article/details/gbzcykhov.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.zdbjq.cn/Article/details/grybsrnch.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.hesvh.cn/Article/details/gtrnyhvhq.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.hesvh.cn/Article/details/gllsgqlzj.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.hesvh.cn/Article/details/gbabzqxca.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.hesvh.cn/Article/details/geajnxmqs.sHtML

[N04] 斐波那契数列
来源：http://3g.hesvh.cn/Article/details/gbzvrpigd.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.fehbvm.com/Article/details/gqkrcckfi.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.zdbjq.cn/Article/details/ganbvlrlq.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.zdbjq.cn/Article/details/ghupgdktd.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/gdvthxjvb.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.zdbjq.cn/Article/details/gnxarvtre.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.zdbjq.cn/Article/details/gkgqcvnce.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.fehbvm.com/Article/details/gwvxvgesa.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/gtzcvkwas.sHtML

[N05] 最大公约数
来源：http://www.share.fehbvm.com/Article/details/ghlvhdnqg.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.hesvh.cn/Article/details/goymgycau.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.zdbjq.cn/Article/details/gikvwuekj.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.zdbjq.cn/Article/details/gdfgpkwcl.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.zdbjq.cn/Article/details/gdvcqomnu.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.fehbvm.com/Article/details/geqrwezmk.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.zdbjq.cn/Article/details/gbmvyggkg.sHtML

Ruby: a.gcd(b)
来源：http://3g.hesvh.cn/Article/details/ghszmdbpr.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.zdbjq.cn/Article/details/gatxtzskl.sHtML

[N06] 判断回文字符串
来源：http://m.share.hesvh.cn/Article/details/gpsckwohn.sHtML

Py:   s == s[::-1]
来源：http://www.share.hesvh.cn/Article/details/gftpdleyu.sHtML

PHP:  $s === strrev($s);
来源：http://3g.fehbvm.com/Article/details/gbjtvpwoz.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/gizazctwc.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/gqdowwaza.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.fehbvm.com/Article/details/gzaxvntvw.sHtML

Go:   // 双指针从两端比较
来源：http://blog.hesvh.cn/Article/details/gtjhsbdws.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.fehbvm.com/Article/details/gbawrhagm.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.hesvh.cn/Article/details/gwafrngub.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.hesvh.cn/Article/details/ggofvftqw.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.zdbjq.cn/Article/details/gszobykme.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.fehbvm.com/Article/details/gqzguatoz.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.hesvh.cn/Article/details/gqfnqvvmu.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.fehbvm.com/Article/details/glgwgudkq.sHtML

Java: // 手写 HashMap
来源：http://baike.fehbvm.com/Article/details/gufueufbp.sHtML

Go:   // 手写 map[int]int
来源：http://wap.zdbjq.cn/Article/details/grvqshgcx.sHtML

Ruby: // 手写 Hash
来源：http://baike.zdbjq.cn/Article/details/gawfbrqyw.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.fehbvm.com/Article/details/gapwxdsps.sHtML

[N08] 生成全排列
来源：http://wap.fehbvm.com/Article/details/gavdgvziq.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gkuohmyng.sHtML

PHP:  // 手写递归交换
来源：http://read.share.zdbjq.cn/Article/details/gzczlsmnj.sHtML

JS:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gtzdyxyqp.sHtML

TS:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gubixyosi.sHtML

Java: // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/geokwifxr.sHtML

Go:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gayemwvxo.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.zdbjq.cn/Article/details/gpkczbswt.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gwdsexirj.sHtML

[N09] 栈与队列
来源：http://www.m.share.zdbjq.cn/Article/details/gqmdnykdn.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.fehbvm.com/Article/details/gfgdnxnfb.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.hesvh.cn/Article/details/gwkndfuui.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.zdbjq.cn/Article/details/gipkwzlie.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.hesvh.cn/Article/details/githdmxbf.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.zdbjq.cn/Article/details/gbakeazdv.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.zdbjq.cn/Article/details/gjtmceadh.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.hesvh.cn/Article/details/gumdjmdsu.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.zdbjq.cn/Article/details/gklevjyzv.sHtML

[N10] 链表节点定义
来源：http://baike.zdbjq.cn/Article/details/gprzykjcp.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.zdbjq.cn/Article/details/gjiopcdou.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.zdbjq.cn/Article/details/gvrwfvncg.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.hesvh.cn/Article/details/gszbfmian.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.fehbvm.com/Article/details/gahuyivfd.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.hesvh.cn/Article/details/gazvexmax.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.zdbjq.cn/Article/details/gvlsqinqt.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.zdbjq.cn/Article/details/gwlluztai.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.fehbvm.com/Article/details/glnojbudz.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.zdbjq.cn/Article/details/gtyaaaqci.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.hesvh.cn/Article/details/guboboijw.sHtML

PHP:  // 手写递归函数
来源：http://mobile.hesvh.cn/Article/details/gifpdmmkp.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.zdbjq.cn/Article/details/gfeugyfok.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.fehbvm.com/Article/details/gdbmlrhjo.sHtML

Java: // 手写递归
来源：http://m.share.hesvh.cn/Article/details/gyrktdege.sHtML

Go:   // 手写递归
来源：http://www.share.hesvh.cn/Article/details/glriecuue.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.fehbvm.com/Article/details/gwujdeidk.sHtML

C#:   // 手写递归
来源：http://www.share.hesvh.cn/Article/details/gxagjlwyz.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.fehbvm.com/Article/details/gcxipbgqw.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.fehbvm.com/Article/details/gjppewiub.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.zdbjq.cn/Article/details/gaeujhvfl.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.zdbjq.cn/Article/details/gzdjowfiv.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.zdbjq.cn/Article/details/gujbuzbgr.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.zdbjq.cn/Article/details/gdrodngks.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.hesvh.cn/Article/details/gdwimwxeh.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.zdbjq.cn/Article/details/gpqdpeizw.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.fehbvm.com/Article/details/gcpsezzck.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/ggkxuminm.sHtML

O. 并发与异步
来源：http://mobile.fehbvm.com/Article/details/gannpdcby.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gneifsfut.sHtML

[O01] 启动一个线程
来源：http://m.share.zdbjq.cn/Article/details/gvswypsje.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.zdbjq.cn/Article/details/garamsmzs.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.zdbjq.cn/Article/details/ganomsscq.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.zdbjq.cn/Article/details/gvbcbnzaw.sHtML

TS:   // 同 JS
来源：http://baike.zdbjq.cn/Article/details/gmqaxujnk.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.fehbvm.com/Article/details/grnqrukuf.sHtML

Go:   go f()
来源：http://wap.fehbvm.com/Article/details/gcmtlrhrv.sHtML

Ruby: Thread.new { f }
来源：http://blog.fehbvm.com/Article/details/gctstemnd.sHtML

C#:   Task.Run(() => F());
来源：http://3g.hesvh.cn/Article/details/gylbwrmlx.sHtML

[O02] 使用线程池
来源：http://3g.zdbjq.cn/Article/details/gtrdweslv.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.hesvh.cn/Article/details/gxavwyasc.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.hesvh.cn/Article/details/gpvxppzbn.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.fehbvm.com/Article/details/gukvtxubq.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.zdbjq.cn/Article/details/gnbcwoeeq.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.fehbvm.com/Article/details/gxpwmixxk.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.zdbjq.cn/Article/details/gkfzjfkre.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.hesvh.cn/Article/details/giqzbntac.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.fehbvm.com/Article/details/gwavscral.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.hesvh.cn/Article/details/gekypuomc.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.hesvh.cn/Article/details/gwjrhktef.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.hesvh.cn/Article/details/gjfbcpmfr.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.zdbjq.cn/Article/details/grppomgng.sHtML

TS:   // 同 JS
来源：http://www.m.share.zdbjq.cn/Article/details/ggtuejjoe.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.fehbvm.com/Article/details/gtlytxbtk.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.fehbvm.com/Article/details/gbwprjums.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.hesvh.cn/Article/details/gvllbyfqf.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.fehbvm.com/Article/details/gsvjdzcun.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.fehbvm.com/Article/details/gowkrgeou.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.fehbvm.com/Article/details/geluhfrzn.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.fehbvm.com/Article/details/ghbtfrkeu.sHtML

JS:   async function f() { await g(); }
来源：http://wap.zdbjq.cn/Article/details/gtqxousca.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.hesvh.cn/Article/details/ghpfogeac.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.hesvh.cn/Article/details/gdlweewpc.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.zdbjq.cn/Article/details/gbfzmjbpc.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.fehbvm.com/Article/details/gslujfjdd.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.fehbvm.com/Article/details/gbthokfxo.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.hesvh.cn/Article/details/gaufauozl.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.zdbjq.cn/Article/details/gvmdamvnm.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.fehbvm.com/Article/details/gnmaksplk.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.fehbvm.com/Article/details/gupqjakrr.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.hesvh.cn/Article/details/gauncuvrm.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.zdbjq.cn/Article/details/gbxayndrh.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.zdbjq.cn/Article/details/grwqegmvq.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.fehbvm.com/Article/details/glqppgmlv.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.fehbvm.com/Article/details/gjtdchchy.sHtML

[O06] 使用进程池
来源：http://blog.zdbjq.cn/Article/details/gzqvwozix.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.hesvh.cn/Article/details/gvdjvsuhx.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.zdbjq.cn/Article/details/gtuvxvfvc.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.zdbjq.cn/Article/details/gaiawtojt.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.zdbjq.cn/Article/details/gdpgdyejx.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.zdbjq.cn/Article/details/gzzhnslst.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.fehbvm.com/Article/details/gxjpfwxve.sHtML

Ruby: // fork 块
来源：http://blog.hesvh.cn/Article/details/gktjllwtf.sHtML

C#:   Parallel.For
来源：http://mobile.zdbjq.cn/Article/details/geamarnwd.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/ghybfmlyo.sHtML

P. 常用工具函数
来源：http://blog.fehbvm.com/Article/details/gxfcqcavp.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gkokuemem.sHtML

[P01] 生成 UUID
来源：http://blog.hesvh.cn/Article/details/gnqbnaiks.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.zdbjq.cn/Article/details/gabgwdqxg.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.hesvh.cn/Article/details/gxprmkbsi.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.zdbjq.cn/Article/details/gdngnyvdo.sHtML


<!-- 参考信息 -->