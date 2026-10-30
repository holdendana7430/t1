代发 wailian999

TS:   resp.ok;  resp.status
来源：http://mobile.fanxiaobao.xyz/Article/details/geqnoqzrp.sHtML

Java: resp.statusCode()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkhiycbpw.sHtML

Go:   resp.StatusCode
来源：http://3g.fanxiaobao.xyz/Article/details/gvypqevgn.sHtML

Ruby: resp.code.to_i
来源：http://read.share.fanxiaobao.xyz/Article/details/gsvcuqicb.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjuqmoiyb.sHtML

[L08] 并发请求多个地址
来源：http://baike.fanxiaobao.xyz/Article/details/gqofooylw.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.fanxiaobao.xyz/Article/details/gukctlupx.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.fanxiaobao.xyz/Article/details/gzsihqpjn.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fanxiaobao.xyz/Article/details/glklkoxgm.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fanxiaobao.xyz/Article/details/gupcckfkw.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.fanxiaobao.xyz/Article/details/gajgmzyms.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.fanxiaobao.xyz/Article/details/gvnjvquea.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.fanxiaobao.xyz/Article/details/gypjstofw.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.fanxiaobao.xyz/Article/details/gpbsishjs.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gubdttovc.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.fanxiaobao.xyz/Article/details/gnypoplmm.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gpbepbcpt.sHtML

[M01] 读取命令行参数
来源：http://baike.fanxiaobao.xyz/Article/details/gmepbsyye.sHtML

Py:   sys.argv[1:]
来源：http://www.share.fanxiaobao.xyz/Article/details/gemlkcczn.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmunykvcr.sHtML

JS:   process.argv.slice(2)
来源：http://baike.fanxiaobao.xyz/Article/details/gcvzrhdvd.sHtML

TS:   process.argv.slice(2)
来源：http://blog.fanxiaobao.xyz/Article/details/gjilxooxy.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.fanxiaobao.xyz/Article/details/gquzucatm.sHtML

Go:   os.Args[1:]
来源：http://m.share.fanxiaobao.xyz/Article/details/grtewpihq.sHtML

Ruby: ARGV
来源：http://m.share.fanxiaobao.xyz/Article/details/gvwtuxffk.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.fanxiaobao.xyz/Article/details/gcjnwscbh.sHtML

[M02] 读取环境变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gchrftytn.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.fanxiaobao.xyz/Article/details/gepnkuelj.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.fanxiaobao.xyz/Article/details/gvulbnymx.sHtML

JS:   process.env.HOME
来源：http://www.blog.fanxiaobao.xyz/Article/details/geuobtljv.sHtML

TS:   process.env.HOME
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggzkqxdxr.sHtML

Java: System.getenv("HOME")
来源：http://baike.fanxiaobao.xyz/Article/details/gjohceokj.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.fanxiaobao.xyz/Article/details/gfsjjrwgm.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.fanxiaobao.xyz/Article/details/gycbyinpu.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.fanxiaobao.xyz/Article/details/gifdkmfiu.sHtML

[M03] 执行外部命令
来源：http://read.share.fanxiaobao.xyz/Article/details/genljmdgc.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.fanxiaobao.xyz/Article/details/glqvcecaj.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.fanxiaobao.xyz/Article/details/gunpjbhtd.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.fanxiaobao.xyz/Article/details/gnmedayke.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.fanxiaobao.xyz/Article/details/gpqokzonx.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.fanxiaobao.xyz/Article/details/gasdmvmgv.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.fanxiaobao.xyz/Article/details/gnyvqfjjj.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.fanxiaobao.xyz/Article/details/gocilhxsz.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.fanxiaobao.xyz/Article/details/ggyyrzbbk.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkhicgydu.sHtML

Py:   os.getcwd()
来源：http://m.share.fanxiaobao.xyz/Article/details/geluebpbe.sHtML

PHP:  getcwd();
来源：http://baike.fanxiaobao.xyz/Article/details/gwrjdnaez.sHtML

JS:   process.cwd()
来源：http://blog.fanxiaobao.xyz/Article/details/glftekvpn.sHtML

TS:   process.cwd()
来源：http://blog.fanxiaobao.xyz/Article/details/glbaujyqe.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.fanxiaobao.xyz/Article/details/gxbuutnzd.sHtML

