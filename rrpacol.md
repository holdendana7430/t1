代发 wailian999

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.zdbjq.cn/Article/details/gelozxdcj.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.zdbjq.cn/Article/details/ghyatglwv.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.hesvh.cn/Article/details/gyxrlhhzm.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.hesvh.cn/Article/details/gjacxxqui.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.fehbvm.com/Article/details/gtwgzlrrf.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.zdbjq.cn/Article/details/gxlygsshs.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.zdbjq.cn/Article/details/gwsimgxrl.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.zdbjq.cn/Article/details/gpnicoeji.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.zdbjq.cn/Article/details/gmffknafr.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.zdbjq.cn/Article/details/gciohikau.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.zdbjq.cn/Article/details/gkjvbvcpo.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.hesvh.cn/Article/details/griqfoclm.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.zdbjq.cn/Article/details/gwskfuqpi.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.zdbjq.cn/Article/details/gkqanpbfx.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.zdbjq.cn/Article/details/gmggbkcam.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.zdbjq.cn/Article/details/galftrepy.sHtML

Py:   resp.json()
来源：http://blog.fehbvm.com/Article/details/gawaeyqdx.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.hesvh.cn/Article/details/gagtfqehv.sHtML

JS:   await resp.json()
来源：http://read.share.hesvh.cn/Article/details/gukppyuly.sHtML

TS:   await resp.json()
来源：http://m.share.zdbjq.cn/Article/details/gxywceagj.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.hesvh.cn/Article/details/gghfzudow.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.fehbvm.com/Article/details/gtfdritfo.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.fehbvm.com/Article/details/gtsaifybd.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.fehbvm.com/Article/details/gslkkawvi.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.fehbvm.com/Article/details/gxhywsauh.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.zdbjq.cn/Article/details/gsptbdlnd.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.zdbjq.cn/Article/details/gcamtthcg.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.fehbvm.com/Article/details/gyttgkmsp.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.fehbvm.com/Article/details/gvlzxmclw.sHtML

Java: resp.statusCode()
来源：http://3g.hesvh.cn/Article/details/groazkbce.sHtML

Go:   resp.StatusCode
来源：http://www.blog.zdbjq.cn/Article/details/gtscqowch.sHtML

Ruby: resp.code.to_i
来源：http://www.share.zdbjq.cn/Article/details/gyzvcxwid.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.fehbvm.com/Article/details/ghzigaqed.sHtML

[L08] 并发请求多个地址
来源：http://blog.zdbjq.cn/Article/details/gkwndtayt.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.fehbvm.com/Article/details/groxdwhdi.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.fehbvm.com/Article/details/gfnrsuuau.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fehbvm.com/Article/details/gvnopihyj.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fehbvm.com/Article/details/gvkmhunzv.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.fehbvm.com/Article/details/gatbmunnj.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.fehbvm.com/Article/details/gsufgxznz.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.fehbvm.com/Article/details/gmhfumihr.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.zdbjq.cn/Article/details/gvsgcrhgb.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gbpmcjozk.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.fehbvm.com/Article/details/gpxngytgy.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gkmynlqho.sHtML

[M01] 读取命令行参数
来源：http://www.blog.hesvh.cn/Article/details/gngayaypq.sHtML

Py:   sys.argv[1:]
来源：http://wap.zdbjq.cn/Article/details/ggjucimoh.sHtML

PHP:  $argv;  $argc;
来源：http://wap.hesvh.cn/Article/details/gyycfbjqw.sHtML

JS:   process.argv.slice(2)
来源：http://3g.zdbjq.cn/Article/details/gzqbqhpax.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.hesvh.cn/Article/details/gqqdyxepz.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.fehbvm.com/Article/details/gftlxwlwg.sHtML

Go:   os.Args[1:]
来源：http://3g.fehbvm.com/Article/details/gclfiuijx.sHtML

Ruby: ARGV
来源：http://read.share.fehbvm.com/Article/details/gcvsbfiww.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.fehbvm.com/Article/details/gzxfwbbuw.sHtML

[M02] 读取环境变量
来源：http://mobile.zdbjq.cn/Article/details/georsfzqk.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.fehbvm.com/Article/details/gfemcnnqt.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.hesvh.cn/Article/details/gpjrpetki.sHtML

JS:   process.env.HOME
来源：http://3g.fehbvm.com/Article/details/gybrjbetl.sHtML

