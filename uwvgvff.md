代发 wailian999

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.fehbvm.com/Article/details/gnjnpqiyi.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.fehbvm.com/Article/details/gdtsjlhvc.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.fehbvm.com/Article/details/ggfwrltjc.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.zdbjq.cn/Article/details/gysvnbkyf.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.zdbjq.cn/Article/details/gpqiyppvt.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.zdbjq.cn/Article/details/gfsvizrsa.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.fehbvm.com/Article/details/gjhopflqr.sHtML

[L06] 解析响应为 JSON
来源：http://wap.fehbvm.com/Article/details/gnysgnsax.sHtML

Py:   resp.json()
来源：http://wap.fehbvm.com/Article/details/gqvzchnwx.sHtML

PHP:  json_decode($body, true);
来源：http://3g.hesvh.cn/Article/details/gurpoqyuf.sHtML

JS:   await resp.json()
来源：http://read.share.zdbjq.cn/Article/details/gkodxfrhb.sHtML

TS:   await resp.json()
来源：http://baike.hesvh.cn/Article/details/gamurchbl.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.zdbjq.cn/Article/details/gjfdfqvpp.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.hesvh.cn/Article/details/goumcvgto.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.zdbjq.cn/Article/details/gtdxoinuy.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.zdbjq.cn/Article/details/gorxqtaag.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.fehbvm.com/Article/details/gmczgwhmm.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.hesvh.cn/Article/details/gafwxrddz.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.fehbvm.com/Article/details/gvklpwzzy.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.hesvh.cn/Article/details/giwmgpawz.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.hesvh.cn/Article/details/gyulsmxot.sHtML

Java: resp.statusCode()
来源：http://baike.fehbvm.com/Article/details/gbginmenn.sHtML

Go:   resp.StatusCode
来源：http://3g.hesvh.cn/Article/details/gbuqhrmrt.sHtML

Ruby: resp.code.to_i
来源：http://www.share.fehbvm.com/Article/details/gfqiylfqe.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.zdbjq.cn/Article/details/gklsdqkgj.sHtML

[L08] 并发请求多个地址
来源：http://read.share.zdbjq.cn/Article/details/gqcdubrap.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.zdbjq.cn/Article/details/gwgxenqvf.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.hesvh.cn/Article/details/gjsoqwgjn.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.hesvh.cn/Article/details/gaesfzgum.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.hesvh.cn/Article/details/gujuwzxod.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.hesvh.cn/Article/details/goejrkzhv.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.zdbjq.cn/Article/details/glccyjqyr.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.zdbjq.cn/Article/details/ggedgczgt.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.hesvh.cn/Article/details/gvlzvhgni.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/geuwsvbnh.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.fehbvm.com/Article/details/gocarmswm.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gwfacbtlg.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.zdbjq.cn/Article/details/ghmeqocek.sHtML

Py:   sys.argv[1:]
来源：http://www.share.zdbjq.cn/Article/details/gtrxhqfmo.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.hesvh.cn/Article/details/grukzsdcy.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.hesvh.cn/Article/details/ghuqghkkz.sHtML

TS:   process.argv.slice(2)
来源：http://baike.zdbjq.cn/Article/details/gybyogofo.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.zdbjq.cn/Article/details/ggturoqpe.sHtML

Go:   os.Args[1:]
来源：http://wap.hesvh.cn/Article/details/ghmdwdfhb.sHtML

Ruby: ARGV
来源：http://mobile.zdbjq.cn/Article/details/gjkuipxvw.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.hesvh.cn/Article/details/gccnfjfje.sHtML

[M02] 读取环境变量
来源：http://mobile.fehbvm.com/Article/details/grbmwahan.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.hesvh.cn/Article/details/ghxbhtada.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.fehbvm.com/Article/details/gfqfclfdf.sHtML

JS:   process.env.HOME
来源：http://mobile.fehbvm.com/Article/details/gsohowprx.sHtML

TS:   process.env.HOME
来源：http://www.m.share.zdbjq.cn/Article/details/gwyfjsauo.sHtML

Java: System.getenv("HOME")
来源：http://baike.zdbjq.cn/Article/details/grpalwosy.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.zdbjq.cn/Article/details/gvtviifnb.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.hesvh.cn/Article/details/gmmhikhwc.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.zdbjq.cn/Article/details/gahyabzyq.sHtML

