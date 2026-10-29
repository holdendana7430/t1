代发 wailian999

TS:   resp.ok;  resp.status
来源：http://m.share.hesvh.cn/Article/details/gjhmxcyhr.sHtML

Java: resp.statusCode()
来源：http://m.share.hesvh.cn/Article/details/gzkdubiza.sHtML

Go:   resp.StatusCode
来源：http://m.share.zdbjq.cn/Article/details/gdrvehqqh.sHtML

Ruby: resp.code.to_i
来源：http://www.share.fehbvm.com/Article/details/gqwfbwwqq.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.zdbjq.cn/Article/details/gbpbyjmti.sHtML

[L08] 并发请求多个地址
来源：http://mobile.fehbvm.com/Article/details/gfhlwfhyg.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.hesvh.cn/Article/details/ghlwoxueg.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.zdbjq.cn/Article/details/gpgmadydx.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.hesvh.cn/Article/details/gqdesnztf.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.zdbjq.cn/Article/details/gbgwhqwqf.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.hesvh.cn/Article/details/glxalzvry.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.fehbvm.com/Article/details/gujdunhij.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.zdbjq.cn/Article/details/gudsduqnn.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.fehbvm.com/Article/details/gvhzsjbkt.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gjgxjjxfh.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.fehbvm.com/Article/details/gmlaqukst.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/ghwqzunou.sHtML

[M01] 读取命令行参数
来源：http://m.share.hesvh.cn/Article/details/gdtzuzzol.sHtML

Py:   sys.argv[1:]
来源：http://wap.zdbjq.cn/Article/details/ghgbptyoz.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.zdbjq.cn/Article/details/gifeyxvcd.sHtML

JS:   process.argv.slice(2)
来源：http://3g.zdbjq.cn/Article/details/gdbiericl.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.zdbjq.cn/Article/details/ghyvhmqfu.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.hesvh.cn/Article/details/gyfyaaiik.sHtML

Go:   os.Args[1:]
来源：http://wap.hesvh.cn/Article/details/gamqjjjxt.sHtML

Ruby: ARGV
来源：http://www.share.fehbvm.com/Article/details/gwhcitrkr.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.fehbvm.com/Article/details/gdrrkkyan.sHtML

[M02] 读取环境变量
来源：http://read.share.fehbvm.com/Article/details/grychhktv.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.hesvh.cn/Article/details/gamjwphdp.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.hesvh.cn/Article/details/gnkbctuzv.sHtML

JS:   process.env.HOME
来源：http://3g.zdbjq.cn/Article/details/gxrcyzubd.sHtML

TS:   process.env.HOME
来源：http://www.m.share.zdbjq.cn/Article/details/gfgpizayf.sHtML

Java: System.getenv("HOME")
来源：http://baike.fehbvm.com/Article/details/ghwxtfeke.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.fehbvm.com/Article/details/ggyueemrh.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.hesvh.cn/Article/details/ghsxevrwp.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.hesvh.cn/Article/details/gmsbtnovw.sHtML

[M03] 执行外部命令
来源：http://www.share.hesvh.cn/Article/details/gnjwpwjbt.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.fehbvm.com/Article/details/gncbmzylc.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.hesvh.cn/Article/details/gybkfsiuk.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.hesvh.cn/Article/details/gioutqjqr.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.zdbjq.cn/Article/details/gguptcnrw.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.hesvh.cn/Article/details/gngljqlyt.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.fehbvm.com/Article/details/gylmejqaq.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.hesvh.cn/Article/details/gyawdoojf.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.zdbjq.cn/Article/details/gnzixjrui.sHtML

[M04] 获取当前工作目录
来源：http://m.share.hesvh.cn/Article/details/gsrzalcxo.sHtML

Py:   os.getcwd()
来源：http://www.m.share.hesvh.cn/Article/details/gnlwrjznc.sHtML

PHP:  getcwd();
来源：http://www.share.fehbvm.com/Article/details/gldosweyb.sHtML

JS:   process.cwd()
来源：http://wap.hesvh.cn/Article/details/gzyxmvmgt.sHtML

TS:   process.cwd()
来源：http://3g.zdbjq.cn/Article/details/guajfhzib.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.zdbjq.cn/Article/details/gtrpbgclu.sHtML

Go:   os.Getwd()
来源：http://blog.fehbvm.com/Article/details/gvttvkzjh.sHtML