TS:   process.env.HOME
来源：http://m.share.hesvh.cn/Article/details/gvlivxjeq.sHtML

Java: System.getenv("HOME")
来源：http://baike.fehbvm.com/Article/details/gdkfyvzrq.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.hesvh.cn/Article/details/gzfkeotzf.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.zdbjq.cn/Article/details/gaabzjejr.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.zdbjq.cn/Article/details/gqjnvrbgg.sHtML

[M03] 执行外部命令
来源：http://www.share.zdbjq.cn/Article/details/gbkbdjbjf.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.zdbjq.cn/Article/details/gnodxfzcr.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.hesvh.cn/Article/details/gceoslxto.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.hesvh.cn/Article/details/gpnjztakg.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.zdbjq.cn/Article/details/gjunbabmk.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.hesvh.cn/Article/details/gvdwxdnaf.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.hesvh.cn/Article/details/gnrkhzfnm.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.fehbvm.com/Article/details/gcqhbtidm.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.zdbjq.cn/Article/details/glcsebwyq.sHtML

[M04] 获取当前工作目录
来源：http://baike.fehbvm.com/Article/details/gyazhuyle.sHtML

Py:   os.getcwd()
来源：http://baike.fehbvm.com/Article/details/gyfppytbi.sHtML

PHP:  getcwd();
来源：http://www.m.share.zdbjq.cn/Article/details/gxyvjyrrb.sHtML

JS:   process.cwd()
来源：http://m.share.fehbvm.com/Article/details/gcvgpdaen.sHtML

TS:   process.cwd()
来源：http://3g.fehbvm.com/Article/details/gdkwsjfzv.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.zdbjq.cn/Article/details/gqdnlqvit.sHtML

Go:   os.Getwd()
来源：http://baike.zdbjq.cn/Article/details/gyqsnynmg.sHtML

Ruby: Dir.pwd
来源：http://wap.fehbvm.com/Article/details/gkxkqrqje.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.hesvh.cn/Article/details/gbpfvpcan.sHtML

[M05] 设置退出码
来源：http://www.m.share.fehbvm.com/Article/details/ghygtltfg.sHtML

Py:   sys.exit(1)
来源：http://m.share.hesvh.cn/Article/details/gebbkkdmy.sHtML

PHP:  exit(1);
来源：http://mobile.hesvh.cn/Article/details/gpvymadyt.sHtML

JS:   process.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gqebsghyu.sHtML

TS:   process.exit(1)
来源：http://3g.hesvh.cn/Article/details/gzdyypfyr.sHtML

Java: System.exit(1)
来源：http://baike.hesvh.cn/Article/details/ghtxbxshx.sHtML

Go:   os.Exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gyszilwxj.sHtML

Ruby: exit 1
来源：http://www.m.share.fehbvm.com/Article/details/givnbcgjq.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.hesvh.cn/Article/details/gejdpmcpg.sHtML

[M06] 向标准错误输出
来源：http://www.blog.hesvh.cn/Article/details/ghqztictt.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.fehbvm.com/Article/details/gkbnjsumx.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.fehbvm.com/Article/details/gfwwruoan.sHtML

JS:   console.error("err")
来源：http://3g.hesvh.cn/Article/details/gsgqhxhua.sHtML

TS:   console.error("err")
来源：http://baike.fehbvm.com/Article/details/grkztymar.sHtML

Java: System.err.println("err")
来源：http://mobile.fehbvm.com/Article/details/gwcbpcgcz.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.hesvh.cn/Article/details/gomettfvf.sHtML

Ruby: warn "err"
来源：http://m.share.hesvh.cn/Article/details/ggyegjbnq.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.fehbvm.com/Article/details/gjvduxtgf.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.hesvh.cn/Article/details/gzzhzfwhm.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.fehbvm.com/Article/details/gjxoouvkk.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.zdbjq.cn/Article/details/gctxiosxb.sHtML

JS:   require.main === module
来源：http://www.blog.fehbvm.com/Article/details/gqwmdbtgk.sHtML

TS:   require.main === module
来源：http://wap.zdbjq.cn/Article/details/grzbcnciv.sHtML

Java: public static void main(String[] args)
来源：http://blog.fehbvm.com/Article/details/gnjuakntn.sHtML

Go:   func main()
来源：http://3g.hesvh.cn/Article/details/glfptpumi.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.hesvh.cn/Article/details/gfqthlpdx.sHtML

