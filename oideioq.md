代发 wailian999

C#:   (int)resp.StatusCode
来源：http://3g.fanxiaobao.xyz/Article/details/gwjpdegtn.sHtML

[L08] 并发请求多个地址
来源：http://www.share.fanxiaobao.xyz/Article/details/gipnraikn.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.fanxiaobao.xyz/Article/details/gwolasocb.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.fanxiaobao.xyz/Article/details/gffdnklsh.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fanxiaobao.xyz/Article/details/gljjhkweb.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fanxiaobao.xyz/Article/details/gtdjbayzt.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.fanxiaobao.xyz/Article/details/gkbwtgzhq.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.fanxiaobao.xyz/Article/details/gefyddxbj.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.fanxiaobao.xyz/Article/details/guipabcfu.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.fanxiaobao.xyz/Article/details/gcxycbhqk.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/ggvvnuswq.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.fanxiaobao.xyz/Article/details/gcshgpmbp.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/grtcancdc.sHtML

[M01] 读取命令行参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gwkcopkit.sHtML

Py:   sys.argv[1:]
来源：http://blog.fanxiaobao.xyz/Article/details/gxqjznaat.sHtML

PHP:  $argv;  $argc;
来源：http://wap.fanxiaobao.xyz/Article/details/guuikxlda.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.fanxiaobao.xyz/Article/details/guzeidpia.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.fanxiaobao.xyz/Article/details/ghrerxbcm.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.fanxiaobao.xyz/Article/details/gocaodhcz.sHtML

Go:   os.Args[1:]
来源：http://3g.fanxiaobao.xyz/Article/details/gysjnfevt.sHtML

Ruby: ARGV
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwijlmlog.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.fanxiaobao.xyz/Article/details/gyhouaqli.sHtML

[M02] 读取环境变量
来源：http://baike.fanxiaobao.xyz/Article/details/gypdkufue.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.fanxiaobao.xyz/Article/details/gnmgaiwdm.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.fanxiaobao.xyz/Article/details/glwklntys.sHtML

JS:   process.env.HOME
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghqfambpu.sHtML

TS:   process.env.HOME
来源：http://baike.fanxiaobao.xyz/Article/details/gmotkhaww.sHtML

Java: System.getenv("HOME")
来源：http://read.share.fanxiaobao.xyz/Article/details/goramhqsz.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.fanxiaobao.xyz/Article/details/gzhfndxou.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gadvbgqwo.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gybfzmkfg.sHtML

[M03] 执行外部命令
来源：http://m.share.fanxiaobao.xyz/Article/details/gmugsgqsd.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.fanxiaobao.xyz/Article/details/gnymlvehr.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnuymqljq.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.fanxiaobao.xyz/Article/details/gvcbhsiis.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.fanxiaobao.xyz/Article/details/gxevoecie.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.fanxiaobao.xyz/Article/details/glgnzgwnz.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.fanxiaobao.xyz/Article/details/gnyzwqjmc.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.fanxiaobao.xyz/Article/details/gxactfnul.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.fanxiaobao.xyz/Article/details/gprzkchnn.sHtML

[M04] 获取当前工作目录
来源：http://blog.fanxiaobao.xyz/Article/details/gmjewyqur.sHtML

Py:   os.getcwd()
来源：http://read.share.fanxiaobao.xyz/Article/details/gycezstao.sHtML

PHP:  getcwd();
来源：http://blog.fanxiaobao.xyz/Article/details/gcjffcehx.sHtML

JS:   process.cwd()
来源：http://wap.fanxiaobao.xyz/Article/details/gfnficikm.sHtML

TS:   process.cwd()
来源：http://www.blog.fanxiaobao.xyz/Article/details/glqbitoqv.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.fanxiaobao.xyz/Article/details/gmqbxgsyq.sHtML

Go:   os.Getwd()
来源：http://www.share.fanxiaobao.xyz/Article/details/gktwvfoao.sHtML

Ruby: Dir.pwd
来源：http://baike.fanxiaobao.xyz/Article/details/gerkhljxf.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.fanxiaobao.xyz/Article/details/gyymfksfz.sHtML

[M05] 设置退出码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzkyqjgxz.sHtML

Py:   sys.exit(1)
来源：http://mobile.fanxiaobao.xyz/Article/details/ghtvjbotm.sHtML

