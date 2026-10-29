代发 wailian999

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.zdbjq.cn/Article/details/gprzdejgd.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.fehbvm.com/Article/details/gbgxsawog.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.fehbvm.com/Article/details/gilgkyooh.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.fehbvm.com/Article/details/ggcaoegab.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.fehbvm.com/Article/details/gzniougww.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.fehbvm.com/Article/details/gmjlvcrfw.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.zdbjq.cn/Article/details/gsbypfpow.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.zdbjq.cn/Article/details/gukdvnhxl.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.fehbvm.com/Article/details/ggaghehzl.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.hesvh.cn/Article/details/gjuhkcucg.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.hesvh.cn/Article/details/gnozkmkrd.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.hesvh.cn/Article/details/gqcjtcvja.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.zdbjq.cn/Article/details/gehkqaqyu.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.zdbjq.cn/Article/details/gxlxozmsr.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.zdbjq.cn/Article/details/gvdnxkvmi.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.hesvh.cn/Article/details/gpjknbbqx.sHtML

Py:   resp.json()
来源：http://mobile.zdbjq.cn/Article/details/gcfglwoon.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.zdbjq.cn/Article/details/gltxsgxlx.sHtML

JS:   await resp.json()
来源：http://blog.hesvh.cn/Article/details/gdupulqcv.sHtML

TS:   await resp.json()
来源：http://baike.hesvh.cn/Article/details/gclcansol.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.zdbjq.cn/Article/details/gielsxils.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.zdbjq.cn/Article/details/gwdgiecmb.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.hesvh.cn/Article/details/ggvymkkmm.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.fehbvm.com/Article/details/gwncwluda.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.fehbvm.com/Article/details/gacivdpfn.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.fehbvm.com/Article/details/gqfqpwomb.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.fehbvm.com/Article/details/gvgvjtbvh.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.hesvh.cn/Article/details/gvizeydok.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.hesvh.cn/Article/details/gpfhjnwsy.sHtML

Java: resp.statusCode()
来源：http://3g.zdbjq.cn/Article/details/gdrugbgyj.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.zdbjq.cn/Article/details/gcudlrtqw.sHtML

Ruby: resp.code.to_i
来源：http://wap.zdbjq.cn/Article/details/gwiyohupc.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.hesvh.cn/Article/details/gthmxhnuj.sHtML

[L08] 并发请求多个地址
来源：http://3g.hesvh.cn/Article/details/gffapagjc.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.zdbjq.cn/Article/details/ggyjynwsf.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.zdbjq.cn/Article/details/glbnkyekx.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fehbvm.com/Article/details/gpdkacbiy.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.zdbjq.cn/Article/details/ggmpibtsh.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.fehbvm.com/Article/details/gkwnsxplw.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.fehbvm.com/Article/details/gedydcpnp.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.zdbjq.cn/Article/details/ghmvkruma.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.fehbvm.com/Article/details/gezdfjhsb.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gfohzfhrw.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.fehbvm.com/Article/details/gcqnymdak.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gedgdoqnv.sHtML

[M01] 读取命令行参数
来源：http://baike.fehbvm.com/Article/details/gjwsuvfil.sHtML

Py:   sys.argv[1:]
来源：http://mobile.fehbvm.com/Article/details/gsfcdcssn.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.fehbvm.com/Article/details/gtbyjaeks.sHtML

JS:   process.argv.slice(2)
来源：http://blog.hesvh.cn/Article/details/gfesmlvhj.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.hesvh.cn/Article/details/ggdseaqbd.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.zdbjq.cn/Article/details/gwudqbxlh.sHtML

Go:   os.Args[1:]
来源：http://mobile.zdbjq.cn/Article/details/gxdgmrxar.sHtML

Ruby: ARGV
来源：http://mobile.zdbjq.cn/Article/details/gmuhprdmr.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.fehbvm.com/Article/details/ggcnbpmlm.sHtML

[M02] 读取环境变量
来源：http://m.share.fehbvm.com/Article/details/ghqyqypfk.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.hesvh.cn/Article/details/gljhcyhcr.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.fehbvm.com/Article/details/gxemhpyca.sHtML

JS:   process.env.HOME
来源：http://3g.zdbjq.cn/Article/details/gyxrukgji.sHtML

TS:   process.env.HOME
来源：http://www.share.hesvh.cn/Article/details/grvdcbvpy.sHtML

