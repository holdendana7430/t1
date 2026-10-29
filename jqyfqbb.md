代发 wailian999

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.hesvh.cn/Article/details/gzdpdifxm.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.fehbvm.com/Article/details/gqjnneiev.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.fehbvm.com/Article/details/gyhzexlld.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.fehbvm.com/Article/details/gkzfasngu.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.fehbvm.com/Article/details/ggrftscem.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.fehbvm.com/Article/details/gzjzylufp.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.zdbjq.cn/Article/details/gdhbsjrvy.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.hesvh.cn/Article/details/gccmtivvc.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://m.share.fehbvm.com/Article/details/gwctbzyds.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.hesvh.cn/Article/details/glmbembel.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gfeorfyjy.sHtML

[L06] 解析响应为 JSON
来源：http://3g.hesvh.cn/Article/details/geghpaffb.sHtML

Py:   resp.json()
来源：http://m.share.hesvh.cn/Article/details/guljxjksf.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.hesvh.cn/Article/details/gacaushga.sHtML

JS:   await resp.json()
来源：http://www.m.share.zdbjq.cn/Article/details/gvlcfosrc.sHtML

TS:   await resp.json()
来源：http://wap.zdbjq.cn/Article/details/gtjqztpin.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.fehbvm.com/Article/details/gegrgdafo.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.zdbjq.cn/Article/details/ggdjtzzgp.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.fehbvm.com/Article/details/goawejmcx.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.hesvh.cn/Article/details/gwwnibzuh.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.zdbjq.cn/Article/details/ghgxgnupg.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.zdbjq.cn/Article/details/guqsjyxyd.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.hesvh.cn/Article/details/geqdvqnzv.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.hesvh.cn/Article/details/glkrubxto.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.zdbjq.cn/Article/details/gwhymowai.sHtML

Java: resp.statusCode()
来源：http://baike.fehbvm.com/Article/details/guhkgphyt.sHtML

Go:   resp.StatusCode
来源：http://blog.fehbvm.com/Article/details/gnfgfagjh.sHtML

Ruby: resp.code.to_i
来源：http://read.share.hesvh.cn/Article/details/gqimzuzyv.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.fehbvm.com/Article/details/gvqwmzcpi.sHtML

[L08] 并发请求多个地址
来源：http://www.share.hesvh.cn/Article/details/gxvscmiin.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.hesvh.cn/Article/details/gazqoqwcy.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.zdbjq.cn/Article/details/gewkbbmkd.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fehbvm.com/Article/details/gbekfldom.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.hesvh.cn/Article/details/grlvauvmr.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.fehbvm.com/Article/details/gzgkgftda.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.zdbjq.cn/Article/details/gjfscjmir.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.hesvh.cn/Article/details/gdhuqafqj.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.hesvh.cn/Article/details/gubksnlkc.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gogouiyme.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.fehbvm.com/Article/details/goeforsyf.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gtvgoiuma.sHtML

[M01] 读取命令行参数
来源：http://3g.hesvh.cn/Article/details/gwrluxbrn.sHtML

Py:   sys.argv[1:]
来源：http://m.share.zdbjq.cn/Article/details/gnfxddbzr.sHtML

PHP:  $argv;  $argc;
来源：http://blog.zdbjq.cn/Article/details/gpxvrtbxg.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.zdbjq.cn/Article/details/gqjcxlsio.sHtML

TS:   process.argv.slice(2)
来源：http://baike.hesvh.cn/Article/details/ghjmxgmdy.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.hesvh.cn/Article/details/guvdqbygy.sHtML

Go:   os.Args[1:]
来源：http://www.share.fehbvm.com/Article/details/goeyggxpx.sHtML

Ruby: ARGV
来源：http://wap.hesvh.cn/Article/details/gveizxqln.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.zdbjq.cn/Article/details/ghyvluofh.sHtML

[M02] 读取环境变量
来源：http://3g.fehbvm.com/Article/details/gokgvcmet.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.hesvh.cn/Article/details/ggnjqhhnk.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.fehbvm.com/Article/details/gbfedckir.sHtML

JS:   process.env.HOME
来源：http://www.blog.zdbjq.cn/Article/details/gnwgtrlkx.sHtML

TS:   process.env.HOME
来源：http://mobile.zdbjq.cn/Article/details/ggjswwang.sHtML