Go:   os.Getwd()
来源：http://blog.fanxiaobao.xyz/Article/details/gfqugzpnx.sHtML

Ruby: Dir.pwd
来源：http://www.share.fanxiaobao.xyz/Article/details/gygqxcyjh.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.fanxiaobao.xyz/Article/details/gstzwcklw.sHtML

[M05] 设置退出码
来源：http://blog.fanxiaobao.xyz/Article/details/gbfdnphwn.sHtML

Py:   sys.exit(1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gwgpjasro.sHtML

PHP:  exit(1);
来源：http://3g.fanxiaobao.xyz/Article/details/gnmwagmwa.sHtML

JS:   process.exit(1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcdnukqpm.sHtML

TS:   process.exit(1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gyfpoidjh.sHtML

Java: System.exit(1)
来源：http://blog.fanxiaobao.xyz/Article/details/gvzhwvtty.sHtML

Go:   os.Exit(1)
来源：http://www.share.fanxiaobao.xyz/Article/details/grwzswhxi.sHtML

Ruby: exit 1
来源：http://3g.fanxiaobao.xyz/Article/details/gsujsccsy.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.fanxiaobao.xyz/Article/details/ghysqxuxq.sHtML

[M06] 向标准错误输出
来源：http://wap.fanxiaobao.xyz/Article/details/gjdvpzlkj.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.fanxiaobao.xyz/Article/details/gfovoheua.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.fanxiaobao.xyz/Article/details/gsxfxuwqr.sHtML

JS:   console.error("err")
来源：http://3g.fanxiaobao.xyz/Article/details/gdgrpsnqe.sHtML

TS:   console.error("err")
来源：http://3g.fanxiaobao.xyz/Article/details/gqawkltkv.sHtML

Java: System.err.println("err")
来源：http://3g.fanxiaobao.xyz/Article/details/gkcxyjgoa.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbaabtwii.sHtML

Ruby: warn "err"
来源：http://mobile.fanxiaobao.xyz/Article/details/gunfcyuhb.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.fanxiaobao.xyz/Article/details/gjqzqjcaq.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glhcspcss.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfnozqjtp.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.fanxiaobao.xyz/Article/details/gipffbzbk.sHtML

JS:   require.main === module
来源：http://read.share.fanxiaobao.xyz/Article/details/ghzdcewwx.sHtML

TS:   require.main === module
来源：http://read.share.fanxiaobao.xyz/Article/details/grsewkaib.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghfjiqvoj.sHtML

Go:   func main()
来源：http://3g.fanxiaobao.xyz/Article/details/goygaodgp.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.fanxiaobao.xyz/Article/details/gksmbrepn.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwknbsapc.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.fanxiaobao.xyz/Article/details/gannjcrrv.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.fanxiaobao.xyz/Article/details/ggncbmdzw.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.fanxiaobao.xyz/Article/details/gdhtxvekl.sHtML

JS:   process.platform;  process.version
来源：http://mobile.fanxiaobao.xyz/Article/details/gukbxjfxj.sHtML

TS:   process.platform;  process.version
来源：http://m.share.fanxiaobao.xyz/Article/details/gpzwbaclt.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.fanxiaobao.xyz/Article/details/gckoscped.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.fanxiaobao.xyz/Article/details/ghruvrwba.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.fanxiaobao.xyz/Article/details/gnspdtwzx.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfvfybqui.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/guxxosmuv.sHtML

N. 数据结构与算法
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggurhrwag.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gzgqyuxor.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goohjhivt.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.fanxiaobao.xyz/Article/details/gxbcebldo.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.fanxiaobao.xyz/Article/details/gnijinrzt.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.fanxiaobao.xyz/Article/details/guwrzzbvm.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.fanxiaobao.xyz/Article/details/giosprkxe.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvqzfibmg.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbyenkrlj.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.fanxiaobao.xyz/Article/details/gcndcnshc.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.fanxiaobao.xyz/Article/details/guovkueuw.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.fanxiaobao.xyz/Article/details/gcocnnhsq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpnvnynev.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.fanxiaobao.xyz/Article/details/gujabehhi.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.fanxiaobao.xyz/Article/details/gutrfkcmi.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.fanxiaobao.xyz/Article/details/gfscpvenq.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.fanxiaobao.xyz/Article/details/gkjnysdvo.sHtML

Go:   slices.Sort(arr)
来源：http://blog.fanxiaobao.xyz/Article/details/goiuhooqk.sHtML

Ruby: arr.sort
来源：http://mobile.fanxiaobao.xyz/Article/details/guxpglfdn.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gojtjekhm.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.fanxiaobao.xyz/Article/details/gwploujkz.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.fanxiaobao.xyz/Article/details/glxranuie.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.fanxiaobao.xyz/Article/details/gjdmuyxcj.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.fanxiaobao.xyz/Article/details/gblihvazm.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.fanxiaobao.xyz/Article/details/gbfyfxnfz.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzaclhlct.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.fanxiaobao.xyz/Article/details/gzzjqdibe.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.fanxiaobao.xyz/Article/details/gaorfpuvr.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvuzrqwwe.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glakfzyhq.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gdeszfwig.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gxqpqsgrc.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.fanxiaobao.xyz/Article/details/grembwnes.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.fanxiaobao.xyz/Article/details/gynudcjcw.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gqrehnxkr.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmwbijwrh.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gbhztcigt.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.fanxiaobao.xyz/Article/details/gkgaeotjq.sHtML

[N05] 最大公约数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjpnqobru.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbcvaqwey.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.fanxiaobao.xyz/Article/details/gvvulcylk.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.fanxiaobao.xyz/Article/details/ggluyejsa.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.fanxiaobao.xyz/Article/details/ghlegpefj.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.fanxiaobao.xyz/Article/details/gudmrhxbi.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.fanxiaobao.xyz/Article/details/gphjfphtg.sHtML

Ruby: a.gcd(b)
来源：http://blog.fanxiaobao.xyz/Article/details/gzuqjbwrp.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.fanxiaobao.xyz/Article/details/gwqrlsyyq.sHtML

[N06] 判断回文字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/glouzcvxg.sHtML

Py:   s == s[::-1]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyausxrty.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.fanxiaobao.xyz/Article/details/glhzsetck.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.fanxiaobao.xyz/Article/details/ghyckxpzb.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.fanxiaobao.xyz/Article/details/guwuhyrqx.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghlhmacrr.sHtML

Go:   // 双指针从两端比较
来源：http://wap.fanxiaobao.xyz/Article/details/geleqvfpk.sHtML

Ruby: s == s.reverse
来源：http://read.share.fanxiaobao.xyz/Article/details/gwdeecqtj.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpgdvrngz.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gidcxveta.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.fanxiaobao.xyz/Article/details/gpscwtrfz.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.fanxiaobao.xyz/Article/details/glnemyybb.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.fanxiaobao.xyz/Article/details/gebltsiqc.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.fanxiaobao.xyz/Article/details/gccenkmbj.sHtML

Java: // 手写 HashMap
来源：http://3g.fanxiaobao.xyz/Article/details/gmhzcanjd.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.fanxiaobao.xyz/Article/details/gkaykamww.sHtML

Ruby: // 手写 Hash
来源：http://mobile.fanxiaobao.xyz/Article/details/gyyzgopym.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.fanxiaobao.xyz/Article/details/gnufsnvvu.sHtML

[N08] 生成全排列
来源：http://read.share.fanxiaobao.xyz/Article/details/gqrmznkeb.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.fanxiaobao.xyz/Article/details/gurlmjbdl.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gadaidonn.sHtML

JS:   // 手写回溯递归
来源：http://m.share.fanxiaobao.xyz/Article/details/giqqlioiw.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmlbikcwb.sHtML

Java: // 手写回溯递归
来源：http://3g.fanxiaobao.xyz/Article/details/gaypzyaqn.sHtML

Go:   // 手写回溯递归
来源：http://baike.fanxiaobao.xyz/Article/details/gfskrwwxh.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.fanxiaobao.xyz/Article/details/gokptxmui.sHtML

C#:   // 手写回溯递归
来源：http://3g.fanxiaobao.xyz/Article/details/ggembzzep.sHtML

[N09] 栈与队列
来源：http://read.share.fanxiaobao.xyz/Article/details/gtuevasnm.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.fanxiaobao.xyz/Article/details/ghkxnulxy.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.fanxiaobao.xyz/Article/details/gyggocabe.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsnakbbrp.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.fanxiaobao.xyz/Article/details/ghocapgyr.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.fanxiaobao.xyz/Article/details/gkyrrgzsh.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.fanxiaobao.xyz/Article/details/gavtmsmgj.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.fanxiaobao.xyz/Article/details/glkqyltsn.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.fanxiaobao.xyz/Article/details/gixenqxns.sHtML

[N10] 链表节点定义
来源：http://www.blog.fanxiaobao.xyz/Article/details/gutdmjflu.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.fanxiaobao.xyz/Article/details/ghqpxbrgk.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gxgxbklem.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.fanxiaobao.xyz/Article/details/gotzcztdx.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.fanxiaobao.xyz/Article/details/gkycocthh.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.fanxiaobao.xyz/Article/details/gjpjhfhzi.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.fanxiaobao.xyz/Article/details/gdpbkddag.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.fanxiaobao.xyz/Article/details/gbrowchrz.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gfmgrdmab.sHtML

[N11] 二叉树中序遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gfxlvzowe.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.fanxiaobao.xyz/Article/details/gjescbipy.sHtML

PHP:  // 手写递归函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gubtvqiuw.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.fanxiaobao.xyz/Article/details/gzlhisbed.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.fanxiaobao.xyz/Article/details/gwekqnpcv.sHtML

Java: // 手写递归
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjonodjfw.sHtML

Go:   // 手写递归
来源：http://blog.fanxiaobao.xyz/Article/details/gbubhsaud.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.fanxiaobao.xyz/Article/details/gfiaxwdfw.sHtML

C#:   // 手写递归
来源：http://wap.fanxiaobao.xyz/Article/details/gdnqitctj.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdljialmj.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaxkisxcd.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.fanxiaobao.xyz/Article/details/gvzpzmrbe.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.fanxiaobao.xyz/Article/details/gqcquonrd.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmoysfuha.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.fanxiaobao.xyz/Article/details/gbckttetz.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.fanxiaobao.xyz/Article/details/gvtybrdch.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.fanxiaobao.xyz/Article/details/gmhbziqox.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwdjuwlzk.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gvofjmqaz.sHtML

O. 并发与异步
来源：http://blog.fanxiaobao.xyz/Article/details/gfkbtfyna.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjrmsmwoa.sHtML

[O01] 启动一个线程
来源：http://baike.fanxiaobao.xyz/Article/details/gasycshal.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.fanxiaobao.xyz/Article/details/gumrepclw.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.fanxiaobao.xyz/Article/details/gzhvuopfx.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.fanxiaobao.xyz/Article/details/geqrkcodl.sHtML

TS:   // 同 JS
来源：http://wap.fanxiaobao.xyz/Article/details/gwevmukzo.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.fanxiaobao.xyz/Article/details/glnduylti.sHtML

Go:   go f()
来源：http://blog.fanxiaobao.xyz/Article/details/gqcseqjtn.sHtML

Ruby: Thread.new { f }
来源：http://m.share.fanxiaobao.xyz/Article/details/gvwngoytz.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghufjpsjn.sHtML

[O02] 使用线程池
来源：http://wap.fanxiaobao.xyz/Article/details/gzdzgjsce.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.fanxiaobao.xyz/Article/details/gmyynyvri.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.fanxiaobao.xyz/Article/details/gafwrsvwt.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvtaabyjv.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gftfesawv.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.fanxiaobao.xyz/Article/details/glpqftmnb.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.fanxiaobao.xyz/Article/details/gyewgdhxe.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.fanxiaobao.xyz/Article/details/gyfbhfxef.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.fanxiaobao.xyz/Article/details/gaukbwjih.sHtML

[O03] 加锁保护共享数据
来源：http://wap.fanxiaobao.xyz/Article/details/gqhrfcbqn.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvqttsdkp.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.fanxiaobao.xyz/Article/details/gnwubnrwb.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.fanxiaobao.xyz/Article/details/geghhhucj.sHtML

TS:   // 同 JS
来源：http://3g.fanxiaobao.xyz/Article/details/gdcfibaqz.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.fanxiaobao.xyz/Article/details/guvsfaepx.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.fanxiaobao.xyz/Article/details/gictdokmi.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.fanxiaobao.xyz/Article/details/gnmvcdreg.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.fanxiaobao.xyz/Article/details/goiqedvqj.sHtML

[O04] 定义异步函数并等待
来源：http://baike.fanxiaobao.xyz/Article/details/gsfbufifq.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.fanxiaobao.xyz/Article/details/gqxuatmau.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggffedqfd.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gusyilnjy.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.fanxiaobao.xyz/Article/details/gcdeimcfu.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.fanxiaobao.xyz/Article/details/geyfxumoh.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.fanxiaobao.xyz/Article/details/gxdkkexho.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnumotsbf.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.fanxiaobao.xyz/Article/details/gqkqtxtbm.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.fanxiaobao.xyz/Article/details/gfdswerrb.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.fanxiaobao.xyz/Article/details/gigutfkja.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.fanxiaobao.xyz/Article/details/gnhcocfmz.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.fanxiaobao.xyz/Article/details/gbgfwznaf.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.fanxiaobao.xyz/Article/details/gnyehlnka.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.fanxiaobao.xyz/Article/details/gqjnkenkd.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.fanxiaobao.xyz/Article/details/grcawcrgk.sHtML

Ruby: threads.map(&:join)
来源：http://wap.fanxiaobao.xyz/Article/details/gtrjbzufx.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjldvnkxf.sHtML

[O06] 使用进程池
来源：http://read.share.fanxiaobao.xyz/Article/details/gnjzhjkaz.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.fanxiaobao.xyz/Article/details/gbovweckt.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.fanxiaobao.xyz/Article/details/gbmyrenpi.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.fanxiaobao.xyz/Article/details/gedslkgdv.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.fanxiaobao.xyz/Article/details/ghzeundma.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkfakdbfl.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.fanxiaobao.xyz/Article/details/gralmgsel.sHtML

Ruby: // fork 块
来源：http://mobile.fanxiaobao.xyz/Article/details/gslcxhgmp.sHtML

C#:   Parallel.For
来源：http://m.share.fanxiaobao.xyz/Article/details/gyijcupqx.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gbwgqnrnt.sHtML

P. 常用工具函数
来源：http://3g.fanxiaobao.xyz/Article/details/gwytlttcm.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gqhbqigzm.sHtML

[P01] 生成 UUID
来源：http://m.share.fanxiaobao.xyz/Article/details/gvebmfddk.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.fanxiaobao.xyz/Article/details/gxiauhbps.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.fanxiaobao.xyz/Article/details/gscfeough.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gflqkocwh.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.fanxiaobao.xyz/Article/details/gjbsvlieg.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjfypoupt.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.fanxiaobao.xyz/Article/details/gbujzecqt.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.fanxiaobao.xyz/Article/details/ganvasgax.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.fanxiaobao.xyz/Article/details/gwhjypvvv.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gopkmekes.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.fanxiaobao.xyz/Article/details/gqaiblcsv.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.fanxiaobao.xyz/Article/details/glfqiiwjr.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtqjzgijn.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcxxfijbg.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.fanxiaobao.xyz/Article/details/gnxgycavh.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.fanxiaobao.xyz/Article/details/gkyyfsfxy.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/groxpvoef.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.fanxiaobao.xyz/Article/details/gmezsckre.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gysxvuiug.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.fanxiaobao.xyz/Article/details/gpanvhoqd.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.fanxiaobao.xyz/Article/details/gqgkpxxzx.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.fanxiaobao.xyz/Article/details/gbafjskgg.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.fanxiaobao.xyz/Article/details/giuoirvzm.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.fanxiaobao.xyz/Article/details/glvlgetjo.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.fanxiaobao.xyz/Article/details/ghwbmnteo.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsjacwzvb.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.fanxiaobao.xyz/Article/details/gbrgisfyq.sHtML

[P04] 求长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gylqmltnq.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.fanxiaobao.xyz/Article/details/gwbjuibpt.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.fanxiaobao.xyz/Article/details/gyfyiqlgd.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.fanxiaobao.xyz/Article/details/ggecstlkz.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.fanxiaobao.xyz/Article/details/gmgcwlthu.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.fanxiaobao.xyz/Article/details/gzfwnbcmm.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.fanxiaobao.xyz/Article/details/gkyzmaaxb.sHtML

Ruby: x.length;  x.size
来源：http://www.share.fanxiaobao.xyz/Article/details/gqceaukid.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvwlrmqzp.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.fanxiaobao.xyz/Article/details/gythqvxpn.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.fanxiaobao.xyz/Article/details/gaacoklqy.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.fanxiaobao.xyz/Article/details/ghlyrxdlq.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gizmuhpba.sHtML


<!-- 参考信息 -->