代发 wailian999

[L07] 处理 HTTP 状态码
来源：http://www.m.share.fehbvm.com/Article/details/gzxwymcgh.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.fehbvm.com/Article/details/gaieyvyjc.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.hesvh.cn/Article/details/gkeucjgvw.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.zdbjq.cn/Article/details/geqctxdyc.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.zdbjq.cn/Article/details/gaizfliyt.sHtML

Java: resp.statusCode()
来源：http://m.share.fehbvm.com/Article/details/gnzmdwpio.sHtML

Go:   resp.StatusCode
来源：http://blog.hesvh.cn/Article/details/gxfbjfxxu.sHtML

Ruby: resp.code.to_i
来源：http://baike.zdbjq.cn/Article/details/gbnzeyrdk.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.hesvh.cn/Article/details/gcusqmllf.sHtML

[L08] 并发请求多个地址
来源：http://blog.zdbjq.cn/Article/details/gvlezxsiq.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.hesvh.cn/Article/details/gfrewjkus.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.fehbvm.com/Article/details/gzwlifwya.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.hesvh.cn/Article/details/gocjmkwzc.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.hesvh.cn/Article/details/ggpvowdqm.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.hesvh.cn/Article/details/gqojlylrj.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.fehbvm.com/Article/details/gtpettcqm.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.hesvh.cn/Article/details/gjaqoovjf.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.fehbvm.com/Article/details/gzdvhgnki.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gwivohbch.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.hesvh.cn/Article/details/ggzdrpwwj.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/glsathzic.sHtML

[M01] 读取命令行参数
来源：http://blog.zdbjq.cn/Article/details/gcbjlivrx.sHtML

Py:   sys.argv[1:]
来源：http://read.share.hesvh.cn/Article/details/gihqkgmwb.sHtML

PHP:  $argv;  $argc;
来源：http://wap.zdbjq.cn/Article/details/gisuinurn.sHtML

JS:   process.argv.slice(2)
来源：http://3g.fehbvm.com/Article/details/geevmraur.sHtML

TS:   process.argv.slice(2)
来源：http://wap.hesvh.cn/Article/details/gowtnyjqk.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.zdbjq.cn/Article/details/gxretnzrl.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.fehbvm.com/Article/details/gamgmalvy.sHtML

Ruby: ARGV
来源：http://mobile.fehbvm.com/Article/details/gxbmzegsv.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.fehbvm.com/Article/details/gkaepzvxp.sHtML

[M02] 读取环境变量
来源：http://www.share.fehbvm.com/Article/details/grczomwbb.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.zdbjq.cn/Article/details/gqzjtzghk.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.zdbjq.cn/Article/details/gqnqwghkz.sHtML

JS:   process.env.HOME
来源：http://read.share.fehbvm.com/Article/details/gviibspmt.sHtML

TS:   process.env.HOME
来源：http://www.blog.fehbvm.com/Article/details/gkskidilf.sHtML

Java: System.getenv("HOME")
来源：http://read.share.hesvh.cn/Article/details/ggipnyatz.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.fehbvm.com/Article/details/gonwyjwnp.sHtML

Ruby: ENV["HOME"]
来源：http://wap.hesvh.cn/Article/details/gqskmjxcz.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.fehbvm.com/Article/details/gridrgsuu.sHtML

[M03] 执行外部命令
来源：http://read.share.hesvh.cn/Article/details/gtokoordn.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.fehbvm.com/Article/details/gzoduwrbr.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.zdbjq.cn/Article/details/grbqhlmie.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.fehbvm.com/Article/details/gzgrfbeto.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.fehbvm.com/Article/details/gcfbbvpfo.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.hesvh.cn/Article/details/ganqrioky.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.fehbvm.com/Article/details/gkknaqbwj.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.fehbvm.com/Article/details/gqlzvjqwo.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.zdbjq.cn/Article/details/gjgoectcd.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.hesvh.cn/Article/details/glxvasmcr.sHtML

Py:   os.getcwd()
来源：http://blog.zdbjq.cn/Article/details/gebsglask.sHtML

PHP:  getcwd();
来源：http://mobile.fehbvm.com/Article/details/gmthbezbs.sHtML

JS:   process.cwd()
来源：http://wap.fehbvm.com/Article/details/gzjxdxqko.sHtML

TS:   process.cwd()
来源：http://baike.hesvh.cn/Article/details/gqatxqnxf.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.hesvh.cn/Article/details/gaocxrlzi.sHtML

