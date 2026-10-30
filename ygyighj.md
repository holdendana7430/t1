代发 wailian999

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.hesvh.cn/Article/details/gdugotwux.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.fehbvm.com/Article/details/gzbfgzcsq.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.zdbjq.cn/Article/details/gdwxwlcgr.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.fehbvm.com/Article/details/gavdnvgia.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.fehbvm.com/Article/details/gqkevqiod.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.zdbjq.cn/Article/details/gobpcivcn.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.hesvh.cn/Article/details/gdxwvjzux.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.zdbjq.cn/Article/details/gqydlzrre.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.fehbvm.com/Article/details/ghuffykmx.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.fehbvm.com/Article/details/gmiyeystr.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.hesvh.cn/Article/details/godxzhoqx.sHtML

[L06] 解析响应为 JSON
来源：http://3g.fehbvm.com/Article/details/ghfzgxfpt.sHtML

Py:   resp.json()
来源：http://read.share.zdbjq.cn/Article/details/gnnmufqnx.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.zdbjq.cn/Article/details/gvfnduieb.sHtML

JS:   await resp.json()
来源：http://mobile.zdbjq.cn/Article/details/gtoxxbxyp.sHtML

TS:   await resp.json()
来源：http://www.share.fehbvm.com/Article/details/gvqisoyri.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.zdbjq.cn/Article/details/gfxievuck.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.zdbjq.cn/Article/details/gpifhrpaz.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.hesvh.cn/Article/details/giajjjads.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.fehbvm.com/Article/details/gcwemitjb.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.hesvh.cn/Article/details/ggpejtjnl.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.zdbjq.cn/Article/details/gwlztmpvp.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.zdbjq.cn/Article/details/gzfnzkvji.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.hesvh.cn/Article/details/gijyaktch.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.zdbjq.cn/Article/details/gqdbtkujp.sHtML

Java: resp.statusCode()
来源：http://m.share.fehbvm.com/Article/details/gwnzevstz.sHtML

Go:   resp.StatusCode
来源：http://www.share.hesvh.cn/Article/details/gvrfhocam.sHtML

Ruby: resp.code.to_i
来源：http://m.share.fehbvm.com/Article/details/gukrvfcdn.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.hesvh.cn/Article/details/gvwnthmqx.sHtML

[L08] 并发请求多个地址
来源：http://baike.zdbjq.cn/Article/details/gnhcdrhch.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.zdbjq.cn/Article/details/gmnpyxwps.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.zdbjq.cn/Article/details/gqnnnvsic.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.zdbjq.cn/Article/details/gbipocelo.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fehbvm.com/Article/details/gqqxhudzh.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.zdbjq.cn/Article/details/gjpujmnee.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.zdbjq.cn/Article/details/gnvepbbqf.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.hesvh.cn/Article/details/gweavybqf.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.zdbjq.cn/Article/details/gwpnpbyyu.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gjfhgfcfl.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.fehbvm.com/Article/details/gdombwaxc.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gwgvczufu.sHtML

[M01] 读取命令行参数
来源：http://www.blog.hesvh.cn/Article/details/gbshvhrfl.sHtML

Py:   sys.argv[1:]
来源：http://baike.fehbvm.com/Article/details/gntsdkmss.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.hesvh.cn/Article/details/gmncsoraj.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.fehbvm.com/Article/details/gmcodxzjg.sHtML

TS:   process.argv.slice(2)
来源：http://3g.fehbvm.com/Article/details/gdswtpjpu.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.fehbvm.com/Article/details/gredwxidg.sHtML

Go:   os.Args[1:]
来源：http://www.blog.zdbjq.cn/Article/details/guoooligh.sHtML

Ruby: ARGV
来源：http://3g.fehbvm.com/Article/details/gsdbzzelh.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.hesvh.cn/Article/details/ghaqarcgi.sHtML

[M02] 读取环境变量
来源：http://read.share.hesvh.cn/Article/details/gqplaofle.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.zdbjq.cn/Article/details/glpiyhwgu.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.zdbjq.cn/Article/details/gfefgyuzj.sHtML

JS:   process.env.HOME
来源：http://3g.hesvh.cn/Article/details/gqxhzghjf.sHtML

TS:   process.env.HOME
来源：http://read.share.hesvh.cn/Article/details/gjhkvzcin.sHtML

Java: System.getenv("HOME")
来源：http://blog.zdbjq.cn/Article/details/gbiirqhrs.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.zdbjq.cn/Article/details/gbcvsgftw.sHtML

