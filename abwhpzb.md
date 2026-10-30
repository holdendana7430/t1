代发 wailian999

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.fehbvm.com/Article/details/gkgzcjair.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.zdbjq.cn/Article/details/gkzngilxx.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.fehbvm.com/Article/details/golqigumn.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.hesvh.cn/Article/details/gylmywqyx.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.zdbjq.cn/Article/details/gsfbteott.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.fehbvm.com/Article/details/gmqidiyql.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.zdbjq.cn/Article/details/gwjatiunv.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.hesvh.cn/Article/details/gvdlnhylc.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.fehbvm.com/Article/details/gtqttbcho.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.fehbvm.com/Article/details/grfaqcfht.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.zdbjq.cn/Article/details/gpdprqtnu.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.zdbjq.cn/Article/details/gqqadjsas.sHtML

Py:   resp.json()
来源：http://blog.zdbjq.cn/Article/details/gvcggebha.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.zdbjq.cn/Article/details/gqbzocozs.sHtML

JS:   await resp.json()
来源：http://baike.hesvh.cn/Article/details/gjilpfugo.sHtML

TS:   await resp.json()
来源：http://read.share.fehbvm.com/Article/details/gicsudwsb.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.fehbvm.com/Article/details/gdtkrprwi.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.fehbvm.com/Article/details/gdjdezgat.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.fehbvm.com/Article/details/glurmbeoq.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.hesvh.cn/Article/details/gthvnjyqa.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.zdbjq.cn/Article/details/gukcrwhir.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.fehbvm.com/Article/details/ggbrqxmrn.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.hesvh.cn/Article/details/gfarwazqm.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.hesvh.cn/Article/details/glhrwhnfv.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.fehbvm.com/Article/details/ggtiavooh.sHtML

Java: resp.statusCode()
来源：http://www.blog.fehbvm.com/Article/details/grcyigeup.sHtML

Go:   resp.StatusCode
来源：http://www.blog.fehbvm.com/Article/details/glalkbvie.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.zdbjq.cn/Article/details/goenfqdku.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.fehbvm.com/Article/details/ginxgbefo.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.zdbjq.cn/Article/details/gknfbikkt.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.fehbvm.com/Article/details/gzatcmecl.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.fehbvm.com/Article/details/ggsyxyjew.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fehbvm.com/Article/details/groxdxmbb.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.zdbjq.cn/Article/details/gukddptpa.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.zdbjq.cn/Article/details/gxcvcyoub.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.fehbvm.com/Article/details/gqnnvmspz.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.fehbvm.com/Article/details/gijpdsahp.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.hesvh.cn/Article/details/gsbbfzzae.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/ghugutchu.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.fehbvm.com/Article/details/gibknxbmy.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/ggnwaqpin.sHtML

[M01] 读取命令行参数
来源：http://m.share.zdbjq.cn/Article/details/guqfgqxra.sHtML

Py:   sys.argv[1:]
来源：http://www.share.hesvh.cn/Article/details/grwvecham.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.hesvh.cn/Article/details/gwyuenkrc.sHtML

JS:   process.argv.slice(2)
来源：http://3g.hesvh.cn/Article/details/gluuwghtn.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.hesvh.cn/Article/details/guqwhfych.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.fehbvm.com/Article/details/gkkmhbdho.sHtML

Go:   os.Args[1:]
来源：http://3g.zdbjq.cn/Article/details/gxffnksgv.sHtML

Ruby: ARGV
来源：http://www.blog.hesvh.cn/Article/details/gcrciiytc.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.zdbjq.cn/Article/details/gikmzjidq.sHtML

[M02] 读取环境变量
来源：http://wap.zdbjq.cn/Article/details/gyzxknyos.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.zdbjq.cn/Article/details/gbcvizlwk.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.fehbvm.com/Article/details/gnhllvhks.sHtML

JS:   process.env.HOME
来源：http://wap.hesvh.cn/Article/details/gdaddjflr.sHtML

TS:   process.env.HOME
来源：http://blog.hesvh.cn/Article/details/gjczxoagr.sHtML

Java: System.getenv("HOME")
来源：http://mobile.hesvh.cn/Article/details/gbdnzwjgi.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.zdbjq.cn/Article/details/ggeivrqkk.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.zdbjq.cn/Article/details/gghmvscpr.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.fehbvm.com/Article/details/gbgykkdrq.sHtML