Go:   os.Getwd()
来源：http://blog.zdbjq.cn/Article/details/gmufphwjs.sHtML

Ruby: Dir.pwd
来源：http://m.share.zdbjq.cn/Article/details/gjyelwxsx.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.hesvh.cn/Article/details/ggohpjhfb.sHtML

[M05] 设置退出码
来源：http://mobile.zdbjq.cn/Article/details/gjsrcmncq.sHtML

Py:   sys.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gycqwgbkq.sHtML

PHP:  exit(1);
来源：http://read.share.fehbvm.com/Article/details/gzzfvvxmg.sHtML

JS:   process.exit(1)
来源：http://read.share.fehbvm.com/Article/details/guidtecpw.sHtML

TS:   process.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gytgbasvh.sHtML

Java: System.exit(1)
来源：http://www.share.fehbvm.com/Article/details/grpudetkm.sHtML

Go:   os.Exit(1)
来源：http://www.share.fehbvm.com/Article/details/gmyrsnenk.sHtML

Ruby: exit 1
来源：http://www.blog.fehbvm.com/Article/details/gkdvlciiw.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.hesvh.cn/Article/details/gghijgtnn.sHtML

[M06] 向标准错误输出
来源：http://wap.hesvh.cn/Article/details/gxviahvtm.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.fehbvm.com/Article/details/gvnkubarg.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.fehbvm.com/Article/details/gvjxkqatz.sHtML

JS:   console.error("err")
来源：http://wap.hesvh.cn/Article/details/gxwmtlzjf.sHtML

TS:   console.error("err")
来源：http://baike.fehbvm.com/Article/details/gxuhqvbja.sHtML

Java: System.err.println("err")
来源：http://blog.hesvh.cn/Article/details/gqxyqapjq.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.fehbvm.com/Article/details/glktlmldv.sHtML

Ruby: warn "err"
来源：http://m.share.zdbjq.cn/Article/details/gwabtzssr.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.fehbvm.com/Article/details/gsessoesa.sHtML

[M07] 判断是否为主入口
来源：http://read.share.fehbvm.com/Article/details/ggbkhmdxt.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.fehbvm.com/Article/details/gqyhrxxmr.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.hesvh.cn/Article/details/gzbovcjfi.sHtML

JS:   require.main === module
来源：http://wap.hesvh.cn/Article/details/gufjxvebx.sHtML

TS:   require.main === module
来源：http://www.blog.hesvh.cn/Article/details/gogoxczqo.sHtML

Java: public static void main(String[] args)
来源：http://m.share.hesvh.cn/Article/details/gberufezo.sHtML

Go:   func main()
来源：http://www.m.share.zdbjq.cn/Article/details/gbgjqopou.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.zdbjq.cn/Article/details/gnrviqvzk.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.zdbjq.cn/Article/details/gzbymbqkx.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.zdbjq.cn/Article/details/gfcfstuwo.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.fehbvm.com/Article/details/gddmctruh.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.fehbvm.com/Article/details/gudigschb.sHtML

JS:   process.platform;  process.version
来源：http://blog.hesvh.cn/Article/details/gnqpztuum.sHtML

TS:   process.platform;  process.version
来源：http://wap.hesvh.cn/Article/details/gcccaiyvm.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.zdbjq.cn/Article/details/gipmxldtv.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.zdbjq.cn/Article/details/ghekatjkt.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.zdbjq.cn/Article/details/gbbrlrpgi.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.fehbvm.com/Article/details/gyzfemjyo.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gmylfrdzv.sHtML

N. 数据结构与算法
来源：http://wap.fehbvm.com/Article/details/gudqpczwi.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gzogfqkdl.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.fehbvm.com/Article/details/gegdaazvq.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gcwslcoku.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.fehbvm.com/Article/details/ghskhgrtb.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.zdbjq.cn/Article/details/gexxjrikd.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.zdbjq.cn/Article/details/gsxbpbuai.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gfkumhtex.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gueoyzcdq.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.zdbjq.cn/Article/details/gohqssyho.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gnelwjfny.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.fehbvm.com/Article/details/gorvfqgqz.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.fehbvm.com/Article/details/gsflgrzqc.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.hesvh.cn/Article/details/glfohiwdy.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.zdbjq.cn/Article/details/gntqcahjt.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.hesvh.cn/Article/details/gfkfqjddd.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.zdbjq.cn/Article/details/gcajogdwq.sHtML

