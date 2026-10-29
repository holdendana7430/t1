代发 wailian999

TS:   resp.ok;  resp.status
来源：http://www.share.fehbvm.com/Article/details/gowjvudlw.sHtML

Java: resp.statusCode()
来源：http://read.share.zdbjq.cn/Article/details/gusqrusvx.sHtML

Go:   resp.StatusCode
来源：http://mobile.zdbjq.cn/Article/details/gdjayoybp.sHtML

Ruby: resp.code.to_i
来源：http://www.share.hesvh.cn/Article/details/gklliaufj.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.hesvh.cn/Article/details/gzydirmtx.sHtML

[L08] 并发请求多个地址
来源：http://read.share.zdbjq.cn/Article/details/geuawwwtn.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.zdbjq.cn/Article/details/gknakclsd.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.hesvh.cn/Article/details/gisgzuyqc.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fehbvm.com/Article/details/gviotebee.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fehbvm.com/Article/details/gwinzacog.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.hesvh.cn/Article/details/gauyoiloy.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.fehbvm.com/Article/details/gqyobxwgh.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.fehbvm.com/Article/details/gdnyjnnyw.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.fehbvm.com/Article/details/gbjrciilm.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gxejyfcsj.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.fehbvm.com/Article/details/gynekewns.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gtlqtwzyx.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.hesvh.cn/Article/details/gzzctgkor.sHtML

Py:   sys.argv[1:]
来源：http://baike.fehbvm.com/Article/details/gbjdpusuc.sHtML

PHP:  $argv;  $argc;
来源：http://wap.fehbvm.com/Article/details/ggiohkkkj.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.hesvh.cn/Article/details/gapebeido.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.fehbvm.com/Article/details/gdjjjbcsg.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.hesvh.cn/Article/details/gxkvjdexm.sHtML

Go:   os.Args[1:]
来源：http://blog.hesvh.cn/Article/details/ggbbtfvdk.sHtML

Ruby: ARGV
来源：http://www.share.zdbjq.cn/Article/details/gumnogcsb.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.hesvh.cn/Article/details/gtvjkasql.sHtML

[M02] 读取环境变量
来源：http://blog.zdbjq.cn/Article/details/gjcnhsdix.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.zdbjq.cn/Article/details/gnidmkjzs.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.hesvh.cn/Article/details/gwrutthjg.sHtML

JS:   process.env.HOME
来源：http://mobile.zdbjq.cn/Article/details/gnyojnjqh.sHtML

TS:   process.env.HOME
来源：http://www.m.share.hesvh.cn/Article/details/geihmkstd.sHtML

Java: System.getenv("HOME")
来源：http://wap.hesvh.cn/Article/details/gauztkjex.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.hesvh.cn/Article/details/gkssivzzy.sHtML

Ruby: ENV["HOME"]
来源：http://3g.hesvh.cn/Article/details/gzmtlbfyc.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.fehbvm.com/Article/details/gfjbevedq.sHtML

[M03] 执行外部命令
来源：http://blog.zdbjq.cn/Article/details/gnyfdacbk.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.fehbvm.com/Article/details/gnhbsbhxy.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.zdbjq.cn/Article/details/gcmacvtye.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.hesvh.cn/Article/details/gdrylujal.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.fehbvm.com/Article/details/gfgbssglo.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.fehbvm.com/Article/details/gxrrglphi.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.fehbvm.com/Article/details/gmiiojony.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.zdbjq.cn/Article/details/gvpwzkhsc.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.hesvh.cn/Article/details/gskkwryvx.sHtML

[M04] 获取当前工作目录
来源：http://3g.fehbvm.com/Article/details/gxlzfpdjc.sHtML

Py:   os.getcwd()
来源：http://wap.hesvh.cn/Article/details/guumkldpg.sHtML

PHP:  getcwd();
来源：http://www.share.hesvh.cn/Article/details/gdqiaphjj.sHtML

JS:   process.cwd()
来源：http://wap.hesvh.cn/Article/details/gbjngswvk.sHtML

TS:   process.cwd()
来源：http://read.share.zdbjq.cn/Article/details/gfxjxlywy.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.zdbjq.cn/Article/details/gybecwexf.sHtML

Go:   os.Getwd()
来源：http://www.m.share.fehbvm.com/Article/details/gfgcuyfcb.sHtML

