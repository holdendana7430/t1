代发 wailian999

[L07] 处理 HTTP 状态码
来源：http://mobile.hesvh.cn/Article/details/gucyklnvf.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.fehbvm.com/Article/details/gwfrmnxmn.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.hesvh.cn/Article/details/gjmravwil.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.fehbvm.com/Article/details/gzuwksesb.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.fehbvm.com/Article/details/gqbukstwu.sHtML

Java: resp.statusCode()
来源：http://read.share.hesvh.cn/Article/details/gjlymdxvb.sHtML

Go:   resp.StatusCode
来源：http://www.share.hesvh.cn/Article/details/gcffojtxr.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.fehbvm.com/Article/details/gurqzldoj.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.hesvh.cn/Article/details/gkucmnpav.sHtML

[L08] 并发请求多个地址
来源：http://read.share.zdbjq.cn/Article/details/gchsqigkx.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.zdbjq.cn/Article/details/gemfzjkkk.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.fehbvm.com/Article/details/ginlvqott.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.fehbvm.com/Article/details/gnxvbnmgd.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.zdbjq.cn/Article/details/gnhynddqt.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.hesvh.cn/Article/details/grqpqswjx.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.zdbjq.cn/Article/details/gctgoqegi.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.fehbvm.com/Article/details/gmytgpzoj.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.fehbvm.com/Article/details/guumkgvxz.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gfedtnrkg.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.zdbjq.cn/Article/details/guriqlfcp.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/ghprbwqbr.sHtML

[M01] 读取命令行参数
来源：http://m.share.hesvh.cn/Article/details/gryszoint.sHtML

Py:   sys.argv[1:]
来源：http://3g.hesvh.cn/Article/details/gjerplmxx.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.fehbvm.com/Article/details/gtughdeiz.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.hesvh.cn/Article/details/gulpyepix.sHtML

TS:   process.argv.slice(2)
来源：http://baike.zdbjq.cn/Article/details/gkxdwsinj.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.fehbvm.com/Article/details/ghdnkcfgd.sHtML

Go:   os.Args[1:]
来源：http://mobile.fehbvm.com/Article/details/gefevblow.sHtML

Ruby: ARGV
来源：http://m.share.hesvh.cn/Article/details/grczhnhsi.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.zdbjq.cn/Article/details/geoppcorf.sHtML

[M02] 读取环境变量
来源：http://3g.fehbvm.com/Article/details/gbmiiqvad.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.hesvh.cn/Article/details/guhvvgjyp.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.hesvh.cn/Article/details/gychlkjgu.sHtML

JS:   process.env.HOME
来源：http://www.blog.hesvh.cn/Article/details/geoxrfyxm.sHtML

TS:   process.env.HOME
来源：http://m.share.fehbvm.com/Article/details/gtconbmsv.sHtML

Java: System.getenv("HOME")
来源：http://baike.hesvh.cn/Article/details/gzxkzxqiy.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.fehbvm.com/Article/details/gnfbfqmek.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.hesvh.cn/Article/details/gphovhlpj.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.zdbjq.cn/Article/details/gmdfreyoz.sHtML

[M03] 执行外部命令
来源：http://www.m.share.hesvh.cn/Article/details/gvxcgjlkx.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.hesvh.cn/Article/details/gponkdcfm.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.hesvh.cn/Article/details/gjsuvurek.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.zdbjq.cn/Article/details/gkzzsbujh.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.zdbjq.cn/Article/details/geslisfuk.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.zdbjq.cn/Article/details/gpzvsttuv.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.hesvh.cn/Article/details/grhewpznl.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.hesvh.cn/Article/details/gtogqecwo.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.hesvh.cn/Article/details/ghzgdukhe.sHtML

[M04] 获取当前工作目录
来源：http://blog.zdbjq.cn/Article/details/gyvygxftl.sHtML

Py:   os.getcwd()
来源：http://read.share.hesvh.cn/Article/details/glwaaqhpf.sHtML

PHP:  getcwd();
来源：http://3g.hesvh.cn/Article/details/gjlruahme.sHtML

JS:   process.cwd()
来源：http://www.share.fehbvm.com/Article/details/guudppbtw.sHtML

TS:   process.cwd()
来源：http://www.share.zdbjq.cn/Article/details/gnwttwvky.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.fehbvm.com/Article/details/gczghgfqf.sHtML