C#:   static void Main(string[] args)
来源：http://blog.zdbjq.cn/Article/details/gjvxppker.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.hesvh.cn/Article/details/giapyybib.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.fehbvm.com/Article/details/glnhjwszc.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.zdbjq.cn/Article/details/gyirwvnsk.sHtML

JS:   process.platform;  process.version
来源：http://read.share.zdbjq.cn/Article/details/gcsdaqyxj.sHtML

TS:   process.platform;  process.version
来源：http://m.share.zdbjq.cn/Article/details/ganwlgrgb.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.zdbjq.cn/Article/details/gjhlxxgnz.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.zdbjq.cn/Article/details/gyhgblpwi.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.zdbjq.cn/Article/details/gifkmoesa.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.fehbvm.com/Article/details/gzrlwctrb.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gqnmwjvtj.sHtML

N. 数据结构与算法
来源：http://www.m.share.zdbjq.cn/Article/details/gwawyzwsj.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gegamupwq.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.zdbjq.cn/Article/details/ggvqdsevk.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/guiunortq.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.fehbvm.com/Article/details/glmoryujz.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.zdbjq.cn/Article/details/gjgxmelic.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.hesvh.cn/Article/details/gxhvwccgi.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.hesvh.cn/Article/details/goeybxtai.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.fehbvm.com/Article/details/ghzsdncbl.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.hesvh.cn/Article/details/gmqxrildu.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gcefamsne.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.fehbvm.com/Article/details/gpllqzpxq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.hesvh.cn/Article/details/gpikdaliz.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.zdbjq.cn/Article/details/gctvvufgf.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.hesvh.cn/Article/details/glhgfdoxe.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.hesvh.cn/Article/details/gdbrjrswn.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.zdbjq.cn/Article/details/gzrxzqoim.sHtML

Go:   slices.Sort(arr)
来源：http://wap.fehbvm.com/Article/details/gwdbsqbzy.sHtML

Ruby: arr.sort
来源：http://www.blog.fehbvm.com/Article/details/gzrydwbej.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.fehbvm.com/Article/details/gtfkzntzu.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.zdbjq.cn/Article/details/gnbactyum.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.fehbvm.com/Article/details/gkdolhvhc.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.zdbjq.cn/Article/details/gkxcemjwj.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.hesvh.cn/Article/details/gfyuuvumv.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.hesvh.cn/Article/details/gvuxgetrv.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.hesvh.cn/Article/details/gfwysuauj.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.zdbjq.cn/Article/details/gzyajvvpq.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.fehbvm.com/Article/details/gmaugfcrg.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.hesvh.cn/Article/details/geqoukwra.sHtML

[N04] 斐波那契数列
来源：http://blog.fehbvm.com/Article/details/gsehxwgdm.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.fehbvm.com/Article/details/gdmbxjswp.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.zdbjq.cn/Article/details/gkzzddauv.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.fehbvm.com/Article/details/gbdesktok.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.hesvh.cn/Article/details/gjfnszxli.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.zdbjq.cn/Article/details/gkwjoxtbg.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.fehbvm.com/Article/details/glpqjdztt.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.hesvh.cn/Article/details/gaggcoicg.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/gcwcsiybq.sHtML

[N05] 最大公约数
来源：http://3g.fehbvm.com/Article/details/gjyzygepq.sHtML

Py:   math.gcd(a, b)
来源：http://3g.fehbvm.com/Article/details/gxjzddndz.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.zdbjq.cn/Article/details/gkibxmdvn.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.zdbjq.cn/Article/details/gpogfiqvt.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.fehbvm.com/Article/details/gisvrjitm.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.fehbvm.com/Article/details/gabqhtbae.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.hesvh.cn/Article/details/gyzbzjmoj.sHtML

Ruby: a.gcd(b)
来源：http://read.share.zdbjq.cn/Article/details/gxypjejvb.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.zdbjq.cn/Article/details/gefceybkv.sHtML

[N06] 判断回文字符串
来源：http://read.share.zdbjq.cn/Article/details/gblcjwexc.sHtML

Py:   s == s[::-1]
来源：http://3g.hesvh.cn/Article/details/gijoxksiu.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.fehbvm.com/Article/details/gczqwkiot.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/gclehsarn.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/gcdvscfzc.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.hesvh.cn/Article/details/gyvlpkqsk.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.fehbvm.com/Article/details/gnpyyrhgo.sHtML

