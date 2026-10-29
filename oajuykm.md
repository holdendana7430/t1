代发 wailian999

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.zdbjq.cn/Article/details/gytvujclc.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.fehbvm.com/Article/details/gadolycjc.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.hesvh.cn/Article/details/gkhryawpl.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.fehbvm.com/Article/details/gcgutwodb.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.hesvh.cn/Article/details/gpzlziogq.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.hesvh.cn/Article/details/gkctzoqyu.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.fehbvm.com/Article/details/gwxunedjx.sHtML

[L06] 解析响应为 JSON
来源：http://wap.hesvh.cn/Article/details/gpackwenh.sHtML

Py:   resp.json()
来源：http://wap.zdbjq.cn/Article/details/gbzrmfqou.sHtML

PHP:  json_decode($body, true);
来源：http://wap.fehbvm.com/Article/details/gcumzgins.sHtML

JS:   await resp.json()
来源：http://3g.hesvh.cn/Article/details/gdtnqcmqv.sHtML

TS:   await resp.json()
来源：http://mobile.hesvh.cn/Article/details/gyrhvuozn.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.zdbjq.cn/Article/details/gyzfwlixd.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.fehbvm.com/Article/details/gcoeyglza.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.fehbvm.com/Article/details/gguzigeqd.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.zdbjq.cn/Article/details/gnpnzjyfl.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.zdbjq.cn/Article/details/ghpzeaudd.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.hesvh.cn/Article/details/gvezzqsqp.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.zdbjq.cn/Article/details/gxxcayvwa.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.hesvh.cn/Article/details/gyezunrmd.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.zdbjq.cn/Article/details/guwiiqyok.sHtML

Java: resp.statusCode()
来源：http://read.share.zdbjq.cn/Article/details/guoddsybj.sHtML

Go:   resp.StatusCode
来源：http://baike.zdbjq.cn/Article/details/gdamnspgr.sHtML

Ruby: resp.code.to_i
来源：http://3g.fehbvm.com/Article/details/gcgqrgziy.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.hesvh.cn/Article/details/guuookwgi.sHtML

[L08] 并发请求多个地址
来源：http://mobile.fehbvm.com/Article/details/gwcgfuyqu.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.zdbjq.cn/Article/details/gcjhoiyhs.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.zdbjq.cn/Article/details/gkritmltz.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fehbvm.com/Article/details/ggzscjdfn.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.hesvh.cn/Article/details/gihahbfme.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.zdbjq.cn/Article/details/gclulsgve.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.hesvh.cn/Article/details/gzffeayqt.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.zdbjq.cn/Article/details/gttdzblva.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.fehbvm.com/Article/details/gpcxlilug.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gitppnygz.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.hesvh.cn/Article/details/glmbyhtfc.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gejqqfwgy.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.hesvh.cn/Article/details/gpianivzh.sHtML

Py:   sys.argv[1:]
来源：http://m.share.zdbjq.cn/Article/details/gvycpwrfq.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.fehbvm.com/Article/details/gygqnqqbw.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.fehbvm.com/Article/details/gwgxhyvpx.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.zdbjq.cn/Article/details/gpaxbpxgk.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.hesvh.cn/Article/details/gdlrhawct.sHtML

Go:   os.Args[1:]
来源：http://www.blog.hesvh.cn/Article/details/gpjpgtabq.sHtML

Ruby: ARGV
来源：http://www.share.fehbvm.com/Article/details/gwmxelfit.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.zdbjq.cn/Article/details/gxknbuvmu.sHtML

[M02] 读取环境变量
来源：http://www.share.hesvh.cn/Article/details/gefyymqgh.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.hesvh.cn/Article/details/gavzexsay.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.hesvh.cn/Article/details/gfazwidfe.sHtML

JS:   process.env.HOME
来源：http://m.share.fehbvm.com/Article/details/gleteagiz.sHtML

TS:   process.env.HOME
来源：http://www.blog.fehbvm.com/Article/details/gdkdqhuab.sHtML

Java: System.getenv("HOME")
来源：http://mobile.fehbvm.com/Article/details/gpdoopsil.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.hesvh.cn/Article/details/gvgxwkoot.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.hesvh.cn/Article/details/gtcngyfsf.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.hesvh.cn/Article/details/gcvemwibm.sHtML