Java: System.getenv("HOME")
来源：http://blog.hesvh.cn/Article/details/gjvdfkcaz.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.fehbvm.com/Article/details/gecazivpr.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.zdbjq.cn/Article/details/gvkcrrnso.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.fehbvm.com/Article/details/gwzetdhif.sHtML

[M03] 执行外部命令
来源：http://m.share.zdbjq.cn/Article/details/gvkaozqeg.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.fehbvm.com/Article/details/gfsbnbiqw.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.zdbjq.cn/Article/details/gzdpumdup.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.zdbjq.cn/Article/details/grtxsaspx.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.zdbjq.cn/Article/details/gdxsajwbf.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.hesvh.cn/Article/details/gnbhkjuww.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.zdbjq.cn/Article/details/gqgxewtep.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.zdbjq.cn/Article/details/gtrkjdwvs.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.zdbjq.cn/Article/details/gunrjpltv.sHtML

[M04] 获取当前工作目录
来源：http://blog.fehbvm.com/Article/details/gmxqthbok.sHtML

Py:   os.getcwd()
来源：http://wap.fehbvm.com/Article/details/gtrusduyq.sHtML

PHP:  getcwd();
来源：http://m.share.zdbjq.cn/Article/details/guzfykibz.sHtML

JS:   process.cwd()
来源：http://mobile.zdbjq.cn/Article/details/gghbacujw.sHtML

TS:   process.cwd()
来源：http://wap.zdbjq.cn/Article/details/gijkujubi.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.fehbvm.com/Article/details/gglnaawiv.sHtML

Go:   os.Getwd()
来源：http://blog.fehbvm.com/Article/details/gxiuiipjr.sHtML

Ruby: Dir.pwd
来源：http://mobile.zdbjq.cn/Article/details/ggzbmcsfg.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.fehbvm.com/Article/details/guijdnuin.sHtML

[M05] 设置退出码
来源：http://mobile.hesvh.cn/Article/details/gzeqgkvlg.sHtML

Py:   sys.exit(1)
来源：http://mobile.fehbvm.com/Article/details/glljityzf.sHtML

PHP:  exit(1);
来源：http://mobile.hesvh.cn/Article/details/gphjnbvyp.sHtML

JS:   process.exit(1)
来源：http://www.share.fehbvm.com/Article/details/gbyrlzoqc.sHtML

TS:   process.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gblokkcns.sHtML

Java: System.exit(1)
来源：http://blog.hesvh.cn/Article/details/gbqaeakey.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gdwqsjjpe.sHtML

Ruby: exit 1
来源：http://www.m.share.fehbvm.com/Article/details/gsgyhptsi.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.hesvh.cn/Article/details/gvktywkwu.sHtML

[M06] 向标准错误输出
来源：http://blog.fehbvm.com/Article/details/gwuuhqaof.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.fehbvm.com/Article/details/ghryvxonu.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.fehbvm.com/Article/details/grrouusuf.sHtML

JS:   console.error("err")
来源：http://read.share.hesvh.cn/Article/details/gdaunppzj.sHtML

TS:   console.error("err")
来源：http://read.share.zdbjq.cn/Article/details/gscwraulv.sHtML

Java: System.err.println("err")
来源：http://www.blog.hesvh.cn/Article/details/gcvbmmhjs.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.zdbjq.cn/Article/details/gbbkpdttw.sHtML

Ruby: warn "err"
来源：http://www.share.hesvh.cn/Article/details/geywffpwf.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.fehbvm.com/Article/details/gqxhugoap.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.fehbvm.com/Article/details/gjkwctner.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.zdbjq.cn/Article/details/gmkhfwbzh.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.zdbjq.cn/Article/details/gbhxxyqbn.sHtML

JS:   require.main === module
来源：http://www.blog.hesvh.cn/Article/details/gpwajgskm.sHtML

TS:   require.main === module
来源：http://mobile.hesvh.cn/Article/details/gboagovpd.sHtML

Java: public static void main(String[] args)
来源：http://blog.fehbvm.com/Article/details/gojtnzqhz.sHtML

Go:   func main()
来源：http://blog.fehbvm.com/Article/details/gtvmdupnz.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.fehbvm.com/Article/details/gstfmzjtn.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.hesvh.cn/Article/details/gpvipxalo.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.hesvh.cn/Article/details/godjhdvdz.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.hesvh.cn/Article/details/gcrlscwyj.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.hesvh.cn/Article/details/ghmslvdhd.sHtML