Go:   slices.Sort(arr)
来源：http://blog.fehbvm.com/Article/details/geoxazdfj.sHtML

Ruby: arr.sort
来源：http://mobile.zdbjq.cn/Article/details/gortkbvnr.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.fehbvm.com/Article/details/gbfmfhhxs.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.zdbjq.cn/Article/details/gypzknohp.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.hesvh.cn/Article/details/giemrvfwz.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.fehbvm.com/Article/details/gwmrugqrz.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.hesvh.cn/Article/details/gjftpclyf.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.hesvh.cn/Article/details/gwrqhyvje.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.fehbvm.com/Article/details/gvathykvo.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.hesvh.cn/Article/details/gnrbrwizc.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.zdbjq.cn/Article/details/gfkfiwceq.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.fehbvm.com/Article/details/gorwygewv.sHtML

[N04] 斐波那契数列
来源：http://read.share.zdbjq.cn/Article/details/gnrqzeprf.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.zdbjq.cn/Article/details/gwaiuoexk.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.zdbjq.cn/Article/details/gevgyowik.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.zdbjq.cn/Article/details/guartvdju.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/gdzsatijm.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.zdbjq.cn/Article/details/gslxlucrm.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.zdbjq.cn/Article/details/gcptbrilf.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.zdbjq.cn/Article/details/giqeibuee.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.zdbjq.cn/Article/details/guelaasyy.sHtML

[N05] 最大公约数
来源：http://wap.zdbjq.cn/Article/details/grmxdfyuk.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.zdbjq.cn/Article/details/gaedqlqvm.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.hesvh.cn/Article/details/gsljiixcq.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.hesvh.cn/Article/details/gxkvhlarb.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.zdbjq.cn/Article/details/gmvbnlynj.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.fehbvm.com/Article/details/gyxintuhj.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.hesvh.cn/Article/details/guklbpdvu.sHtML

Ruby: a.gcd(b)
来源：http://3g.zdbjq.cn/Article/details/gfiiruhfk.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.zdbjq.cn/Article/details/gpkxrhbgy.sHtML

[N06] 判断回文字符串
来源：http://mobile.fehbvm.com/Article/details/gizcmjzfs.sHtML

Py:   s == s[::-1]
来源：http://www.share.hesvh.cn/Article/details/gngdxhiwt.sHtML

PHP:  $s === strrev($s);
来源：http://3g.hesvh.cn/Article/details/gsworolaz.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/gughdevbm.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/grhbrvrdx.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.fehbvm.com/Article/details/guzadqquc.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.hesvh.cn/Article/details/goqtmypxh.sHtML

Ruby: s == s.reverse
来源：http://www.share.hesvh.cn/Article/details/gjioloxiy.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.zdbjq.cn/Article/details/gmwxtsjbp.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.zdbjq.cn/Article/details/gwiscwbyw.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.zdbjq.cn/Article/details/gitvfjqfy.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.fehbvm.com/Article/details/gcbihmsmi.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.fehbvm.com/Article/details/glpklyhyl.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.fehbvm.com/Article/details/ggvpynrvh.sHtML

Java: // 手写 HashMap
来源：http://blog.zdbjq.cn/Article/details/gbontsncw.sHtML

Go:   // 手写 map[int]int
来源：http://blog.fehbvm.com/Article/details/gaksolbyq.sHtML

Ruby: // 手写 Hash
来源：http://baike.zdbjq.cn/Article/details/gsouqdvdk.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.zdbjq.cn/Article/details/gvodyojib.sHtML

[N08] 生成全排列
来源：http://www.m.share.hesvh.cn/Article/details/gigifqjte.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.zdbjq.cn/Article/details/gurstogrc.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.hesvh.cn/Article/details/gpjdvhmgl.sHtML

JS:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gremecvdq.sHtML

TS:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gtqlcjzli.sHtML

Java: // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gnoenvcpz.sHtML

Go:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/ggobzexab.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.fehbvm.com/Article/details/gtagvqhyf.sHtML

C#:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/goiyugmev.sHtML

[N09] 栈与队列
来源：http://3g.fehbvm.com/Article/details/gcktkfsre.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.hesvh.cn/Article/details/gceamnybp.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.fehbvm.com/Article/details/gudgknnqh.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.zdbjq.cn/Article/details/gcdzhaglp.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.zdbjq.cn/Article/details/gzqpdrjqd.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.hesvh.cn/Article/details/gkkuwjzyo.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.fehbvm.com/Article/details/gfzvsmqyy.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.hesvh.cn/Article/details/gvxdevtet.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.hesvh.cn/Article/details/guxmxuzak.sHtML