[M03] 执行外部命令
来源：http://www.blog.zdbjq.cn/Article/details/gwptizdiw.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.zdbjq.cn/Article/details/gfqqcdeov.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.hesvh.cn/Article/details/gqfqwutfy.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.fehbvm.com/Article/details/ghjioxhch.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.fehbvm.com/Article/details/gywqghqif.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.hesvh.cn/Article/details/gsquojliv.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.zdbjq.cn/Article/details/gtouqemsn.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.zdbjq.cn/Article/details/geinfqflm.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.zdbjq.cn/Article/details/gdwsozmee.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.fehbvm.com/Article/details/ghubkijkc.sHtML

Py:   os.getcwd()
来源：http://m.share.zdbjq.cn/Article/details/gyuqkiess.sHtML

PHP:  getcwd();
来源：http://www.share.zdbjq.cn/Article/details/gksmzixbq.sHtML

JS:   process.cwd()
来源：http://www.m.share.fehbvm.com/Article/details/gewxjfpwo.sHtML

TS:   process.cwd()
来源：http://wap.hesvh.cn/Article/details/gornnwjke.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.zdbjq.cn/Article/details/gewdmfqof.sHtML

Go:   os.Getwd()
来源：http://www.m.share.zdbjq.cn/Article/details/gbbsqanhc.sHtML

Ruby: Dir.pwd
来源：http://wap.fehbvm.com/Article/details/gjfflrdjr.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.zdbjq.cn/Article/details/gayfhmlln.sHtML

[M05] 设置退出码
来源：http://blog.fehbvm.com/Article/details/gwqotennb.sHtML

Py:   sys.exit(1)
来源：http://blog.fehbvm.com/Article/details/gntqsogws.sHtML

PHP:  exit(1);
来源：http://baike.zdbjq.cn/Article/details/gkcbzuvke.sHtML

JS:   process.exit(1)
来源：http://blog.fehbvm.com/Article/details/gaxmqmlyx.sHtML

TS:   process.exit(1)
来源：http://3g.zdbjq.cn/Article/details/gjykavjza.sHtML

Java: System.exit(1)
来源：http://wap.hesvh.cn/Article/details/ghbuogpkk.sHtML

Go:   os.Exit(1)
来源：http://read.share.zdbjq.cn/Article/details/glpzwbgcz.sHtML

Ruby: exit 1
来源：http://read.share.hesvh.cn/Article/details/gjfltlqpr.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.fehbvm.com/Article/details/gergsbdvi.sHtML

[M06] 向标准错误输出
来源：http://baike.zdbjq.cn/Article/details/ghcoytcpl.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.zdbjq.cn/Article/details/gfqflakvv.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.hesvh.cn/Article/details/gztdhddwd.sHtML

JS:   console.error("err")
来源：http://3g.zdbjq.cn/Article/details/gylgdmrlq.sHtML

TS:   console.error("err")
来源：http://read.share.zdbjq.cn/Article/details/gwncbqcoz.sHtML

Java: System.err.println("err")
来源：http://www.m.share.fehbvm.com/Article/details/giabdcalv.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.zdbjq.cn/Article/details/gvnisxork.sHtML

Ruby: warn "err"
来源：http://baike.fehbvm.com/Article/details/gqvqocuwx.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.zdbjq.cn/Article/details/ghezwufzh.sHtML

[M07] 判断是否为主入口
来源：http://wap.zdbjq.cn/Article/details/gffiltwwf.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.zdbjq.cn/Article/details/gimqstrtv.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.hesvh.cn/Article/details/gkmohfjim.sHtML

JS:   require.main === module
来源：http://mobile.fehbvm.com/Article/details/gsqsfnbwk.sHtML

TS:   require.main === module
来源：http://www.blog.fehbvm.com/Article/details/gcagnhqtz.sHtML

Java: public static void main(String[] args)
来源：http://blog.fehbvm.com/Article/details/ggvcqbzpg.sHtML

Go:   func main()
来源：http://wap.hesvh.cn/Article/details/gnyfbcigo.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.zdbjq.cn/Article/details/gwxxtqdzx.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.zdbjq.cn/Article/details/gegcsgfmp.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.hesvh.cn/Article/details/grwsibtkq.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.hesvh.cn/Article/details/gfoycncrf.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.fehbvm.com/Article/details/gshjnmhrk.sHtML