Ruby: s == s.reverse
来源：http://blog.zdbjq.cn/Article/details/gtcolnipt.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.fehbvm.com/Article/details/gaupadjmm.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.fehbvm.com/Article/details/ghnncyzos.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.zdbjq.cn/Article/details/gmnzvbpws.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.hesvh.cn/Article/details/gxslzbnrf.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.fehbvm.com/Article/details/grayljyps.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.hesvh.cn/Article/details/gqzvvtecd.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.zdbjq.cn/Article/details/gwqwmjytp.sHtML

Go:   // 手写 map[int]int
来源：http://3g.fehbvm.com/Article/details/gfgvivace.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.zdbjq.cn/Article/details/gtnbnkemv.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.zdbjq.cn/Article/details/gnmpmexah.sHtML

[N08] 生成全排列
来源：http://wap.hesvh.cn/Article/details/gaenyjxah.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.fehbvm.com/Article/details/gufzrogvo.sHtML

PHP:  // 手写递归交换
来源：http://blog.hesvh.cn/Article/details/gjcxvdbod.sHtML

JS:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gcoimgevu.sHtML

TS:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gnwienojc.sHtML

Java: // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/ghdcotmta.sHtML

Go:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gjekihlll.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.zdbjq.cn/Article/details/gfbbitxla.sHtML

C#:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gidzlbovf.sHtML

[N09] 栈与队列
来源：http://3g.hesvh.cn/Article/details/gezzozzmg.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.fehbvm.com/Article/details/glcjpluut.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.hesvh.cn/Article/details/gimvdvxtn.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.fehbvm.com/Article/details/gcmjjzvai.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.hesvh.cn/Article/details/glggtaott.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.zdbjq.cn/Article/details/gzrlcmumq.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.hesvh.cn/Article/details/gpzkpkoro.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.fehbvm.com/Article/details/godrkotok.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.fehbvm.com/Article/details/gompoigkf.sHtML

[N10] 链表节点定义
来源：http://baike.zdbjq.cn/Article/details/gmbisdrua.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.zdbjq.cn/Article/details/gqzrmoydc.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.hesvh.cn/Article/details/gqtpndyqq.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.fehbvm.com/Article/details/gwigorykk.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.zdbjq.cn/Article/details/glughqbgy.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.zdbjq.cn/Article/details/goxkhggni.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.fehbvm.com/Article/details/gbhwyodcc.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.hesvh.cn/Article/details/gzlsueaec.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.fehbvm.com/Article/details/gaafecply.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.fehbvm.com/Article/details/gqwddfyrh.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.hesvh.cn/Article/details/gnoqmycqy.sHtML

PHP:  // 手写递归函数
来源：http://wap.fehbvm.com/Article/details/gfpujpimf.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.fehbvm.com/Article/details/girrfajis.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.zdbjq.cn/Article/details/ghuxkqesh.sHtML

Java: // 手写递归
来源：http://wap.fehbvm.com/Article/details/gsflffcnv.sHtML

Go:   // 手写递归
来源：http://blog.hesvh.cn/Article/details/gtidcmfta.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.hesvh.cn/Article/details/gezunqkns.sHtML

C#:   // 手写递归
来源：http://m.share.hesvh.cn/Article/details/ggbfzcifw.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.fehbvm.com/Article/details/garmxhjua.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.zdbjq.cn/Article/details/garxmitoc.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.hesvh.cn/Article/details/gktvfahbf.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.fehbvm.com/Article/details/gvrcewrbu.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.hesvh.cn/Article/details/giiyipvqm.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.hesvh.cn/Article/details/gwyrrwkbx.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.hesvh.cn/Article/details/ggvkqploe.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.fehbvm.com/Article/details/gpznyaxfe.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.hesvh.cn/Article/details/ghxiekcjt.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gxmqbyflb.sHtML

O. 并发与异步
来源：http://wap.hesvh.cn/Article/details/gfagtgphg.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gpvbunfpy.sHtML

[O01] 启动一个线程
来源：http://wap.zdbjq.cn/Article/details/gxcqoymfw.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.zdbjq.cn/Article/details/gwittrbhc.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.zdbjq.cn/Article/details/gtbgtzepf.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.fehbvm.com/Article/details/gpryeitpl.sHtML

TS:   // 同 JS
来源：http://www.blog.hesvh.cn/Article/details/ghubwfmoj.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.zdbjq.cn/Article/details/gapowpbgg.sHtML