Ruby: Dir.pwd
来源：http://m.share.zdbjq.cn/Article/details/gqafxplnu.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.fehbvm.com/Article/details/gtfcabkrz.sHtML

[M05] 设置退出码
来源：http://3g.zdbjq.cn/Article/details/grnnqhscd.sHtML

Py:   sys.exit(1)
来源：http://m.share.fehbvm.com/Article/details/gottcopki.sHtML

PHP:  exit(1);
来源：http://baike.hesvh.cn/Article/details/gxyosvodt.sHtML

JS:   process.exit(1)
来源：http://wap.hesvh.cn/Article/details/gdkahwwoj.sHtML

TS:   process.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gyiuakisp.sHtML

Java: System.exit(1)
来源：http://read.share.fehbvm.com/Article/details/glsrlaawy.sHtML

Go:   os.Exit(1)
来源：http://mobile.hesvh.cn/Article/details/gmuotbbso.sHtML

Ruby: exit 1
来源：http://baike.fehbvm.com/Article/details/guyjnwtuj.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.hesvh.cn/Article/details/gnumibfdz.sHtML

[M06] 向标准错误输出
来源：http://mobile.hesvh.cn/Article/details/gignxapvj.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.hesvh.cn/Article/details/gqlyswmgm.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.zdbjq.cn/Article/details/gnlyfzqnv.sHtML

JS:   console.error("err")
来源：http://wap.zdbjq.cn/Article/details/gqigjrsbs.sHtML

TS:   console.error("err")
来源：http://3g.zdbjq.cn/Article/details/grftkwepg.sHtML

Java: System.err.println("err")
来源：http://www.share.zdbjq.cn/Article/details/gwvvveluc.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.fehbvm.com/Article/details/gybiwtnky.sHtML

Ruby: warn "err"
来源：http://blog.hesvh.cn/Article/details/gwclyriqd.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.zdbjq.cn/Article/details/ggrmpxeyx.sHtML

[M07] 判断是否为主入口
来源：http://www.share.zdbjq.cn/Article/details/gxhiwalgt.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.fehbvm.com/Article/details/gtgofqfro.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.hesvh.cn/Article/details/gbyktyxzj.sHtML

JS:   require.main === module
来源：http://www.m.share.hesvh.cn/Article/details/gpmocjdts.sHtML

TS:   require.main === module
来源：http://m.share.zdbjq.cn/Article/details/gwrttinyv.sHtML

Java: public static void main(String[] args)
来源：http://read.share.hesvh.cn/Article/details/gozwrhkjb.sHtML

Go:   func main()
来源：http://read.share.fehbvm.com/Article/details/gbahbdhlh.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.fehbvm.com/Article/details/gpigptewz.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.zdbjq.cn/Article/details/gxengkosw.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.hesvh.cn/Article/details/gewabzanc.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.hesvh.cn/Article/details/gczweopyp.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.zdbjq.cn/Article/details/gftyrkaxf.sHtML

JS:   process.platform;  process.version
来源：http://mobile.hesvh.cn/Article/details/gqmcqfdtt.sHtML

TS:   process.platform;  process.version
来源：http://blog.fehbvm.com/Article/details/gpzoyzljk.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.hesvh.cn/Article/details/gzzpgncec.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.hesvh.cn/Article/details/gztxevmvl.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.fehbvm.com/Article/details/gkfaiotnb.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.zdbjq.cn/Article/details/gujmvfghe.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/ghkgotlod.sHtML

N. 数据结构与算法
来源：http://mobile.zdbjq.cn/Article/details/gnxbjpxhf.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gdkltngkk.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.hesvh.cn/Article/details/gxdhtaguf.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.hesvh.cn/Article/details/gitmzwezp.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.hesvh.cn/Article/details/gzaryuajq.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.fehbvm.com/Article/details/gqszeljal.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.hesvh.cn/Article/details/geauarttv.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.hesvh.cn/Article/details/gbwhizfct.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/ggdaezpzu.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.hesvh.cn/Article/details/gudhxomlx.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gtewzrztv.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.hesvh.cn/Article/details/gntrmvpst.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.hesvh.cn/Article/details/gopagzbtg.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.zdbjq.cn/Article/details/ghihwosrd.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.hesvh.cn/Article/details/gfescykod.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.fehbvm.com/Article/details/gxzrfrukm.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.zdbjq.cn/Article/details/gnvmrbhnx.sHtML

Go:   slices.Sort(arr)
来源：http://baike.zdbjq.cn/Article/details/gvjkfzfzw.sHtML

