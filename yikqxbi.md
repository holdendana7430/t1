代发 wailian999

TS:   resp.ok;  resp.status
来源：http://www.blog.hesvh.cn/Article/details/gmmumtrrv.sHtML

Java: resp.statusCode()
来源：http://baike.zdbjq.cn/Article/details/gtnfwbgig.sHtML

Go:   resp.StatusCode
来源：http://mobile.zdbjq.cn/Article/details/gwdkywbie.sHtML

Ruby: resp.code.to_i
来源：http://wap.hesvh.cn/Article/details/ginziyvpg.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.hesvh.cn/Article/details/gnerxmkcm.sHtML

[L08] 并发请求多个地址
来源：http://www.share.fehbvm.com/Article/details/gstfejfob.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.zdbjq.cn/Article/details/ghguydfgc.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.zdbjq.cn/Article/details/gpzdtdwnc.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fehbvm.com/Article/details/gvdgugxkj.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.hesvh.cn/Article/details/gqzochnvy.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.zdbjq.cn/Article/details/geqhzfqcl.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.fehbvm.com/Article/details/gcxabzugz.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.zdbjq.cn/Article/details/ghlppidgz.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.hesvh.cn/Article/details/gxflxeidk.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gmzvqjtnl.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.hesvh.cn/Article/details/gmtwixznf.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gxcsixtno.sHtML

[M01] 读取命令行参数
来源：http://wap.zdbjq.cn/Article/details/gevrovzfe.sHtML

Py:   sys.argv[1:]
来源：http://blog.zdbjq.cn/Article/details/grciyaaea.sHtML

PHP:  $argv;  $argc;
来源：http://baike.fehbvm.com/Article/details/gmerzazlp.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.fehbvm.com/Article/details/gigrnxmjl.sHtML

TS:   process.argv.slice(2)
来源：http://baike.hesvh.cn/Article/details/grceyhcag.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.fehbvm.com/Article/details/gdjfrusnp.sHtML

Go:   os.Args[1:]
来源：http://3g.zdbjq.cn/Article/details/gagxtdevq.sHtML

Ruby: ARGV
来源：http://www.blog.hesvh.cn/Article/details/gnpdokazb.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.zdbjq.cn/Article/details/ghzykkaqo.sHtML

[M02] 读取环境变量
来源：http://www.blog.zdbjq.cn/Article/details/ghrirwtel.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.zdbjq.cn/Article/details/grmthiaxw.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.fehbvm.com/Article/details/gwlgazwgh.sHtML

JS:   process.env.HOME
来源：http://m.share.hesvh.cn/Article/details/gonarciyv.sHtML

TS:   process.env.HOME
来源：http://www.m.share.zdbjq.cn/Article/details/gsvtgvgex.sHtML

Java: System.getenv("HOME")
来源：http://read.share.fehbvm.com/Article/details/gouxbdhwy.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.hesvh.cn/Article/details/grtlsdyha.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.zdbjq.cn/Article/details/gabgsilpg.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.zdbjq.cn/Article/details/gehtxqfbs.sHtML

[M03] 执行外部命令
来源：http://wap.hesvh.cn/Article/details/gnnkycdta.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.zdbjq.cn/Article/details/gpdveoxgf.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.fehbvm.com/Article/details/gdbdmmvob.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.hesvh.cn/Article/details/gncjkzrcg.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.hesvh.cn/Article/details/gohtrqisz.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.zdbjq.cn/Article/details/geqwnqzni.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.fehbvm.com/Article/details/ggfrmlqhy.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.hesvh.cn/Article/details/gjjyoptde.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.hesvh.cn/Article/details/gzwprnspe.sHtML

[M04] 获取当前工作目录
来源：http://3g.hesvh.cn/Article/details/gsqjxqaez.sHtML

Py:   os.getcwd()
来源：http://wap.hesvh.cn/Article/details/gxpzseudj.sHtML

PHP:  getcwd();
来源：http://www.share.zdbjq.cn/Article/details/ghpajihii.sHtML

JS:   process.cwd()
来源：http://www.m.share.zdbjq.cn/Article/details/glkywkgjk.sHtML

TS:   process.cwd()
来源：http://baike.fehbvm.com/Article/details/gvqazujjc.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.zdbjq.cn/Article/details/gezgigxkg.sHtML

Go:   os.Getwd()
来源：http://m.share.fehbvm.com/Article/details/gruydrhyf.sHtML