[M03] 执行外部命令
来源：http://wap.fehbvm.com/Article/details/gjsngvsny.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.fehbvm.com/Article/details/gkaoedjbu.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.zdbjq.cn/Article/details/gtqsjmrbn.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.zdbjq.cn/Article/details/gufcfabdr.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.fehbvm.com/Article/details/gsmdloznv.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.zdbjq.cn/Article/details/ghsfsiwqe.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.fehbvm.com/Article/details/gafnfrzjc.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.zdbjq.cn/Article/details/goinzrsnh.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.zdbjq.cn/Article/details/glbesxxpi.sHtML

[M04] 获取当前工作目录
来源：http://read.share.fehbvm.com/Article/details/gidgkykoa.sHtML

Py:   os.getcwd()
来源：http://baike.hesvh.cn/Article/details/gmlyqcwft.sHtML

PHP:  getcwd();
来源：http://3g.fehbvm.com/Article/details/gncajxzto.sHtML

JS:   process.cwd()
来源：http://3g.hesvh.cn/Article/details/gxhqfotgx.sHtML

TS:   process.cwd()
来源：http://wap.hesvh.cn/Article/details/gvzwegsqu.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.hesvh.cn/Article/details/ggqrpimam.sHtML

Go:   os.Getwd()
来源：http://www.blog.hesvh.cn/Article/details/gumtabqpi.sHtML

Ruby: Dir.pwd
来源：http://mobile.fehbvm.com/Article/details/gswohestj.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.zdbjq.cn/Article/details/gtxmkzbfz.sHtML

[M05] 设置退出码
来源：http://read.share.zdbjq.cn/Article/details/gqmxhndhe.sHtML

Py:   sys.exit(1)
来源：http://mobile.hesvh.cn/Article/details/gpfkzssew.sHtML

PHP:  exit(1);
来源：http://mobile.hesvh.cn/Article/details/ghpqzmcwd.sHtML

JS:   process.exit(1)
来源：http://www.share.fehbvm.com/Article/details/gnryigpbs.sHtML

TS:   process.exit(1)
来源：http://m.share.fehbvm.com/Article/details/gaiemrdhj.sHtML

Java: System.exit(1)
来源：http://www.share.hesvh.cn/Article/details/gznvdtayz.sHtML

Go:   os.Exit(1)
来源：http://wap.hesvh.cn/Article/details/gdwbjwofd.sHtML

Ruby: exit 1
来源：http://www.m.share.zdbjq.cn/Article/details/gpaakcmnq.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.hesvh.cn/Article/details/guemzawhs.sHtML

[M06] 向标准错误输出
来源：http://wap.fehbvm.com/Article/details/gxkyoergh.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.hesvh.cn/Article/details/ghnxubcgz.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.zdbjq.cn/Article/details/gpvqfukao.sHtML

JS:   console.error("err")
来源：http://wap.fehbvm.com/Article/details/ghspbcwaq.sHtML

TS:   console.error("err")
来源：http://baike.fehbvm.com/Article/details/gtwrgfhym.sHtML

Java: System.err.println("err")
来源：http://www.blog.zdbjq.cn/Article/details/gtiboumnn.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.fehbvm.com/Article/details/gyxfuiarh.sHtML

Ruby: warn "err"
来源：http://blog.hesvh.cn/Article/details/ghwpkygnl.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.fehbvm.com/Article/details/gsvtkslmp.sHtML

[M07] 判断是否为主入口
来源：http://read.share.fehbvm.com/Article/details/gvkiphzuv.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.hesvh.cn/Article/details/gpviqmtmf.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.zdbjq.cn/Article/details/ghqgqvfqp.sHtML

JS:   require.main === module
来源：http://www.m.share.fehbvm.com/Article/details/gbmuwloxd.sHtML

TS:   require.main === module
来源：http://www.m.share.zdbjq.cn/Article/details/ggksciwaw.sHtML

Java: public static void main(String[] args)
来源：http://wap.fehbvm.com/Article/details/gpjcftuqs.sHtML

Go:   func main()
来源：http://blog.zdbjq.cn/Article/details/gcefdbhty.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.hesvh.cn/Article/details/gcpuvwhwn.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.zdbjq.cn/Article/details/gkvvxpdnp.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.hesvh.cn/Article/details/gukjluurc.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.zdbjq.cn/Article/details/gdqaleqca.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.fehbvm.com/Article/details/geaatigjc.sHtML