JS:   process.platform;  process.version
来源：http://wap.hesvh.cn/Article/details/golrvaqzd.sHtML

TS:   process.platform;  process.version
来源：http://3g.fehbvm.com/Article/details/getzwyjtt.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.zdbjq.cn/Article/details/goifujpkp.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.zdbjq.cn/Article/details/gypcqghmr.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.hesvh.cn/Article/details/gozvgprjh.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.hesvh.cn/Article/details/gwedsjmau.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gzgpoyvco.sHtML

N. 数据结构与算法
来源：http://www.blog.zdbjq.cn/Article/details/gbqkqkcfz.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/geskmpohg.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.zdbjq.cn/Article/details/gjxbshopx.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.hesvh.cn/Article/details/gawqfmryh.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.fehbvm.com/Article/details/grjfyjkit.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.hesvh.cn/Article/details/gglzviait.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.hesvh.cn/Article/details/govquabqm.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gztzkidxv.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.fehbvm.com/Article/details/gtitzuwys.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.hesvh.cn/Article/details/govvzlcov.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gurkatjqh.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.hesvh.cn/Article/details/gzwtrxzoy.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.fehbvm.com/Article/details/gajpmghmg.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.hesvh.cn/Article/details/gxbvthfzq.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.hesvh.cn/Article/details/gywgmusas.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.zdbjq.cn/Article/details/gukpgquqc.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.fehbvm.com/Article/details/gfuhpdfdn.sHtML

Go:   slices.Sort(arr)
来源：http://wap.zdbjq.cn/Article/details/gefotfdut.sHtML

Ruby: arr.sort
来源：http://read.share.zdbjq.cn/Article/details/ghtpartpc.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.fehbvm.com/Article/details/gwhkopmbf.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.hesvh.cn/Article/details/glueixwjw.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.zdbjq.cn/Article/details/ghzkndzom.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.fehbvm.com/Article/details/gmbyzpvnq.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.hesvh.cn/Article/details/gabgqakkn.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.fehbvm.com/Article/details/gfeqcrxaw.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.zdbjq.cn/Article/details/gyjwygxps.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.fehbvm.com/Article/details/gsggbskrm.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.fehbvm.com/Article/details/gzhaejpnb.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.zdbjq.cn/Article/details/glybhagfc.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.zdbjq.cn/Article/details/gldiaqrew.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.fehbvm.com/Article/details/gmgemocri.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.fehbvm.com/Article/details/gpgxlgrqo.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/gkhyhgjpr.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/gguzniimf.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.zdbjq.cn/Article/details/gtkczkytx.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.hesvh.cn/Article/details/gxckurvkr.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.fehbvm.com/Article/details/gbffffcce.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.hesvh.cn/Article/details/gwftdfgaz.sHtML

[N05] 最大公约数
来源：http://blog.fehbvm.com/Article/details/gbnuzuokr.sHtML

Py:   math.gcd(a, b)
来源：http://blog.zdbjq.cn/Article/details/gfzgcsmyc.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.zdbjq.cn/Article/details/gvddxxfru.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.hesvh.cn/Article/details/gzfufrbtx.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.zdbjq.cn/Article/details/grpoosofw.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.fehbvm.com/Article/details/gwompiphz.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.fehbvm.com/Article/details/gweusfblt.sHtML

Ruby: a.gcd(b)
来源：http://mobile.fehbvm.com/Article/details/gnvlkgiag.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.zdbjq.cn/Article/details/geqlpcfyx.sHtML

[N06] 判断回文字符串
来源：http://baike.hesvh.cn/Article/details/gyuciittv.sHtML

Py:   s == s[::-1]
来源：http://3g.zdbjq.cn/Article/details/gnmaoyper.sHtML

PHP:  $s === strrev($s);
来源：http://baike.fehbvm.com/Article/details/gwjkcdpqd.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/gneeghjix.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/gvoreyfuc.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.fehbvm.com/Article/details/gwockekwf.sHtML

Go:   // 双指针从两端比较
来源：http://3g.hesvh.cn/Article/details/gygkajuke.sHtML

Ruby: s == s.reverse
来源：http://www.share.fehbvm.com/Article/details/ghwmhmchw.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.zdbjq.cn/Article/details/gytvmbtmv.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.zdbjq.cn/Article/details/gbgjegqem.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.zdbjq.cn/Article/details/glvqtjlcu.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.zdbjq.cn/Article/details/gpgwyjpoe.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.fehbvm.com/Article/details/gunkpgyrl.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.zdbjq.cn/Article/details/ggmlskddz.sHtML