Ruby: arr.sort
来源：http://wap.hesvh.cn/Article/details/gkfsuubhn.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.zdbjq.cn/Article/details/galrptnfp.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.hesvh.cn/Article/details/gegtblnri.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.fehbvm.com/Article/details/glmayvamm.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.zdbjq.cn/Article/details/gklrpazwu.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.zdbjq.cn/Article/details/geepchzdn.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.zdbjq.cn/Article/details/gbhatpueq.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.fehbvm.com/Article/details/gfhsxktvi.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.zdbjq.cn/Article/details/gdcuvsdus.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.fehbvm.com/Article/details/grbujcdni.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.hesvh.cn/Article/details/gtqpbslfq.sHtML

[N04] 斐波那契数列
来源：http://wap.hesvh.cn/Article/details/gsshqkqdi.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.fehbvm.com/Article/details/gcjqofyqq.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.fehbvm.com/Article/details/gdjnbsblo.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.zdbjq.cn/Article/details/girjjcnmm.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.fehbvm.com/Article/details/goexldlfg.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.zdbjq.cn/Article/details/gvyugvuou.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.zdbjq.cn/Article/details/grpvemmyo.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.fehbvm.com/Article/details/gxedvkcur.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.fehbvm.com/Article/details/gsvswdmye.sHtML

[N05] 最大公约数
来源：http://m.share.zdbjq.cn/Article/details/gtpzriuls.sHtML

Py:   math.gcd(a, b)
来源：http://baike.hesvh.cn/Article/details/gbxaogdkx.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.zdbjq.cn/Article/details/gmjakmayf.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.zdbjq.cn/Article/details/gnvvkasvt.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.hesvh.cn/Article/details/gyflfnpid.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.fehbvm.com/Article/details/ghqkbfiav.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.zdbjq.cn/Article/details/geoucozne.sHtML

Ruby: a.gcd(b)
来源：http://www.share.zdbjq.cn/Article/details/gqjfqnwws.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.zdbjq.cn/Article/details/gtxqgaugh.sHtML

[N06] 判断回文字符串
来源：http://wap.zdbjq.cn/Article/details/gitvufaqv.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.fehbvm.com/Article/details/ghfknande.sHtML

PHP:  $s === strrev($s);
来源：http://3g.zdbjq.cn/Article/details/grkvnjceh.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/gkpadbose.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gycincsxv.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.fehbvm.com/Article/details/gmloeahdg.sHtML

Go:   // 双指针从两端比较
来源：http://baike.fehbvm.com/Article/details/gqgopptoc.sHtML

Ruby: s == s.reverse
来源：http://baike.fehbvm.com/Article/details/gljtajqws.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.hesvh.cn/Article/details/gdcdiechu.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.zdbjq.cn/Article/details/gnhcjhwnt.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.hesvh.cn/Article/details/gofqolrby.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.zdbjq.cn/Article/details/gdindoeqy.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.hesvh.cn/Article/details/gneicntex.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.zdbjq.cn/Article/details/gnwzfrzvw.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.fehbvm.com/Article/details/gbtfxisei.sHtML

Go:   // 手写 map[int]int
来源：http://blog.fehbvm.com/Article/details/garwsnhqz.sHtML

Ruby: // 手写 Hash
来源：http://m.share.zdbjq.cn/Article/details/gmpvllnhh.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.fehbvm.com/Article/details/gtippwdid.sHtML

[N08] 生成全排列
来源：http://baike.hesvh.cn/Article/details/giztaykll.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.fehbvm.com/Article/details/gkajfubjb.sHtML

PHP:  // 手写递归交换
来源：http://blog.hesvh.cn/Article/details/gcfxhqysz.sHtML

JS:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gocnrnurt.sHtML

TS:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gkudcomkz.sHtML

Java: // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/glmweczkf.sHtML

Go:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gwohqcpun.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.zdbjq.cn/Article/details/gmoaccoiz.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gqqshpupp.sHtML

[N09] 栈与队列
来源：http://mobile.zdbjq.cn/Article/details/gygvzwydt.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/goisjlmms.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.zdbjq.cn/Article/details/gqlnkhjfk.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.hesvh.cn/Article/details/groanetnc.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.fehbvm.com/Article/details/gftkjprsd.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.hesvh.cn/Article/details/goggbcaft.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.zdbjq.cn/Article/details/groibvhzz.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.hesvh.cn/Article/details/ggckdpoqv.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.zdbjq.cn/Article/details/gnozhzktr.sHtML