Go:   go f()
来源：http://3g.zdbjq.cn/Article/details/gtemdarqk.sHtML

Ruby: Thread.new { f }
来源：http://mobile.zdbjq.cn/Article/details/gtqaxdlrx.sHtML

C#:   Task.Run(() => F());
来源：http://3g.fehbvm.com/Article/details/gjprvghha.sHtML

[O02] 使用线程池
来源：http://3g.zdbjq.cn/Article/details/gyyjhfadz.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.fehbvm.com/Article/details/glvhagwfr.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.fehbvm.com/Article/details/grpjqpspu.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.zdbjq.cn/Article/details/gbyfyozvn.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.zdbjq.cn/Article/details/gwcqbufni.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.fehbvm.com/Article/details/gmueddjzq.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.hesvh.cn/Article/details/ggdwzpkzo.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.hesvh.cn/Article/details/gstlmqcfa.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.zdbjq.cn/Article/details/glxyoupcy.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.zdbjq.cn/Article/details/gzfdgmwvs.sHtML

Py:   with lock: shared += 1
来源：http://baike.fehbvm.com/Article/details/gviqqypqy.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.hesvh.cn/Article/details/gwhwldmlf.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.fehbvm.com/Article/details/ggpyscilg.sHtML

TS:   // 同 JS
来源：http://www.blog.zdbjq.cn/Article/details/gvoydngap.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.hesvh.cn/Article/details/ghkouprrr.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.fehbvm.com/Article/details/grcshexcm.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.zdbjq.cn/Article/details/gqjnqufvn.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.zdbjq.cn/Article/details/gqycfglqv.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.hesvh.cn/Article/details/gffsomzcu.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.hesvh.cn/Article/details/gyxpcwsvv.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.fehbvm.com/Article/details/gtiwgupgm.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.hesvh.cn/Article/details/gbfpkotoh.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.zdbjq.cn/Article/details/gsjbwajpp.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.zdbjq.cn/Article/details/golfqzrri.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.fehbvm.com/Article/details/gbvccgtjc.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.fehbvm.com/Article/details/gsysrbonn.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.hesvh.cn/Article/details/gtsxpsbdp.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.zdbjq.cn/Article/details/gfmnnyhba.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.zdbjq.cn/Article/details/gqmorcgco.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.zdbjq.cn/Article/details/ghqyvwopo.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.hesvh.cn/Article/details/grfddixyu.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.hesvh.cn/Article/details/gkearifdf.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.hesvh.cn/Article/details/gelfnxwis.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.fehbvm.com/Article/details/gmrsvniol.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.fehbvm.com/Article/details/gqiewoliq.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.hesvh.cn/Article/details/gayrqzomg.sHtML

[O06] 使用进程池
来源：http://3g.fehbvm.com/Article/details/gvegyqmam.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.fehbvm.com/Article/details/gsrmqhikm.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.zdbjq.cn/Article/details/glrvfnxxy.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.hesvh.cn/Article/details/gkxsvxxfr.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.hesvh.cn/Article/details/gpnprvzvl.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.zdbjq.cn/Article/details/ggzjowetv.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.fehbvm.com/Article/details/gajowxzvz.sHtML

Ruby: // fork 块
来源：http://read.share.hesvh.cn/Article/details/gitwivkff.sHtML

C#:   Parallel.For
来源：http://www.share.zdbjq.cn/Article/details/gywwpawwb.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/guxfdvtke.sHtML

P. 常用工具函数
来源：http://www.m.share.zdbjq.cn/Article/details/gbqomoaol.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gjuhzqjfv.sHtML

[P01] 生成 UUID
来源：http://www.m.share.hesvh.cn/Article/details/gilrlastu.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.hesvh.cn/Article/details/gwmuewmqp.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.fehbvm.com/Article/details/ghngbzjyi.sHtML

JS:   crypto.randomUUID()
来源：http://baike.fehbvm.com/Article/details/gvenhbsyp.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.hesvh.cn/Article/details/gvjrrtckb.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.hesvh.cn/Article/details/gczgxgcph.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.fehbvm.com/Article/details/gzcozxxcu.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.fehbvm.com/Article/details/ggkuqibbr.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.zdbjq.cn/Article/details/gkticrwim.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.zdbjq.cn/Article/details/gvytdxhjo.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.hesvh.cn/Article/details/gdmzjjsxa.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.hesvh.cn/Article/details/gayvsxjun.sHtML


<!-- 参考信息 -->