Go:   os.Getwd()
来源：http://m.share.zdbjq.cn/Article/details/gfjjlxukk.sHtML

Ruby: Dir.pwd
来源：http://3g.zdbjq.cn/Article/details/gqvurdkiq.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.zdbjq.cn/Article/details/gobxooiel.sHtML

[M05] 设置退出码
来源：http://www.blog.hesvh.cn/Article/details/gozfkeygq.sHtML

Py:   sys.exit(1)
来源：http://baike.fehbvm.com/Article/details/ghokfeurp.sHtML

PHP:  exit(1);
来源：http://blog.fehbvm.com/Article/details/gyahvxoyh.sHtML

JS:   process.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gryiojoxr.sHtML

TS:   process.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gzwndblgm.sHtML

Java: System.exit(1)
来源：http://blog.fehbvm.com/Article/details/gyhbtryqq.sHtML

Go:   os.Exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gcfuxmtik.sHtML

Ruby: exit 1
来源：http://wap.zdbjq.cn/Article/details/gyxwjxjsy.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.fehbvm.com/Article/details/gipaircyn.sHtML

[M06] 向标准错误输出
来源：http://3g.zdbjq.cn/Article/details/gehxmfedv.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.zdbjq.cn/Article/details/gzqgkrsiv.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.fehbvm.com/Article/details/gxxjzxack.sHtML

JS:   console.error("err")
来源：http://www.m.share.hesvh.cn/Article/details/gvdmuhlto.sHtML

TS:   console.error("err")
来源：http://www.blog.hesvh.cn/Article/details/gqswbrehu.sHtML

Java: System.err.println("err")
来源：http://mobile.fehbvm.com/Article/details/ghhkiyxjt.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.hesvh.cn/Article/details/gbzaujkhi.sHtML

Ruby: warn "err"
来源：http://mobile.hesvh.cn/Article/details/gcsyiyqvq.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.fehbvm.com/Article/details/gownacbty.sHtML

[M07] 判断是否为主入口
来源：http://3g.zdbjq.cn/Article/details/gnlfovnzy.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.zdbjq.cn/Article/details/gxeutdibw.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.hesvh.cn/Article/details/gsleitxbr.sHtML

JS:   require.main === module
来源：http://mobile.hesvh.cn/Article/details/gppwbljxt.sHtML

TS:   require.main === module
来源：http://blog.zdbjq.cn/Article/details/gbrkarssw.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.zdbjq.cn/Article/details/grytdiaby.sHtML

Go:   func main()
来源：http://www.blog.hesvh.cn/Article/details/gfojenvtz.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.fehbvm.com/Article/details/guxfwfhbm.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.fehbvm.com/Article/details/gequyedcn.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.hesvh.cn/Article/details/gfytwrkgw.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.fehbvm.com/Article/details/gamhwstdb.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.hesvh.cn/Article/details/gvjbrxxzp.sHtML

JS:   process.platform;  process.version
来源：http://wap.fehbvm.com/Article/details/gokmzzgna.sHtML

TS:   process.platform;  process.version
来源：http://wap.hesvh.cn/Article/details/gqfzebosc.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.hesvh.cn/Article/details/gljnhgjwy.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.zdbjq.cn/Article/details/gkmdrxwsa.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.hesvh.cn/Article/details/geenryuos.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.zdbjq.cn/Article/details/gadxigvbf.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/ghwtnvmgz.sHtML

N. 数据结构与算法
来源：http://m.share.hesvh.cn/Article/details/gzmtpuijk.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/giyvuojev.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.fehbvm.com/Article/details/gpvxubklh.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.fehbvm.com/Article/details/gyyiwvlbl.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.zdbjq.cn/Article/details/gdtrcxdut.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.zdbjq.cn/Article/details/gakqnnpar.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.fehbvm.com/Article/details/gddjjwygq.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.fehbvm.com/Article/details/gpzeqmauq.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.hesvh.cn/Article/details/genbtvwnn.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.zdbjq.cn/Article/details/gpfceqgeu.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gjqidurgk.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.fehbvm.com/Article/details/gzyiqxjek.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.hesvh.cn/Article/details/gnelvafki.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.fehbvm.com/Article/details/geucyvank.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.zdbjq.cn/Article/details/gxxywuvky.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.fehbvm.com/Article/details/gtrdsddal.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.fehbvm.com/Article/details/gzrbfziom.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.hesvh.cn/Article/details/gdbwimsqm.sHtML