Ruby: Dir.pwd
来源：http://mobile.hesvh.cn/Article/details/gpjazbzbl.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.zdbjq.cn/Article/details/gavdhtsct.sHtML

[M05] 设置退出码
来源：http://wap.zdbjq.cn/Article/details/gxywvejio.sHtML

Py:   sys.exit(1)
来源：http://3g.zdbjq.cn/Article/details/gkxsmitmz.sHtML

PHP:  exit(1);
来源：http://m.share.hesvh.cn/Article/details/gajhtihmn.sHtML

JS:   process.exit(1)
来源：http://read.share.fehbvm.com/Article/details/gbavxcttq.sHtML

TS:   process.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gtcdkytjs.sHtML

Java: System.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gmuwonalq.sHtML

Go:   os.Exit(1)
来源：http://baike.hesvh.cn/Article/details/gloxwjwgv.sHtML

Ruby: exit 1
来源：http://read.share.hesvh.cn/Article/details/gdfqwmlqe.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.zdbjq.cn/Article/details/gxowhifvb.sHtML

[M06] 向标准错误输出
来源：http://3g.fehbvm.com/Article/details/gkrcbzlxb.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.zdbjq.cn/Article/details/goffxhmar.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.zdbjq.cn/Article/details/gncxpvlvc.sHtML

JS:   console.error("err")
来源：http://3g.fehbvm.com/Article/details/gifnycclj.sHtML

TS:   console.error("err")
来源：http://www.share.zdbjq.cn/Article/details/gapuuetcg.sHtML

Java: System.err.println("err")
来源：http://baike.hesvh.cn/Article/details/gmnhqwpah.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.zdbjq.cn/Article/details/gxixwbzaf.sHtML

Ruby: warn "err"
来源：http://m.share.zdbjq.cn/Article/details/gxydogfze.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.zdbjq.cn/Article/details/gzvhzlcmc.sHtML

[M07] 判断是否为主入口
来源：http://blog.fehbvm.com/Article/details/gbgafihgd.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.fehbvm.com/Article/details/grpwaxsgz.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.hesvh.cn/Article/details/gbnieiybz.sHtML

JS:   require.main === module
来源：http://www.blog.hesvh.cn/Article/details/gyzblnhaz.sHtML

TS:   require.main === module
来源：http://wap.fehbvm.com/Article/details/gicgzkfpd.sHtML

Java: public static void main(String[] args)
来源：http://baike.hesvh.cn/Article/details/guuqbfptm.sHtML

Go:   func main()
来源：http://mobile.fehbvm.com/Article/details/gzqtcussu.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.zdbjq.cn/Article/details/gunrfhrng.sHtML

C#:   static void Main(string[] args)
来源：http://wap.zdbjq.cn/Article/details/goanyxeqd.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.fehbvm.com/Article/details/giqckotan.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.fehbvm.com/Article/details/gzzbpmana.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.hesvh.cn/Article/details/gxwsivbja.sHtML

JS:   process.platform;  process.version
来源：http://mobile.zdbjq.cn/Article/details/gttbscnfr.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.hesvh.cn/Article/details/gnlhoggim.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.hesvh.cn/Article/details/gsrjxixqq.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.hesvh.cn/Article/details/gqegwkmjm.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.hesvh.cn/Article/details/gfcwqgncy.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.fehbvm.com/Article/details/grqprssvr.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gfpuymhan.sHtML

N. 数据结构与算法
来源：http://m.share.zdbjq.cn/Article/details/gwjfxoelx.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gstxssjhf.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.zdbjq.cn/Article/details/gqaluwgoa.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/grzlboele.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.hesvh.cn/Article/details/ggjhkmejl.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.hesvh.cn/Article/details/gvxnpdfan.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.zdbjq.cn/Article/details/gtqcmpvva.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.fehbvm.com/Article/details/gzljvbokn.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.fehbvm.com/Article/details/ggccrqfwi.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.fehbvm.com/Article/details/gleoqerkd.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gajouwdkh.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.fehbvm.com/Article/details/gqzzuszct.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.fehbvm.com/Article/details/ghufijyha.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.hesvh.cn/Article/details/gnuoeceld.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.zdbjq.cn/Article/details/grjpgfegq.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.fehbvm.com/Article/details/gtdhcsith.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.fehbvm.com/Article/details/gezdugrge.sHtML

Go:   slices.Sort(arr)
来源：http://baike.fehbvm.com/Article/details/gejgootar.sHtML

