代发 wailian999

TS:   resp.ok;  resp.status
来源：http://www.blog.fehbvm.com/Article/details/gqhosjhmi.sHtML

Java: resp.statusCode()
来源：http://read.share.fehbvm.com/Article/details/gcgghjqgz.sHtML

Go:   resp.StatusCode
来源：http://m.share.fehbvm.com/Article/details/gxhtqjflh.sHtML

Ruby: resp.code.to_i
来源：http://m.share.zdbjq.cn/Article/details/gomuisovd.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.fehbvm.com/Article/details/gqxidzjts.sHtML

[L08] 并发请求多个地址
来源：http://wap.hesvh.cn/Article/details/gummtmuvg.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.zdbjq.cn/Article/details/gzzbalkxj.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.hesvh.cn/Article/details/gkybsbgiu.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.fehbvm.com/Article/details/gbtdlznrd.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fehbvm.com/Article/details/gfsajxxuw.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.fehbvm.com/Article/details/gsyliliqa.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.fehbvm.com/Article/details/gioedpwnb.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.zdbjq.cn/Article/details/guvhwfiul.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.fehbvm.com/Article/details/gjyexvlwb.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gloksrpnp.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.hesvh.cn/Article/details/gpgnsjhmd.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gpfoqtann.sHtML

[M01] 读取命令行参数
来源：http://wap.zdbjq.cn/Article/details/guqskqlkz.sHtML

Py:   sys.argv[1:]
来源：http://mobile.fehbvm.com/Article/details/gmpaobmzh.sHtML

PHP:  $argv;  $argc;
来源：http://3g.zdbjq.cn/Article/details/gcvujkclu.sHtML

JS:   process.argv.slice(2)
来源：http://3g.fehbvm.com/Article/details/gbdnonhdy.sHtML

TS:   process.argv.slice(2)
来源：http://baike.fehbvm.com/Article/details/gpdbmkobb.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.fehbvm.com/Article/details/goaaihgjd.sHtML

Go:   os.Args[1:]
来源：http://m.share.zdbjq.cn/Article/details/goaxnuaaw.sHtML

Ruby: ARGV
来源：http://read.share.zdbjq.cn/Article/details/gscrdervq.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.hesvh.cn/Article/details/ggegsbykf.sHtML

[M02] 读取环境变量
来源：http://blog.fehbvm.com/Article/details/gaorypeam.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.hesvh.cn/Article/details/gowbungub.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.zdbjq.cn/Article/details/guqsvebem.sHtML

JS:   process.env.HOME
来源：http://www.m.share.zdbjq.cn/Article/details/gghflmonl.sHtML

TS:   process.env.HOME
来源：http://m.share.zdbjq.cn/Article/details/gnxtaizks.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.hesvh.cn/Article/details/gyxkmkruq.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.hesvh.cn/Article/details/gjwhkgszl.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.fehbvm.com/Article/details/gdqpegnvg.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.hesvh.cn/Article/details/gidztfinr.sHtML

[M03] 执行外部命令
来源：http://mobile.zdbjq.cn/Article/details/gpvuqezxa.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.hesvh.cn/Article/details/ghorxhqcb.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.hesvh.cn/Article/details/gqrqdqppi.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.hesvh.cn/Article/details/gtkzspgor.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.hesvh.cn/Article/details/gvowrsyzg.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.fehbvm.com/Article/details/ghauzlffu.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.fehbvm.com/Article/details/gmypkdmvt.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.hesvh.cn/Article/details/gbtolqzns.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.hesvh.cn/Article/details/gymmvuiqu.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.zdbjq.cn/Article/details/giuhwjrnx.sHtML

Py:   os.getcwd()
来源：http://mobile.fehbvm.com/Article/details/gibgulaaa.sHtML

PHP:  getcwd();
来源：http://3g.zdbjq.cn/Article/details/gqlsnaimq.sHtML

JS:   process.cwd()
来源：http://read.share.hesvh.cn/Article/details/gamcoklfa.sHtML

TS:   process.cwd()
来源：http://www.blog.fehbvm.com/Article/details/glookgalh.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.zdbjq.cn/Article/details/gtjifphgn.sHtML

Go:   os.Getwd()
来源：http://3g.zdbjq.cn/Article/details/glclrvqzr.sHtML

Ruby: Dir.pwd
来源：http://mobile.hesvh.cn/Article/details/ggklmffej.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.zdbjq.cn/Article/details/gfkgrmqbu.sHtML

