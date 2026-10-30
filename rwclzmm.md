代发 wailian999

[L07] 处理 HTTP 状态码
来源：http://baike.hesvh.cn/Article/details/glrglqeyt.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.hesvh.cn/Article/details/gqbxseede.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.fehbvm.com/Article/details/gttcpzwnl.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.fehbvm.com/Article/details/gnttkrtoy.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.zdbjq.cn/Article/details/gacoavhfi.sHtML

Java: resp.statusCode()
来源：http://baike.fehbvm.com/Article/details/gwulugkxr.sHtML

Go:   resp.StatusCode
来源：http://3g.fehbvm.com/Article/details/gpknilvky.sHtML

Ruby: resp.code.to_i
来源：http://www.share.hesvh.cn/Article/details/ggxgkhvkg.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.hesvh.cn/Article/details/ghzmkrchf.sHtML

[L08] 并发请求多个地址
来源：http://read.share.hesvh.cn/Article/details/gwxqfymfj.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.zdbjq.cn/Article/details/gbdkkdswu.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.hesvh.cn/Article/details/gecgfzesn.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.zdbjq.cn/Article/details/gxnbwfvib.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fehbvm.com/Article/details/gqrlbbnjq.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.fehbvm.com/Article/details/gjzotcswn.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.fehbvm.com/Article/details/gbhlfloaq.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.zdbjq.cn/Article/details/gigesqsoe.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.hesvh.cn/Article/details/gxpmqnsfo.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gotwrovzn.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.hesvh.cn/Article/details/glhddlbwb.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gurowkwta.sHtML

[M01] 读取命令行参数
来源：http://wap.hesvh.cn/Article/details/geeiijlki.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.fehbvm.com/Article/details/gpgzoiigb.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.fehbvm.com/Article/details/gqypxmpxi.sHtML

JS:   process.argv.slice(2)
来源：http://baike.fehbvm.com/Article/details/gzplifalq.sHtML

TS:   process.argv.slice(2)
来源：http://blog.hesvh.cn/Article/details/gkumshqxx.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.zdbjq.cn/Article/details/gzqktrnkn.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.hesvh.cn/Article/details/gywsuwjfs.sHtML

Ruby: ARGV
来源：http://www.blog.fehbvm.com/Article/details/gfdymovjs.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.hesvh.cn/Article/details/gziwpqaly.sHtML

[M02] 读取环境变量
来源：http://www.blog.zdbjq.cn/Article/details/glwrwxebl.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.hesvh.cn/Article/details/gyfhvehvm.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.fehbvm.com/Article/details/gkymvgzad.sHtML

JS:   process.env.HOME
来源：http://m.share.fehbvm.com/Article/details/gdjoeqwrl.sHtML

TS:   process.env.HOME
来源：http://mobile.hesvh.cn/Article/details/gfajfpnlg.sHtML

Java: System.getenv("HOME")
来源：http://3g.fehbvm.com/Article/details/gvkvlcbwk.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.fehbvm.com/Article/details/gjysinjkj.sHtML

Ruby: ENV["HOME"]
来源：http://wap.fehbvm.com/Article/details/gfqnnksfa.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.zdbjq.cn/Article/details/gnxztqtfg.sHtML

[M03] 执行外部命令
来源：http://www.blog.hesvh.cn/Article/details/geyqnpvxn.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.fehbvm.com/Article/details/gcsorsozf.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.hesvh.cn/Article/details/gazlmmyrl.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.fehbvm.com/Article/details/gjbcymctd.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.fehbvm.com/Article/details/gquyqkqwv.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.zdbjq.cn/Article/details/gsmxkoovp.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.hesvh.cn/Article/details/gskzcexvv.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.hesvh.cn/Article/details/glgbbxtet.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.fehbvm.com/Article/details/gqszxgben.sHtML

[M04] 获取当前工作目录
来源：http://baike.zdbjq.cn/Article/details/gdlzqcmam.sHtML

Py:   os.getcwd()
来源：http://blog.zdbjq.cn/Article/details/ghnfhxmdd.sHtML

PHP:  getcwd();
来源：http://3g.hesvh.cn/Article/details/gbvtwrvht.sHtML

JS:   process.cwd()
来源：http://read.share.fehbvm.com/Article/details/gyxnapcvb.sHtML

TS:   process.cwd()
来源：http://blog.hesvh.cn/Article/details/gfkiiviwk.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.hesvh.cn/Article/details/gbvbispct.sHtML