Ruby: arr.sort
来源：http://read.share.zdbjq.cn/Article/details/gukixwnbi.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.zdbjq.cn/Article/details/getjscbgb.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.zdbjq.cn/Article/details/gwxfptpoy.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.fehbvm.com/Article/details/gkvzywmxy.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.fehbvm.com/Article/details/gqlozdojs.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.hesvh.cn/Article/details/gwbirjgil.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.hesvh.cn/Article/details/gbnteogtk.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.fehbvm.com/Article/details/gcitamtpv.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.hesvh.cn/Article/details/gsoufyido.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.zdbjq.cn/Article/details/ggnkfmeng.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.fehbvm.com/Article/details/gkcmsmqvf.sHtML

[N04] 斐波那契数列
来源：http://blog.fehbvm.com/Article/details/gzbcmrlcv.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.zdbjq.cn/Article/details/giizmvcor.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.fehbvm.com/Article/details/gczaeepoh.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.zdbjq.cn/Article/details/gbqggnsqu.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/gkjbsumur.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.fehbvm.com/Article/details/gefydarsc.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.zdbjq.cn/Article/details/gzsdrjnuj.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.hesvh.cn/Article/details/gcirpzzuo.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/glddkggpr.sHtML

[N05] 最大公约数
来源：http://baike.fehbvm.com/Article/details/gsorkmnml.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.zdbjq.cn/Article/details/gnlcmmsuk.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.fehbvm.com/Article/details/gntmzvues.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.fehbvm.com/Article/details/gjaebrbwu.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.zdbjq.cn/Article/details/gukvafhmm.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.zdbjq.cn/Article/details/gnyqywbef.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.hesvh.cn/Article/details/gvagyvops.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.hesvh.cn/Article/details/gvmizahxc.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.zdbjq.cn/Article/details/gpsutwxlp.sHtML

[N06] 判断回文字符串
来源：http://baike.fehbvm.com/Article/details/gkvnjzzck.sHtML

Py:   s == s[::-1]
来源：http://www.share.hesvh.cn/Article/details/gejxbuzdz.sHtML

PHP:  $s === strrev($s);
来源：http://wap.fehbvm.com/Article/details/gfrijbmtm.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/gmmokxqkb.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/gmmyhjnon.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.fehbvm.com/Article/details/gmcxiofpn.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.zdbjq.cn/Article/details/gsjmwaohy.sHtML

Ruby: s == s.reverse
来源：http://www.share.zdbjq.cn/Article/details/grdsxquba.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.hesvh.cn/Article/details/gccccuciv.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.hesvh.cn/Article/details/gvqdfofva.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.zdbjq.cn/Article/details/gkwdlyklh.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.fehbvm.com/Article/details/gerjoroga.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.zdbjq.cn/Article/details/gejnustvo.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.zdbjq.cn/Article/details/gkqdtiejo.sHtML

Java: // 手写 HashMap
来源：http://www.blog.fehbvm.com/Article/details/gqiijgzic.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.fehbvm.com/Article/details/gaznhoder.sHtML

Ruby: // 手写 Hash
来源：http://3g.zdbjq.cn/Article/details/giqxxflks.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.zdbjq.cn/Article/details/gupgewlub.sHtML

[N08] 生成全排列
来源：http://blog.zdbjq.cn/Article/details/gbxpwdssr.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.fehbvm.com/Article/details/gyzpnokfx.sHtML

PHP:  // 手写递归交换
来源：http://wap.fehbvm.com/Article/details/gvnbcknpn.sHtML

JS:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gsblmrvsk.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gpzukitmk.sHtML

Java: // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gapsraokd.sHtML

Go:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gbqlivuem.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.fehbvm.com/Article/details/ggqaufqgp.sHtML

C#:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gdpkqxclx.sHtML

[N09] 栈与队列
来源：http://3g.fehbvm.com/Article/details/gcxzbpdxw.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.zdbjq.cn/Article/details/gmccljmtq.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.fehbvm.com/Article/details/gyfvwkoez.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/gstlsmqov.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.hesvh.cn/Article/details/gnfrojqnp.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.fehbvm.com/Article/details/gpluxuryn.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.hesvh.cn/Article/details/gswbvqygy.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.hesvh.cn/Article/details/ghchyjqeo.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.zdbjq.cn/Article/details/grfamdfpt.sHtML