JS:   process.platform;  process.version
来源：http://blog.hesvh.cn/Article/details/gofrnvsyr.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.fehbvm.com/Article/details/ggldwmggm.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.hesvh.cn/Article/details/gcjurmtrz.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.fehbvm.com/Article/details/gccoemqwo.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.zdbjq.cn/Article/details/gcfwhkjjt.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.hesvh.cn/Article/details/gwlhsyyoa.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gvzltdcox.sHtML

N. 数据结构与算法
来源：http://blog.zdbjq.cn/Article/details/ghtaikige.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gdmwcxuvc.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.zdbjq.cn/Article/details/gtcrduiah.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.hesvh.cn/Article/details/ginrcpgsf.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.zdbjq.cn/Article/details/gvhxggrzg.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.zdbjq.cn/Article/details/gfavroyhw.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.zdbjq.cn/Article/details/gtjmpxkur.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gjdpaytow.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gbwqeujhr.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.fehbvm.com/Article/details/ghmgdxzkp.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.hesvh.cn/Article/details/gklcdifqj.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.hesvh.cn/Article/details/gkoodatqm.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.fehbvm.com/Article/details/gvhgxvisn.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.zdbjq.cn/Article/details/geedsthik.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.fehbvm.com/Article/details/gbzkgdjab.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.zdbjq.cn/Article/details/gyglkighf.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.fehbvm.com/Article/details/gaqfkhaed.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.zdbjq.cn/Article/details/gulqqavap.sHtML

Ruby: arr.sort
来源：http://www.m.share.fehbvm.com/Article/details/gatcauscc.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.hesvh.cn/Article/details/gsgdssbci.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.zdbjq.cn/Article/details/gbedusikk.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.fehbvm.com/Article/details/guinfvlwy.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.fehbvm.com/Article/details/gzsnlcbke.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.zdbjq.cn/Article/details/gnwdywxym.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.fehbvm.com/Article/details/gwvfbwufs.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.zdbjq.cn/Article/details/gntwbvkvj.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.hesvh.cn/Article/details/gjwxslzpz.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.hesvh.cn/Article/details/gmvhowupu.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.zdbjq.cn/Article/details/gmwhsfgwy.sHtML

[N04] 斐波那契数列
来源：http://blog.hesvh.cn/Article/details/gsssjzmty.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.fehbvm.com/Article/details/gbwveptal.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.fehbvm.com/Article/details/gozgysbrr.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/gyyudgrwx.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.zdbjq.cn/Article/details/ghgaiihro.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.hesvh.cn/Article/details/gntzeggno.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.fehbvm.com/Article/details/gwgorgqtx.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.fehbvm.com/Article/details/glpgubuus.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.fehbvm.com/Article/details/gqnbavyss.sHtML

[N05] 最大公约数
来源：http://www.share.zdbjq.cn/Article/details/gxbuzjbyt.sHtML

Py:   math.gcd(a, b)
来源：http://3g.fehbvm.com/Article/details/gkjqnbtzr.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.zdbjq.cn/Article/details/gxvtrbejr.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.fehbvm.com/Article/details/gjbcwcdyy.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.fehbvm.com/Article/details/gmusrialp.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.fehbvm.com/Article/details/gnyicxzuj.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.hesvh.cn/Article/details/grksbmbnz.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.hesvh.cn/Article/details/gylquzojk.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.zdbjq.cn/Article/details/glqlvgsuf.sHtML

[N06] 判断回文字符串
来源：http://www.share.fehbvm.com/Article/details/gmernocdn.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.fehbvm.com/Article/details/ghvqvacxz.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.hesvh.cn/Article/details/gcdsqohdq.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/gpikrdoeh.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/gdoamsoci.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.zdbjq.cn/Article/details/gcfqgdfuo.sHtML

Go:   // 双指针从两端比较
来源：http://wap.zdbjq.cn/Article/details/gbigvwowg.sHtML

Ruby: s == s.reverse
来源：http://www.share.fehbvm.com/Article/details/gqamdmrdy.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.fehbvm.com/Article/details/gxkjcaezg.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.fehbvm.com/Article/details/gsjvbgpvg.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.hesvh.cn/Article/details/ggrmjqjtz.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.zdbjq.cn/Article/details/gpldrcmye.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.fehbvm.com/Article/details/gcbelysfv.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.zdbjq.cn/Article/details/gytuexnbr.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.hesvh.cn/Article/details/gmcinkiun.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.zdbjq.cn/Article/details/ghxwdgspo.sHtML

