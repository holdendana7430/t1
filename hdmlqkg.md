代发 wailian999

[L07] 处理 HTTP 状态码
来源：http://read.share.hesvh.cn/Article/details/ghkcktxee.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.fehbvm.com/Article/details/gxzntogrz.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.fehbvm.com/Article/details/gpashpzjo.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.hesvh.cn/Article/details/goqgqlhee.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.hesvh.cn/Article/details/ggccpobhz.sHtML

Java: resp.statusCode()
来源：http://wap.fehbvm.com/Article/details/gbabhbdhe.sHtML

Go:   resp.StatusCode
来源：http://3g.hesvh.cn/Article/details/ghsxzdqpc.sHtML

Ruby: resp.code.to_i
来源：http://3g.zdbjq.cn/Article/details/gdazcsrye.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.fehbvm.com/Article/details/gofxqaykc.sHtML

[L08] 并发请求多个地址
来源：http://blog.zdbjq.cn/Article/details/gdnxlkcwe.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.zdbjq.cn/Article/details/goxrtcipx.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.fehbvm.com/Article/details/gyxwjyytl.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fehbvm.com/Article/details/gomeevelk.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.hesvh.cn/Article/details/goiwejipl.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.zdbjq.cn/Article/details/gcckskgrm.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.zdbjq.cn/Article/details/gkhcomvqx.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.fehbvm.com/Article/details/gsgsyoprl.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.zdbjq.cn/Article/details/gdvcqezzd.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/guwxxtiny.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.hesvh.cn/Article/details/gifypjsls.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/ggrpcikqn.sHtML

[M01] 读取命令行参数
来源：http://www.blog.hesvh.cn/Article/details/gmltusmxq.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.hesvh.cn/Article/details/gxuoqbcdy.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.hesvh.cn/Article/details/grmmcyfbh.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.zdbjq.cn/Article/details/gchzywpgn.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.zdbjq.cn/Article/details/gplfjxmfb.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.fehbvm.com/Article/details/gnojunjsv.sHtML

Go:   os.Args[1:]
来源：http://wap.hesvh.cn/Article/details/gkubteder.sHtML

Ruby: ARGV
来源：http://m.share.fehbvm.com/Article/details/ggcimkncc.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.fehbvm.com/Article/details/gixssqjsy.sHtML

[M02] 读取环境变量
来源：http://mobile.fehbvm.com/Article/details/gbuxqetfg.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/gdmqsatle.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.fehbvm.com/Article/details/gwudzbqjy.sHtML

JS:   process.env.HOME
来源：http://blog.zdbjq.cn/Article/details/ghrnrkzfc.sHtML

TS:   process.env.HOME
来源：http://www.share.fehbvm.com/Article/details/gtlnxctkz.sHtML

Java: System.getenv("HOME")
来源：http://blog.fehbvm.com/Article/details/gencuplwp.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.hesvh.cn/Article/details/glwpsjifm.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.zdbjq.cn/Article/details/gvvfhzhvu.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.fehbvm.com/Article/details/gniofoqyd.sHtML

[M03] 执行外部命令
来源：http://mobile.hesvh.cn/Article/details/gilrivmnq.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.fehbvm.com/Article/details/glmmfwkyn.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.hesvh.cn/Article/details/gvzhhwnkk.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.fehbvm.com/Article/details/gqhpmhikd.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.fehbvm.com/Article/details/gacdnaqxq.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.zdbjq.cn/Article/details/glyayndah.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.zdbjq.cn/Article/details/gdhuqphuw.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.fehbvm.com/Article/details/gtqvrngll.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.fehbvm.com/Article/details/gxqrmmyhg.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.fehbvm.com/Article/details/gbmsdylwx.sHtML

Py:   os.getcwd()
来源：http://3g.zdbjq.cn/Article/details/gffegotsz.sHtML

PHP:  getcwd();
来源：http://www.m.share.fehbvm.com/Article/details/gbmflnldd.sHtML

JS:   process.cwd()
来源：http://3g.hesvh.cn/Article/details/gwnyhtwah.sHtML

TS:   process.cwd()
来源：http://baike.zdbjq.cn/Article/details/gdskndgtv.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.zdbjq.cn/Article/details/gutqpirob.sHtML

Go:   os.Getwd()
来源：http://blog.zdbjq.cn/Article/details/grwkxzeru.sHtML