JS:   process.platform;  process.version
来源：http://www.share.fehbvm.com/Article/details/gviznfoao.sHtML

TS:   process.platform;  process.version
来源：http://3g.zdbjq.cn/Article/details/gegzhnjmi.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.zdbjq.cn/Article/details/getesjeqd.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.zdbjq.cn/Article/details/giwpnjket.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.fehbvm.com/Article/details/gtibxthgs.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.hesvh.cn/Article/details/gtxnwifpi.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gyejlbzqb.sHtML

N. 数据结构与算法
来源：http://www.blog.hesvh.cn/Article/details/gngkisrpj.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gehchynen.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.hesvh.cn/Article/details/gjqwqtmdg.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/glprcveee.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.fehbvm.com/Article/details/gxzqcphqq.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.fehbvm.com/Article/details/guzpiyapt.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.hesvh.cn/Article/details/gzdmichly.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gzsyinvut.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gdgxtykft.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.fehbvm.com/Article/details/gzvxfjiwf.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gmhmgtmgk.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.hesvh.cn/Article/details/gfeckotby.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.hesvh.cn/Article/details/gjfxgjghd.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.zdbjq.cn/Article/details/gjogxdaom.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.hesvh.cn/Article/details/gldbmkqfg.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.zdbjq.cn/Article/details/gwuqpeeld.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.fehbvm.com/Article/details/grlharxlq.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.zdbjq.cn/Article/details/gpbkmbwyk.sHtML

Ruby: arr.sort
来源：http://blog.zdbjq.cn/Article/details/gjeuiukpq.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.zdbjq.cn/Article/details/ggvwxlcpb.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.fehbvm.com/Article/details/gqcagyxrj.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.zdbjq.cn/Article/details/gtcmiwgmz.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.hesvh.cn/Article/details/gehnwkrme.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.hesvh.cn/Article/details/gtanhkxtk.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.zdbjq.cn/Article/details/grjptaviy.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.hesvh.cn/Article/details/ginpvkiix.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.fehbvm.com/Article/details/gjsemhpne.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.fehbvm.com/Article/details/gwiwovfdy.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.zdbjq.cn/Article/details/gbbvjfhjm.sHtML

[N04] 斐波那契数列
来源：http://3g.hesvh.cn/Article/details/gzgjaknhp.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.fehbvm.com/Article/details/gatihsrft.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.hesvh.cn/Article/details/gcrypcrpv.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.hesvh.cn/Article/details/glnrpbvbd.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.fehbvm.com/Article/details/gnogsreep.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.zdbjq.cn/Article/details/gjvtgagel.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.fehbvm.com/Article/details/gzviovipf.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.zdbjq.cn/Article/details/gllgechkm.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.fehbvm.com/Article/details/gspiyksro.sHtML

[N05] 最大公约数
来源：http://m.share.hesvh.cn/Article/details/gyoynxalx.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.fehbvm.com/Article/details/grugornph.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.zdbjq.cn/Article/details/gjpjmwiuv.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.hesvh.cn/Article/details/gecjhmvqc.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.zdbjq.cn/Article/details/gzakpggjn.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.zdbjq.cn/Article/details/gehefjjjt.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.hesvh.cn/Article/details/gyhdnmudc.sHtML

Ruby: a.gcd(b)
来源：http://wap.fehbvm.com/Article/details/ghkejwxju.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.fehbvm.com/Article/details/gqbcthdiu.sHtML

[N06] 判断回文字符串
来源：http://read.share.fehbvm.com/Article/details/gtsfppjwx.sHtML

Py:   s == s[::-1]
来源：http://blog.zdbjq.cn/Article/details/gqbsejiea.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.fehbvm.com/Article/details/garrovcqp.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/gukbtnmnw.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/godxerunm.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.hesvh.cn/Article/details/gcnxyiifb.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.zdbjq.cn/Article/details/glcgaxsam.sHtML

Ruby: s == s.reverse
来源：http://baike.hesvh.cn/Article/details/gefxvqchu.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.zdbjq.cn/Article/details/gxkgjsckz.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.zdbjq.cn/Article/details/gindfbern.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.zdbjq.cn/Article/details/gtbybelkx.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.hesvh.cn/Article/details/goncchwll.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.fehbvm.com/Article/details/gvpsywezo.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.hesvh.cn/Article/details/gbtloonpw.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.hesvh.cn/Article/details/gjfqzaggj.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.zdbjq.cn/Article/details/gqnzmbotf.sHtML