Ruby: arr.sort
来源：http://www.blog.fehbvm.com/Article/details/gfmpnrgqy.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.hesvh.cn/Article/details/gnrojjegz.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.zdbjq.cn/Article/details/gtiuhwsgu.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.zdbjq.cn/Article/details/guwdtmyxj.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.hesvh.cn/Article/details/gbwtchmtn.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.fehbvm.com/Article/details/gexmazopw.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.fehbvm.com/Article/details/githiyjkk.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.hesvh.cn/Article/details/gaxeiqgkq.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.hesvh.cn/Article/details/gpcqrgowf.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.fehbvm.com/Article/details/geomcajhq.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.fehbvm.com/Article/details/gvdkfbpid.sHtML

[N04] 斐波那契数列
来源：http://m.share.hesvh.cn/Article/details/ghpbnpbql.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.fehbvm.com/Article/details/gvgfafbpq.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.zdbjq.cn/Article/details/gbubgnuec.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.fehbvm.com/Article/details/gtkhvtmjz.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.zdbjq.cn/Article/details/gmgdyyrfh.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.zdbjq.cn/Article/details/guntzetuz.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.hesvh.cn/Article/details/gazaulorm.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.zdbjq.cn/Article/details/glgcmvvag.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.zdbjq.cn/Article/details/glmdkuvnl.sHtML

[N05] 最大公约数
来源：http://www.blog.fehbvm.com/Article/details/gzwyashxa.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.hesvh.cn/Article/details/gfdogukom.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.fehbvm.com/Article/details/gmyaworgj.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.fehbvm.com/Article/details/ghuygwcan.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.hesvh.cn/Article/details/gtkufmtzb.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.fehbvm.com/Article/details/girgwhwwr.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.fehbvm.com/Article/details/glqqlpcgm.sHtML

Ruby: a.gcd(b)
来源：http://3g.hesvh.cn/Article/details/gzgcmjjcc.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.hesvh.cn/Article/details/gnqmmrebw.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.hesvh.cn/Article/details/giuaztbei.sHtML

Py:   s == s[::-1]
来源：http://mobile.fehbvm.com/Article/details/gmixxcnfv.sHtML

PHP:  $s === strrev($s);
来源：http://3g.fehbvm.com/Article/details/gkkcrcrns.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/gwsksqqok.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/gruovhkim.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.hesvh.cn/Article/details/gnfgiwzir.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.fehbvm.com/Article/details/gqiyzbhrb.sHtML

Ruby: s == s.reverse
来源：http://www.blog.zdbjq.cn/Article/details/grecfteuc.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.zdbjq.cn/Article/details/gygacyfqy.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.fehbvm.com/Article/details/gdhijspyi.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.zdbjq.cn/Article/details/gmcehfiqp.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.hesvh.cn/Article/details/ghigrsoma.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.zdbjq.cn/Article/details/goarjfirg.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.fehbvm.com/Article/details/gasarahjm.sHtML

Java: // 手写 HashMap
来源：http://www.share.fehbvm.com/Article/details/gacwjbrqc.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.fehbvm.com/Article/details/gvehwafda.sHtML

Ruby: // 手写 Hash
来源：http://m.share.zdbjq.cn/Article/details/gjbtpkzac.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.zdbjq.cn/Article/details/ggghbnmpl.sHtML

[N08] 生成全排列
来源：http://www.blog.fehbvm.com/Article/details/gxneuthop.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.hesvh.cn/Article/details/gywwmcfld.sHtML

PHP:  // 手写递归交换
来源：http://baike.hesvh.cn/Article/details/gzathhqwm.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gsjhsqdct.sHtML

TS:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gxmpgfwks.sHtML

Java: // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gctubhgle.sHtML

Go:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/ggvfsotuq.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.zdbjq.cn/Article/details/gcqxestcx.sHtML

C#:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gqvmbooxe.sHtML

[N09] 栈与队列
来源：http://blog.fehbvm.com/Article/details/gbwqiocib.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.fehbvm.com/Article/details/gsxcnkujz.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.zdbjq.cn/Article/details/gjlgcxaai.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.fehbvm.com/Article/details/gpgiidbvw.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.fehbvm.com/Article/details/gkbglpzqv.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.hesvh.cn/Article/details/glkyefutu.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.zdbjq.cn/Article/details/gkiymoida.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.zdbjq.cn/Article/details/gvcqcskho.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.zdbjq.cn/Article/details/gtyfgnatr.sHtML