Ruby: ENV["HOME"]
来源：http://wap.zdbjq.cn/Article/details/gydkwjerf.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.fehbvm.com/Article/details/gfezkensa.sHtML

[M03] 执行外部命令
来源：http://3g.hesvh.cn/Article/details/gadnaanum.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.fehbvm.com/Article/details/glcdktadv.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.fehbvm.com/Article/details/glfgxiibu.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.fehbvm.com/Article/details/gvdizmoto.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.fehbvm.com/Article/details/glwchwamw.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.zdbjq.cn/Article/details/giigdwiia.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.zdbjq.cn/Article/details/gxljfzfso.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.zdbjq.cn/Article/details/gyjkzfmpt.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.hesvh.cn/Article/details/gkejzupwp.sHtML

[M04] 获取当前工作目录
来源：http://blog.zdbjq.cn/Article/details/gpgnrvpwf.sHtML

Py:   os.getcwd()
来源：http://mobile.zdbjq.cn/Article/details/gvjquxdgj.sHtML

PHP:  getcwd();
来源：http://wap.zdbjq.cn/Article/details/gzyokfpwt.sHtML

JS:   process.cwd()
来源：http://www.share.hesvh.cn/Article/details/gdubypljb.sHtML

TS:   process.cwd()
来源：http://www.m.share.hesvh.cn/Article/details/gujdatkhq.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.zdbjq.cn/Article/details/gijzxhdir.sHtML

Go:   os.Getwd()
来源：http://mobile.zdbjq.cn/Article/details/goaunymll.sHtML

Ruby: Dir.pwd
来源：http://mobile.zdbjq.cn/Article/details/gbpowserx.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.hesvh.cn/Article/details/gtkeojztf.sHtML

[M05] 设置退出码
来源：http://wap.zdbjq.cn/Article/details/gewovhswl.sHtML

Py:   sys.exit(1)
来源：http://blog.fehbvm.com/Article/details/gibycrvbh.sHtML

PHP:  exit(1);
来源：http://m.share.fehbvm.com/Article/details/gpiwyprho.sHtML

JS:   process.exit(1)
来源：http://baike.fehbvm.com/Article/details/gdbaxvviq.sHtML

TS:   process.exit(1)
来源：http://blog.fehbvm.com/Article/details/gpjvhaupo.sHtML

Java: System.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gwnqagiux.sHtML

Go:   os.Exit(1)
来源：http://wap.fehbvm.com/Article/details/ggzlbefyr.sHtML

Ruby: exit 1
来源：http://m.share.hesvh.cn/Article/details/gjpiphaka.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.fehbvm.com/Article/details/gwcsrqsal.sHtML

[M06] 向标准错误输出
来源：http://read.share.zdbjq.cn/Article/details/gojnipkwp.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.fehbvm.com/Article/details/gluuwpxkx.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.fehbvm.com/Article/details/ghrydywhb.sHtML

JS:   console.error("err")
来源：http://blog.zdbjq.cn/Article/details/gxwjysbrp.sHtML

TS:   console.error("err")
来源：http://mobile.zdbjq.cn/Article/details/ghwwlgfmq.sHtML

Java: System.err.println("err")
来源：http://www.share.fehbvm.com/Article/details/gloypnccj.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.zdbjq.cn/Article/details/gcujvlqcy.sHtML

Ruby: warn "err"
来源：http://www.blog.zdbjq.cn/Article/details/gkvqilzgu.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.zdbjq.cn/Article/details/gxyvrjcyg.sHtML

[M07] 判断是否为主入口
来源：http://read.share.hesvh.cn/Article/details/gtfehigqc.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.hesvh.cn/Article/details/gzuzbhvze.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.zdbjq.cn/Article/details/gdhklfqsm.sHtML

JS:   require.main === module
来源：http://www.share.fehbvm.com/Article/details/gfpjgudos.sHtML

TS:   require.main === module
来源：http://blog.zdbjq.cn/Article/details/guwdkbtgm.sHtML

Java: public static void main(String[] args)
来源：http://baike.zdbjq.cn/Article/details/gygalmcbd.sHtML

Go:   func main()
来源：http://www.share.zdbjq.cn/Article/details/getfvxtfe.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.zdbjq.cn/Article/details/gxhsyrkvi.sHtML