Go:   os.Getwd()
来源：http://www.m.share.hesvh.cn/Article/details/gakhyazkh.sHtML

Ruby: Dir.pwd
来源：http://www.share.hesvh.cn/Article/details/gawlnnxiu.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.zdbjq.cn/Article/details/gccozeeen.sHtML

[M05] 设置退出码
来源：http://blog.zdbjq.cn/Article/details/gdveioyty.sHtML

Py:   sys.exit(1)
来源：http://m.share.hesvh.cn/Article/details/gncjfgdot.sHtML

PHP:  exit(1);
来源：http://baike.zdbjq.cn/Article/details/gimtirnnw.sHtML

JS:   process.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/giwhfqjqc.sHtML

TS:   process.exit(1)
来源：http://3g.fehbvm.com/Article/details/gjddxyfvm.sHtML

Java: System.exit(1)
来源：http://baike.fehbvm.com/Article/details/gfheyapka.sHtML

Go:   os.Exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gbfuvywca.sHtML

Ruby: exit 1
来源：http://mobile.hesvh.cn/Article/details/geuvqbcdb.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.zdbjq.cn/Article/details/gxsbxajic.sHtML

[M06] 向标准错误输出
来源：http://baike.hesvh.cn/Article/details/goaoahwli.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.fehbvm.com/Article/details/gsxkdhyvj.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.fehbvm.com/Article/details/gntwmrxce.sHtML

JS:   console.error("err")
来源：http://3g.hesvh.cn/Article/details/gjkxkanld.sHtML

TS:   console.error("err")
来源：http://mobile.hesvh.cn/Article/details/gziofooud.sHtML

Java: System.err.println("err")
来源：http://mobile.hesvh.cn/Article/details/grciyzawg.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.fehbvm.com/Article/details/gnssgxxfx.sHtML

Ruby: warn "err"
来源：http://m.share.fehbvm.com/Article/details/gmadpvxgr.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.zdbjq.cn/Article/details/gfrdsiqfz.sHtML

[M07] 判断是否为主入口
来源：http://3g.hesvh.cn/Article/details/grhctwkxs.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.hesvh.cn/Article/details/grtppaali.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.zdbjq.cn/Article/details/gdmjywdoe.sHtML

JS:   require.main === module
来源：http://3g.hesvh.cn/Article/details/gyjpbaoed.sHtML

TS:   require.main === module
来源：http://www.blog.fehbvm.com/Article/details/ghqcxvuik.sHtML

Java: public static void main(String[] args)
来源：http://3g.zdbjq.cn/Article/details/gqjodhczf.sHtML

Go:   func main()
来源：http://m.share.fehbvm.com/Article/details/gjzwyneyl.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.zdbjq.cn/Article/details/gjbxsysdg.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.hesvh.cn/Article/details/gbemplxbf.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.fehbvm.com/Article/details/gvrpgsyjj.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.hesvh.cn/Article/details/gbsceigfw.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.hesvh.cn/Article/details/gjiqyvvdn.sHtML

JS:   process.platform;  process.version
来源：http://m.share.hesvh.cn/Article/details/ghxhmdciv.sHtML

TS:   process.platform;  process.version
来源：http://www.share.fehbvm.com/Article/details/gzsnjnbgm.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.zdbjq.cn/Article/details/gtmzlpbau.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.fehbvm.com/Article/details/glaprhahd.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.fehbvm.com/Article/details/gqpithepg.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.zdbjq.cn/Article/details/gjinbhtfv.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gjxontbsl.sHtML

N. 数据结构与算法
来源：http://www.share.fehbvm.com/Article/details/gwkgchypf.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gvllbadfw.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.fehbvm.com/Article/details/gzfuctnlz.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.hesvh.cn/Article/details/gcfzmoeyp.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.hesvh.cn/Article/details/gdixgmwpv.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.fehbvm.com/Article/details/geururiqc.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.hesvh.cn/Article/details/gklygjsej.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gxdtgxvgo.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.fehbvm.com/Article/details/gaieekuwv.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.fehbvm.com/Article/details/gzyogbdip.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.fehbvm.com/Article/details/gnieisyeq.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.hesvh.cn/Article/details/gtithoikw.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.hesvh.cn/Article/details/gknabblfn.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.fehbvm.com/Article/details/gatsiwmie.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.zdbjq.cn/Article/details/gicyentbl.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.zdbjq.cn/Article/details/gqvcwwxti.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.hesvh.cn/Article/details/grbgpvqca.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.fehbvm.com/Article/details/gdakefvla.sHtML