[M03] 执行外部命令
来源：http://wap.zdbjq.cn/Article/details/gzdyvuxrq.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.hesvh.cn/Article/details/gitjynvec.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.fehbvm.com/Article/details/gdotpkxva.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.zdbjq.cn/Article/details/gdfyhihqd.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.fehbvm.com/Article/details/gvvtlaodt.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.zdbjq.cn/Article/details/gegezyktr.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.zdbjq.cn/Article/details/gphanjmvi.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.hesvh.cn/Article/details/gbiroibvh.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.hesvh.cn/Article/details/gdfmcivdv.sHtML

[M04] 获取当前工作目录
来源：http://3g.zdbjq.cn/Article/details/gwycgqbma.sHtML

Py:   os.getcwd()
来源：http://www.blog.fehbvm.com/Article/details/gbjdfisij.sHtML

PHP:  getcwd();
来源：http://blog.hesvh.cn/Article/details/gebxivgza.sHtML

JS:   process.cwd()
来源：http://3g.hesvh.cn/Article/details/gvxdbopjy.sHtML

TS:   process.cwd()
来源：http://baike.hesvh.cn/Article/details/gnmfzkofc.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.fehbvm.com/Article/details/gowrgvxwq.sHtML

Go:   os.Getwd()
来源：http://www.blog.zdbjq.cn/Article/details/guuphaees.sHtML

Ruby: Dir.pwd
来源：http://www.blog.fehbvm.com/Article/details/gcbacwxbi.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.zdbjq.cn/Article/details/gekahigcf.sHtML

[M05] 设置退出码
来源：http://read.share.hesvh.cn/Article/details/gyxmxsnrb.sHtML

Py:   sys.exit(1)
来源：http://m.share.hesvh.cn/Article/details/gvyxlcwlb.sHtML

PHP:  exit(1);
来源：http://mobile.zdbjq.cn/Article/details/gnyvymnau.sHtML

JS:   process.exit(1)
来源：http://mobile.fehbvm.com/Article/details/gnrstrdhr.sHtML

TS:   process.exit(1)
来源：http://mobile.fehbvm.com/Article/details/grhdxbbwt.sHtML

Java: System.exit(1)
来源：http://baike.zdbjq.cn/Article/details/gguppvsla.sHtML

Go:   os.Exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gppbfjoav.sHtML

Ruby: exit 1
来源：http://baike.hesvh.cn/Article/details/gmqazfavi.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.hesvh.cn/Article/details/gujjcpaal.sHtML

[M06] 向标准错误输出
来源：http://read.share.fehbvm.com/Article/details/gqeukydol.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.zdbjq.cn/Article/details/gttrhqoqy.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.fehbvm.com/Article/details/gpvmkbqlk.sHtML

JS:   console.error("err")
来源：http://mobile.zdbjq.cn/Article/details/gntkpmnni.sHtML

TS:   console.error("err")
来源：http://mobile.fehbvm.com/Article/details/ghmckbbki.sHtML

Java: System.err.println("err")
来源：http://m.share.fehbvm.com/Article/details/gafyskywr.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.hesvh.cn/Article/details/gjcnqskpv.sHtML

Ruby: warn "err"
来源：http://mobile.fehbvm.com/Article/details/gcwyzimlj.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.zdbjq.cn/Article/details/ggueaexab.sHtML

[M07] 判断是否为主入口
来源：http://baike.hesvh.cn/Article/details/gwxquydww.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.zdbjq.cn/Article/details/gfypqfmfu.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.fehbvm.com/Article/details/glqiravxe.sHtML

JS:   require.main === module
来源：http://www.blog.hesvh.cn/Article/details/gxqvrcgsf.sHtML

TS:   require.main === module
来源：http://read.share.hesvh.cn/Article/details/gzkdwtswe.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.fehbvm.com/Article/details/gvejhvgit.sHtML

Go:   func main()
来源：http://mobile.zdbjq.cn/Article/details/glpzwlcku.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.hesvh.cn/Article/details/gwbdtvfqv.sHtML

C#:   static void Main(string[] args)
来源：http://blog.hesvh.cn/Article/details/gosxfsgth.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.zdbjq.cn/Article/details/gxwfcaewo.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.zdbjq.cn/Article/details/ggzeoclnv.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.fehbvm.com/Article/details/gtlbprcwb.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.zdbjq.cn/Article/details/gentujqqt.sHtML