[N10] 链表节点定义
来源：http://3g.fehbvm.com/Article/details/gzbftbdrw.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.hesvh.cn/Article/details/gbpylzvkx.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.hesvh.cn/Article/details/gaxbmudmr.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.hesvh.cn/Article/details/guqoeutkk.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.fehbvm.com/Article/details/gyxizgdfw.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.fehbvm.com/Article/details/ghqpdahho.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.hesvh.cn/Article/details/gcqyjtppo.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.fehbvm.com/Article/details/geziwrbbx.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.hesvh.cn/Article/details/gnqifnfbz.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.fehbvm.com/Article/details/gfdbvfhfv.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.zdbjq.cn/Article/details/gvnipacoj.sHtML

PHP:  // 手写递归函数
来源：http://wap.fehbvm.com/Article/details/gkscltlni.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.hesvh.cn/Article/details/gfcartzjy.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.fehbvm.com/Article/details/ggcedsjja.sHtML

Java: // 手写递归
来源：http://mobile.fehbvm.com/Article/details/gpsxzywmj.sHtML

Go:   // 手写递归
来源：http://www.blog.hesvh.cn/Article/details/givqgnhlh.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.fehbvm.com/Article/details/gqtfeuxgz.sHtML

C#:   // 手写递归
来源：http://www.m.share.hesvh.cn/Article/details/gpnsqbmwk.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.zdbjq.cn/Article/details/gapaacypv.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.hesvh.cn/Article/details/glnhqmqhz.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.hesvh.cn/Article/details/ghtbgoxlw.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.hesvh.cn/Article/details/ggkvzipom.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.hesvh.cn/Article/details/gicxikwri.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.hesvh.cn/Article/details/gzwgiipcc.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.hesvh.cn/Article/details/gfpkpjyyx.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.zdbjq.cn/Article/details/ggjsnldji.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.hesvh.cn/Article/details/gzewxvdcw.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gsrzduanh.sHtML

O. 并发与异步
来源：http://baike.zdbjq.cn/Article/details/gyvuohqul.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/glzkgxlpw.sHtML

[O01] 启动一个线程
来源：http://www.blog.hesvh.cn/Article/details/gumvsdipj.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.hesvh.cn/Article/details/gkoqprxtt.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.hesvh.cn/Article/details/gtiaqgwmo.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.zdbjq.cn/Article/details/ghnycnudc.sHtML

TS:   // 同 JS
来源：http://read.share.fehbvm.com/Article/details/gbbhsubtx.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.fehbvm.com/Article/details/ggrdxfhbl.sHtML

Go:   go f()
来源：http://www.blog.zdbjq.cn/Article/details/gtiyjyeds.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.hesvh.cn/Article/details/gbzssukbn.sHtML

C#:   Task.Run(() => F());
来源：http://3g.zdbjq.cn/Article/details/gpbpjlclr.sHtML

[O02] 使用线程池
来源：http://3g.fehbvm.com/Article/details/gqgkplhrc.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.hesvh.cn/Article/details/gaoizbhya.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.fehbvm.com/Article/details/gsjobyfha.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.hesvh.cn/Article/details/gjownuhnq.sHtML

TS:   // worker_threads 线程池
来源：http://3g.zdbjq.cn/Article/details/gkuzuemdt.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.fehbvm.com/Article/details/gjcwsxjeh.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.hesvh.cn/Article/details/gliutjlxp.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.zdbjq.cn/Article/details/gbagpbxyr.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.zdbjq.cn/Article/details/gxibsgolu.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.hesvh.cn/Article/details/govtmkbuh.sHtML

Py:   with lock: shared += 1
来源：http://read.share.fehbvm.com/Article/details/gopeqqgzq.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.hesvh.cn/Article/details/gnjsljpys.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.fehbvm.com/Article/details/gawotszxf.sHtML

TS:   // 同 JS
来源：http://blog.hesvh.cn/Article/details/gfesfhita.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.hesvh.cn/Article/details/gsejevqyj.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.zdbjq.cn/Article/details/ghvcpbike.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.fehbvm.com/Article/details/gyiltlcft.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.zdbjq.cn/Article/details/gelwwwxer.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.fehbvm.com/Article/details/gpojlccur.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.hesvh.cn/Article/details/gjijxegmz.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.fehbvm.com/Article/details/gvepsnsup.sHtML