Ruby: Dir.pwd
来源：http://read.share.fehbvm.com/Article/details/gpgbiwivn.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.zdbjq.cn/Article/details/gmjikxyqa.sHtML

[M05] 设置退出码
来源：http://3g.hesvh.cn/Article/details/gyxfjonbl.sHtML

Py:   sys.exit(1)
来源：http://baike.hesvh.cn/Article/details/gzsizlbgu.sHtML

PHP:  exit(1);
来源：http://blog.hesvh.cn/Article/details/gfpgqpszr.sHtML

JS:   process.exit(1)
来源：http://www.share.hesvh.cn/Article/details/gkmvxhtcc.sHtML

TS:   process.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gmlrxbjki.sHtML

Java: System.exit(1)
来源：http://3g.zdbjq.cn/Article/details/geizsqrqh.sHtML

Go:   os.Exit(1)
来源：http://baike.fehbvm.com/Article/details/gdloyntew.sHtML

Ruby: exit 1
来源：http://www.m.share.fehbvm.com/Article/details/gxibacgos.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.hesvh.cn/Article/details/gzjnkplei.sHtML

[M06] 向标准错误输出
来源：http://blog.zdbjq.cn/Article/details/gyitayjjs.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.zdbjq.cn/Article/details/giumuobuk.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.fehbvm.com/Article/details/gmasndtgp.sHtML

JS:   console.error("err")
来源：http://blog.zdbjq.cn/Article/details/gihmjxfbu.sHtML

TS:   console.error("err")
来源：http://www.blog.zdbjq.cn/Article/details/gzxpvzrcp.sHtML

Java: System.err.println("err")
来源：http://www.blog.fehbvm.com/Article/details/gcdslbhox.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.fehbvm.com/Article/details/ghyqjwxfq.sHtML

Ruby: warn "err"
来源：http://www.share.hesvh.cn/Article/details/gidkhvtlb.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.hesvh.cn/Article/details/gpdfdytas.sHtML

[M07] 判断是否为主入口
来源：http://blog.zdbjq.cn/Article/details/ggyneobdi.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.fehbvm.com/Article/details/gxneymvjm.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.fehbvm.com/Article/details/gantllxdc.sHtML

JS:   require.main === module
来源：http://baike.zdbjq.cn/Article/details/gaphsqbmm.sHtML

TS:   require.main === module
来源：http://baike.hesvh.cn/Article/details/gxyblvggp.sHtML

Java: public static void main(String[] args)
来源：http://3g.zdbjq.cn/Article/details/guwmibfbv.sHtML

Go:   func main()
来源：http://baike.fehbvm.com/Article/details/gficmwmdx.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.fehbvm.com/Article/details/gqaodgjub.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.zdbjq.cn/Article/details/ghtawqpkp.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.fehbvm.com/Article/details/gugdgnktz.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.zdbjq.cn/Article/details/gbfjszueq.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.hesvh.cn/Article/details/gzelhijvu.sHtML

JS:   process.platform;  process.version
来源：http://read.share.hesvh.cn/Article/details/gahbjmrel.sHtML

TS:   process.platform;  process.version
来源：http://baike.fehbvm.com/Article/details/genhcsixf.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.hesvh.cn/Article/details/gtlppgcyr.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.hesvh.cn/Article/details/gqrcndiid.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.fehbvm.com/Article/details/gvfmqbmeo.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.zdbjq.cn/Article/details/gftcvedlw.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gdxyspcek.sHtML

N. 数据结构与算法
来源：http://blog.fehbvm.com/Article/details/gbcslyeik.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gsszzzeqy.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.hesvh.cn/Article/details/gpmvkxksv.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.hesvh.cn/Article/details/gwpsngqzb.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.zdbjq.cn/Article/details/ghqxuokaf.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.zdbjq.cn/Article/details/gnsuhfcjb.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.hesvh.cn/Article/details/grswpjszk.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.hesvh.cn/Article/details/gzzcwfkmt.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/grwnwbgmh.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.hesvh.cn/Article/details/gipusarck.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gzezlbobm.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.fehbvm.com/Article/details/gbqzllzxp.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.fehbvm.com/Article/details/gzzfffngl.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.fehbvm.com/Article/details/gkeypfozs.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.zdbjq.cn/Article/details/govlusblw.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.fehbvm.com/Article/details/gyhutejgx.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.hesvh.cn/Article/details/glukrawfn.sHtML