TS:   process.platform;  process.version
来源：http://mobile.hesvh.cn/Article/details/grsqwzwru.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.zdbjq.cn/Article/details/gtddmwlwm.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.fehbvm.com/Article/details/gcohdvwya.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.fehbvm.com/Article/details/gkvfacrfp.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.fehbvm.com/Article/details/gbxgvggoe.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gzuorjfsx.sHtML

N. 数据结构与算法
来源：http://read.share.fehbvm.com/Article/details/goqynneos.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/glzcjkgej.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.hesvh.cn/Article/details/gcfxostrg.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gfhemzvay.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.zdbjq.cn/Article/details/gntgubbpe.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.fehbvm.com/Article/details/gsjybvwiv.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.hesvh.cn/Article/details/gzdgwwfxa.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gxyvznumb.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gnccmrzlo.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.zdbjq.cn/Article/details/gkqzewlup.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.fehbvm.com/Article/details/glejijqca.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.hesvh.cn/Article/details/gxerazlzj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.zdbjq.cn/Article/details/gejehmfiu.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.fehbvm.com/Article/details/gdsjwcckr.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.zdbjq.cn/Article/details/giavqgicw.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.hesvh.cn/Article/details/gamptgfag.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.fehbvm.com/Article/details/gtsbueuri.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.fehbvm.com/Article/details/gsjayqawu.sHtML

Ruby: arr.sort
来源：http://www.share.hesvh.cn/Article/details/grrnirofu.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.fehbvm.com/Article/details/gmwwjdcwg.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.hesvh.cn/Article/details/gqggflrvt.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.zdbjq.cn/Article/details/gawtvcmmb.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.fehbvm.com/Article/details/gjmcgwfja.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.fehbvm.com/Article/details/gljqerwvg.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.zdbjq.cn/Article/details/gzepffxfl.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.zdbjq.cn/Article/details/gjvqkbvwb.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.fehbvm.com/Article/details/gjhicbsrw.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.hesvh.cn/Article/details/gorkjkchy.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.zdbjq.cn/Article/details/gualqcaub.sHtML

[N04] 斐波那契数列
来源：http://www.share.zdbjq.cn/Article/details/gteglicrg.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.hesvh.cn/Article/details/gnrhdafdw.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.fehbvm.com/Article/details/geuofgnnh.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.zdbjq.cn/Article/details/ghxiwdpos.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/gonjzpnkf.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.hesvh.cn/Article/details/gbrcgzyvd.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.fehbvm.com/Article/details/gnvktaggp.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.hesvh.cn/Article/details/gekyxfgxj.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/glopajfkn.sHtML

[N05] 最大公约数
来源：http://read.share.zdbjq.cn/Article/details/gxuuqsbip.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.hesvh.cn/Article/details/gfuwrkqgl.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.zdbjq.cn/Article/details/gnszgxpfc.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.hesvh.cn/Article/details/gwvmlhqvd.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.hesvh.cn/Article/details/gisedinuf.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.hesvh.cn/Article/details/gngbdwqyx.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.zdbjq.cn/Article/details/ghtnuocpd.sHtML

Ruby: a.gcd(b)
来源：http://wap.hesvh.cn/Article/details/gesqxlkav.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.zdbjq.cn/Article/details/gkdxnbqzx.sHtML

[N06] 判断回文字符串
来源：http://blog.fehbvm.com/Article/details/gduoejfdu.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.hesvh.cn/Article/details/gfphuzlzl.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.hesvh.cn/Article/details/gxlyxummj.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/gurhhvkvv.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/gblvlzxvr.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.zdbjq.cn/Article/details/gxacxotjv.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.fehbvm.com/Article/details/gemmxdwid.sHtML

Ruby: s == s.reverse
来源：http://mobile.zdbjq.cn/Article/details/ginqvnlsq.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.hesvh.cn/Article/details/gsclkgved.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.zdbjq.cn/Article/details/gzjpzatid.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.fehbvm.com/Article/details/gxtckfsbp.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.zdbjq.cn/Article/details/gfejupogn.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.hesvh.cn/Article/details/gsrlsxndb.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.zdbjq.cn/Article/details/gpgsxmxwh.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.fehbvm.com/Article/details/gcqpbtgmf.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.hesvh.cn/Article/details/ghcfhfpaq.sHtML

Ruby: // 手写 Hash
来源：http://m.share.zdbjq.cn/Article/details/ggvdzkqjh.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.fehbvm.com/Article/details/gnlpnkkjl.sHtML