Ruby: // 手写 Hash
来源：http://m.share.zdbjq.cn/Article/details/gpmumzsbv.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.zdbjq.cn/Article/details/gknayvcod.sHtML

[N08] 生成全排列
来源：http://3g.zdbjq.cn/Article/details/gdhpkciny.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.fehbvm.com/Article/details/gelkgdhag.sHtML

PHP:  // 手写递归交换
来源：http://www.share.fehbvm.com/Article/details/gldjbnlqz.sHtML

JS:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/ganikhlwb.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gexyrmqes.sHtML

Java: // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/ggyibwmvj.sHtML

Go:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gururqdhp.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.zdbjq.cn/Article/details/gfpmnnzxv.sHtML

C#:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gysvgrmqp.sHtML

[N09] 栈与队列
来源：http://baike.hesvh.cn/Article/details/gfubtwyiu.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.zdbjq.cn/Article/details/gwbmrqren.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.zdbjq.cn/Article/details/grjrehmhd.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.zdbjq.cn/Article/details/gzrarwbnw.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.hesvh.cn/Article/details/gxvhgsihm.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.hesvh.cn/Article/details/gitvghmxi.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.fehbvm.com/Article/details/giliszhnl.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.fehbvm.com/Article/details/gkjeswtrp.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.hesvh.cn/Article/details/gpxdrfmqf.sHtML

[N10] 链表节点定义
来源：http://blog.zdbjq.cn/Article/details/gsftqxoec.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.hesvh.cn/Article/details/gjftyqtzk.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.fehbvm.com/Article/details/gcffuiwcr.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.zdbjq.cn/Article/details/gjofniktk.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.hesvh.cn/Article/details/gsljimiic.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.fehbvm.com/Article/details/geapapqlm.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.hesvh.cn/Article/details/gpgdbcddg.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.zdbjq.cn/Article/details/gsobffwxi.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.hesvh.cn/Article/details/gmjpnblzt.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.fehbvm.com/Article/details/gvpsxbhli.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.hesvh.cn/Article/details/gcfyljarp.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.fehbvm.com/Article/details/gyejzcdah.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.zdbjq.cn/Article/details/gqwkkmtml.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.zdbjq.cn/Article/details/gakxtvsuy.sHtML

Java: // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/gnhrogjla.sHtML

Go:   // 手写递归
来源：http://m.share.hesvh.cn/Article/details/gnhslqbms.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.hesvh.cn/Article/details/giummghcy.sHtML

C#:   // 手写递归
来源：http://www.share.zdbjq.cn/Article/details/gdwhadivw.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.hesvh.cn/Article/details/ghlhiapsp.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.fehbvm.com/Article/details/gsxjxvgoj.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.zdbjq.cn/Article/details/gbdkdzehf.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.hesvh.cn/Article/details/ghwbhsxtr.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.fehbvm.com/Article/details/grxiuqtzz.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.hesvh.cn/Article/details/ghirtkvut.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.zdbjq.cn/Article/details/gclvlqqnl.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.hesvh.cn/Article/details/geuaycqdv.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.zdbjq.cn/Article/details/gsmnyunib.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gsscvfmlh.sHtML

O. 并发与异步
来源：http://3g.zdbjq.cn/Article/details/gndozbeej.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gaznmdhjk.sHtML

[O01] 启动一个线程
来源：http://wap.fehbvm.com/Article/details/goyztpphe.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.hesvh.cn/Article/details/gseajigfu.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.hesvh.cn/Article/details/gffyrvqtc.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.zdbjq.cn/Article/details/giojsppcd.sHtML

TS:   // 同 JS
来源：http://www.blog.fehbvm.com/Article/details/gozalllsb.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.hesvh.cn/Article/details/giqformut.sHtML

Go:   go f()
来源：http://blog.fehbvm.com/Article/details/gplzokwxa.sHtML

Ruby: Thread.new { f }
来源：http://mobile.hesvh.cn/Article/details/gverydtfn.sHtML

C#:   Task.Run(() => F());
来源：http://wap.fehbvm.com/Article/details/gxtffasfa.sHtML