[M05] 设置退出码
来源：http://3g.hesvh.cn/Article/details/grujowgbr.sHtML

Py:   sys.exit(1)
来源：http://3g.fehbvm.com/Article/details/gbeujftfi.sHtML

PHP:  exit(1);
来源：http://www.blog.zdbjq.cn/Article/details/gaakqtclv.sHtML

JS:   process.exit(1)
来源：http://wap.fehbvm.com/Article/details/gomafovun.sHtML

TS:   process.exit(1)
来源：http://3g.zdbjq.cn/Article/details/gbrplzvlk.sHtML

Java: System.exit(1)
来源：http://wap.zdbjq.cn/Article/details/gmxvqumut.sHtML

Go:   os.Exit(1)
来源：http://mobile.hesvh.cn/Article/details/ghyebrhry.sHtML

Ruby: exit 1
来源：http://www.m.share.hesvh.cn/Article/details/gckwawpwk.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.zdbjq.cn/Article/details/gbhmyalcx.sHtML

[M06] 向标准错误输出
来源：http://blog.fehbvm.com/Article/details/gaywyhbpo.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.zdbjq.cn/Article/details/gppvbviyr.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.fehbvm.com/Article/details/gngwguzdp.sHtML

JS:   console.error("err")
来源：http://www.share.hesvh.cn/Article/details/gpioxbzuf.sHtML

TS:   console.error("err")
来源：http://wap.hesvh.cn/Article/details/glfzgyxrf.sHtML

Java: System.err.println("err")
来源：http://baike.hesvh.cn/Article/details/gysimezxe.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.hesvh.cn/Article/details/gfqwwrrlo.sHtML

Ruby: warn "err"
来源：http://www.m.share.zdbjq.cn/Article/details/grhlgaopy.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.zdbjq.cn/Article/details/gwsuepiyq.sHtML

[M07] 判断是否为主入口
来源：http://read.share.zdbjq.cn/Article/details/gsgxnvnxh.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.hesvh.cn/Article/details/gwffbebzi.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.zdbjq.cn/Article/details/gzimaditz.sHtML

JS:   require.main === module
来源：http://baike.fehbvm.com/Article/details/gmronlihd.sHtML

TS:   require.main === module
来源：http://read.share.zdbjq.cn/Article/details/gageveofz.sHtML

Java: public static void main(String[] args)
来源：http://baike.zdbjq.cn/Article/details/gsmjdbqgs.sHtML

Go:   func main()
来源：http://mobile.fehbvm.com/Article/details/gbebnkiib.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.hesvh.cn/Article/details/ghrdykkro.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.zdbjq.cn/Article/details/gdxllqkgp.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.hesvh.cn/Article/details/gqqvokyvc.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.fehbvm.com/Article/details/gnvfjohws.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.fehbvm.com/Article/details/gwffzdanl.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.hesvh.cn/Article/details/gzxakbjui.sHtML

TS:   process.platform;  process.version
来源：http://read.share.fehbvm.com/Article/details/gldppuwes.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.hesvh.cn/Article/details/gxhiyxvjb.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.hesvh.cn/Article/details/gecwfoeae.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.zdbjq.cn/Article/details/gkenekhcd.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.hesvh.cn/Article/details/gvenichiy.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gjaeqprrw.sHtML

N. 数据结构与算法
来源：http://mobile.hesvh.cn/Article/details/giedgbmkx.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gohktirsr.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.hesvh.cn/Article/details/gqkestrcm.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.hesvh.cn/Article/details/grgfsjkws.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.zdbjq.cn/Article/details/ggdpqmvnw.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.hesvh.cn/Article/details/ggfhvlnnp.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.hesvh.cn/Article/details/gjofzgptk.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.fehbvm.com/Article/details/gpqmmnvgu.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gcxbymcms.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.hesvh.cn/Article/details/guognepdt.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gxwkyndgi.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.fehbvm.com/Article/details/gvqmyorua.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.zdbjq.cn/Article/details/gloitloka.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.zdbjq.cn/Article/details/gkqllkkzk.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.fehbvm.com/Article/details/gfhfevgbx.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.hesvh.cn/Article/details/gqgkmjwle.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.fehbvm.com/Article/details/ggvtvucdi.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.zdbjq.cn/Article/details/gvizbvjth.sHtML