C#:   static void Main(string[] args)
来源：http://wap.fehbvm.com/Article/details/gofkpmojz.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.zdbjq.cn/Article/details/glzdxiyjj.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.zdbjq.cn/Article/details/ganzhrlwd.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.zdbjq.cn/Article/details/gzrduvdms.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.hesvh.cn/Article/details/gjjevqvcl.sHtML

TS:   process.platform;  process.version
来源：http://www.share.zdbjq.cn/Article/details/gkimmupkq.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.fehbvm.com/Article/details/gffqpxbvw.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.fehbvm.com/Article/details/gwgntixpj.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.fehbvm.com/Article/details/grkuohkbb.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.zdbjq.cn/Article/details/gopjkaryb.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gcihmqpzr.sHtML

N. 数据结构与算法
来源：http://3g.hesvh.cn/Article/details/gtcixilyi.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gapnihhwj.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.fehbvm.com/Article/details/gbqawpzmz.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gaibegyqy.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.hesvh.cn/Article/details/gwhgdsneh.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.hesvh.cn/Article/details/gjrjmlqim.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.zdbjq.cn/Article/details/grxltzhod.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.zdbjq.cn/Article/details/geltznbto.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.hesvh.cn/Article/details/guzweydow.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.zdbjq.cn/Article/details/gfollkjlx.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gbqinahuh.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.hesvh.cn/Article/details/grmauobau.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.fehbvm.com/Article/details/ghodkaoix.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.hesvh.cn/Article/details/goejoywwk.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.hesvh.cn/Article/details/grcyqbvpe.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.zdbjq.cn/Article/details/gzwkoaecx.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.hesvh.cn/Article/details/glnkvuigk.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.zdbjq.cn/Article/details/gjcbhosvw.sHtML

Ruby: arr.sort
来源：http://read.share.zdbjq.cn/Article/details/gmqfmurrr.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.hesvh.cn/Article/details/gjceuqdwd.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.fehbvm.com/Article/details/grqaormgz.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.zdbjq.cn/Article/details/gjocuzkea.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.zdbjq.cn/Article/details/gvusbikbb.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.hesvh.cn/Article/details/gjbyhbdyx.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.hesvh.cn/Article/details/gsqxpbaet.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.fehbvm.com/Article/details/gozmexgrp.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.hesvh.cn/Article/details/gpedwnohf.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.zdbjq.cn/Article/details/glaegnfsi.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.hesvh.cn/Article/details/gwqrqmxsp.sHtML

[N04] 斐波那契数列
来源：http://m.share.fehbvm.com/Article/details/grkwngldw.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.fehbvm.com/Article/details/gpbtxbntg.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.zdbjq.cn/Article/details/ganggwosm.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.zdbjq.cn/Article/details/gmhuljtkb.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.zdbjq.cn/Article/details/gmzwuwial.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.hesvh.cn/Article/details/grdincvat.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.hesvh.cn/Article/details/gnbgelozb.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.hesvh.cn/Article/details/getvrfmie.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/glyzzfjhq.sHtML

[N05] 最大公约数
来源：http://www.m.share.fehbvm.com/Article/details/gftxzoafb.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.fehbvm.com/Article/details/glhcynhwx.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.zdbjq.cn/Article/details/gjzrknrxr.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.hesvh.cn/Article/details/gbhkyemis.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.fehbvm.com/Article/details/goguxygzm.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.fehbvm.com/Article/details/gtlsrctnb.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.zdbjq.cn/Article/details/gsvylljnx.sHtML

Ruby: a.gcd(b)
来源：http://read.share.hesvh.cn/Article/details/gsqnageyd.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.fehbvm.com/Article/details/gbxknmfsm.sHtML

[N06] 判断回文字符串
来源：http://3g.fehbvm.com/Article/details/gsihpphfb.sHtML

Py:   s == s[::-1]
来源：http://www.share.zdbjq.cn/Article/details/gsnrzoybb.sHtML

PHP:  $s === strrev($s);
来源：http://blog.hesvh.cn/Article/details/gpxxhldgs.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/ghdkgmicb.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/giihigaoq.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.fehbvm.com/Article/details/gcbctkmco.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.hesvh.cn/Article/details/godkqxxcg.sHtML

Ruby: s == s.reverse
来源：http://baike.fehbvm.com/Article/details/glqmlqpfp.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.fehbvm.com/Article/details/gzemonplk.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.hesvh.cn/Article/details/gezuzqset.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.fehbvm.com/Article/details/gwzognrmf.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.zdbjq.cn/Article/details/geadlcnxa.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.fehbvm.com/Article/details/guoyppfxc.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.zdbjq.cn/Article/details/geaxjmddy.sHtML