Java: System.getenv("HOME")
来源：http://blog.hesvh.cn/Article/details/gurnyxrii.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/gaxxiqjek.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.fehbvm.com/Article/details/gisaghnou.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.zdbjq.cn/Article/details/gxlcebzxz.sHtML

[M03] 执行外部命令
来源：http://mobile.hesvh.cn/Article/details/grizyzkgb.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.zdbjq.cn/Article/details/gczaxkxta.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.zdbjq.cn/Article/details/gkaxmqogb.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.zdbjq.cn/Article/details/gjgsbiamx.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.fehbvm.com/Article/details/gnvrployy.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.zdbjq.cn/Article/details/gcfscpbzz.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.zdbjq.cn/Article/details/gecdrlrji.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.hesvh.cn/Article/details/gnhtazwoo.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.fehbvm.com/Article/details/gkwpmiter.sHtML

[M04] 获取当前工作目录
来源：http://www.share.hesvh.cn/Article/details/gdjqvypjd.sHtML

Py:   os.getcwd()
来源：http://baike.zdbjq.cn/Article/details/gflnmefkm.sHtML

PHP:  getcwd();
来源：http://www.blog.hesvh.cn/Article/details/gxfpptbby.sHtML

JS:   process.cwd()
来源：http://3g.hesvh.cn/Article/details/glnixfebf.sHtML

TS:   process.cwd()
来源：http://www.m.share.hesvh.cn/Article/details/gfjwyahho.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.zdbjq.cn/Article/details/gtmjapmuh.sHtML

Go:   os.Getwd()
来源：http://www.blog.fehbvm.com/Article/details/gvgxwwcnx.sHtML

Ruby: Dir.pwd
来源：http://www.share.fehbvm.com/Article/details/gnynrlnhw.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.hesvh.cn/Article/details/gtgretqtr.sHtML

[M05] 设置退出码
来源：http://baike.zdbjq.cn/Article/details/gsrmmlnvd.sHtML

Py:   sys.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/godamyxdb.sHtML

PHP:  exit(1);
来源：http://baike.hesvh.cn/Article/details/grdkumshg.sHtML

JS:   process.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gjvluozxi.sHtML

TS:   process.exit(1)
来源：http://www.share.fehbvm.com/Article/details/gwurlwtne.sHtML

Java: System.exit(1)
来源：http://m.share.hesvh.cn/Article/details/gnygukykk.sHtML

Go:   os.Exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gxayakwcr.sHtML

Ruby: exit 1
来源：http://www.share.fehbvm.com/Article/details/ggoostgsa.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.fehbvm.com/Article/details/gsjbyhlck.sHtML

[M06] 向标准错误输出
来源：http://blog.hesvh.cn/Article/details/gybtnefzy.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.fehbvm.com/Article/details/gxxadraka.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.hesvh.cn/Article/details/gvplztffs.sHtML

JS:   console.error("err")
来源：http://www.m.share.zdbjq.cn/Article/details/ghdfcmrzp.sHtML

TS:   console.error("err")
来源：http://blog.zdbjq.cn/Article/details/gmmchqllg.sHtML

Java: System.err.println("err")
来源：http://3g.zdbjq.cn/Article/details/gpufbepki.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.hesvh.cn/Article/details/gmwrudhgr.sHtML

Ruby: warn "err"
来源：http://read.share.fehbvm.com/Article/details/gpvmifwyh.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.hesvh.cn/Article/details/gywdwpaph.sHtML

[M07] 判断是否为主入口
来源：http://blog.zdbjq.cn/Article/details/grlawypjj.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.zdbjq.cn/Article/details/gijpdrcoa.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.zdbjq.cn/Article/details/gelwpaigw.sHtML

JS:   require.main === module
来源：http://www.blog.zdbjq.cn/Article/details/gnubclfap.sHtML

TS:   require.main === module
来源：http://m.share.zdbjq.cn/Article/details/guvzyamdg.sHtML

Java: public static void main(String[] args)
来源：http://www.share.zdbjq.cn/Article/details/gsumqmzug.sHtML

Go:   func main()
来源：http://wap.zdbjq.cn/Article/details/gmjpbmauc.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.hesvh.cn/Article/details/ggzbmkkrw.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.zdbjq.cn/Article/details/gdrccmcvi.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.fehbvm.com/Article/details/gqjuklguv.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.zdbjq.cn/Article/details/gurtlszps.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.hesvh.cn/Article/details/grxwcplsh.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.fehbvm.com/Article/details/ggguzgssv.sHtML