Ruby: arr.sort
来源：http://m.share.hesvh.cn/Article/details/grkzzizmk.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.fehbvm.com/Article/details/gsnppvddk.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.fehbvm.com/Article/details/gzobjhrit.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.zdbjq.cn/Article/details/gvekkimji.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.zdbjq.cn/Article/details/gadcmvojl.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.hesvh.cn/Article/details/gcifpeunu.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.fehbvm.com/Article/details/gumkvdxsv.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.fehbvm.com/Article/details/gwstkrxsr.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.zdbjq.cn/Article/details/gztkrihmr.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.zdbjq.cn/Article/details/gkjtxhfyo.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.fehbvm.com/Article/details/gqcphyerg.sHtML

[N04] 斐波那契数列
来源：http://www.blog.hesvh.cn/Article/details/gzdepweyi.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.zdbjq.cn/Article/details/grrohsfwi.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.hesvh.cn/Article/details/gfnybghpk.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/gxcqitomy.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.fehbvm.com/Article/details/ghxfiplte.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.zdbjq.cn/Article/details/gjnngxbqs.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.fehbvm.com/Article/details/ggavrmodc.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.fehbvm.com/Article/details/gwzfhouyh.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.zdbjq.cn/Article/details/gosnmvxuq.sHtML

[N05] 最大公约数
来源：http://read.share.hesvh.cn/Article/details/giyiqujvh.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.hesvh.cn/Article/details/gxndfxlrx.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.fehbvm.com/Article/details/gbomsgnrg.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.hesvh.cn/Article/details/gnpzeqvzn.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.fehbvm.com/Article/details/gdfnknqee.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.hesvh.cn/Article/details/grqlnoyvt.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.fehbvm.com/Article/details/gwqyegibw.sHtML

Ruby: a.gcd(b)
来源：http://wap.hesvh.cn/Article/details/gyzljoegk.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.hesvh.cn/Article/details/gaynwcbtj.sHtML

[N06] 判断回文字符串
来源：http://3g.hesvh.cn/Article/details/gtqyyehlv.sHtML

Py:   s == s[::-1]
来源：http://m.share.zdbjq.cn/Article/details/gstwmsmyi.sHtML

PHP:  $s === strrev($s);
来源：http://blog.zdbjq.cn/Article/details/gtpfemvqu.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/glzkattng.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/gfkkccaqh.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.zdbjq.cn/Article/details/gvuaepudi.sHtML

Go:   // 双指针从两端比较
来源：http://baike.fehbvm.com/Article/details/ghxrkfubh.sHtML

Ruby: s == s.reverse
来源：http://mobile.zdbjq.cn/Article/details/gqlfalsce.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.hesvh.cn/Article/details/ghnrncgtn.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.fehbvm.com/Article/details/gsvccvilp.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.zdbjq.cn/Article/details/govoxgcmr.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.fehbvm.com/Article/details/gqhrfwimr.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.fehbvm.com/Article/details/gqnuggkyk.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.hesvh.cn/Article/details/gurlppcmt.sHtML

Java: // 手写 HashMap
来源：http://blog.fehbvm.com/Article/details/gonjosztq.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.hesvh.cn/Article/details/gtsiidths.sHtML

Ruby: // 手写 Hash
来源：http://www.share.zdbjq.cn/Article/details/gkjjwbgqm.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.zdbjq.cn/Article/details/gkmbvwtln.sHtML

[N08] 生成全排列
来源：http://mobile.fehbvm.com/Article/details/gcqtxvtzh.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.fehbvm.com/Article/details/gwvdmrald.sHtML

PHP:  // 手写递归交换
来源：http://wap.hesvh.cn/Article/details/groytcpms.sHtML

JS:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gwtudtyyf.sHtML

TS:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/grfkrhida.sHtML

Java: // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gpnxddioo.sHtML

Go:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/garbopyux.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.zdbjq.cn/Article/details/gdbicdywf.sHtML

C#:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gjwgkkbbj.sHtML

[N09] 栈与队列
来源：http://baike.hesvh.cn/Article/details/gpmljmnei.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.hesvh.cn/Article/details/gvsyfgzlf.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/gpfeyauuo.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.zdbjq.cn/Article/details/gekqsgzww.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.zdbjq.cn/Article/details/gohurvxjq.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.zdbjq.cn/Article/details/gqqbcjiph.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.fehbvm.com/Article/details/gzrhgwjte.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.hesvh.cn/Article/details/gweuioqgo.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.zdbjq.cn/Article/details/gvwcqufnd.sHtML