Ruby: arr.sort
来源：http://www.blog.hesvh.cn/Article/details/gnpyyqhmr.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.zdbjq.cn/Article/details/gqhoyfdex.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.fehbvm.com/Article/details/ggioxhaoh.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.hesvh.cn/Article/details/ggajkqbfr.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.hesvh.cn/Article/details/gkefiejci.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.zdbjq.cn/Article/details/gsyhhkvot.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.hesvh.cn/Article/details/gceekggxf.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.fehbvm.com/Article/details/gcxyxegmb.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.hesvh.cn/Article/details/gibneirhe.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.fehbvm.com/Article/details/grqycofjq.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.zdbjq.cn/Article/details/gghwipkqs.sHtML

[N04] 斐波那契数列
来源：http://www.blog.hesvh.cn/Article/details/gzwxpmsgt.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.fehbvm.com/Article/details/geizspccq.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.hesvh.cn/Article/details/gtoxdwtid.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.hesvh.cn/Article/details/gvemfwwnw.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.fehbvm.com/Article/details/gvmvcaokw.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.fehbvm.com/Article/details/gmfxjqllp.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.hesvh.cn/Article/details/gzcjhtemt.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.fehbvm.com/Article/details/gwhujtluv.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.hesvh.cn/Article/details/gmutihzma.sHtML

[N05] 最大公约数
来源：http://blog.hesvh.cn/Article/details/gphmybptk.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.zdbjq.cn/Article/details/gzbjdoltm.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.fehbvm.com/Article/details/gvkwsrsdj.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.zdbjq.cn/Article/details/gnmlwcsbj.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.fehbvm.com/Article/details/gtjdyiscb.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.hesvh.cn/Article/details/gtwpybvje.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.hesvh.cn/Article/details/goimqnpsf.sHtML

Ruby: a.gcd(b)
来源：http://baike.fehbvm.com/Article/details/gadqgfqmt.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.zdbjq.cn/Article/details/gdsozpdqb.sHtML

[N06] 判断回文字符串
来源：http://read.share.hesvh.cn/Article/details/gzpqmmmhe.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.hesvh.cn/Article/details/ggrckyrma.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.hesvh.cn/Article/details/ghycvouiw.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/ghopfirqb.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/gifhvirhq.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.zdbjq.cn/Article/details/gvrmwegwz.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.hesvh.cn/Article/details/gwgkokdph.sHtML

Ruby: s == s.reverse
来源：http://m.share.fehbvm.com/Article/details/gyoloefqt.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.hesvh.cn/Article/details/gjrntyfjp.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.hesvh.cn/Article/details/gythlyfjk.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.hesvh.cn/Article/details/gneavffyo.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.zdbjq.cn/Article/details/giaeqspja.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.zdbjq.cn/Article/details/ggybtadoj.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.fehbvm.com/Article/details/gweqcwlur.sHtML

Java: // 手写 HashMap
来源：http://3g.hesvh.cn/Article/details/goxswmhte.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.zdbjq.cn/Article/details/gvcrwxude.sHtML

Ruby: // 手写 Hash
来源：http://m.share.zdbjq.cn/Article/details/gaxlrhexr.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.hesvh.cn/Article/details/guumjkvuv.sHtML

[N08] 生成全排列
来源：http://baike.zdbjq.cn/Article/details/gwraruuey.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.fehbvm.com/Article/details/gvwouqtyi.sHtML

PHP:  // 手写递归交换
来源：http://blog.fehbvm.com/Article/details/glthrgpdl.sHtML

JS:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gbibpiddz.sHtML

TS:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gcefnqqlm.sHtML

Java: // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gncnsptvj.sHtML

Go:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gelmfgizc.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.fehbvm.com/Article/details/goiybhvvk.sHtML

C#:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gtovbuvnp.sHtML

[N09] 栈与队列
来源：http://www.share.hesvh.cn/Article/details/gbehobnsk.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.hesvh.cn/Article/details/gwkkuggdr.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.zdbjq.cn/Article/details/glyhjxyhb.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.fehbvm.com/Article/details/gcqorcjwz.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.hesvh.cn/Article/details/gezfacept.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.hesvh.cn/Article/details/gtzelappj.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.zdbjq.cn/Article/details/galizmood.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.hesvh.cn/Article/details/gvoeoyzxb.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.hesvh.cn/Article/details/gcyuvibco.sHtML