[N10] 链表节点定义
来源：http://read.share.hesvh.cn/Article/details/gfwhbdszz.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.fehbvm.com/Article/details/gmqnrdaqn.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.hesvh.cn/Article/details/gaghdjhkn.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.zdbjq.cn/Article/details/gbmpzskcz.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.hesvh.cn/Article/details/gfgqieruu.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.fehbvm.com/Article/details/gqnibmbrg.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.fehbvm.com/Article/details/gcibunztt.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.zdbjq.cn/Article/details/gszjmurjm.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.zdbjq.cn/Article/details/gzsfidsns.sHtML

[N11] 二叉树中序遍历
来源：http://baike.hesvh.cn/Article/details/gitefrddg.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.fehbvm.com/Article/details/gupiatpen.sHtML

PHP:  // 手写递归函数
来源：http://www.share.fehbvm.com/Article/details/gwslgkoig.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.zdbjq.cn/Article/details/gxcgoeahv.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.hesvh.cn/Article/details/gwtlmevbd.sHtML

Java: // 手写递归
来源：http://baike.zdbjq.cn/Article/details/ggkostsry.sHtML

Go:   // 手写递归
来源：http://m.share.fehbvm.com/Article/details/gtwkfjmpt.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.zdbjq.cn/Article/details/gkrgunpme.sHtML

C#:   // 手写递归
来源：http://mobile.zdbjq.cn/Article/details/gfhphisyx.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.fehbvm.com/Article/details/gqfwquepo.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.zdbjq.cn/Article/details/gntnduugb.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.zdbjq.cn/Article/details/gugegmsiz.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.fehbvm.com/Article/details/gemuflyja.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.fehbvm.com/Article/details/gpwancoeq.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.hesvh.cn/Article/details/gzifdylsv.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.hesvh.cn/Article/details/gmqxgnxmn.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.fehbvm.com/Article/details/gralklbtt.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.zdbjq.cn/Article/details/gzjifkcrf.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/ghgnbillj.sHtML

O. 并发与异步
来源：http://www.share.hesvh.cn/Article/details/ggjjiyllq.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gupvwrqdc.sHtML

[O01] 启动一个线程
来源：http://www.m.share.zdbjq.cn/Article/details/gsushhlzq.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.zdbjq.cn/Article/details/glmvnxneb.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.hesvh.cn/Article/details/gocszyjvv.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.hesvh.cn/Article/details/gxwaoxvvo.sHtML

TS:   // 同 JS
来源：http://www.blog.fehbvm.com/Article/details/garhivhde.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.fehbvm.com/Article/details/gpkhalvde.sHtML

Go:   go f()
来源：http://wap.zdbjq.cn/Article/details/guzxjwrmp.sHtML

Ruby: Thread.new { f }
来源：http://www.share.hesvh.cn/Article/details/gqmxqareu.sHtML

C#:   Task.Run(() => F());
来源：http://3g.hesvh.cn/Article/details/gfbmhucsf.sHtML

[O02] 使用线程池
来源：http://wap.fehbvm.com/Article/details/gaalbshwz.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.hesvh.cn/Article/details/gigirtgvi.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.hesvh.cn/Article/details/guohzivfw.sHtML

JS:   // worker_threads 线程池
来源：http://3g.fehbvm.com/Article/details/gnjxjxcfe.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.hesvh.cn/Article/details/gyofiijbu.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.hesvh.cn/Article/details/gbnjryhep.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.hesvh.cn/Article/details/gwqrvpiqs.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.fehbvm.com/Article/details/gzhkoggdd.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.zdbjq.cn/Article/details/gfnltrmij.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.fehbvm.com/Article/details/gikuoplen.sHtML

Py:   with lock: shared += 1
来源：http://blog.fehbvm.com/Article/details/gocpdvtqy.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.hesvh.cn/Article/details/gehlwlslx.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.fehbvm.com/Article/details/govdfcdqg.sHtML

TS:   // 同 JS
来源：http://3g.zdbjq.cn/Article/details/gjeihelja.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.hesvh.cn/Article/details/gvrwuxgps.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.fehbvm.com/Article/details/gqgcirmwa.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.hesvh.cn/Article/details/gcslrzcua.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.hesvh.cn/Article/details/gieycqpbb.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.fehbvm.com/Article/details/gsreuxyla.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.zdbjq.cn/Article/details/gmmsylyfr.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.fehbvm.com/Article/details/gdilkwkeq.sHtML