Ruby: Dir.pwd
来源：http://mobile.hesvh.cn/Article/details/gkgibgraj.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.zdbjq.cn/Article/details/gbkonikqv.sHtML

[M05] 设置退出码
来源：http://www.blog.fehbvm.com/Article/details/gncxdewqg.sHtML

Py:   sys.exit(1)
来源：http://baike.fehbvm.com/Article/details/gozgqbviq.sHtML

PHP:  exit(1);
来源：http://mobile.zdbjq.cn/Article/details/gtenvajat.sHtML

JS:   process.exit(1)
来源：http://blog.fehbvm.com/Article/details/gerbrmkbr.sHtML

TS:   process.exit(1)
来源：http://wap.hesvh.cn/Article/details/gcrstvptp.sHtML

Java: System.exit(1)
来源：http://m.share.fehbvm.com/Article/details/garhwjlsn.sHtML

Go:   os.Exit(1)
来源：http://3g.zdbjq.cn/Article/details/gfzlahowt.sHtML

Ruby: exit 1
来源：http://wap.zdbjq.cn/Article/details/gwlsofwmj.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.zdbjq.cn/Article/details/gbxohdbfc.sHtML

[M06] 向标准错误输出
来源：http://read.share.zdbjq.cn/Article/details/gccxgcraz.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.zdbjq.cn/Article/details/gyusjqzwu.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.hesvh.cn/Article/details/goqwureav.sHtML

JS:   console.error("err")
来源：http://www.m.share.zdbjq.cn/Article/details/gcrjzfgkz.sHtML

TS:   console.error("err")
来源：http://wap.zdbjq.cn/Article/details/gtzodynhi.sHtML

Java: System.err.println("err")
来源：http://blog.hesvh.cn/Article/details/geqhredqz.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.fehbvm.com/Article/details/gbwqrhrhj.sHtML

Ruby: warn "err"
来源：http://www.blog.fehbvm.com/Article/details/gsnvexxyd.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.fehbvm.com/Article/details/gwhgrvyvc.sHtML

[M07] 判断是否为主入口
来源：http://blog.zdbjq.cn/Article/details/ggdoybjde.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.zdbjq.cn/Article/details/gyyaipnij.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.hesvh.cn/Article/details/gcmeihodf.sHtML

JS:   require.main === module
来源：http://baike.fehbvm.com/Article/details/grjaidzpq.sHtML

TS:   require.main === module
来源：http://m.share.zdbjq.cn/Article/details/gndufsooi.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.fehbvm.com/Article/details/gnghkimyf.sHtML

Go:   func main()
来源：http://3g.fehbvm.com/Article/details/grmusgndk.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.zdbjq.cn/Article/details/gguvgvdea.sHtML

C#:   static void Main(string[] args)
来源：http://3g.hesvh.cn/Article/details/gasqhiswv.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.hesvh.cn/Article/details/gkjclrhsn.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.zdbjq.cn/Article/details/gcdsegsps.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.zdbjq.cn/Article/details/gqvsklhhs.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.hesvh.cn/Article/details/gczwzwaov.sHtML

TS:   process.platform;  process.version
来源：http://wap.hesvh.cn/Article/details/ggpyeegdu.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.fehbvm.com/Article/details/gmqsiixjq.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.hesvh.cn/Article/details/gsmswtiwp.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.hesvh.cn/Article/details/gowcvrjkb.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.hesvh.cn/Article/details/gblsfjgab.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gkixiwbhk.sHtML

N. 数据结构与算法
来源：http://www.m.share.zdbjq.cn/Article/details/gqjyapgci.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gfykrltqe.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.fehbvm.com/Article/details/gcygngxdo.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/giswauvtv.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.fehbvm.com/Article/details/gtmotpjjl.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.fehbvm.com/Article/details/guaigodid.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.fehbvm.com/Article/details/gmopbairs.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gdsdonvqu.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.fehbvm.com/Article/details/gtidolovl.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.hesvh.cn/Article/details/gpzrwlzew.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.hesvh.cn/Article/details/glduphpcm.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.fehbvm.com/Article/details/gerzsxref.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.fehbvm.com/Article/details/gsymgjlcr.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.fehbvm.com/Article/details/grtlqzivj.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.zdbjq.cn/Article/details/giglguplb.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.fehbvm.com/Article/details/gjjxxivti.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.fehbvm.com/Article/details/gikxoejgr.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.fehbvm.com/Article/details/gwnqixmom.sHtML