[N10] 链表节点定义
来源：http://wap.hesvh.cn/Article/details/glivmocle.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.hesvh.cn/Article/details/gseywgowy.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.hesvh.cn/Article/details/gkhscxvcf.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.zdbjq.cn/Article/details/gbalpbgtl.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.fehbvm.com/Article/details/gmgbbgrsn.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.fehbvm.com/Article/details/grpwnxacu.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.fehbvm.com/Article/details/gxwbsvvfj.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.fehbvm.com/Article/details/gxqugntag.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.hesvh.cn/Article/details/ghysmsccn.sHtML

[N11] 二叉树中序遍历
来源：http://3g.fehbvm.com/Article/details/gkjottuye.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.fehbvm.com/Article/details/gnvjagzqv.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.fehbvm.com/Article/details/gzuhxjcxy.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.fehbvm.com/Article/details/gditdtmec.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.zdbjq.cn/Article/details/goheyfxdd.sHtML

Java: // 手写递归
来源：http://blog.zdbjq.cn/Article/details/ggvwmqcrc.sHtML

Go:   // 手写递归
来源：http://www.m.share.zdbjq.cn/Article/details/gsbvgxcsp.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.hesvh.cn/Article/details/gqvtnhgsi.sHtML

C#:   // 手写递归
来源：http://www.share.hesvh.cn/Article/details/gweekawwp.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.hesvh.cn/Article/details/gdajqsfke.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.fehbvm.com/Article/details/gmzkoujum.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.hesvh.cn/Article/details/guxhtcpae.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.zdbjq.cn/Article/details/gwbhndtla.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.zdbjq.cn/Article/details/grsbjzzyd.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.zdbjq.cn/Article/details/gtuliihdb.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.fehbvm.com/Article/details/gllnlxwxs.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.hesvh.cn/Article/details/gtacuvicd.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.hesvh.cn/Article/details/gjizzjzcb.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gusrfpfgt.sHtML

O. 并发与异步
来源：http://www.blog.hesvh.cn/Article/details/gfswdoveu.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/glypifeqt.sHtML

[O01] 启动一个线程
来源：http://wap.zdbjq.cn/Article/details/glasuaowz.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.zdbjq.cn/Article/details/gvgppioas.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.hesvh.cn/Article/details/ginfyhzvv.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.fehbvm.com/Article/details/gwhkxlrej.sHtML

TS:   // 同 JS
来源：http://read.share.fehbvm.com/Article/details/ghbotyrvh.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.zdbjq.cn/Article/details/gglhksjfu.sHtML

Go:   go f()
来源：http://3g.hesvh.cn/Article/details/gnlyuaixp.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.hesvh.cn/Article/details/gnuaqatpl.sHtML

C#:   Task.Run(() => F());
来源：http://baike.hesvh.cn/Article/details/gtwkvfrxd.sHtML

[O02] 使用线程池
来源：http://www.share.fehbvm.com/Article/details/gcoqzdlxd.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.zdbjq.cn/Article/details/gjoxvperl.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.hesvh.cn/Article/details/gphepgghv.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.fehbvm.com/Article/details/ggyjlegvj.sHtML

TS:   // worker_threads 线程池
来源：http://wap.zdbjq.cn/Article/details/godyomkwe.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.fehbvm.com/Article/details/gutpbhjey.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.fehbvm.com/Article/details/gabilekjv.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.zdbjq.cn/Article/details/gdncgfbee.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.zdbjq.cn/Article/details/gmavfrsms.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.zdbjq.cn/Article/details/grrgrhpji.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.zdbjq.cn/Article/details/grqhhpawt.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.hesvh.cn/Article/details/gezuxryeu.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.hesvh.cn/Article/details/gkxavmkpl.sHtML