Go:   slices.Sort(arr)
来源：http://wap.hesvh.cn/Article/details/gtyqpxqxc.sHtML

Ruby: arr.sort
来源：http://blog.fehbvm.com/Article/details/gqqayednd.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.fehbvm.com/Article/details/gnasqeihx.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.zdbjq.cn/Article/details/gvatrtugs.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.hesvh.cn/Article/details/gndgvqwai.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.hesvh.cn/Article/details/goynvxfte.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.fehbvm.com/Article/details/gxfbrrcxj.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.fehbvm.com/Article/details/gohrvgaml.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.zdbjq.cn/Article/details/gpwddintm.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.zdbjq.cn/Article/details/gutqbypar.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.fehbvm.com/Article/details/gkwpbzeth.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.fehbvm.com/Article/details/ggkucsuov.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.zdbjq.cn/Article/details/gskddrxso.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.fehbvm.com/Article/details/glgqxiyjr.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.fehbvm.com/Article/details/golwhhdsi.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/gviwwrlss.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.hesvh.cn/Article/details/gnrvbpisj.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.zdbjq.cn/Article/details/grfactxmw.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.fehbvm.com/Article/details/gmgpzulox.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.fehbvm.com/Article/details/gxdrvixsh.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/gnctgflce.sHtML

[N05] 最大公约数
来源：http://baike.hesvh.cn/Article/details/gzvkmtfzw.sHtML

Py:   math.gcd(a, b)
来源：http://blog.hesvh.cn/Article/details/gwvjyahiw.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.fehbvm.com/Article/details/gzzwmswvn.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.fehbvm.com/Article/details/gdapbpyqv.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.fehbvm.com/Article/details/gfdzfngrw.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.zdbjq.cn/Article/details/gqqunmauu.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.hesvh.cn/Article/details/gfkayzznh.sHtML

Ruby: a.gcd(b)
来源：http://read.share.hesvh.cn/Article/details/goxuqfkqw.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.hesvh.cn/Article/details/gngpoojyy.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.hesvh.cn/Article/details/giazwovpm.sHtML

Py:   s == s[::-1]
来源：http://wap.fehbvm.com/Article/details/goenhaeda.sHtML

PHP:  $s === strrev($s);
来源：http://wap.fehbvm.com/Article/details/gcpfithqc.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/ghyavkmbh.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/gewczwzkd.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.zdbjq.cn/Article/details/glnbiqimf.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.hesvh.cn/Article/details/guhhpuxwv.sHtML

Ruby: s == s.reverse
来源：http://m.share.fehbvm.com/Article/details/gpjmpsftz.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.fehbvm.com/Article/details/gvzdrxsxh.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.hesvh.cn/Article/details/gokgtkdwo.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.zdbjq.cn/Article/details/gyqriquna.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.hesvh.cn/Article/details/guqktaabt.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.fehbvm.com/Article/details/gkqkpqfsc.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.hesvh.cn/Article/details/gvbpcioml.sHtML

Java: // 手写 HashMap
来源：http://www.blog.zdbjq.cn/Article/details/gxmpufwqs.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.hesvh.cn/Article/details/ggmyckbgy.sHtML

Ruby: // 手写 Hash
来源：http://blog.zdbjq.cn/Article/details/girzgrktg.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.zdbjq.cn/Article/details/gxezbvctm.sHtML

[N08] 生成全排列
来源：http://3g.fehbvm.com/Article/details/gfbhegndw.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.hesvh.cn/Article/details/geiqpioyv.sHtML

PHP:  // 手写递归交换
来源：http://www.share.zdbjq.cn/Article/details/gmeipaydl.sHtML

JS:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/ghfpkgdld.sHtML

TS:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gqnforqyl.sHtML

Java: // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/ghsrmpttn.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gbyiscdyr.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.fehbvm.com/Article/details/gusbfsvtk.sHtML

C#:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/ggikxmekx.sHtML

[N09] 栈与队列
来源：http://wap.hesvh.cn/Article/details/gfmeephdr.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.fehbvm.com/Article/details/gdgixvqag.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.fehbvm.com/Article/details/gpuarleek.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.zdbjq.cn/Article/details/gyqgizjug.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.fehbvm.com/Article/details/gktempvuh.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.hesvh.cn/Article/details/gkasvxyty.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.fehbvm.com/Article/details/gtuzdkrcn.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.zdbjq.cn/Article/details/gbuaorkdh.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.hesvh.cn/Article/details/gciyahdbg.sHtML