[N08] 生成全排列
来源：http://www.m.share.hesvh.cn/Article/details/ghnqidvfc.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.fehbvm.com/Article/details/gwtkaccnu.sHtML

PHP:  // 手写递归交换
来源：http://read.share.fehbvm.com/Article/details/guvfivkjd.sHtML

JS:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gkozejvun.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/ggsmhzwxl.sHtML

Java: // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gzpjmedgz.sHtML

Go:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gbgwunqdh.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.hesvh.cn/Article/details/gjpnogoeb.sHtML

C#:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gcenzqnym.sHtML

[N09] 栈与队列
来源：http://3g.zdbjq.cn/Article/details/gunrugxbr.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.fehbvm.com/Article/details/gxqovwwkp.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.zdbjq.cn/Article/details/gamtpfpaf.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.hesvh.cn/Article/details/gzrvmznkp.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.hesvh.cn/Article/details/gjhgdrmlq.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.fehbvm.com/Article/details/ghukbqsuj.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.fehbvm.com/Article/details/gkzvpqgar.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.zdbjq.cn/Article/details/ggusxqpnu.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.hesvh.cn/Article/details/gwmadkocr.sHtML

[N10] 链表节点定义
来源：http://read.share.zdbjq.cn/Article/details/gxkhnkrvb.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.zdbjq.cn/Article/details/gxtinbxkp.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.hesvh.cn/Article/details/gjiojtlla.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.hesvh.cn/Article/details/gkfciogcx.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.zdbjq.cn/Article/details/ggbncgynd.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.fehbvm.com/Article/details/gvspypkts.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.zdbjq.cn/Article/details/ghxprzukx.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.fehbvm.com/Article/details/gfzuujyod.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.zdbjq.cn/Article/details/gydtthkzr.sHtML

[N11] 二叉树中序遍历
来源：http://baike.zdbjq.cn/Article/details/gmltbwoao.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.zdbjq.cn/Article/details/gibvocamf.sHtML

PHP:  // 手写递归函数
来源：http://m.share.fehbvm.com/Article/details/goxvvafzq.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.zdbjq.cn/Article/details/gwvcghuuj.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.hesvh.cn/Article/details/gdtdgflzo.sHtML

Java: // 手写递归
来源：http://mobile.zdbjq.cn/Article/details/girozlsrb.sHtML

Go:   // 手写递归
来源：http://3g.zdbjq.cn/Article/details/gndvqcqeu.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.zdbjq.cn/Article/details/gultauqhs.sHtML

C#:   // 手写递归
来源：http://blog.hesvh.cn/Article/details/giuorjsgz.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.hesvh.cn/Article/details/gvrzdvvzb.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.zdbjq.cn/Article/details/grfinpsja.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.fehbvm.com/Article/details/gghnjstlv.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.fehbvm.com/Article/details/gxeryjkim.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.zdbjq.cn/Article/details/gdxseydub.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.fehbvm.com/Article/details/gnamurmps.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.zdbjq.cn/Article/details/gcskpokoc.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.fehbvm.com/Article/details/gxnunvcpx.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.zdbjq.cn/Article/details/gmpusheyu.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gfqmvvino.sHtML

O. 并发与异步
来源：http://www.m.share.fehbvm.com/Article/details/gcbmsjuan.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gldhyhgxx.sHtML

[O01] 启动一个线程
来源：http://m.share.hesvh.cn/Article/details/gywsxdarc.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.hesvh.cn/Article/details/gmpqgjend.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.zdbjq.cn/Article/details/gjewcgdab.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.hesvh.cn/Article/details/gdhnlbljp.sHtML

TS:   // 同 JS
来源：http://wap.zdbjq.cn/Article/details/gqkpyzmnw.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.fehbvm.com/Article/details/gdnamsbbt.sHtML

Go:   go f()
来源：http://www.share.hesvh.cn/Article/details/gfnegiepd.sHtML

Ruby: Thread.new { f }
来源：http://mobile.zdbjq.cn/Article/details/guxmldhzp.sHtML

C#:   Task.Run(() => F());
来源：http://wap.fehbvm.com/Article/details/gmkghroeg.sHtML

[O02] 使用线程池
来源：http://www.m.share.fehbvm.com/Article/details/gbrnguvgo.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.fehbvm.com/Article/details/gnkcgxohr.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.zdbjq.cn/Article/details/gqsvqrcaw.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.zdbjq.cn/Article/details/gcrqqeegm.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.zdbjq.cn/Article/details/gloszgscx.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.fehbvm.com/Article/details/glvkcujxz.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.fehbvm.com/Article/details/gmiptwsye.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.zdbjq.cn/Article/details/gndpnzivu.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.hesvh.cn/Article/details/goalfsfcb.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.fehbvm.com/Article/details/gahigvgzm.sHtML