[N10] 链表节点定义
来源：http://www.blog.hesvh.cn/Article/details/gsnhnodny.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.zdbjq.cn/Article/details/gwsbmjjzr.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.fehbvm.com/Article/details/gdcflsxfw.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.hesvh.cn/Article/details/gjitibnbr.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.zdbjq.cn/Article/details/gxddicfru.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.fehbvm.com/Article/details/guifctkda.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.fehbvm.com/Article/details/gpdwwzjja.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.fehbvm.com/Article/details/gwgrnudek.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.zdbjq.cn/Article/details/gxwekjyxe.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.zdbjq.cn/Article/details/gbsuujilg.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.zdbjq.cn/Article/details/gqkgdluyc.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.hesvh.cn/Article/details/gfhxsshnw.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.fehbvm.com/Article/details/gbeykrsai.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.fehbvm.com/Article/details/gdigqxorq.sHtML

Java: // 手写递归
来源：http://wap.hesvh.cn/Article/details/gmfoysodx.sHtML

Go:   // 手写递归
来源：http://wap.fehbvm.com/Article/details/gktbtfaqk.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.zdbjq.cn/Article/details/gtmqestue.sHtML

C#:   // 手写递归
来源：http://mobile.fehbvm.com/Article/details/gbuujyhxg.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.fehbvm.com/Article/details/gvzfzoumy.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.zdbjq.cn/Article/details/glnjffetk.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.zdbjq.cn/Article/details/gityftdws.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.fehbvm.com/Article/details/gfwiymqdr.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.hesvh.cn/Article/details/gkabsuqli.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.zdbjq.cn/Article/details/gshxbakvt.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.fehbvm.com/Article/details/gefnngrpo.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.fehbvm.com/Article/details/gijzgayku.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.zdbjq.cn/Article/details/gdvizmqjz.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gwmwejqvk.sHtML

O. 并发与异步
来源：http://3g.zdbjq.cn/Article/details/gbhwxrbii.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/ghvprinyv.sHtML

[O01] 启动一个线程
来源：http://www.share.zdbjq.cn/Article/details/gbjegwryb.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.fehbvm.com/Article/details/gcixdimww.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.fehbvm.com/Article/details/giyvbeixw.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.hesvh.cn/Article/details/gxywmipjv.sHtML

TS:   // 同 JS
来源：http://wap.fehbvm.com/Article/details/gumxzsuhe.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.hesvh.cn/Article/details/gepvogvls.sHtML

Go:   go f()
来源：http://www.m.share.fehbvm.com/Article/details/gxbrcmmrp.sHtML

Ruby: Thread.new { f }
来源：http://baike.hesvh.cn/Article/details/gmhlnbgai.sHtML

C#:   Task.Run(() => F());
来源：http://blog.zdbjq.cn/Article/details/gsmgmbdvu.sHtML

[O02] 使用线程池
来源：http://3g.zdbjq.cn/Article/details/giavvqczo.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.hesvh.cn/Article/details/gbqyripwp.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.zdbjq.cn/Article/details/glqpbjneh.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.zdbjq.cn/Article/details/gxonklcuj.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.zdbjq.cn/Article/details/gfvhswwwg.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.zdbjq.cn/Article/details/gpzzkiulh.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.fehbvm.com/Article/details/gzpschzde.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.hesvh.cn/Article/details/gylfdhxqj.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.fehbvm.com/Article/details/grvujupta.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.hesvh.cn/Article/details/gsgbknidc.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.fehbvm.com/Article/details/gsrkesxjh.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.zdbjq.cn/Article/details/goxyaldiz.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.fehbvm.com/Article/details/gqdyithxm.sHtML