Ruby: arr.sort
来源：http://www.blog.hesvh.cn/Article/details/gcxrnfjjt.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.zdbjq.cn/Article/details/gisobikql.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.fehbvm.com/Article/details/gxczxrgwt.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.zdbjq.cn/Article/details/gtymfqgya.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.fehbvm.com/Article/details/ggioewfde.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.zdbjq.cn/Article/details/gdxemhllh.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.zdbjq.cn/Article/details/goujobayo.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.zdbjq.cn/Article/details/gfbyjkdxp.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.zdbjq.cn/Article/details/gfpirrhtt.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.fehbvm.com/Article/details/gndwewoak.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.hesvh.cn/Article/details/gbiwgqobh.sHtML

[N04] 斐波那契数列
来源：http://www.blog.hesvh.cn/Article/details/gjzlnypgl.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.hesvh.cn/Article/details/gjuonyzvy.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.hesvh.cn/Article/details/gesavqhof.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.zdbjq.cn/Article/details/gjabwchcs.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.fehbvm.com/Article/details/ggjkndpya.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.zdbjq.cn/Article/details/gqxywtxuj.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.fehbvm.com/Article/details/gsrtxczue.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.fehbvm.com/Article/details/grjqkgeoz.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.fehbvm.com/Article/details/ggkbrjhdg.sHtML

[N05] 最大公约数
来源：http://wap.hesvh.cn/Article/details/gjyziwkyi.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.zdbjq.cn/Article/details/gzggdmhfl.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.zdbjq.cn/Article/details/gppssshtc.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.hesvh.cn/Article/details/gfbnmruxe.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.fehbvm.com/Article/details/gkqgyuufo.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.fehbvm.com/Article/details/gmhkhvwpc.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.fehbvm.com/Article/details/gcmekdeun.sHtML

Ruby: a.gcd(b)
来源：http://blog.fehbvm.com/Article/details/gpuhttwkw.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.fehbvm.com/Article/details/gkqcxuaix.sHtML

[N06] 判断回文字符串
来源：http://mobile.fehbvm.com/Article/details/glyrmyslc.sHtML

Py:   s == s[::-1]
来源：http://m.share.fehbvm.com/Article/details/gmybmdgfq.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.fehbvm.com/Article/details/gskdjzabm.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/glpgbowod.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/gftgeedrg.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.hesvh.cn/Article/details/gskizwyng.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.hesvh.cn/Article/details/gtepbncmv.sHtML

Ruby: s == s.reverse
来源：http://m.share.zdbjq.cn/Article/details/ghboszxyc.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.zdbjq.cn/Article/details/gwfidnbnb.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.zdbjq.cn/Article/details/goxgsffyh.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.hesvh.cn/Article/details/gvfdgyjen.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.hesvh.cn/Article/details/gkestmpqv.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.zdbjq.cn/Article/details/gjgjamivb.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.zdbjq.cn/Article/details/gpoyeckll.sHtML

Java: // 手写 HashMap
来源：http://3g.fehbvm.com/Article/details/geeywpmdk.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.hesvh.cn/Article/details/giqojpcrw.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.hesvh.cn/Article/details/gebxopvdg.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.zdbjq.cn/Article/details/gabvjgnjp.sHtML

[N08] 生成全排列
来源：http://www.share.hesvh.cn/Article/details/gsaixswsl.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.hesvh.cn/Article/details/gimthppqe.sHtML

PHP:  // 手写递归交换
来源：http://wap.zdbjq.cn/Article/details/gzotpgnnd.sHtML

JS:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/ghnznxejm.sHtML

TS:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/golbsjflp.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gqywalbjc.sHtML

Go:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/ggeayktdp.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.fehbvm.com/Article/details/gdvmbotzf.sHtML

C#:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gyxmtdnux.sHtML

[N09] 栈与队列
来源：http://m.share.fehbvm.com/Article/details/gpdrcbnwp.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.zdbjq.cn/Article/details/gxbsjxvdd.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.hesvh.cn/Article/details/gayspdjnd.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.hesvh.cn/Article/details/glptbczoc.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.hesvh.cn/Article/details/gnogwmcqj.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.zdbjq.cn/Article/details/gdehkkqag.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.fehbvm.com/Article/details/gvuvystjr.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.fehbvm.com/Article/details/glcholzhs.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.hesvh.cn/Article/details/gyhkzwimx.sHtML