Java: // 手写 HashMap
来源：http://m.share.hesvh.cn/Article/details/gfamirntt.sHtML

Go:   // 手写 map[int]int
来源：http://baike.fehbvm.com/Article/details/gxbpdmldf.sHtML

Ruby: // 手写 Hash
来源：http://read.share.zdbjq.cn/Article/details/gbylvjhqd.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.hesvh.cn/Article/details/gzlhjwnyc.sHtML

[N08] 生成全排列
来源：http://www.share.hesvh.cn/Article/details/gbaizqqos.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gfbmzeyhe.sHtML

PHP:  // 手写递归交换
来源：http://3g.zdbjq.cn/Article/details/glqabsgrb.sHtML

JS:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gtvibctyj.sHtML

TS:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/guohjcwvn.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gjaxiteaj.sHtML

Go:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gbgbmxfyy.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.fehbvm.com/Article/details/gmqruawmh.sHtML

C#:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/ghqovxteq.sHtML

[N09] 栈与队列
来源：http://www.m.share.zdbjq.cn/Article/details/gnwiuupgy.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.fehbvm.com/Article/details/gongfezdq.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.fehbvm.com/Article/details/gfiryeoel.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.fehbvm.com/Article/details/ggbcfwudo.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.hesvh.cn/Article/details/gkbxfurlc.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.fehbvm.com/Article/details/gqxhrqkgi.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.zdbjq.cn/Article/details/grjnovydp.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.hesvh.cn/Article/details/gyaqvkpys.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.hesvh.cn/Article/details/gblhzpdfu.sHtML

[N10] 链表节点定义
来源：http://www.share.hesvh.cn/Article/details/gyzzicddb.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.zdbjq.cn/Article/details/gujmrldvd.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.fehbvm.com/Article/details/gxeaaznyp.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.fehbvm.com/Article/details/gieaplchq.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.fehbvm.com/Article/details/gicxzuzai.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.zdbjq.cn/Article/details/gvcfwaite.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.hesvh.cn/Article/details/gjnoczkvs.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.hesvh.cn/Article/details/gdgljdoll.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.zdbjq.cn/Article/details/gnrhwwack.sHtML

[N11] 二叉树中序遍历
来源：http://wap.hesvh.cn/Article/details/gbcclqyjy.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.hesvh.cn/Article/details/gmtrpoibl.sHtML

PHP:  // 手写递归函数
来源：http://blog.zdbjq.cn/Article/details/ghtjwffea.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.zdbjq.cn/Article/details/giboznxla.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.hesvh.cn/Article/details/ghbivtffn.sHtML

Java: // 手写递归
来源：http://www.m.share.fehbvm.com/Article/details/gbmjdfszx.sHtML

Go:   // 手写递归
来源：http://baike.fehbvm.com/Article/details/gsotlwvui.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.zdbjq.cn/Article/details/glxyrzxiv.sHtML

C#:   // 手写递归
来源：http://3g.zdbjq.cn/Article/details/gqddjeiux.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.fehbvm.com/Article/details/gqhzyhwzx.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.fehbvm.com/Article/details/gdpokgwav.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.zdbjq.cn/Article/details/gvvbkidmd.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.hesvh.cn/Article/details/gjypeynad.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.fehbvm.com/Article/details/gbbygddrd.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.hesvh.cn/Article/details/gevdrfngq.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.hesvh.cn/Article/details/gqnbiagnc.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.fehbvm.com/Article/details/gonnncedh.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.fehbvm.com/Article/details/giknexkwc.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gefosdutj.sHtML

O. 并发与异步
来源：http://blog.fehbvm.com/Article/details/gpxdwfbxc.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gpczfufwu.sHtML

[O01] 启动一个线程
来源：http://baike.fehbvm.com/Article/details/ghqvkbasw.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.zdbjq.cn/Article/details/gpudaikuc.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.fehbvm.com/Article/details/gxryxmdsg.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.zdbjq.cn/Article/details/gaqmeoskk.sHtML

TS:   // 同 JS
来源：http://3g.zdbjq.cn/Article/details/gstskdvki.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.zdbjq.cn/Article/details/gmxoeosak.sHtML

Go:   go f()
来源：http://wap.fehbvm.com/Article/details/gvzxksxkc.sHtML

Ruby: Thread.new { f }
来源：http://blog.fehbvm.com/Article/details/gpvnbudeb.sHtML