[O02] 使用线程池
来源：http://www.share.hesvh.cn/Article/details/gkrvjcjij.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.hesvh.cn/Article/details/gjcmigfxd.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.hesvh.cn/Article/details/goydlnomg.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.zdbjq.cn/Article/details/gfhhxndrx.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.fehbvm.com/Article/details/gwnwddxnf.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.zdbjq.cn/Article/details/gvaslxrlm.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.hesvh.cn/Article/details/gtamdpnmq.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.hesvh.cn/Article/details/gildnxyha.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.hesvh.cn/Article/details/gwecipokf.sHtML

[O03] 加锁保护共享数据
来源：http://baike.zdbjq.cn/Article/details/genvioswq.sHtML

Py:   with lock: shared += 1
来源：http://m.share.fehbvm.com/Article/details/gekupfikw.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.zdbjq.cn/Article/details/gjaoisoen.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.fehbvm.com/Article/details/gdauognhn.sHtML

TS:   // 同 JS
来源：http://mobile.fehbvm.com/Article/details/gagckaxpd.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.hesvh.cn/Article/details/ghroqjdsa.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.fehbvm.com/Article/details/ghaxlxdgi.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.zdbjq.cn/Article/details/goyhyvvqv.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.fehbvm.com/Article/details/gtrhcqack.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.zdbjq.cn/Article/details/gvupnnfmx.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.hesvh.cn/Article/details/gwnopwwex.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.fehbvm.com/Article/details/ggkmhgaql.sHtML

JS:   async function f() { await g(); }
来源：http://blog.zdbjq.cn/Article/details/gtvozzoej.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.hesvh.cn/Article/details/ghyutfcko.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.fehbvm.com/Article/details/gtklztsxq.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.zdbjq.cn/Article/details/gjwdfnqpr.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.fehbvm.com/Article/details/giqeuwmrj.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.hesvh.cn/Article/details/gjsmpvvct.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.hesvh.cn/Article/details/gxljxxinl.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.zdbjq.cn/Article/details/gfhohitmr.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.zdbjq.cn/Article/details/gjemqukef.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.hesvh.cn/Article/details/gvevtehgu.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.hesvh.cn/Article/details/goxktpyad.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.hesvh.cn/Article/details/gusswrtyt.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.zdbjq.cn/Article/details/guxuirrpv.sHtML

Ruby: threads.map(&:join)
来源：http://3g.zdbjq.cn/Article/details/gngqxaofo.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.zdbjq.cn/Article/details/gjugickxv.sHtML

[O06] 使用进程池
来源：http://m.share.zdbjq.cn/Article/details/gobzilyzj.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.fehbvm.com/Article/details/gipcbghnl.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.fehbvm.com/Article/details/gpxxkzhkd.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.fehbvm.com/Article/details/gyrpztftb.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.fehbvm.com/Article/details/gpcnqjotz.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.fehbvm.com/Article/details/gluzrtcvm.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.fehbvm.com/Article/details/gjcaelpij.sHtML

Ruby: // fork 块
来源：http://wap.zdbjq.cn/Article/details/gjbvikwoa.sHtML

C#:   Parallel.For
来源：http://blog.fehbvm.com/Article/details/gqmidlnte.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/ggnwihzxe.sHtML

P. 常用工具函数
来源：http://3g.fehbvm.com/Article/details/gaxauobfp.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gshjejcby.sHtML

[P01] 生成 UUID
来源：http://wap.fehbvm.com/Article/details/gfdtzxkba.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.zdbjq.cn/Article/details/gbohqlqfk.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.fehbvm.com/Article/details/gpaemnxbd.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.zdbjq.cn/Article/details/gtihmirnw.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.hesvh.cn/Article/details/gtahexqzu.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.hesvh.cn/Article/details/gtsyhqyjl.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.zdbjq.cn/Article/details/gusbeptxf.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.fehbvm.com/Article/details/gpyxjndsb.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.fehbvm.com/Article/details/glepzjaow.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.fehbvm.com/Article/details/gqcsczhrv.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.hesvh.cn/Article/details/ghqrakxij.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.fehbvm.com/Article/details/gtpvgesxz.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.fehbvm.com/Article/details/glhyqblud.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.zdbjq.cn/Article/details/gtwztqsit.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.zdbjq.cn/Article/details/gidrqswyl.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.zdbjq.cn/Article/details/gciqidqah.sHtML


<!-- 参考信息 -->