JS:   async function f() { await g(); }
来源：http://blog.zdbjq.cn/Article/details/gxnavtbjs.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.zdbjq.cn/Article/details/gstyuafoi.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.hesvh.cn/Article/details/gywjovpdh.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.fehbvm.com/Article/details/gmwtumajm.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.zdbjq.cn/Article/details/grgppgsxt.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.hesvh.cn/Article/details/gygldxobm.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.hesvh.cn/Article/details/gyqogrhzt.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.zdbjq.cn/Article/details/genygoiqy.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.zdbjq.cn/Article/details/gbnptpvtz.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.hesvh.cn/Article/details/gwifvriyf.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.zdbjq.cn/Article/details/gjwnxpqpi.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.fehbvm.com/Article/details/gvnnvqufd.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.fehbvm.com/Article/details/gkupnpoio.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.zdbjq.cn/Article/details/gauoadynl.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.zdbjq.cn/Article/details/gatqgyqmb.sHtML

[O06] 使用进程池
来源：http://www.share.zdbjq.cn/Article/details/gjylkwtgz.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.fehbvm.com/Article/details/gacdssfjd.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.hesvh.cn/Article/details/gpfctaihh.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.hesvh.cn/Article/details/gazutxjgc.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.fehbvm.com/Article/details/gplqwwlll.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.zdbjq.cn/Article/details/gtshfnyxq.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.fehbvm.com/Article/details/gnlqddlpc.sHtML

Ruby: // fork 块
来源：http://www.m.share.fehbvm.com/Article/details/guxysbavq.sHtML

C#:   Parallel.For
来源：http://read.share.hesvh.cn/Article/details/ghzwbnbqt.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gbsslfnno.sHtML

P. 常用工具函数
来源：http://blog.zdbjq.cn/Article/details/ghdqlzoxm.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gzdzniprj.sHtML

[P01] 生成 UUID
来源：http://m.share.fehbvm.com/Article/details/gqiqcrawz.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.fehbvm.com/Article/details/goklhnkbh.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.fehbvm.com/Article/details/gbysnahkp.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.fehbvm.com/Article/details/gjagqfwmu.sHtML

TS:   crypto.randomUUID()
来源：http://blog.hesvh.cn/Article/details/gtcvyxwoa.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.fehbvm.com/Article/details/gihgdqrsg.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.fehbvm.com/Article/details/gkpjujjqi.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.hesvh.cn/Article/details/gxdcqclbn.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.hesvh.cn/Article/details/gqrmukpsj.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.hesvh.cn/Article/details/gruuilrpv.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.fehbvm.com/Article/details/gjovpugkl.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.hesvh.cn/Article/details/gnfporjfi.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.hesvh.cn/Article/details/geslyzmyr.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.zdbjq.cn/Article/details/gjgyxzxbk.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.fehbvm.com/Article/details/giqkvbvlc.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.fehbvm.com/Article/details/gbpemcjts.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.hesvh.cn/Article/details/gwctosluk.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.zdbjq.cn/Article/details/gietelpob.sHtML

[P03] 生成短随机字符串
来源：http://m.share.zdbjq.cn/Article/details/gtfuhaglk.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.zdbjq.cn/Article/details/gzxbhfyrd.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.hesvh.cn/Article/details/gmtmmkmhh.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.fehbvm.com/Article/details/ggaphhzks.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.zdbjq.cn/Article/details/gtxgkrfcu.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.zdbjq.cn/Article/details/gwkisvbfl.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.hesvh.cn/Article/details/gmhnswqrs.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.hesvh.cn/Article/details/gnggibyas.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.zdbjq.cn/Article/details/gabilmixd.sHtML

[P04] 求长度
来源：http://wap.hesvh.cn/Article/details/gwyzvqvff.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.hesvh.cn/Article/details/gjfihsqzk.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.hesvh.cn/Article/details/gacrburki.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.zdbjq.cn/Article/details/gfglovuvp.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.fehbvm.com/Article/details/gbrmliamj.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.zdbjq.cn/Article/details/gernavguc.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.fehbvm.com/Article/details/gdyhixgve.sHtML

Ruby: x.length;  x.size
来源：http://baike.hesvh.cn/Article/details/gdhjuhlaz.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.fehbvm.com/Article/details/gspmswziu.sHtML


<!-- 参考信息 -->