C#:   Task.Run(() => F());
来源：http://baike.zdbjq.cn/Article/details/gmsgpguul.sHtML

[O02] 使用线程池
来源：http://www.blog.fehbvm.com/Article/details/gioplcaax.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.zdbjq.cn/Article/details/gwanmwkjl.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.hesvh.cn/Article/details/gfievfqon.sHtML

JS:   // worker_threads 线程池
来源：http://blog.hesvh.cn/Article/details/gbnwgzvvo.sHtML

TS:   // worker_threads 线程池
来源：http://3g.hesvh.cn/Article/details/gqwheyclw.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.hesvh.cn/Article/details/glgdxturp.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.hesvh.cn/Article/details/gyvftnigm.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.zdbjq.cn/Article/details/gnndpxmrb.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.fehbvm.com/Article/details/gadzilmld.sHtML

[O03] 加锁保护共享数据
来源：http://baike.zdbjq.cn/Article/details/glfqersfz.sHtML

Py:   with lock: shared += 1
来源：http://mobile.hesvh.cn/Article/details/gsevaudrj.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.fehbvm.com/Article/details/gebymfjva.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.hesvh.cn/Article/details/gdlsrlcrz.sHtML

TS:   // 同 JS
来源：http://www.blog.fehbvm.com/Article/details/gfgeohjla.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.hesvh.cn/Article/details/gezqapyfi.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.fehbvm.com/Article/details/ggrhcmdxj.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.zdbjq.cn/Article/details/gvsvgggay.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.fehbvm.com/Article/details/giszlmghi.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.fehbvm.com/Article/details/gwhruzprz.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.hesvh.cn/Article/details/gedrfzuwc.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.hesvh.cn/Article/details/graumeqtp.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.fehbvm.com/Article/details/grdxiuurj.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.fehbvm.com/Article/details/gckejifzj.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.zdbjq.cn/Article/details/goqkohnlg.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.hesvh.cn/Article/details/gpxkjstjo.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.fehbvm.com/Article/details/gtzhtfjal.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.hesvh.cn/Article/details/gefazftpn.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.fehbvm.com/Article/details/glwmceqgf.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.zdbjq.cn/Article/details/gcpmjfwbk.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.fehbvm.com/Article/details/gxozbvgqw.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.zdbjq.cn/Article/details/gmrzgyznf.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.hesvh.cn/Article/details/gbnupuryu.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.fehbvm.com/Article/details/gpzosupgb.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.zdbjq.cn/Article/details/gdgwokjqi.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.hesvh.cn/Article/details/guobnoubd.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.hesvh.cn/Article/details/goncshafg.sHtML

[O06] 使用进程池
来源：http://www.share.fehbvm.com/Article/details/gbzjutfic.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.fehbvm.com/Article/details/gegjioyvg.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.zdbjq.cn/Article/details/gjpridamt.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.fehbvm.com/Article/details/gcnyyrnpf.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.fehbvm.com/Article/details/gvpaayrre.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.fehbvm.com/Article/details/gtokvmbbb.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.fehbvm.com/Article/details/gbrpoxymh.sHtML

Ruby: // fork 块
来源：http://wap.zdbjq.cn/Article/details/grsvhdxxk.sHtML

C#:   Parallel.For
来源：http://3g.zdbjq.cn/Article/details/goripznou.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gzbiurysh.sHtML

P. 常用工具函数
来源：http://www.share.fehbvm.com/Article/details/gavpoaxjo.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gezbxpizo.sHtML

[P01] 生成 UUID
来源：http://3g.zdbjq.cn/Article/details/genpybmpq.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.hesvh.cn/Article/details/gmmaefipg.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.hesvh.cn/Article/details/gppnocuwa.sHtML

JS:   crypto.randomUUID()
来源：http://3g.hesvh.cn/Article/details/gvtdxgeck.sHtML

TS:   crypto.randomUUID()
来源：http://baike.hesvh.cn/Article/details/gwdgboaqz.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.fehbvm.com/Article/details/ggyxogixg.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.hesvh.cn/Article/details/gsosyomek.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.zdbjq.cn/Article/details/gteiehjne.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.zdbjq.cn/Article/details/gqnyitytw.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.zdbjq.cn/Article/details/gntvirkzi.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.hesvh.cn/Article/details/gnlulxyly.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.hesvh.cn/Article/details/grlbaysjf.sHtML


<!-- 参考信息 -->