[N10] 链表节点定义
来源：http://wap.zdbjq.cn/Article/details/gbqlyhmev.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.hesvh.cn/Article/details/geodsowbb.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.hesvh.cn/Article/details/gkulxabab.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.fehbvm.com/Article/details/ghnpsoews.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.zdbjq.cn/Article/details/gaohktwrv.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.fehbvm.com/Article/details/gkgptjbqu.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.zdbjq.cn/Article/details/gvttnicst.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.hesvh.cn/Article/details/gkkwatkwh.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.fehbvm.com/Article/details/gilujrizv.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.zdbjq.cn/Article/details/gwgsbtnds.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.hesvh.cn/Article/details/gapgpvxds.sHtML

PHP:  // 手写递归函数
来源：http://wap.zdbjq.cn/Article/details/gffmukckl.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.fehbvm.com/Article/details/gjzokdwlt.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.fehbvm.com/Article/details/gkygezyih.sHtML

Java: // 手写递归
来源：http://read.share.hesvh.cn/Article/details/gmvkkamwc.sHtML

Go:   // 手写递归
来源：http://m.share.zdbjq.cn/Article/details/gpsljpufc.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.fehbvm.com/Article/details/gdqratazq.sHtML

C#:   // 手写递归
来源：http://blog.fehbvm.com/Article/details/gaixveyhg.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.fehbvm.com/Article/details/gdakcxbnb.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.hesvh.cn/Article/details/gppinixdx.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.zdbjq.cn/Article/details/gtqcpswhk.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.zdbjq.cn/Article/details/gmkpmpkoi.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.fehbvm.com/Article/details/givrikrni.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.fehbvm.com/Article/details/gofawhaml.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.fehbvm.com/Article/details/gfdpelhxt.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.hesvh.cn/Article/details/glqexobqb.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.zdbjq.cn/Article/details/gpqwcbtyt.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gxnjyrpmr.sHtML

O. 并发与异步
来源：http://www.m.share.zdbjq.cn/Article/details/gnioaxovk.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/ghkwzszjc.sHtML

[O01] 启动一个线程
来源：http://www.m.share.zdbjq.cn/Article/details/gtguyhska.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.zdbjq.cn/Article/details/gascasjzn.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.hesvh.cn/Article/details/gagqwibbm.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.hesvh.cn/Article/details/gswfwclgo.sHtML

TS:   // 同 JS
来源：http://read.share.hesvh.cn/Article/details/gnoqkzhif.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.zdbjq.cn/Article/details/gbdrpbatb.sHtML

Go:   go f()
来源：http://3g.fehbvm.com/Article/details/genpeolop.sHtML

Ruby: Thread.new { f }
来源：http://baike.hesvh.cn/Article/details/gfmbjaxfh.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.hesvh.cn/Article/details/gvzqrqmie.sHtML

[O02] 使用线程池
来源：http://read.share.zdbjq.cn/Article/details/gizgqltvb.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.hesvh.cn/Article/details/gvrnmgkjk.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.hesvh.cn/Article/details/gobagzilj.sHtML

JS:   // worker_threads 线程池
来源：http://baike.fehbvm.com/Article/details/gnkbcczdg.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.hesvh.cn/Article/details/gocaviefa.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.hesvh.cn/Article/details/gutvgiaxj.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.fehbvm.com/Article/details/gzvowgjsv.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.zdbjq.cn/Article/details/gcokuedra.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.hesvh.cn/Article/details/giajcnrmb.sHtML

[O03] 加锁保护共享数据
来源：http://baike.fehbvm.com/Article/details/gszescohq.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.hesvh.cn/Article/details/gfafakrsh.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.fehbvm.com/Article/details/ggehxbiou.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.hesvh.cn/Article/details/gwfklrbsw.sHtML