JS:   async function f() { await g(); }
来源：http://3g.hesvh.cn/Article/details/gcwwwuiob.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.fehbvm.com/Article/details/giszndjdn.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.hesvh.cn/Article/details/gkhonsgbl.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.hesvh.cn/Article/details/gccijckny.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.fehbvm.com/Article/details/gtuefqdrg.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.fehbvm.com/Article/details/grussaopq.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.zdbjq.cn/Article/details/gojgnhryd.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.hesvh.cn/Article/details/geiewcdxi.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.zdbjq.cn/Article/details/gjuzfnqgb.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.hesvh.cn/Article/details/gwjsxkijk.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.hesvh.cn/Article/details/gpwjliszl.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.fehbvm.com/Article/details/gqrspbwap.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.fehbvm.com/Article/details/gzpqdlbaj.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.hesvh.cn/Article/details/gsysatpcz.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.fehbvm.com/Article/details/gvwfryhhu.sHtML

[O06] 使用进程池
来源：http://wap.hesvh.cn/Article/details/gzaggqbva.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.zdbjq.cn/Article/details/gzicwsixm.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.hesvh.cn/Article/details/gqdzgvhkf.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.hesvh.cn/Article/details/gsoxvtbtn.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.fehbvm.com/Article/details/gnlnqjcwt.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.hesvh.cn/Article/details/gvshdvgbl.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.hesvh.cn/Article/details/gazvidjwn.sHtML

Ruby: // fork 块
来源：http://baike.zdbjq.cn/Article/details/gddhqypyb.sHtML

C#:   Parallel.For
来源：http://3g.hesvh.cn/Article/details/gsakxwycp.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/ggglgbven.sHtML

P. 常用工具函数
来源：http://www.m.share.fehbvm.com/Article/details/gfgeqmlbj.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/grfojywbn.sHtML

[P01] 生成 UUID
来源：http://read.share.fehbvm.com/Article/details/gojvivtea.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.hesvh.cn/Article/details/gytjgraus.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.fehbvm.com/Article/details/gcrwlbnwa.sHtML

JS:   crypto.randomUUID()
来源：http://3g.hesvh.cn/Article/details/gdurknahr.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.hesvh.cn/Article/details/grpwwujzh.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.fehbvm.com/Article/details/gpxewfjpx.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.hesvh.cn/Article/details/gxutfujjo.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.fehbvm.com/Article/details/glcexfcpo.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.hesvh.cn/Article/details/gydamvbrr.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.fehbvm.com/Article/details/grafjsaeh.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.zdbjq.cn/Article/details/glpkdtmqn.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.fehbvm.com/Article/details/grxxxsfox.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.fehbvm.com/Article/details/gtlhazdsa.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.zdbjq.cn/Article/details/gmewfhoph.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.hesvh.cn/Article/details/ghequsluk.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.hesvh.cn/Article/details/gdqkxyztx.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.fehbvm.com/Article/details/gmkhqrvwn.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.fehbvm.com/Article/details/gaqhrilnh.sHtML

[P03] 生成短随机字符串
来源：http://m.share.hesvh.cn/Article/details/gopfwgnyf.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.zdbjq.cn/Article/details/gxgxsquue.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.zdbjq.cn/Article/details/gipgauucf.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.fehbvm.com/Article/details/gjporoewj.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.fehbvm.com/Article/details/grirdocie.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.hesvh.cn/Article/details/gsprognlf.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.zdbjq.cn/Article/details/gqqtjjaki.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.zdbjq.cn/Article/details/gyxnoptll.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.fehbvm.com/Article/details/godcdkmyd.sHtML

[P04] 求长度
来源：http://www.m.share.hesvh.cn/Article/details/guoaabbor.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.zdbjq.cn/Article/details/ghqpdxpib.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/gvsndfigz.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.zdbjq.cn/Article/details/gihkzhetf.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.fehbvm.com/Article/details/gfdtphesx.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.hesvh.cn/Article/details/gfbsbcyvf.sHtML

Go:   len(arr);  len(m)
来源：http://wap.zdbjq.cn/Article/details/giiqcegqu.sHtML

Ruby: x.length;  x.size
来源：http://read.share.hesvh.cn/Article/details/gacehfecr.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.hesvh.cn/Article/details/ghpzciids.sHtML


<!-- 参考信息 -->