[N10] 链表节点定义
来源：http://www.m.share.hesvh.cn/Article/details/guodcynsa.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.zdbjq.cn/Article/details/grzvlvobs.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.zdbjq.cn/Article/details/gbzqhizdq.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.zdbjq.cn/Article/details/gbdzqxfkt.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.hesvh.cn/Article/details/galekfifx.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.fehbvm.com/Article/details/grmocqimq.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.zdbjq.cn/Article/details/gbxmirotd.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.hesvh.cn/Article/details/gerzbxiop.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.fehbvm.com/Article/details/gnrenkehq.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.hesvh.cn/Article/details/gcordvmrg.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.hesvh.cn/Article/details/gcpxiqcmb.sHtML

PHP:  // 手写递归函数
来源：http://read.share.hesvh.cn/Article/details/ghotmmcpf.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.hesvh.cn/Article/details/gibflfstl.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.fehbvm.com/Article/details/gkwzupuib.sHtML

Java: // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/gjyddlubp.sHtML

Go:   // 手写递归
来源：http://wap.fehbvm.com/Article/details/gcqaepjgh.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.zdbjq.cn/Article/details/grzkzxjhg.sHtML

C#:   // 手写递归
来源：http://read.share.fehbvm.com/Article/details/gysbqmjcz.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.fehbvm.com/Article/details/gcguccghf.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.fehbvm.com/Article/details/gyaslbwfo.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.zdbjq.cn/Article/details/gxnlokvjm.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.zdbjq.cn/Article/details/ghslxsztv.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.fehbvm.com/Article/details/gtezgahee.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.fehbvm.com/Article/details/ghsyqrejb.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.zdbjq.cn/Article/details/gvyxswgbw.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.zdbjq.cn/Article/details/gbtvqywdy.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.fehbvm.com/Article/details/ggryaohks.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/glntgcwvo.sHtML

O. 并发与异步
来源：http://www.blog.zdbjq.cn/Article/details/ggdmjiggi.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gqpqgxfyn.sHtML

[O01] 启动一个线程
来源：http://www.m.share.fehbvm.com/Article/details/gknlhmszo.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.hesvh.cn/Article/details/gqgfllnhx.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.hesvh.cn/Article/details/gjpcryfax.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.hesvh.cn/Article/details/gzybxgerg.sHtML

TS:   // 同 JS
来源：http://mobile.fehbvm.com/Article/details/gahniigud.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.fehbvm.com/Article/details/gkfxiteoj.sHtML

Go:   go f()
来源：http://www.m.share.hesvh.cn/Article/details/gjbnmpuir.sHtML

Ruby: Thread.new { f }
来源：http://wap.fehbvm.com/Article/details/guwhxuibh.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.hesvh.cn/Article/details/gfvfpfluy.sHtML

[O02] 使用线程池
来源：http://www.m.share.hesvh.cn/Article/details/gummazxvt.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.zdbjq.cn/Article/details/gnphehgqz.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.hesvh.cn/Article/details/gttxamrgg.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.hesvh.cn/Article/details/greftwdpl.sHtML

TS:   // worker_threads 线程池
来源：http://3g.hesvh.cn/Article/details/glnndgpdn.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.fehbvm.com/Article/details/guouyubur.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.hesvh.cn/Article/details/gbaptlosp.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.hesvh.cn/Article/details/gfgfcjcyd.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.zdbjq.cn/Article/details/gdxrmptdh.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.zdbjq.cn/Article/details/gwyxiyhvq.sHtML

Py:   with lock: shared += 1
来源：http://wap.zdbjq.cn/Article/details/gcwhxktef.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.zdbjq.cn/Article/details/gjvqfdqpw.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.hesvh.cn/Article/details/gxjkcstju.sHtML

TS:   // 同 JS
来源：http://3g.hesvh.cn/Article/details/gyfmrwexy.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.hesvh.cn/Article/details/gljwakhwe.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.zdbjq.cn/Article/details/gamybcyqf.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.fehbvm.com/Article/details/gjjmsejhs.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.hesvh.cn/Article/details/gojphcsni.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.fehbvm.com/Article/details/gfylkyzto.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.fehbvm.com/Article/details/gqkdtkfqg.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.hesvh.cn/Article/details/gjbjzntnz.sHtML