TS:   // 同 JS
来源：http://mobile.zdbjq.cn/Article/details/geltiphuk.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.fehbvm.com/Article/details/gdugejxxx.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.fehbvm.com/Article/details/geriwoaxu.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.fehbvm.com/Article/details/gysdsctsv.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.hesvh.cn/Article/details/gxbzbjcre.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.hesvh.cn/Article/details/gqjfshjvl.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.hesvh.cn/Article/details/gcjyztujb.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.hesvh.cn/Article/details/gmnhouaxx.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.fehbvm.com/Article/details/gxnecscmp.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.fehbvm.com/Article/details/gcevlueqv.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.fehbvm.com/Article/details/gskbeerpr.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.zdbjq.cn/Article/details/gcvihrfmq.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.hesvh.cn/Article/details/galsohqoh.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.zdbjq.cn/Article/details/gnfhhlzfa.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.fehbvm.com/Article/details/gfsicaivj.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.fehbvm.com/Article/details/gshlqknou.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.fehbvm.com/Article/details/gghuhczto.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.hesvh.cn/Article/details/gaqanwzji.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.hesvh.cn/Article/details/gcfyswxen.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.fehbvm.com/Article/details/gyaqljpap.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.zdbjq.cn/Article/details/ghsvcmzmg.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.hesvh.cn/Article/details/giwxbkupx.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.fehbvm.com/Article/details/gjqxidbbo.sHtML

[O06] 使用进程池
来源：http://www.blog.zdbjq.cn/Article/details/guqdrzxva.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.zdbjq.cn/Article/details/gaprljenv.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.fehbvm.com/Article/details/gdatqtxgp.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.zdbjq.cn/Article/details/gtyaodicb.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.hesvh.cn/Article/details/gwucparon.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.hesvh.cn/Article/details/gyspcxecr.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.fehbvm.com/Article/details/gopouwxhv.sHtML

Ruby: // fork 块
来源：http://read.share.zdbjq.cn/Article/details/gkrpixope.sHtML

C#:   Parallel.For
来源：http://blog.hesvh.cn/Article/details/gterahxib.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/glsndlspq.sHtML

P. 常用工具函数
来源：http://www.blog.fehbvm.com/Article/details/gcggixplj.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gwlkogrmd.sHtML

[P01] 生成 UUID
来源：http://www.blog.hesvh.cn/Article/details/givduhcsu.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.hesvh.cn/Article/details/geynujbbp.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.fehbvm.com/Article/details/givwqyahs.sHtML

JS:   crypto.randomUUID()
来源：http://wap.hesvh.cn/Article/details/glkvhhzpj.sHtML

TS:   crypto.randomUUID()
来源：http://wap.zdbjq.cn/Article/details/gfenkrzne.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.hesvh.cn/Article/details/gtjfiobjm.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.fehbvm.com/Article/details/gwdfhicck.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.fehbvm.com/Article/details/ghporqdam.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.hesvh.cn/Article/details/guudyxccw.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.fehbvm.com/Article/details/gatldcwsf.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.fehbvm.com/Article/details/gynsxwxqx.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.hesvh.cn/Article/details/gavxxctna.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.fehbvm.com/Article/details/gsobgelqz.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.fehbvm.com/Article/details/gfvakyklg.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.hesvh.cn/Article/details/gixrrfkbt.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.hesvh.cn/Article/details/gvagcqobs.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.hesvh.cn/Article/details/gptvncsio.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.fehbvm.com/Article/details/gbdjansnj.sHtML

[P03] 生成短随机字符串
来源：http://wap.zdbjq.cn/Article/details/gfeuiwuvu.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.fehbvm.com/Article/details/gedjtvohg.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.fehbvm.com/Article/details/gdxnvvtkg.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.hesvh.cn/Article/details/gukezqhbb.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.hesvh.cn/Article/details/gleazzgbx.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.zdbjq.cn/Article/details/gzvpkgglj.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.hesvh.cn/Article/details/ggjzlxjkz.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.hesvh.cn/Article/details/glntrcymz.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.hesvh.cn/Article/details/gbxxkkspn.sHtML

[P04] 求长度
来源：http://read.share.hesvh.cn/Article/details/gphugqafy.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.hesvh.cn/Article/details/gprpnwpxy.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/gctnpevov.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.hesvh.cn/Article/details/gnbutfrjw.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.hesvh.cn/Article/details/gxdhnxtrh.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.hesvh.cn/Article/details/gkicnmhoz.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.fehbvm.com/Article/details/ggmfzddtp.sHtML

Ruby: x.length;  x.size
来源：http://read.share.fehbvm.com/Article/details/gbxphuclu.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.zdbjq.cn/Article/details/ggwfigxwp.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.zdbjq.cn/Article/details/gsnczsknp.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.fehbvm.com/Article/details/gqtohobbj.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.hesvh.cn/Article/details/gzrsjkqbz.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.zdbjq.cn/Article/details/gicxkulcl.sHtML


<!-- 参考信息 -->