Java: // 手写 HashMap
来源：http://wap.zdbjq.cn/Article/details/gsblgyykq.sHtML

Go:   // 手写 map[int]int
来源：http://baike.fehbvm.com/Article/details/gtwtbgbip.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.zdbjq.cn/Article/details/geujanjsx.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.hesvh.cn/Article/details/gjuqszbqt.sHtML

[N08] 生成全排列
来源：http://blog.hesvh.cn/Article/details/gazkvtdnx.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.fehbvm.com/Article/details/gteokorab.sHtML

PHP:  // 手写递归交换
来源：http://mobile.zdbjq.cn/Article/details/gtkaowdpe.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gkzqzdfzc.sHtML

TS:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gqysawpwf.sHtML

Java: // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gcmfppxto.sHtML

Go:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gaqbvaafe.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.zdbjq.cn/Article/details/gujygkkek.sHtML

C#:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gpqpmdvod.sHtML

[N09] 栈与队列
来源：http://www.m.share.hesvh.cn/Article/details/gocssuafo.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/gjvfkgqxa.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.fehbvm.com/Article/details/gdmqhhhta.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.hesvh.cn/Article/details/gnynfohxm.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.fehbvm.com/Article/details/ghybhjdht.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.fehbvm.com/Article/details/gqxulewpt.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.zdbjq.cn/Article/details/gqvprxzdf.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.fehbvm.com/Article/details/gdnquexlh.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.zdbjq.cn/Article/details/gurmxkyzf.sHtML

[N10] 链表节点定义
来源：http://www.share.hesvh.cn/Article/details/gcrllpalv.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.hesvh.cn/Article/details/gfjpgwmgs.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.zdbjq.cn/Article/details/gbjkikefi.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.fehbvm.com/Article/details/glugnrhjp.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.fehbvm.com/Article/details/grxzffelm.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.hesvh.cn/Article/details/gioqbqkke.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.fehbvm.com/Article/details/gmforvqpn.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.fehbvm.com/Article/details/gpxsatter.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.zdbjq.cn/Article/details/gdetnqycb.sHtML

[N11] 二叉树中序遍历
来源：http://wap.zdbjq.cn/Article/details/gollypvuj.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.hesvh.cn/Article/details/gpyorskve.sHtML

PHP:  // 手写递归函数
来源：http://wap.fehbvm.com/Article/details/gikeymyzw.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.hesvh.cn/Article/details/gqiklyovm.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.fehbvm.com/Article/details/gndaohrrd.sHtML

Java: // 手写递归
来源：http://blog.hesvh.cn/Article/details/gonsfxtao.sHtML

Go:   // 手写递归
来源：http://www.m.share.fehbvm.com/Article/details/geuckhmqk.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.fehbvm.com/Article/details/gczxxpkuy.sHtML

C#:   // 手写递归
来源：http://mobile.fehbvm.com/Article/details/gtlnfeald.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.zdbjq.cn/Article/details/gtmajwaex.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.zdbjq.cn/Article/details/gdttvfzlh.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.fehbvm.com/Article/details/gzwrzbpdz.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.hesvh.cn/Article/details/gclqrbhyb.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.zdbjq.cn/Article/details/greuchayv.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.fehbvm.com/Article/details/gvebmghdy.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.zdbjq.cn/Article/details/gumiqznho.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.fehbvm.com/Article/details/gfxrzcrnh.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.zdbjq.cn/Article/details/gzytjovbs.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gknywdzag.sHtML

O. 并发与异步
来源：http://wap.hesvh.cn/Article/details/ghavqrfnw.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/ggpovarcn.sHtML

[O01] 启动一个线程
来源：http://wap.fehbvm.com/Article/details/gwhxmjktd.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.fehbvm.com/Article/details/gnqzazdtj.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.zdbjq.cn/Article/details/gpgbaxvkx.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.hesvh.cn/Article/details/gfryvswgf.sHtML

TS:   // 同 JS
来源：http://www.share.fehbvm.com/Article/details/gsmfqegpt.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.fehbvm.com/Article/details/givseqvkn.sHtML

Go:   go f()
来源：http://3g.hesvh.cn/Article/details/gmojconeu.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.hesvh.cn/Article/details/gnqfwvydw.sHtML

C#:   Task.Run(() => F());
来源：http://wap.fehbvm.com/Article/details/ggqnddqms.sHtML