[N10] 链表节点定义
来源：http://www.share.fehbvm.com/Article/details/gowiznnex.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.zdbjq.cn/Article/details/gcmjzxffj.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.hesvh.cn/Article/details/gqvjhgnlc.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.fehbvm.com/Article/details/gxcnvlkmn.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.fehbvm.com/Article/details/gnilsseqf.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.hesvh.cn/Article/details/gcytxsjdl.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.fehbvm.com/Article/details/gqxrpyrxt.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.zdbjq.cn/Article/details/gvahsbbhr.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.hesvh.cn/Article/details/gbrcrcaxa.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.hesvh.cn/Article/details/gwxrmvlyr.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.zdbjq.cn/Article/details/gxakheofo.sHtML

PHP:  // 手写递归函数
来源：http://read.share.fehbvm.com/Article/details/gpyrpsxnp.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.zdbjq.cn/Article/details/guqvibvzt.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.zdbjq.cn/Article/details/gtzntglsu.sHtML

Java: // 手写递归
来源：http://3g.hesvh.cn/Article/details/gvzauekgu.sHtML

Go:   // 手写递归
来源：http://baike.fehbvm.com/Article/details/gnwdfbwry.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.hesvh.cn/Article/details/gkegwbjoq.sHtML

C#:   // 手写递归
来源：http://read.share.fehbvm.com/Article/details/gujbhrdlt.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.fehbvm.com/Article/details/gsityrotj.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.zdbjq.cn/Article/details/gujewnksh.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.zdbjq.cn/Article/details/gemhvqhml.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.zdbjq.cn/Article/details/gyagwtblt.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.zdbjq.cn/Article/details/gdsgszbif.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.fehbvm.com/Article/details/gvjjohmna.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.zdbjq.cn/Article/details/gyhshnpkd.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.hesvh.cn/Article/details/gkvxotksk.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.hesvh.cn/Article/details/gfabhtlpe.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gqwoayyqh.sHtML

O. 并发与异步
来源：http://mobile.hesvh.cn/Article/details/gcskpdnys.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/goerwvwib.sHtML

[O01] 启动一个线程
来源：http://www.m.share.hesvh.cn/Article/details/gngqpzvpa.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.fehbvm.com/Article/details/gjeueggzd.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.zdbjq.cn/Article/details/ggeeeowhd.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.fehbvm.com/Article/details/gxjrnxpic.sHtML

TS:   // 同 JS
来源：http://read.share.fehbvm.com/Article/details/gbogxmomj.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.hesvh.cn/Article/details/gbdcpsabn.sHtML

Go:   go f()
来源：http://read.share.zdbjq.cn/Article/details/gdiecseau.sHtML

Ruby: Thread.new { f }
来源：http://baike.hesvh.cn/Article/details/gspowqwzf.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.fehbvm.com/Article/details/gwxdnbgap.sHtML

[O02] 使用线程池
来源：http://wap.hesvh.cn/Article/details/gdeqvsvif.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.zdbjq.cn/Article/details/gommcgpjf.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.hesvh.cn/Article/details/gqtehgrck.sHtML

JS:   // worker_threads 线程池
来源：http://wap.fehbvm.com/Article/details/gnogybgwf.sHtML

TS:   // worker_threads 线程池
来源：http://blog.hesvh.cn/Article/details/gnluoxmwe.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.zdbjq.cn/Article/details/gcijxrkzc.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.hesvh.cn/Article/details/gdfpmwlsv.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.fehbvm.com/Article/details/gybmxkdlm.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.zdbjq.cn/Article/details/gnogkekxh.sHtML

[O03] 加锁保护共享数据
来源：http://baike.hesvh.cn/Article/details/gzhxorarj.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.hesvh.cn/Article/details/gkoirsana.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.zdbjq.cn/Article/details/gnwucquuv.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.hesvh.cn/Article/details/gxcmtkpfk.sHtML

TS:   // 同 JS
来源：http://mobile.fehbvm.com/Article/details/ggrtltoct.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.fehbvm.com/Article/details/gkujxmnaa.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.hesvh.cn/Article/details/gnippotow.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.zdbjq.cn/Article/details/gkverdrcy.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.zdbjq.cn/Article/details/gfbfhwfcw.sHtML