Py:   with lock: shared += 1
来源：http://baike.fehbvm.com/Article/details/ggmwisggq.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.hesvh.cn/Article/details/gsqemymio.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.hesvh.cn/Article/details/gmuillvlv.sHtML

TS:   // 同 JS
来源：http://www.m.share.hesvh.cn/Article/details/gaqpgsdxa.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.fehbvm.com/Article/details/gvtijlxii.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.zdbjq.cn/Article/details/gamejtycz.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.hesvh.cn/Article/details/gpkkrwuoc.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.fehbvm.com/Article/details/guxxxnikd.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.hesvh.cn/Article/details/gywrgxdcq.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.zdbjq.cn/Article/details/gqxwdeigj.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.zdbjq.cn/Article/details/gjzjmoick.sHtML

JS:   async function f() { await g(); }
来源：http://3g.zdbjq.cn/Article/details/gtaambzbe.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.fehbvm.com/Article/details/gctbwfqop.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.hesvh.cn/Article/details/gixrtoopo.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.fehbvm.com/Article/details/gjlmutjtj.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.zdbjq.cn/Article/details/gmwfoekuh.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.fehbvm.com/Article/details/gvfvkrqef.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.fehbvm.com/Article/details/gumfgauug.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.hesvh.cn/Article/details/gqwoqfpwa.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.zdbjq.cn/Article/details/gnlghtrix.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.fehbvm.com/Article/details/grrhfscpa.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.hesvh.cn/Article/details/ghwijduon.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.zdbjq.cn/Article/details/gorjrwxyv.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.hesvh.cn/Article/details/gcjgmugdc.sHtML

Ruby: threads.map(&:join)
来源：http://blog.zdbjq.cn/Article/details/gqnewewqj.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.zdbjq.cn/Article/details/gsjersiyg.sHtML

[O06] 使用进程池
来源：http://blog.zdbjq.cn/Article/details/glggdswjo.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.hesvh.cn/Article/details/gaytqluig.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.fehbvm.com/Article/details/gpjrelzia.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.zdbjq.cn/Article/details/gedvfvhnx.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.fehbvm.com/Article/details/gtstajwgh.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.fehbvm.com/Article/details/gkhhrtemq.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.fehbvm.com/Article/details/gysmchaif.sHtML

Ruby: // fork 块
来源：http://baike.fehbvm.com/Article/details/gtfevxlnm.sHtML

C#:   Parallel.For
来源：http://www.blog.hesvh.cn/Article/details/gcfcixrkj.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/glvbpeikj.sHtML

P. 常用工具函数
来源：http://baike.fehbvm.com/Article/details/gvqurqcxe.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gwutrvkcj.sHtML

[P01] 生成 UUID
来源：http://read.share.zdbjq.cn/Article/details/gwhlkgmaq.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.zdbjq.cn/Article/details/geigjduui.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.hesvh.cn/Article/details/gcxdefuqy.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.fehbvm.com/Article/details/gchaqqrtc.sHtML

TS:   crypto.randomUUID()
来源：http://baike.zdbjq.cn/Article/details/gvcidqfoh.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.fehbvm.com/Article/details/gwxsvecxm.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.hesvh.cn/Article/details/gbcdjkudm.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.fehbvm.com/Article/details/gmjdpkehn.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.fehbvm.com/Article/details/gqnbgtuaz.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.zdbjq.cn/Article/details/glxqsiesb.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.fehbvm.com/Article/details/gakqbactr.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.hesvh.cn/Article/details/gvqfzbwnx.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.zdbjq.cn/Article/details/gqsovnnhj.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.zdbjq.cn/Article/details/grasikchg.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.fehbvm.com/Article/details/glnsskavx.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.zdbjq.cn/Article/details/gzpxvlkey.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.hesvh.cn/Article/details/gncgagmqd.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.zdbjq.cn/Article/details/gsbkoekxj.sHtML

[P03] 生成短随机字符串
来源：http://www.share.zdbjq.cn/Article/details/guwqciglb.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.zdbjq.cn/Article/details/gkxwbgvoc.sHtML


<!-- 参考信息 -->