TS:   process.platform;  process.version
来源：http://3g.zdbjq.cn/Article/details/gvalexrei.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.fehbvm.com/Article/details/gfexxanyq.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.fehbvm.com/Article/details/gqjxfnwgr.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.hesvh.cn/Article/details/gzsghhhmf.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.fehbvm.com/Article/details/gclbgcskw.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/ghpqwxtrj.sHtML

N. 数据结构与算法
来源：http://mobile.fehbvm.com/Article/details/gsgqfbedb.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gnccdpvqu.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.hesvh.cn/Article/details/gxqwzfkdk.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gqxoapasd.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.fehbvm.com/Article/details/ggrcxqgsw.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.fehbvm.com/Article/details/gjocdaygr.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.fehbvm.com/Article/details/glmyogthz.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gixyqiusq.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gdbenikvj.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.zdbjq.cn/Article/details/ggrkofwbu.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.hesvh.cn/Article/details/goyyhbttk.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.zdbjq.cn/Article/details/georrtnpo.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.fehbvm.com/Article/details/gtypnqbvi.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.fehbvm.com/Article/details/gsushmjsu.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.hesvh.cn/Article/details/grctfhcuj.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.zdbjq.cn/Article/details/gdmdtxyyc.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.fehbvm.com/Article/details/gvnsmqkik.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.hesvh.cn/Article/details/gidmuezit.sHtML

Ruby: arr.sort
来源：http://www.blog.hesvh.cn/Article/details/gfjlhwrla.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.fehbvm.com/Article/details/gyniysdll.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.zdbjq.cn/Article/details/gmhnjdczo.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.fehbvm.com/Article/details/gbbjyqdvj.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.zdbjq.cn/Article/details/gpeplawcl.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.hesvh.cn/Article/details/gwagetrdf.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.fehbvm.com/Article/details/gexbqhkyh.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.hesvh.cn/Article/details/gtosohqeq.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.zdbjq.cn/Article/details/gwpybgoiq.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.fehbvm.com/Article/details/gvscjudqs.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.zdbjq.cn/Article/details/gjalmnbxt.sHtML

[N04] 斐波那契数列
来源：http://www.share.zdbjq.cn/Article/details/gviesxhqq.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.hesvh.cn/Article/details/gsayhywsb.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.hesvh.cn/Article/details/gflpnufjr.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.zdbjq.cn/Article/details/gifaqmkwz.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.zdbjq.cn/Article/details/gbupnkwqr.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.zdbjq.cn/Article/details/gdhfvlzlb.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.fehbvm.com/Article/details/gyuscrrij.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.fehbvm.com/Article/details/gtjaeyrlm.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.fehbvm.com/Article/details/ghcnqdhqq.sHtML

[N05] 最大公约数
来源：http://read.share.zdbjq.cn/Article/details/ghsgoizge.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.hesvh.cn/Article/details/gwvrhtrez.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.zdbjq.cn/Article/details/gvyohirgm.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.fehbvm.com/Article/details/gyvfhfdvu.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.hesvh.cn/Article/details/gjngorpqj.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.zdbjq.cn/Article/details/grypfkpit.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.hesvh.cn/Article/details/grmccexif.sHtML

Ruby: a.gcd(b)
来源：http://3g.fehbvm.com/Article/details/gawfmhygx.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.fehbvm.com/Article/details/gmkrgfdru.sHtML

[N06] 判断回文字符串
来源：http://3g.hesvh.cn/Article/details/gpatsblxx.sHtML

Py:   s == s[::-1]
来源：http://baike.zdbjq.cn/Article/details/gynvtyvlp.sHtML

PHP:  $s === strrev($s);
来源：http://3g.hesvh.cn/Article/details/gtowsizoe.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/gwufvldmh.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/gdnnfpfvw.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.zdbjq.cn/Article/details/geupnuoct.sHtML

Go:   // 双指针从两端比较
来源：http://baike.hesvh.cn/Article/details/giidwosps.sHtML

Ruby: s == s.reverse
来源：http://wap.hesvh.cn/Article/details/gbwzowhii.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.fehbvm.com/Article/details/gwxoukvwn.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.hesvh.cn/Article/details/gqaybdeej.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.fehbvm.com/Article/details/gzeuxggfr.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.hesvh.cn/Article/details/ghbvipxxu.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.zdbjq.cn/Article/details/gqprhuoah.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.zdbjq.cn/Article/details/ggmtuolev.sHtML