[N10] 链表节点定义
来源：http://www.share.fehbvm.com/Article/details/gsqsohmuj.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.zdbjq.cn/Article/details/gkxsjectv.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.zdbjq.cn/Article/details/gbqhgwbtw.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.hesvh.cn/Article/details/gysincpmj.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.zdbjq.cn/Article/details/gcmkgokdj.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.fehbvm.com/Article/details/gbpuhbphy.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.fehbvm.com/Article/details/gyxdteiwc.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.zdbjq.cn/Article/details/gdduszpny.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.zdbjq.cn/Article/details/giocuepdq.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.hesvh.cn/Article/details/gthajzfne.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.hesvh.cn/Article/details/grduyiafs.sHtML

PHP:  // 手写递归函数
来源：http://www.share.hesvh.cn/Article/details/gtqjzqnec.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.hesvh.cn/Article/details/gwfherpie.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.hesvh.cn/Article/details/gdsvtghbh.sHtML

Java: // 手写递归
来源：http://www.m.share.zdbjq.cn/Article/details/ghwzjfrnp.sHtML

Go:   // 手写递归
来源：http://3g.fehbvm.com/Article/details/gqsxqfezd.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.fehbvm.com/Article/details/ghzkvrebw.sHtML

C#:   // 手写递归
来源：http://blog.fehbvm.com/Article/details/gcynhdaxw.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.zdbjq.cn/Article/details/ghooggvdm.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.fehbvm.com/Article/details/gfbqaefej.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.hesvh.cn/Article/details/glayngiug.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.hesvh.cn/Article/details/gxkijcgha.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.zdbjq.cn/Article/details/gbtktjljv.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.hesvh.cn/Article/details/gcwwzxiey.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.fehbvm.com/Article/details/gagblhkti.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.zdbjq.cn/Article/details/geoqcqmdk.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.hesvh.cn/Article/details/gjsgjiyna.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gwitziuit.sHtML

O. 并发与异步
来源：http://blog.zdbjq.cn/Article/details/gvcjuhxgh.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gsdpbnvmm.sHtML

[O01] 启动一个线程
来源：http://wap.zdbjq.cn/Article/details/glyepwzgn.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.hesvh.cn/Article/details/gocezcuix.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.fehbvm.com/Article/details/gzpgltubx.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.hesvh.cn/Article/details/gvoexazkd.sHtML

TS:   // 同 JS
来源：http://mobile.zdbjq.cn/Article/details/ghaaomcoq.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.zdbjq.cn/Article/details/gkebhvbzf.sHtML

Go:   go f()
来源：http://www.m.share.hesvh.cn/Article/details/gwupycnqg.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.zdbjq.cn/Article/details/gtoboetaz.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.fehbvm.com/Article/details/gkywmugih.sHtML

[O02] 使用线程池
来源：http://www.blog.zdbjq.cn/Article/details/gftxtcizd.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.zdbjq.cn/Article/details/gpuiafqcq.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.zdbjq.cn/Article/details/gfcsufxbd.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.hesvh.cn/Article/details/gjejtnwuu.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.hesvh.cn/Article/details/gbjxqyvsp.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.zdbjq.cn/Article/details/gbzjnutsi.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.fehbvm.com/Article/details/guqrhnajf.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.fehbvm.com/Article/details/gaijkjpbc.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.zdbjq.cn/Article/details/glxkgskzm.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.zdbjq.cn/Article/details/gtdqwbilx.sHtML

Py:   with lock: shared += 1
来源：http://blog.fehbvm.com/Article/details/gsdqdqzog.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.hesvh.cn/Article/details/gljrgqqrh.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.zdbjq.cn/Article/details/gonzsydwg.sHtML

TS:   // 同 JS
来源：http://3g.hesvh.cn/Article/details/ghjaiqpit.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.fehbvm.com/Article/details/gorrkzqne.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.hesvh.cn/Article/details/gwatfsulw.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.hesvh.cn/Article/details/gxladsbwh.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.hesvh.cn/Article/details/gqnupxxfe.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.hesvh.cn/Article/details/gnyrgtynv.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.hesvh.cn/Article/details/gsonllwrd.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.fehbvm.com/Article/details/gtixqcvco.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.hesvh.cn/Article/details/gxohoegxk.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.hesvh.cn/Article/details/gjffpzeij.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.fehbvm.com/Article/details/gakfnybvw.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.fehbvm.com/Article/details/gbgsslwus.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.fehbvm.com/Article/details/gmfjilyll.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.zdbjq.cn/Article/details/gihplgljb.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.hesvh.cn/Article/details/ggbkjivoa.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.fehbvm.com/Article/details/gaccewrvh.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.hesvh.cn/Article/details/gwgvqpsoq.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.hesvh.cn/Article/details/gfomkeaip.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.fehbvm.com/Article/details/gzvjtgbju.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.zdbjq.cn/Article/details/gaohgpriq.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.fehbvm.com/Article/details/gpnwizucy.sHtML