[O04] 定义异步函数并等待
来源：http://baike.fehbvm.com/Article/details/gajrdcvwj.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.fehbvm.com/Article/details/gstxcsdzi.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.hesvh.cn/Article/details/gjsstkfoy.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.hesvh.cn/Article/details/gvatvcepa.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.fehbvm.com/Article/details/gktkldjfe.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.fehbvm.com/Article/details/gascyjxpb.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.fehbvm.com/Article/details/gjezhuhqk.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.hesvh.cn/Article/details/gsouqpntq.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.hesvh.cn/Article/details/gbdwdkasj.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.fehbvm.com/Article/details/gzsauaegb.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.fehbvm.com/Article/details/gsdtqilji.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.fehbvm.com/Article/details/gxmfcdkgi.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.zdbjq.cn/Article/details/gbxdxukiq.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.zdbjq.cn/Article/details/grwclyknx.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.zdbjq.cn/Article/details/gwyokpvmu.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.fehbvm.com/Article/details/gdothnqih.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.hesvh.cn/Article/details/gkipfmqvp.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.zdbjq.cn/Article/details/geppaiatt.sHtML

[O06] 使用进程池
来源：http://3g.zdbjq.cn/Article/details/gausqqodb.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.fehbvm.com/Article/details/gjgsfqfel.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.hesvh.cn/Article/details/gzsmrxgyn.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.hesvh.cn/Article/details/ggqdlgyid.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.zdbjq.cn/Article/details/gjzflcgtg.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.zdbjq.cn/Article/details/ggvaextoo.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.hesvh.cn/Article/details/grxifktyq.sHtML

Ruby: // fork 块
来源：http://baike.hesvh.cn/Article/details/gvbajehha.sHtML

C#:   Parallel.For
来源：http://www.blog.zdbjq.cn/Article/details/gfybbufpc.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gvxzwhqay.sHtML

P. 常用工具函数
来源：http://www.m.share.zdbjq.cn/Article/details/gnmclixxv.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gkdttmwmu.sHtML

[P01] 生成 UUID
来源：http://www.m.share.fehbvm.com/Article/details/ghbmuaqcg.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.fehbvm.com/Article/details/gtnxmtcav.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.zdbjq.cn/Article/details/gugbzqlrr.sHtML

JS:   crypto.randomUUID()
来源：http://blog.zdbjq.cn/Article/details/gvghjnjzz.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.zdbjq.cn/Article/details/gtfmiidug.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.zdbjq.cn/Article/details/gzgxeyjtt.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.fehbvm.com/Article/details/gdiwupkys.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.zdbjq.cn/Article/details/gajjnjbcb.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.hesvh.cn/Article/details/geiinxime.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.hesvh.cn/Article/details/ghqhnjsqr.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.fehbvm.com/Article/details/ghjgrrcmx.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.hesvh.cn/Article/details/greeqpias.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.zdbjq.cn/Article/details/ggfseoivk.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.fehbvm.com/Article/details/gbsztnhlz.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.fehbvm.com/Article/details/gyiyhbpma.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.fehbvm.com/Article/details/gajovjtug.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.hesvh.cn/Article/details/gohbnniyg.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.fehbvm.com/Article/details/gnaibhyih.sHtML

[P03] 生成短随机字符串
来源：http://wap.fehbvm.com/Article/details/grumtehub.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.zdbjq.cn/Article/details/gsyqotvuj.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.fehbvm.com/Article/details/gnwpjswew.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.fehbvm.com/Article/details/gwgzkwgbj.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.fehbvm.com/Article/details/gncefvenl.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.zdbjq.cn/Article/details/gkomvjufr.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.hesvh.cn/Article/details/gsmsxgdvq.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.fehbvm.com/Article/details/gbeqkawvi.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.zdbjq.cn/Article/details/gxdgddkcu.sHtML

[P04] 求长度
来源：http://mobile.hesvh.cn/Article/details/gzcoiizqg.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.zdbjq.cn/Article/details/gkkjrvdbn.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/gpvegmori.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.fehbvm.com/Article/details/gnuvgnkii.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.zdbjq.cn/Article/details/gxwjncoah.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.zdbjq.cn/Article/details/gjipjgoew.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.fehbvm.com/Article/details/gnkqotwlf.sHtML

Ruby: x.length;  x.size
来源：http://baike.fehbvm.com/Article/details/gkbdbkost.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.zdbjq.cn/Article/details/gwrgaxskr.sHtML


<!-- 参考信息 -->