JS:   async function f() { await g(); }
来源：http://wap.zdbjq.cn/Article/details/gmjulcagc.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.hesvh.cn/Article/details/gcadnmfbm.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.fehbvm.com/Article/details/ghjrrkfdr.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.fehbvm.com/Article/details/gahjihhnw.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.hesvh.cn/Article/details/gfbumpjmb.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.hesvh.cn/Article/details/gvsufcahj.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.zdbjq.cn/Article/details/gjhclpqsu.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.hesvh.cn/Article/details/gqgnsbbdx.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.hesvh.cn/Article/details/gytogoxlr.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.hesvh.cn/Article/details/guziwctve.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.fehbvm.com/Article/details/gxnzxcwuu.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.hesvh.cn/Article/details/gxulgxqgm.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.fehbvm.com/Article/details/ghybdsenw.sHtML

Ruby: threads.map(&:join)
来源：http://wap.hesvh.cn/Article/details/goerspxgy.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.fehbvm.com/Article/details/ghqkuhibs.sHtML

[O06] 使用进程池
来源：http://read.share.fehbvm.com/Article/details/gbjpgckuw.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.zdbjq.cn/Article/details/glgfjwpfw.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.zdbjq.cn/Article/details/gdrbsbluz.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.zdbjq.cn/Article/details/gzzgtydub.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.hesvh.cn/Article/details/ghgvovhxx.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.zdbjq.cn/Article/details/gbbnjxbnv.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.hesvh.cn/Article/details/gbrrxadhz.sHtML

Ruby: // fork 块
来源：http://wap.hesvh.cn/Article/details/gjxhqnloc.sHtML

C#:   Parallel.For
来源：http://wap.hesvh.cn/Article/details/gpevfvegi.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gtgvdhnjl.sHtML

P. 常用工具函数
来源：http://mobile.fehbvm.com/Article/details/gvjibqbup.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gfvxygtgn.sHtML

[P01] 生成 UUID
来源：http://blog.fehbvm.com/Article/details/gdlfjpdrq.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.hesvh.cn/Article/details/gmrnhmrgc.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.hesvh.cn/Article/details/gpcmukxqc.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.hesvh.cn/Article/details/gonqlugud.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.zdbjq.cn/Article/details/gfaeylzca.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.fehbvm.com/Article/details/geprxhfmg.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.hesvh.cn/Article/details/gcihkbdgg.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.hesvh.cn/Article/details/gorvhrejt.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.fehbvm.com/Article/details/gpdmyaflj.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.zdbjq.cn/Article/details/gdtiuweim.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.hesvh.cn/Article/details/gkjasmmnj.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.fehbvm.com/Article/details/gkeqwpidk.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.fehbvm.com/Article/details/gohynaggn.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.zdbjq.cn/Article/details/gfsdxejrn.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.zdbjq.cn/Article/details/gfqtdsolp.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.zdbjq.cn/Article/details/gmuoznkqc.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.zdbjq.cn/Article/details/ggvcqodnk.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.hesvh.cn/Article/details/gbcejxklu.sHtML

[P03] 生成短随机字符串
来源：http://3g.hesvh.cn/Article/details/giklfknvj.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.hesvh.cn/Article/details/gzozclqaa.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.fehbvm.com/Article/details/guttwalxa.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.zdbjq.cn/Article/details/gmeilfgrf.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.fehbvm.com/Article/details/giioozxdv.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.hesvh.cn/Article/details/grdlrpoid.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.hesvh.cn/Article/details/gizjmjmeu.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.fehbvm.com/Article/details/gbtjjfttu.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.hesvh.cn/Article/details/gzvnenwoi.sHtML

[P04] 求长度
来源：http://mobile.hesvh.cn/Article/details/gkhxxmzln.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.fehbvm.com/Article/details/gatbcitnj.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/gjnjrjqdb.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.hesvh.cn/Article/details/ghhxcahbz.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.zdbjq.cn/Article/details/gsswmvmzd.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.zdbjq.cn/Article/details/gxgwxkksn.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.hesvh.cn/Article/details/gynyplzbc.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.fehbvm.com/Article/details/grkeysiyd.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.zdbjq.cn/Article/details/gujykmvcp.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.zdbjq.cn/Article/details/grmzapfin.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.zdbjq.cn/Article/details/getfxxlrn.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.zdbjq.cn/Article/details/gpzgoxxff.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.fehbvm.com/Article/details/gwkzgvays.sHtML


<!-- 参考信息 -->