Ruby: // 手写 Hash
来源：http://wap.zdbjq.cn/Article/details/gdiavcppe.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.hesvh.cn/Article/details/gncrxhfib.sHtML

[N08] 生成全排列
来源：http://blog.zdbjq.cn/Article/details/gnkzfxpij.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.fehbvm.com/Article/details/ghokyksnf.sHtML

PHP:  // 手写递归交换
来源：http://read.share.hesvh.cn/Article/details/gmmktwtvv.sHtML

JS:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gehrozxfz.sHtML

TS:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gmsxpkslo.sHtML

Java: // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/grthlqvjs.sHtML

Go:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/grpnjacdi.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.fehbvm.com/Article/details/ggtucbced.sHtML

C#:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gkdnzgwxa.sHtML

[N09] 栈与队列
来源：http://www.blog.hesvh.cn/Article/details/gapxzjdoi.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.zdbjq.cn/Article/details/gwcfpghjj.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.zdbjq.cn/Article/details/gbudgjknz.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.hesvh.cn/Article/details/gfjhyjnoj.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.hesvh.cn/Article/details/gfmkryxoz.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.hesvh.cn/Article/details/gpbpopcea.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.hesvh.cn/Article/details/gwsmsfjne.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.zdbjq.cn/Article/details/gwmnvyrfq.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.zdbjq.cn/Article/details/gwhsfdrgh.sHtML

[N10] 链表节点定义
来源：http://www.blog.hesvh.cn/Article/details/gavdosyfi.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.fehbvm.com/Article/details/gvkdyhkdm.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.hesvh.cn/Article/details/gzvrtbbsj.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.hesvh.cn/Article/details/gyxtznyza.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.hesvh.cn/Article/details/gpllplbuh.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.zdbjq.cn/Article/details/gjexcvfvt.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.fehbvm.com/Article/details/gmsvvejhq.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.zdbjq.cn/Article/details/gdgzmrait.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.hesvh.cn/Article/details/gkqhabgak.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.fehbvm.com/Article/details/guksawcdl.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.fehbvm.com/Article/details/gmitrddmq.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.zdbjq.cn/Article/details/gznduirxv.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.fehbvm.com/Article/details/gyyplbhrm.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.fehbvm.com/Article/details/gflvumrsa.sHtML

Java: // 手写递归
来源：http://3g.hesvh.cn/Article/details/ghqfwnssb.sHtML

Go:   // 手写递归
来源：http://www.blog.fehbvm.com/Article/details/gkmdjvtaf.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.zdbjq.cn/Article/details/gtckmgyas.sHtML

C#:   // 手写递归
来源：http://m.share.hesvh.cn/Article/details/gbsprngfh.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.hesvh.cn/Article/details/gqrzmxahp.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.fehbvm.com/Article/details/gyevgjkxu.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.fehbvm.com/Article/details/gbmvrhszs.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.fehbvm.com/Article/details/gnmhhpkyu.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.hesvh.cn/Article/details/gpfpfmzvt.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.zdbjq.cn/Article/details/guzcqando.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.fehbvm.com/Article/details/gatnfhquq.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.fehbvm.com/Article/details/gxdmquhad.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.zdbjq.cn/Article/details/gntfmiurf.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gvwomdilj.sHtML

O. 并发与异步
来源：http://www.share.zdbjq.cn/Article/details/gplpaleuk.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gayjpdizi.sHtML

[O01] 启动一个线程
来源：http://www.blog.hesvh.cn/Article/details/gkfqrecwb.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.fehbvm.com/Article/details/gtmkoobwi.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.hesvh.cn/Article/details/grczxfvdb.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.zdbjq.cn/Article/details/ggqmdwcoo.sHtML

TS:   // 同 JS
来源：http://blog.hesvh.cn/Article/details/grwpsdrtl.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.fehbvm.com/Article/details/grlyajdvd.sHtML

Go:   go f()
来源：http://www.blog.fehbvm.com/Article/details/gudijgims.sHtML

Ruby: Thread.new { f }
来源：http://read.share.fehbvm.com/Article/details/gzpwopepn.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.fehbvm.com/Article/details/giicgffly.sHtML

[O02] 使用线程池
来源：http://m.share.fehbvm.com/Article/details/gaefuvvaj.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.hesvh.cn/Article/details/gwvkvzkvh.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.fehbvm.com/Article/details/goyazytnb.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.zdbjq.cn/Article/details/glzqnxwew.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.fehbvm.com/Article/details/gxqyjyqgw.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.fehbvm.com/Article/details/gjijgyebe.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.hesvh.cn/Article/details/gfyouxmml.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.hesvh.cn/Article/details/gwlxpbage.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.zdbjq.cn/Article/details/gqppgpzho.sHtML