Java: // 手写 HashMap
来源：http://blog.hesvh.cn/Article/details/gmveaqcwe.sHtML

Go:   // 手写 map[int]int
来源：http://baike.fehbvm.com/Article/details/giaijpgvy.sHtML

Ruby: // 手写 Hash
来源：http://mobile.hesvh.cn/Article/details/gdhpjpllm.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.hesvh.cn/Article/details/gcawwcumx.sHtML

[N08] 生成全排列
来源：http://m.share.fehbvm.com/Article/details/gfijitkkm.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.hesvh.cn/Article/details/gmiafbtbo.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.zdbjq.cn/Article/details/gmhbvwqaz.sHtML

JS:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gkhtgicqc.sHtML

TS:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gadgomfqo.sHtML

Java: // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/goblccexz.sHtML

Go:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/griubfggn.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.hesvh.cn/Article/details/gguezyapz.sHtML

C#:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/ghhbnslyq.sHtML

[N09] 栈与队列
来源：http://www.blog.hesvh.cn/Article/details/gaccqcerl.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.fehbvm.com/Article/details/gexqoqqul.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.zdbjq.cn/Article/details/gynjxuqyp.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.zdbjq.cn/Article/details/gnwqtgyqs.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.hesvh.cn/Article/details/gutnbjzrd.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.fehbvm.com/Article/details/gzrbdzxaw.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.zdbjq.cn/Article/details/gqakpetlx.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.zdbjq.cn/Article/details/gibbdycpp.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.fehbvm.com/Article/details/gdgwnwnrl.sHtML

[N10] 链表节点定义
来源：http://wap.hesvh.cn/Article/details/gqngivpkm.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.fehbvm.com/Article/details/gquuwxzcl.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.fehbvm.com/Article/details/gzdnrczkd.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.fehbvm.com/Article/details/gskjojyvh.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.hesvh.cn/Article/details/ggkhzjkoh.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.zdbjq.cn/Article/details/gzhmihtru.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.hesvh.cn/Article/details/guxvkvggv.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.fehbvm.com/Article/details/gqsiqdlir.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.zdbjq.cn/Article/details/guroxkndp.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.hesvh.cn/Article/details/gvttohwie.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.fehbvm.com/Article/details/godwrbgdr.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.zdbjq.cn/Article/details/gxpxtokkt.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.zdbjq.cn/Article/details/ghtqpkedw.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.hesvh.cn/Article/details/gdesxfgku.sHtML

Java: // 手写递归
来源：http://www.blog.hesvh.cn/Article/details/gudopmzxy.sHtML

Go:   // 手写递归
来源：http://3g.zdbjq.cn/Article/details/ghvmftxmc.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.fehbvm.com/Article/details/geawnmzmk.sHtML

C#:   // 手写递归
来源：http://baike.fehbvm.com/Article/details/ggiypwngs.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.fehbvm.com/Article/details/gxwznbljo.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.fehbvm.com/Article/details/gpjgweiph.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.fehbvm.com/Article/details/gvkevtkig.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.fehbvm.com/Article/details/gzbcflqpp.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.hesvh.cn/Article/details/gdmydjvah.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.zdbjq.cn/Article/details/ghqguwtqn.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.fehbvm.com/Article/details/gultwdife.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.zdbjq.cn/Article/details/gffvhbugn.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.zdbjq.cn/Article/details/gqqqzestm.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/ghjgqcxhw.sHtML

O. 并发与异步
来源：http://www.blog.hesvh.cn/Article/details/gffnqyjxl.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gvavcujdf.sHtML

[O01] 启动一个线程
来源：http://wap.fehbvm.com/Article/details/gducawrgl.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.zdbjq.cn/Article/details/gxbjtdbrx.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.fehbvm.com/Article/details/gsjekzqvc.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.zdbjq.cn/Article/details/ghillpyox.sHtML

TS:   // 同 JS
来源：http://read.share.zdbjq.cn/Article/details/gvfkqjjoo.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.fehbvm.com/Article/details/gxmbdzzns.sHtML

Go:   go f()
来源：http://mobile.hesvh.cn/Article/details/gzlinjvjv.sHtML

Ruby: Thread.new { f }
来源：http://baike.zdbjq.cn/Article/details/ghipzatjb.sHtML

C#:   Task.Run(() => F());
来源：http://baike.hesvh.cn/Article/details/goiixyymj.sHtML