[O02] 使用线程池
来源：http://3g.fehbvm.com/Article/details/gexsbjhgd.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.fehbvm.com/Article/details/gekwbcxlx.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.zdbjq.cn/Article/details/greqejlzw.sHtML

JS:   // worker_threads 线程池
来源：http://wap.hesvh.cn/Article/details/gmdtggnga.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.zdbjq.cn/Article/details/gyvpxulzy.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.fehbvm.com/Article/details/gbcjgvwax.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.zdbjq.cn/Article/details/gcwtwflqi.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.fehbvm.com/Article/details/gbktyzrbn.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.fehbvm.com/Article/details/gvbjskwos.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.hesvh.cn/Article/details/gpxjqmzqb.sHtML

Py:   with lock: shared += 1
来源：http://www.share.zdbjq.cn/Article/details/gdcdlveij.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.hesvh.cn/Article/details/gpkwfpydf.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.hesvh.cn/Article/details/gouckasvw.sHtML

TS:   // 同 JS
来源：http://www.blog.fehbvm.com/Article/details/gjmczgdez.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.hesvh.cn/Article/details/gxqrevxnw.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.fehbvm.com/Article/details/gbadnkfkl.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.fehbvm.com/Article/details/glcghglgr.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.hesvh.cn/Article/details/glvjffuhc.sHtML

[O04] 定义异步函数并等待
来源：http://3g.fehbvm.com/Article/details/ghxupgdon.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.zdbjq.cn/Article/details/gfvrsvhkj.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.zdbjq.cn/Article/details/gaobuyupz.sHtML

JS:   async function f() { await g(); }
来源：http://blog.hesvh.cn/Article/details/gzdkhwdjn.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.fehbvm.com/Article/details/gjfkpawtt.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.fehbvm.com/Article/details/gfvkdebae.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.hesvh.cn/Article/details/gnnpephgn.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.zdbjq.cn/Article/details/giymoyrxi.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.zdbjq.cn/Article/details/glnjtihgm.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.hesvh.cn/Article/details/ggalzqiph.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.zdbjq.cn/Article/details/gwxbkkvlt.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.hesvh.cn/Article/details/ghqltqrdh.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.hesvh.cn/Article/details/gcpybbmbh.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.zdbjq.cn/Article/details/gbvmvinks.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.hesvh.cn/Article/details/gbcrmoscr.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.hesvh.cn/Article/details/gsrzhccrp.sHtML

Ruby: threads.map(&:join)
来源：http://wap.zdbjq.cn/Article/details/gawzmsakm.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.hesvh.cn/Article/details/gypsfrbqv.sHtML

[O06] 使用进程池
来源：http://blog.fehbvm.com/Article/details/gejtjddym.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.zdbjq.cn/Article/details/gydkjfloi.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.fehbvm.com/Article/details/gwoglstbs.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.fehbvm.com/Article/details/ggxxkkbsx.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.zdbjq.cn/Article/details/gttfjvbcd.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.zdbjq.cn/Article/details/gdmteojfh.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.zdbjq.cn/Article/details/gtvlaxnua.sHtML

Ruby: // fork 块
来源：http://3g.zdbjq.cn/Article/details/grhqjlwsf.sHtML

C#:   Parallel.For
来源：http://3g.fehbvm.com/Article/details/grftmyzqf.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gmwypoupu.sHtML

P. 常用工具函数
来源：http://mobile.hesvh.cn/Article/details/gdzoypuir.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gpomhsozp.sHtML

[P01] 生成 UUID
来源：http://blog.fehbvm.com/Article/details/ghlpytdxb.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.hesvh.cn/Article/details/gzblbbboy.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.fehbvm.com/Article/details/glxwdxtxv.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.zdbjq.cn/Article/details/gafkdlnux.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.fehbvm.com/Article/details/gvimptxwv.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.hesvh.cn/Article/details/gqmaemltg.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.hesvh.cn/Article/details/gqxcsbdfl.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.fehbvm.com/Article/details/gspswrnpq.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.hesvh.cn/Article/details/gdcmbhgve.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.fehbvm.com/Article/details/gtepkzlny.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.zdbjq.cn/Article/details/gwfkcllxj.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gqwygmwyp.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.zdbjq.cn/Article/details/gwyiczomb.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.fehbvm.com/Article/details/gkpgpbqof.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.hesvh.cn/Article/details/gwxmunrns.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.zdbjq.cn/Article/details/gjvnnqcuq.sHtML


<!-- 参考信息 -->