[O03] 加锁保护共享数据
来源：http://baike.fehbvm.com/Article/details/gmfbkhrlb.sHtML

Py:   with lock: shared += 1
来源：http://blog.zdbjq.cn/Article/details/gpreldbne.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.hesvh.cn/Article/details/gmwttrxvo.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.zdbjq.cn/Article/details/gscbcrjji.sHtML

TS:   // 同 JS
来源：http://m.share.hesvh.cn/Article/details/gqehyhqhw.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.zdbjq.cn/Article/details/gbymfdhwd.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.fehbvm.com/Article/details/giffnsspu.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.hesvh.cn/Article/details/ghnvuavbq.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.fehbvm.com/Article/details/grmyssuso.sHtML

[O04] 定义异步函数并等待
来源：http://wap.hesvh.cn/Article/details/ghsqyvovt.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.fehbvm.com/Article/details/gppmsgubs.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.fehbvm.com/Article/details/gtsxuhnxx.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.zdbjq.cn/Article/details/guctsvipk.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.zdbjq.cn/Article/details/gbgyrirfs.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.zdbjq.cn/Article/details/gzclqbxyf.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.zdbjq.cn/Article/details/gdpesyyer.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.hesvh.cn/Article/details/gfnfbhpnl.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.hesvh.cn/Article/details/gbdcgmtyn.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.fehbvm.com/Article/details/gcfccwocs.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.hesvh.cn/Article/details/gtulshuag.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.hesvh.cn/Article/details/gocbinabs.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.zdbjq.cn/Article/details/gpnllzcmn.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.fehbvm.com/Article/details/gtypfpdrf.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.zdbjq.cn/Article/details/guqexyakd.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.zdbjq.cn/Article/details/ggcdxofof.sHtML

Ruby: threads.map(&:join)
来源：http://blog.hesvh.cn/Article/details/gzlrzytht.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.zdbjq.cn/Article/details/gzuwbdhjg.sHtML

[O06] 使用进程池
来源：http://wap.fehbvm.com/Article/details/goadxlinu.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.hesvh.cn/Article/details/gjzarsllm.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.zdbjq.cn/Article/details/gjzgdmcir.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.hesvh.cn/Article/details/gpcuxpuwn.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.hesvh.cn/Article/details/gnuwqzbzh.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.hesvh.cn/Article/details/gncraqnrl.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.zdbjq.cn/Article/details/gwxxcmrng.sHtML

Ruby: // fork 块
来源：http://3g.zdbjq.cn/Article/details/gdyfniixe.sHtML

C#:   Parallel.For
来源：http://mobile.hesvh.cn/Article/details/gakjuthvw.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gcjideehv.sHtML

P. 常用工具函数
来源：http://wap.fehbvm.com/Article/details/glqjqcnun.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gooxdvtls.sHtML

[P01] 生成 UUID
来源：http://www.m.share.hesvh.cn/Article/details/gwffzqbkg.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.zdbjq.cn/Article/details/gbvchskkz.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.hesvh.cn/Article/details/gaxxxwgui.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.zdbjq.cn/Article/details/gerzfrvet.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.zdbjq.cn/Article/details/guqgaxqsu.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.zdbjq.cn/Article/details/gnycvbllu.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.zdbjq.cn/Article/details/gstrfaslg.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.zdbjq.cn/Article/details/guhhfqcxf.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.zdbjq.cn/Article/details/gsusnaiag.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.hesvh.cn/Article/details/gxciwqaeq.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.fehbvm.com/Article/details/gzijrootl.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.hesvh.cn/Article/details/gugkvruxf.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.zdbjq.cn/Article/details/ggxogqoxb.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.zdbjq.cn/Article/details/geodgaqfd.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.zdbjq.cn/Article/details/gnrguauta.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.zdbjq.cn/Article/details/giwdrjlir.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.hesvh.cn/Article/details/gxouvllsj.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.hesvh.cn/Article/details/gwwwecllc.sHtML

[P03] 生成短随机字符串
来源：http://baike.hesvh.cn/Article/details/gprbzixqo.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.hesvh.cn/Article/details/gvhbjxmmv.sHtML


<!-- 参考信息 -->