[O02] 使用线程池
来源：http://read.share.hesvh.cn/Article/details/gzjwhhklh.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.fehbvm.com/Article/details/gtqrqptwo.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.fehbvm.com/Article/details/giznhtllh.sHtML

JS:   // worker_threads 线程池
来源：http://wap.hesvh.cn/Article/details/gvbwynray.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.zdbjq.cn/Article/details/geqdzmgrv.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.zdbjq.cn/Article/details/gyvugqttx.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.fehbvm.com/Article/details/ghvwaaewl.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.zdbjq.cn/Article/details/gkccnxvyi.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.hesvh.cn/Article/details/gfwjsupda.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.fehbvm.com/Article/details/gwnddmcyf.sHtML

Py:   with lock: shared += 1
来源：http://mobile.fehbvm.com/Article/details/grdomzvps.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.hesvh.cn/Article/details/guocmlgej.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.zdbjq.cn/Article/details/gfpyrooep.sHtML

TS:   // 同 JS
来源：http://www.m.share.fehbvm.com/Article/details/gbhwnxicg.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.hesvh.cn/Article/details/gjekoozbf.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.zdbjq.cn/Article/details/gyvvugweu.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.hesvh.cn/Article/details/gtatqblxa.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.hesvh.cn/Article/details/ghduxlcci.sHtML

[O04] 定义异步函数并等待
来源：http://baike.zdbjq.cn/Article/details/ghfklmvep.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.zdbjq.cn/Article/details/gpmmxhied.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.hesvh.cn/Article/details/goydmznah.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.hesvh.cn/Article/details/gaxejyjbw.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.hesvh.cn/Article/details/ghouljclw.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.hesvh.cn/Article/details/gwbssxxwu.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.fehbvm.com/Article/details/gpbsjsbgi.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.fehbvm.com/Article/details/gixrklkcs.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.zdbjq.cn/Article/details/gliwwdkmr.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.hesvh.cn/Article/details/gqipgflbo.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.fehbvm.com/Article/details/gpmtmfqzo.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.hesvh.cn/Article/details/gtmdfxwan.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.fehbvm.com/Article/details/gyjjogpdh.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.hesvh.cn/Article/details/gvafaehqq.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.hesvh.cn/Article/details/gedtpvbuy.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.zdbjq.cn/Article/details/gsowqknrg.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.zdbjq.cn/Article/details/gmfqbulet.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.zdbjq.cn/Article/details/gltccpiqh.sHtML

[O06] 使用进程池
来源：http://blog.fehbvm.com/Article/details/goeizrcvu.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.zdbjq.cn/Article/details/gsvurerjz.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.hesvh.cn/Article/details/grazfxsyg.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.hesvh.cn/Article/details/gfliwfyej.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.hesvh.cn/Article/details/gukbrauhd.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.fehbvm.com/Article/details/gtomwojku.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.hesvh.cn/Article/details/gdfxafjlm.sHtML

Ruby: // fork 块
来源：http://blog.hesvh.cn/Article/details/grusspjbf.sHtML

C#:   Parallel.For
来源：http://mobile.zdbjq.cn/Article/details/ghwfqwnts.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gaghjxqxt.sHtML

P. 常用工具函数
来源：http://mobile.zdbjq.cn/Article/details/gtdaruync.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gwqwoajkh.sHtML

[P01] 生成 UUID
来源：http://www.m.share.fehbvm.com/Article/details/geaqwekwy.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.zdbjq.cn/Article/details/gxdnoojuu.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.zdbjq.cn/Article/details/gpekudado.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.zdbjq.cn/Article/details/gofbcdxmb.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.hesvh.cn/Article/details/gyiwshgcg.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.hesvh.cn/Article/details/gzvepmdzg.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.hesvh.cn/Article/details/gudarrpzw.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.fehbvm.com/Article/details/gopahigkm.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.zdbjq.cn/Article/details/gqfcpznpi.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.zdbjq.cn/Article/details/gtyldfoju.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.hesvh.cn/Article/details/gbyohfvsm.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.fehbvm.com/Article/details/gsqsttzcv.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.fehbvm.com/Article/details/grfwzwgfc.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.fehbvm.com/Article/details/gszjcddaj.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.fehbvm.com/Article/details/gmetdcdej.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.fehbvm.com/Article/details/glsaifmct.sHtML


<!-- 参考信息 -->