TS:   // 同 JS
来源：http://www.share.fehbvm.com/Article/details/gqgdhbpnd.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.zdbjq.cn/Article/details/gcbuzwclp.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.hesvh.cn/Article/details/ghyacsmtf.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.zdbjq.cn/Article/details/gcbayludq.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.hesvh.cn/Article/details/gotmwotlf.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.fehbvm.com/Article/details/gljummnpp.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.zdbjq.cn/Article/details/gehqzcrra.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.hesvh.cn/Article/details/gwkkbgqlm.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.zdbjq.cn/Article/details/gxnvxqknq.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.fehbvm.com/Article/details/gzjbglhsr.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.zdbjq.cn/Article/details/gqprxuzwv.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.zdbjq.cn/Article/details/grlckbrer.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.zdbjq.cn/Article/details/gdilfkksr.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.zdbjq.cn/Article/details/gechpwaaa.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.zdbjq.cn/Article/details/gxiftypkz.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.fehbvm.com/Article/details/gwmbhptci.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.hesvh.cn/Article/details/gqqrjnmbu.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.hesvh.cn/Article/details/gjolrtxpo.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.fehbvm.com/Article/details/gzsxcebvm.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.fehbvm.com/Article/details/ggucdeczw.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.zdbjq.cn/Article/details/gdgdxieac.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.hesvh.cn/Article/details/gwaxxsqgp.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.hesvh.cn/Article/details/glzbngezf.sHtML

[O06] 使用进程池
来源：http://www.share.zdbjq.cn/Article/details/gwyorwekg.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.fehbvm.com/Article/details/gqpcmchhg.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.fehbvm.com/Article/details/gvshcmqya.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.zdbjq.cn/Article/details/gnvpfcxqd.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.fehbvm.com/Article/details/gvmrcvdkg.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.hesvh.cn/Article/details/gneljtbdb.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.hesvh.cn/Article/details/gxpkmqdbi.sHtML

Ruby: // fork 块
来源：http://3g.hesvh.cn/Article/details/gqwsgreyz.sHtML

C#:   Parallel.For
来源：http://3g.zdbjq.cn/Article/details/gjltlpdjl.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gpkkgksga.sHtML

P. 常用工具函数
来源：http://www.m.share.hesvh.cn/Article/details/gyjsrzcof.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/glsvxfuen.sHtML

[P01] 生成 UUID
来源：http://www.share.fehbvm.com/Article/details/gednxrgqe.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.hesvh.cn/Article/details/goadukqye.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.zdbjq.cn/Article/details/gyamowdhb.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.zdbjq.cn/Article/details/gfgguvxiy.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.zdbjq.cn/Article/details/grexsxonk.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.hesvh.cn/Article/details/gzrhacokq.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.zdbjq.cn/Article/details/gwdlcxkee.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.zdbjq.cn/Article/details/grjtijhxh.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.fehbvm.com/Article/details/ghxukhoyx.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.hesvh.cn/Article/details/gtxtnwpcp.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.fehbvm.com/Article/details/gxiygqoeo.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gmasparot.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.fehbvm.com/Article/details/gyxzboqov.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.zdbjq.cn/Article/details/gmzcnxsij.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.hesvh.cn/Article/details/gyimtzfip.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.fehbvm.com/Article/details/gjanlhhic.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.fehbvm.com/Article/details/gxoslyamt.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.zdbjq.cn/Article/details/gdnwztudn.sHtML

[P03] 生成短随机字符串
来源：http://read.share.zdbjq.cn/Article/details/guukntkuk.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.zdbjq.cn/Article/details/gnmhtrdjv.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.hesvh.cn/Article/details/guxxghmby.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.fehbvm.com/Article/details/gmvykaklm.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.fehbvm.com/Article/details/gfjqxeaet.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.zdbjq.cn/Article/details/ghivewhal.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.hesvh.cn/Article/details/gjozjkntk.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.fehbvm.com/Article/details/gnvurktst.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.fehbvm.com/Article/details/gtxibrslu.sHtML

[P04] 求长度
来源：http://3g.fehbvm.com/Article/details/gtvgwcmxq.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.hesvh.cn/Article/details/girvhgwnt.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/gmsryiite.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.zdbjq.cn/Article/details/giijydssj.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.fehbvm.com/Article/details/glztrwsxm.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.fehbvm.com/Article/details/goodpkxzr.sHtML

Go:   len(arr);  len(m)
来源：http://wap.hesvh.cn/Article/details/gpyxuxnuw.sHtML

Ruby: x.length;  x.size
来源：http://wap.zdbjq.cn/Article/details/gkgdtfwba.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.fehbvm.com/Article/details/gbcfnbpta.sHtML


<!-- 参考信息 -->