PHP:  exit(1);
来源：http://read.share.fanxiaobao.xyz/Article/details/gydbspsly.sHtML

JS:   process.exit(1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gbonztslj.sHtML

TS:   process.exit(1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gplesjczk.sHtML

Java: System.exit(1)
来源：http://www.share.fanxiaobao.xyz/Article/details/ggnetwomm.sHtML

Go:   os.Exit(1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gnkglazhz.sHtML

Ruby: exit 1
来源：http://www.share.fanxiaobao.xyz/Article/details/gmynebdrf.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.fanxiaobao.xyz/Article/details/ggcdvqgyv.sHtML

[M06] 向标准错误输出
来源：http://www.share.fanxiaobao.xyz/Article/details/ghemowawo.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.fanxiaobao.xyz/Article/details/gyukfkqvj.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.fanxiaobao.xyz/Article/details/gamoysosf.sHtML

JS:   console.error("err")
来源：http://blog.fanxiaobao.xyz/Article/details/gtzeruhxj.sHtML

TS:   console.error("err")
来源：http://baike.fanxiaobao.xyz/Article/details/gawjbezof.sHtML

Java: System.err.println("err")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtwtblvnm.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.fanxiaobao.xyz/Article/details/gtkkuciax.sHtML

Ruby: warn "err"
来源：http://www.share.fanxiaobao.xyz/Article/details/gvkcifoim.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.fanxiaobao.xyz/Article/details/gcwihfmca.sHtML

[M07] 判断是否为主入口
来源：http://baike.fanxiaobao.xyz/Article/details/gbxapdrlc.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.fanxiaobao.xyz/Article/details/gyhvkmsyg.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkuklpnse.sHtML

JS:   require.main === module
来源：http://blog.fanxiaobao.xyz/Article/details/gayxyatpd.sHtML

TS:   require.main === module
来源：http://baike.fanxiaobao.xyz/Article/details/gtewabnlf.sHtML

Java: public static void main(String[] args)
来源：http://mobile.fanxiaobao.xyz/Article/details/gyvrzahgz.sHtML

Go:   func main()
来源：http://wap.fanxiaobao.xyz/Article/details/gytzrgbal.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.fanxiaobao.xyz/Article/details/gwjlaeped.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpdhmiyui.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.fanxiaobao.xyz/Article/details/gzbccenbb.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.fanxiaobao.xyz/Article/details/gvyiiczeg.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.fanxiaobao.xyz/Article/details/gvebpatvx.sHtML

JS:   process.platform;  process.version
来源：http://read.share.fanxiaobao.xyz/Article/details/gillomsze.sHtML

TS:   process.platform;  process.version
来源：http://read.share.fanxiaobao.xyz/Article/details/gsfgpnvjl.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.fanxiaobao.xyz/Article/details/gyixvtykn.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.fanxiaobao.xyz/Article/details/guxdqkfbz.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.fanxiaobao.xyz/Article/details/guseeqipq.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.fanxiaobao.xyz/Article/details/gredgspmo.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gzvfpxdlr.sHtML

N. 数据结构与算法
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goncnfrwr.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/goxmsvfiw.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.fanxiaobao.xyz/Article/details/gfwgfofhs.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.fanxiaobao.xyz/Article/details/gdpdynhdb.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.fanxiaobao.xyz/Article/details/glxewjejo.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.fanxiaobao.xyz/Article/details/gvzbdhjmq.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.fanxiaobao.xyz/Article/details/gwmmwdulv.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.fanxiaobao.xyz/Article/details/ghfnwcfkg.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.fanxiaobao.xyz/Article/details/gptieegvz.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.fanxiaobao.xyz/Article/details/gkdyrybvd.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.fanxiaobao.xyz/Article/details/gywiqnfnv.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.fanxiaobao.xyz/Article/details/grdzxwleu.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.fanxiaobao.xyz/Article/details/gzyeubqsi.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwqggnzue.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqzengtnf.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtumiprlq.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.fanxiaobao.xyz/Article/details/ghokghbhs.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.fanxiaobao.xyz/Article/details/gkcdgllob.sHtML

Ruby: arr.sort
来源：http://www.blog.fanxiaobao.xyz/Article/details/grqniylhr.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.fanxiaobao.xyz/Article/details/gzcyxcqgp.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.fanxiaobao.xyz/Article/details/gjzmhzndc.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.fanxiaobao.xyz/Article/details/gbiombtey.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.fanxiaobao.xyz/Article/details/gcibeycqc.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.fanxiaobao.xyz/Article/details/gnvcqjaop.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.fanxiaobao.xyz/Article/details/gojxitlyw.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.fanxiaobao.xyz/Article/details/gixjmzegg.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.fanxiaobao.xyz/Article/details/gknknrgmt.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.fanxiaobao.xyz/Article/details/giierrsep.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.fanxiaobao.xyz/Article/details/gdoaccxwi.sHtML

[N04] 斐波那契数列
来源：http://www.share.fanxiaobao.xyz/Article/details/goltcfpsa.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gygujmsax.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtiodzziv.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.fanxiaobao.xyz/Article/details/gwhukkznm.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.fanxiaobao.xyz/Article/details/gnxxpawpv.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghdlebatb.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.fanxiaobao.xyz/Article/details/gpmkhcvqn.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gwfcsaejg.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyfaomzxp.sHtML

[N05] 最大公约数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqlxpwmgj.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.fanxiaobao.xyz/Article/details/gufkhoolk.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gahyeebub.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqgxufmis.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdqaybehc.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.fanxiaobao.xyz/Article/details/gjzxlowni.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghvxtvwpi.sHtML

Ruby: a.gcd(b)
来源：http://m.share.fanxiaobao.xyz/Article/details/gtojikqbi.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gyyypsvuv.sHtML

[N06] 判断回文字符串
来源：http://wap.fanxiaobao.xyz/Article/details/ggaxjsxyt.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwfnwmyjp.sHtML

PHP:  $s === strrev($s);
来源：http://blog.fanxiaobao.xyz/Article/details/gcdlqqtpu.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.fanxiaobao.xyz/Article/details/gbyemlhay.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnfaucjug.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.fanxiaobao.xyz/Article/details/guobfjalo.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.fanxiaobao.xyz/Article/details/goypallbg.sHtML

Ruby: s == s.reverse
来源：http://m.share.fanxiaobao.xyz/Article/details/gkhvasglg.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.fanxiaobao.xyz/Article/details/glefrsqxr.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.fanxiaobao.xyz/Article/details/gbhpskxfm.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.fanxiaobao.xyz/Article/details/gjockbdrc.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.fanxiaobao.xyz/Article/details/gkjjikpqq.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.fanxiaobao.xyz/Article/details/govalgyhe.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.fanxiaobao.xyz/Article/details/gkqmrdaiz.sHtML

Java: // 手写 HashMap
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzgzsyzib.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.fanxiaobao.xyz/Article/details/gemyvlufv.sHtML

Ruby: // 手写 Hash
来源：http://www.share.fanxiaobao.xyz/Article/details/gyezlusxi.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.fanxiaobao.xyz/Article/details/girtfvklr.sHtML

[N08] 生成全排列
来源：http://baike.fanxiaobao.xyz/Article/details/gzpbvmqgi.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.fanxiaobao.xyz/Article/details/gwzzrrokc.sHtML

PHP:  // 手写递归交换
来源：http://m.share.fanxiaobao.xyz/Article/details/gzkupwzpn.sHtML

JS:   // 手写回溯递归
来源：http://wap.fanxiaobao.xyz/Article/details/gsinivqra.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.fanxiaobao.xyz/Article/details/glesowsms.sHtML

Java: // 手写回溯递归
来源：http://baike.fanxiaobao.xyz/Article/details/govmksumu.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjgssbgew.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.fanxiaobao.xyz/Article/details/glajwbtcq.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyfylchgt.sHtML

[N09] 栈与队列
来源：http://blog.fanxiaobao.xyz/Article/details/gmuqfrucr.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.fanxiaobao.xyz/Article/details/ggvdocxxj.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.fanxiaobao.xyz/Article/details/gswmhmytt.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gswaazxoo.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.fanxiaobao.xyz/Article/details/gypvtjfmp.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.fanxiaobao.xyz/Article/details/gnrntaijd.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbygjuwsj.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.fanxiaobao.xyz/Article/details/giemicwya.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsqaarkmq.sHtML

[N10] 链表节点定义
来源：http://wap.fanxiaobao.xyz/Article/details/gtrqijhwr.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.fanxiaobao.xyz/Article/details/gpktyxwpy.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.fanxiaobao.xyz/Article/details/gdasxzmrb.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.fanxiaobao.xyz/Article/details/gyxlnrdpq.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.fanxiaobao.xyz/Article/details/gawstrvfv.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gouglrfsq.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.fanxiaobao.xyz/Article/details/gynggmigf.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.fanxiaobao.xyz/Article/details/giohoycdx.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.fanxiaobao.xyz/Article/details/gjbyoimlf.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gkozvyedm.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbamqnsfa.sHtML

PHP:  // 手写递归函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gawpvbmai.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.fanxiaobao.xyz/Article/details/gusudhuje.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfkjymzqv.sHtML

Java: // 手写递归
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggmyfvhpq.sHtML

Go:   // 手写递归
来源：http://3g.fanxiaobao.xyz/Article/details/gqvyyyeyx.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.fanxiaobao.xyz/Article/details/ghthedvat.sHtML

C#:   // 手写递归
来源：http://wap.fanxiaobao.xyz/Article/details/glsklhskh.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.fanxiaobao.xyz/Article/details/goottdnxy.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdozzlgqv.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.fanxiaobao.xyz/Article/details/ggxxrhtlk.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.fanxiaobao.xyz/Article/details/goimtumsf.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbgpvucte.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.fanxiaobao.xyz/Article/details/gkzabttta.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gncwekzhj.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.fanxiaobao.xyz/Article/details/glabsdbpl.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.fanxiaobao.xyz/Article/details/giupvwfnl.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/geriwrbqb.sHtML

O. 并发与异步
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtzcdzfjg.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gjzkbavpj.sHtML

[O01] 启动一个线程
来源：http://read.share.fanxiaobao.xyz/Article/details/gridgkaxc.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.fanxiaobao.xyz/Article/details/gjsnvyhlj.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.fanxiaobao.xyz/Article/details/gokdmqkuy.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqiapmsra.sHtML

TS:   // 同 JS
来源：http://wap.fanxiaobao.xyz/Article/details/gxcxfhvjz.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.fanxiaobao.xyz/Article/details/gbfjbvxyr.sHtML

Go:   go f()
来源：http://read.share.fanxiaobao.xyz/Article/details/gmhmnmowk.sHtML

Ruby: Thread.new { f }
来源：http://baike.fanxiaobao.xyz/Article/details/gaujlrssm.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjhprpdcv.sHtML

[O02] 使用线程池
来源：http://wap.fanxiaobao.xyz/Article/details/gmfmhqivw.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.fanxiaobao.xyz/Article/details/ggysmgqfw.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.fanxiaobao.xyz/Article/details/gmgiiddxd.sHtML

JS:   // worker_threads 线程池
来源：http://wap.fanxiaobao.xyz/Article/details/grouzkjbo.sHtML

TS:   // worker_threads 线程池
来源：http://blog.fanxiaobao.xyz/Article/details/ghfgndnnx.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.fanxiaobao.xyz/Article/details/gorncoari.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqlhusuer.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.fanxiaobao.xyz/Article/details/gkxfqfjlk.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.fanxiaobao.xyz/Article/details/giaqbfqps.sHtML

[O03] 加锁保护共享数据
来源：http://baike.fanxiaobao.xyz/Article/details/ggwjuiomt.sHtML

Py:   with lock: shared += 1
来源：http://baike.fanxiaobao.xyz/Article/details/gxbonfyrh.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjzgjnuos.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.fanxiaobao.xyz/Article/details/gdbcbmxsl.sHtML

TS:   // 同 JS
来源：http://wap.fanxiaobao.xyz/Article/details/gytywfvsh.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjoymufyt.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.fanxiaobao.xyz/Article/details/gbhabldhq.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.fanxiaobao.xyz/Article/details/gdhqygugy.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.fanxiaobao.xyz/Article/details/grfxrwkqs.sHtML

[O04] 定义异步函数并等待
来源：http://blog.fanxiaobao.xyz/Article/details/gbviaxths.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.fanxiaobao.xyz/Article/details/gqnkgrvif.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.fanxiaobao.xyz/Article/details/ginvexbrz.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gygmirdyh.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpmzfikxi.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.fanxiaobao.xyz/Article/details/gbgwwcafv.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gouzfooya.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.fanxiaobao.xyz/Article/details/gcjcqqjqo.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.fanxiaobao.xyz/Article/details/gevgdyoux.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.fanxiaobao.xyz/Article/details/gzyydaxmu.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.fanxiaobao.xyz/Article/details/gurhzxypw.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.fanxiaobao.xyz/Article/details/gktmxkwez.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.fanxiaobao.xyz/Article/details/gyfdfzsuj.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/genxaskrn.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfxgxqafd.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqxqcmnun.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.fanxiaobao.xyz/Article/details/ginpzomrd.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.fanxiaobao.xyz/Article/details/gqubmxupu.sHtML

[O06] 使用进程池
来源：http://wap.fanxiaobao.xyz/Article/details/gtsofewkd.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.fanxiaobao.xyz/Article/details/gaazubufj.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.fanxiaobao.xyz/Article/details/gwjziwrun.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.fanxiaobao.xyz/Article/details/glalrcmtp.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.fanxiaobao.xyz/Article/details/gmvizoqor.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.fanxiaobao.xyz/Article/details/grlebtsbx.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.fanxiaobao.xyz/Article/details/gealiohsx.sHtML

Ruby: // fork 块
来源：http://baike.fanxiaobao.xyz/Article/details/gqauapgvu.sHtML

C#:   Parallel.For
来源：http://wap.fanxiaobao.xyz/Article/details/guglubhmm.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gbrkookhk.sHtML

P. 常用工具函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gjuhebgwu.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gybzfmrwm.sHtML

[P01] 生成 UUID
来源：http://3g.fanxiaobao.xyz/Article/details/gsdctuxnl.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.fanxiaobao.xyz/Article/details/gqnspiknr.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.fanxiaobao.xyz/Article/details/gobrmfkzw.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gydypvbsw.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.fanxiaobao.xyz/Article/details/gnbvewaxz.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.fanxiaobao.xyz/Article/details/gtjofuzae.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.fanxiaobao.xyz/Article/details/gwutajqsg.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.fanxiaobao.xyz/Article/details/gsqrlrpdq.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.fanxiaobao.xyz/Article/details/gaefpzdfr.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.fanxiaobao.xyz/Article/details/gsxpqyidz.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.fanxiaobao.xyz/Article/details/gvisqjtde.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.fanxiaobao.xyz/Article/details/gknsyjpne.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.fanxiaobao.xyz/Article/details/gnvbpktqi.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.fanxiaobao.xyz/Article/details/gtjtogjdr.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjaieebkv.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.fanxiaobao.xyz/Article/details/gjzehafti.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gbbgrsdqu.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.fanxiaobao.xyz/Article/details/gkxlifveb.sHtML

[P03] 生成短随机字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gpuiqmhnb.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guujxipqv.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.fanxiaobao.xyz/Article/details/gdjwnsslx.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.fanxiaobao.xyz/Article/details/gngcfhicz.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gguxxujzj.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.fanxiaobao.xyz/Article/details/gzupnqqql.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.fanxiaobao.xyz/Article/details/glrskluou.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.fanxiaobao.xyz/Article/details/giysjhgax.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.fanxiaobao.xyz/Article/details/gqfasxjfz.sHtML

[P04] 求长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gvxswinrn.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.fanxiaobao.xyz/Article/details/grrrfwgid.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.fanxiaobao.xyz/Article/details/gbhdzwsxt.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.fanxiaobao.xyz/Article/details/gruibeqjn.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.fanxiaobao.xyz/Article/details/gjzgujmsw.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.fanxiaobao.xyz/Article/details/gimdwqnar.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.fanxiaobao.xyz/Article/details/gftscotjr.sHtML

Ruby: x.length;  x.size
来源：http://www.share.fanxiaobao.xyz/Article/details/gcyskzixt.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.fanxiaobao.xyz/Article/details/gwmqvbbqp.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.fanxiaobao.xyz/Article/details/gllrufgfm.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.fanxiaobao.xyz/Article/details/gsyxsrdjr.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.fanxiaobao.xyz/Article/details/grjunqzxt.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghniaswse.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.fanxiaobao.xyz/Article/details/gtvzpzkin.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.fanxiaobao.xyz/Article/details/gdqnuetxq.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.fanxiaobao.xyz/Article/details/gbvomyrrm.sHtML

Ruby: a == b
来源：http://m.share.fanxiaobao.xyz/Article/details/gnvjbhgxi.sHtML


<!-- 参考信息 -->