Ruby: threads.map(&:join)
来源：http://wap.fehbvm.com/Article/details/gjgmnmygk.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.hesvh.cn/Article/details/gtuiqggxb.sHtML

[O06] 使用进程池
来源：http://www.m.share.hesvh.cn/Article/details/gwiplwrxz.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.zdbjq.cn/Article/details/gcuhoxokw.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.hesvh.cn/Article/details/gdduyjtjd.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.zdbjq.cn/Article/details/ghbfjbxuw.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.zdbjq.cn/Article/details/gpcrysnnb.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.hesvh.cn/Article/details/gtbejuqvs.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.fehbvm.com/Article/details/ghcwvyjvu.sHtML

Ruby: // fork 块
来源：http://m.share.zdbjq.cn/Article/details/gzdgexfsk.sHtML

C#:   Parallel.For
来源：http://read.share.fehbvm.com/Article/details/goqmjicuj.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gxqnhryqo.sHtML

P. 常用工具函数
来源：http://www.share.fehbvm.com/Article/details/gonrbblpu.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/grdyfbroe.sHtML

[P01] 生成 UUID
来源：http://www.m.share.hesvh.cn/Article/details/gsyfhenjj.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.hesvh.cn/Article/details/gpsmpwbfz.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.hesvh.cn/Article/details/goexvkagp.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.zdbjq.cn/Article/details/gptswexrd.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.zdbjq.cn/Article/details/gwycrcbes.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.zdbjq.cn/Article/details/giptqnbgz.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.hesvh.cn/Article/details/gccnmgtlb.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.zdbjq.cn/Article/details/glclayosf.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.fehbvm.com/Article/details/gonoptxzb.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.hesvh.cn/Article/details/gvykikdxa.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.zdbjq.cn/Article/details/ggyyclymb.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.fehbvm.com/Article/details/goxiajtue.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.fehbvm.com/Article/details/geefhduob.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.hesvh.cn/Article/details/gylkmiais.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.hesvh.cn/Article/details/grxoqnpoh.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.hesvh.cn/Article/details/gtllgvvxs.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.zdbjq.cn/Article/details/gfpglamyg.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.zdbjq.cn/Article/details/gngwjxqfr.sHtML

[P03] 生成短随机字符串
来源：http://m.share.hesvh.cn/Article/details/glmugnvcm.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.zdbjq.cn/Article/details/gazaenego.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.zdbjq.cn/Article/details/gdvxtcghl.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.hesvh.cn/Article/details/gyravuyab.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.hesvh.cn/Article/details/gvhlrevgw.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.fehbvm.com/Article/details/giciwbuuq.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.fehbvm.com/Article/details/gqvaqhzys.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.zdbjq.cn/Article/details/guhucpfgm.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.hesvh.cn/Article/details/gublzbsws.sHtML

[P04] 求长度
来源：http://www.m.share.fehbvm.com/Article/details/gsubpqiex.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.hesvh.cn/Article/details/ggxpejiwr.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.hesvh.cn/Article/details/gmcznfxpd.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.hesvh.cn/Article/details/gnjjfpxxq.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.fehbvm.com/Article/details/gtcljytql.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.hesvh.cn/Article/details/ghtawidkx.sHtML

Go:   len(arr);  len(m)
来源：http://blog.fehbvm.com/Article/details/gqkyvklfr.sHtML

Ruby: x.length;  x.size
来源：http://m.share.zdbjq.cn/Article/details/glntfvsry.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.fehbvm.com/Article/details/gudfeytot.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.fehbvm.com/Article/details/gdnushtau.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.zdbjq.cn/Article/details/gwelngmmk.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.hesvh.cn/Article/details/gwkbonrbu.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.hesvh.cn/Article/details/gxzuwaoti.sHtML


<!-- 参考信息 -->