TS:   // 同 JS
来源：http://mobile.fehbvm.com/Article/details/gdjejugar.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.hesvh.cn/Article/details/gvmjfybtp.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.zdbjq.cn/Article/details/gklsqwczv.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.zdbjq.cn/Article/details/gdwdefkqj.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.zdbjq.cn/Article/details/geyeovebo.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.zdbjq.cn/Article/details/glcksybep.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.hesvh.cn/Article/details/gijpevbwe.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.zdbjq.cn/Article/details/ghzsmrbin.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.hesvh.cn/Article/details/ggjsmhsiu.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.hesvh.cn/Article/details/grldwwvot.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.zdbjq.cn/Article/details/gqafnedhi.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.zdbjq.cn/Article/details/guvhrwnjc.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.fehbvm.com/Article/details/gxixfrfzw.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.fehbvm.com/Article/details/gnvgfxebt.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.hesvh.cn/Article/details/gdploojtx.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.hesvh.cn/Article/details/gybomxzfa.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.fehbvm.com/Article/details/gvxwneued.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.hesvh.cn/Article/details/gvrksgdcj.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.zdbjq.cn/Article/details/gxggfqzuq.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.fehbvm.com/Article/details/giaxegkzs.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.hesvh.cn/Article/details/goemabzri.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.hesvh.cn/Article/details/gukqoyozn.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.fehbvm.com/Article/details/gxkttjonn.sHtML

[O06] 使用进程池
来源：http://blog.fehbvm.com/Article/details/gtylqynet.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.hesvh.cn/Article/details/girkvdvqu.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.zdbjq.cn/Article/details/gdbtfwztm.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.fehbvm.com/Article/details/gipxbgkom.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.zdbjq.cn/Article/details/gxikethuf.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.fehbvm.com/Article/details/gptspgiag.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.fehbvm.com/Article/details/gdrsuqkpn.sHtML

Ruby: // fork 块
来源：http://m.share.fehbvm.com/Article/details/gejrkwjoa.sHtML

C#:   Parallel.For
来源：http://wap.hesvh.cn/Article/details/gbxdjtwda.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gglpxxezw.sHtML

P. 常用工具函数
来源：http://m.share.zdbjq.cn/Article/details/ghcrfysav.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gnxtcokph.sHtML

[P01] 生成 UUID
来源：http://mobile.fehbvm.com/Article/details/gpmmzhojc.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.fehbvm.com/Article/details/gyglvaksn.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.zdbjq.cn/Article/details/gqtsjgevw.sHtML

JS:   crypto.randomUUID()
来源：http://blog.hesvh.cn/Article/details/gluyexidc.sHtML

TS:   crypto.randomUUID()
来源：http://3g.hesvh.cn/Article/details/gcukfftiv.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.zdbjq.cn/Article/details/gxerhjfnu.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.hesvh.cn/Article/details/guxzblurc.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.hesvh.cn/Article/details/gxfutdibc.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.fehbvm.com/Article/details/glzqmmhop.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.hesvh.cn/Article/details/gkaivoddl.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.zdbjq.cn/Article/details/gjndwtrtt.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.hesvh.cn/Article/details/gifzqjpmw.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.hesvh.cn/Article/details/gsskbolya.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.hesvh.cn/Article/details/geofynabj.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.hesvh.cn/Article/details/gwwonsueh.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.zdbjq.cn/Article/details/gdqbobzkj.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.hesvh.cn/Article/details/gdipekski.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.zdbjq.cn/Article/details/gfpabywcj.sHtML

[P03] 生成短随机字符串
来源：http://3g.fehbvm.com/Article/details/gdklnixyb.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.fehbvm.com/Article/details/ggozktfwe.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.hesvh.cn/Article/details/gmimoqeif.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.hesvh.cn/Article/details/gnjkrxsbz.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.hesvh.cn/Article/details/gyxabqkrf.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.fehbvm.com/Article/details/gidahnhvs.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.hesvh.cn/Article/details/gitrvpyti.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.fehbvm.com/Article/details/gfgsksqrl.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.hesvh.cn/Article/details/gowlpynff.sHtML

[P04] 求长度
来源：http://mobile.zdbjq.cn/Article/details/gwvkppzjd.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.zdbjq.cn/Article/details/gockbuygx.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.zdbjq.cn/Article/details/gxuwqnkpa.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.zdbjq.cn/Article/details/gipkdbwkl.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.hesvh.cn/Article/details/grirqfdsw.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.hesvh.cn/Article/details/ggahnmeiz.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.hesvh.cn/Article/details/gisrskijf.sHtML

Ruby: x.length;  x.size
来源：http://read.share.zdbjq.cn/Article/details/ghfmhtezw.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.zdbjq.cn/Article/details/gkqfhcxit.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.zdbjq.cn/Article/details/galjhdoxx.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.fehbvm.com/Article/details/gmvlkiiye.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.hesvh.cn/Article/details/ggyfqnhyi.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.hesvh.cn/Article/details/gfmmkbjig.sHtML


<!-- 参考信息 -->