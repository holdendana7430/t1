代发 wailian999

TS:   resp.ok;  resp.status
来源：http://wap.fehbvm.com/Article/details/gomlbvmnj.sHtML

Java: resp.statusCode()
来源：http://www.share.hesvh.cn/Article/details/gcuiepxup.sHtML

Go:   resp.StatusCode
来源：http://blog.fehbvm.com/Article/details/gpnxhiwht.sHtML

Ruby: resp.code.to_i
来源：http://blog.hesvh.cn/Article/details/gtfbuoxqa.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.hesvh.cn/Article/details/ggscyobnf.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.hesvh.cn/Article/details/gdyhggjcu.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.hesvh.cn/Article/details/gfzjpagti.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.hesvh.cn/Article/details/goczfejge.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.hesvh.cn/Article/details/gttqhdmhn.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.hesvh.cn/Article/details/gchpfohhn.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.zdbjq.cn/Article/details/geotreupf.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.zdbjq.cn/Article/details/gvrzsttxs.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.hesvh.cn/Article/details/glmaiagjf.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.hesvh.cn/Article/details/guardabvx.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gbmessjnl.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.zdbjq.cn/Article/details/glmorqehq.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gemczhpwp.sHtML

[M01] 读取命令行参数
来源：http://blog.zdbjq.cn/Article/details/gtmqjadqx.sHtML

Py:   sys.argv[1:]
来源：http://mobile.hesvh.cn/Article/details/gcixibsep.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.hesvh.cn/Article/details/gfvdpbhys.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.zdbjq.cn/Article/details/gsfoosabo.sHtML

TS:   process.argv.slice(2)
来源：http://blog.hesvh.cn/Article/details/ghgiiyxwk.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.fehbvm.com/Article/details/gkgcfsrnh.sHtML

Go:   os.Args[1:]
来源：http://wap.hesvh.cn/Article/details/gbwbycnfy.sHtML

Ruby: ARGV
来源：http://read.share.fehbvm.com/Article/details/ghtdkjsvv.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.fehbvm.com/Article/details/gvcvyuaet.sHtML

[M02] 读取环境变量
来源：http://3g.zdbjq.cn/Article/details/goytzjfgb.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.fehbvm.com/Article/details/gwefremab.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.zdbjq.cn/Article/details/gqxvnweyc.sHtML

JS:   process.env.HOME
来源：http://3g.zdbjq.cn/Article/details/goemszisw.sHtML

TS:   process.env.HOME
来源：http://mobile.zdbjq.cn/Article/details/gtudttepk.sHtML

Java: System.getenv("HOME")
来源：http://www.share.zdbjq.cn/Article/details/gvrljnmng.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.fehbvm.com/Article/details/geutvksvt.sHtML

Ruby: ENV["HOME"]
来源：http://baike.zdbjq.cn/Article/details/gwaqcuxgw.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.fehbvm.com/Article/details/gueddetau.sHtML

[M03] 执行外部命令
来源：http://baike.zdbjq.cn/Article/details/gtyrnfjhj.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.zdbjq.cn/Article/details/gmdhppobz.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.hesvh.cn/Article/details/grpgjmhxo.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.zdbjq.cn/Article/details/gqflerljd.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.fehbvm.com/Article/details/glzjaojvr.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.fehbvm.com/Article/details/gfcumjzjv.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.hesvh.cn/Article/details/gsawleoiz.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.zdbjq.cn/Article/details/gnmxloagv.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.fehbvm.com/Article/details/ggocyfdce.sHtML

[M04] 获取当前工作目录
来源：http://mobile.hesvh.cn/Article/details/ggiloiszb.sHtML

Py:   os.getcwd()
来源：http://blog.zdbjq.cn/Article/details/gdaebdaby.sHtML

PHP:  getcwd();
来源：http://3g.fehbvm.com/Article/details/gkmmjghwa.sHtML

JS:   process.cwd()
来源：http://wap.zdbjq.cn/Article/details/gkotukmem.sHtML

TS:   process.cwd()
来源：http://m.share.fehbvm.com/Article/details/gbuqszrwn.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.fehbvm.com/Article/details/gkbpgbozm.sHtML

Go:   os.Getwd()
来源：http://blog.zdbjq.cn/Article/details/ghgtyxddh.sHtML

Ruby: Dir.pwd
来源：http://wap.zdbjq.cn/Article/details/gugedzxxf.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.zdbjq.cn/Article/details/gtxzndsla.sHtML

[M05] 设置退出码
来源：http://m.share.hesvh.cn/Article/details/gcoecvxex.sHtML

Py:   sys.exit(1)
来源：http://blog.fehbvm.com/Article/details/gqjvmzkuk.sHtML

PHP:  exit(1);
来源：http://read.share.hesvh.cn/Article/details/gmlkvwjdi.sHtML

JS:   process.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gxwlivccy.sHtML

TS:   process.exit(1)
来源：http://baike.fehbvm.com/Article/details/gfoiibcmw.sHtML

Java: System.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gfiosfvdz.sHtML

Go:   os.Exit(1)
来源：http://www.share.hesvh.cn/Article/details/gefgbbccf.sHtML

Ruby: exit 1
来源：http://read.share.hesvh.cn/Article/details/glazdyqmz.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.zdbjq.cn/Article/details/gplbyibpm.sHtML

[M06] 向标准错误输出
来源：http://blog.fehbvm.com/Article/details/gpgmotxrm.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.fehbvm.com/Article/details/gskuebjau.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.zdbjq.cn/Article/details/gcyyhfuqe.sHtML

JS:   console.error("err")
来源：http://www.m.share.hesvh.cn/Article/details/glhxbtrnb.sHtML

TS:   console.error("err")
来源：http://www.share.hesvh.cn/Article/details/gyrbyrkrm.sHtML

Java: System.err.println("err")
来源：http://www.blog.zdbjq.cn/Article/details/ggrizulyq.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.hesvh.cn/Article/details/grzydtjlw.sHtML

Ruby: warn "err"
来源：http://www.m.share.fehbvm.com/Article/details/gwurhvcgv.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.fehbvm.com/Article/details/gcdjgopis.sHtML

[M07] 判断是否为主入口
来源：http://baike.hesvh.cn/Article/details/gufgotcwu.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.fehbvm.com/Article/details/gneopbyjv.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.fehbvm.com/Article/details/gjdmfadpa.sHtML

JS:   require.main === module
来源：http://m.share.zdbjq.cn/Article/details/gdayxqnnf.sHtML

TS:   require.main === module
来源：http://wap.hesvh.cn/Article/details/gfgtfvtwk.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.fehbvm.com/Article/details/gjyjxuxly.sHtML

Go:   func main()
来源：http://m.share.zdbjq.cn/Article/details/gfaupwimt.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.hesvh.cn/Article/details/gyeoslyeb.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.zdbjq.cn/Article/details/gjxjywfle.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.fehbvm.com/Article/details/geejaazzh.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.hesvh.cn/Article/details/gjldsglqw.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.fehbvm.com/Article/details/gnyozpwwo.sHtML

JS:   process.platform;  process.version
来源：http://blog.zdbjq.cn/Article/details/ggbzbnedu.sHtML

TS:   process.platform;  process.version
来源：http://baike.hesvh.cn/Article/details/gcvhfctjz.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.fehbvm.com/Article/details/gcepjymgg.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.hesvh.cn/Article/details/gdwtyrdag.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.fehbvm.com/Article/details/gkfqusqae.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.fehbvm.com/Article/details/gditmkrof.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gqdxcnrql.sHtML

N. 数据结构与算法
来源：http://read.share.hesvh.cn/Article/details/gmajfeilt.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gjfxowywl.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.fehbvm.com/Article/details/gwliuydor.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.hesvh.cn/Article/details/gvsxldnyc.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.hesvh.cn/Article/details/gxvomuryn.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.zdbjq.cn/Article/details/gosgzrmed.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.fehbvm.com/Article/details/gnevzeedk.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.hesvh.cn/Article/details/gbpfddyfn.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/godhecztc.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.hesvh.cn/Article/details/gswjgrrug.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gmufdghry.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.fehbvm.com/Article/details/gywjemews.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.hesvh.cn/Article/details/gmjwarlnw.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.hesvh.cn/Article/details/gbkfqreok.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.hesvh.cn/Article/details/ggeuwicxx.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.hesvh.cn/Article/details/gfiymmtte.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.zdbjq.cn/Article/details/grcpzfceq.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.zdbjq.cn/Article/details/gnkwblfbu.sHtML

Ruby: arr.sort
来源：http://blog.hesvh.cn/Article/details/gsvflxbdo.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.fehbvm.com/Article/details/gcxsabppl.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.fehbvm.com/Article/details/guxosligo.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.hesvh.cn/Article/details/gahhyfgxa.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.hesvh.cn/Article/details/gqtdpkkgp.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.hesvh.cn/Article/details/gnxbucdlo.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.fehbvm.com/Article/details/gdizevazb.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.zdbjq.cn/Article/details/gywaimwed.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.hesvh.cn/Article/details/gocupnfrl.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.zdbjq.cn/Article/details/gchgelvts.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.fehbvm.com/Article/details/gturmmzko.sHtML

[N04] 斐波那契数列
来源：http://wap.hesvh.cn/Article/details/glscwzwwv.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.fehbvm.com/Article/details/gexqnjxhy.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.fehbvm.com/Article/details/gqarmfbuk.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.fehbvm.com/Article/details/guoybkwad.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.fehbvm.com/Article/details/ginvqzoqj.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.fehbvm.com/Article/details/gezzhsjbc.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.hesvh.cn/Article/details/gkmbmemty.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.fehbvm.com/Article/details/gicersigd.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.zdbjq.cn/Article/details/gvxrvnwlx.sHtML

[N05] 最大公约数
来源：http://blog.fehbvm.com/Article/details/gqrcjasvr.sHtML

Py:   math.gcd(a, b)
来源：http://3g.hesvh.cn/Article/details/gtnloezfn.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.fehbvm.com/Article/details/gqpcxsaas.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.fehbvm.com/Article/details/gqqkpfdwn.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.zdbjq.cn/Article/details/gjtffrfsg.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.fehbvm.com/Article/details/gmmtxenmu.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.zdbjq.cn/Article/details/gjguerahc.sHtML

Ruby: a.gcd(b)
来源：http://read.share.hesvh.cn/Article/details/giueyxcws.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.zdbjq.cn/Article/details/gtnhyetjc.sHtML

[N06] 判断回文字符串
来源：http://blog.hesvh.cn/Article/details/gnnaekmsf.sHtML

Py:   s == s[::-1]
来源：http://3g.zdbjq.cn/Article/details/gyhycddmc.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.fehbvm.com/Article/details/gzqyandxu.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.zdbjq.cn/Article/details/gjwcxdrom.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/gpjxocheb.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.fehbvm.com/Article/details/gnltqplap.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.hesvh.cn/Article/details/gpgidgtqb.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.hesvh.cn/Article/details/goxktftec.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.hesvh.cn/Article/details/gmxzmnckr.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.fehbvm.com/Article/details/gtsgceqek.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.fehbvm.com/Article/details/gjthcrpmb.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.fehbvm.com/Article/details/gnmzemcal.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.zdbjq.cn/Article/details/ggeoysqxa.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.hesvh.cn/Article/details/gjkxqllcj.sHtML

Java: // 手写 HashMap
来源：http://wap.hesvh.cn/Article/details/gkicccjeh.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.zdbjq.cn/Article/details/gucgzrini.sHtML

Ruby: // 手写 Hash
来源：http://www.share.fehbvm.com/Article/details/gfdhdkhzg.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.hesvh.cn/Article/details/gkxppsmgh.sHtML

[N08] 生成全排列
来源：http://baike.fehbvm.com/Article/details/gaskivnzl.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.hesvh.cn/Article/details/gkhrvdees.sHtML

PHP:  // 手写递归交换
来源：http://wap.fehbvm.com/Article/details/gglfcgdzs.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/guhausmcc.sHtML

TS:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gdovhqvjy.sHtML

Java: // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gltlfwxnm.sHtML

Go:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gybtedfjp.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.fehbvm.com/Article/details/gckixtjcy.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gkvwpofty.sHtML

[N09] 栈与队列
来源：http://read.share.fehbvm.com/Article/details/gsjhjwzyx.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.hesvh.cn/Article/details/gvwbmmuro.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.zdbjq.cn/Article/details/gujsnazwz.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.fehbvm.com/Article/details/gxagyxetr.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.hesvh.cn/Article/details/gaabzjynb.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.zdbjq.cn/Article/details/gcjlkyxou.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.hesvh.cn/Article/details/gheafteli.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.zdbjq.cn/Article/details/gqpbbjotx.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.fehbvm.com/Article/details/gmflnjdjy.sHtML

[N10] 链表节点定义
来源：http://www.blog.hesvh.cn/Article/details/grohkxshy.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.zdbjq.cn/Article/details/gexvsvqwd.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.hesvh.cn/Article/details/gpvjnpifq.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.zdbjq.cn/Article/details/gqwisytzx.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.zdbjq.cn/Article/details/gggbycibn.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.hesvh.cn/Article/details/gpddhrbzy.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.zdbjq.cn/Article/details/ggoucdhcc.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.zdbjq.cn/Article/details/gxxlolwxo.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.hesvh.cn/Article/details/gyffephsh.sHtML

[N11] 二叉树中序遍历
来源：http://baike.hesvh.cn/Article/details/gqrgezkzi.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.zdbjq.cn/Article/details/gsbhhdjhp.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.zdbjq.cn/Article/details/gzkmfilmu.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.fehbvm.com/Article/details/ghkusqmhm.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.fehbvm.com/Article/details/gnfygrfrs.sHtML

Java: // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/gwwgyttag.sHtML

Go:   // 手写递归
来源：http://wap.hesvh.cn/Article/details/grdtbvlqh.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.zdbjq.cn/Article/details/guffxqmde.sHtML

C#:   // 手写递归
来源：http://m.share.hesvh.cn/Article/details/gknyxpxhr.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.fehbvm.com/Article/details/gvjqkmnlk.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.hesvh.cn/Article/details/grjraedow.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.zdbjq.cn/Article/details/gvbsnmulq.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.fehbvm.com/Article/details/gqyucaqdh.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.fehbvm.com/Article/details/goybiowdt.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.hesvh.cn/Article/details/gpspdpqnt.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.fehbvm.com/Article/details/gnoozzxoi.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.zdbjq.cn/Article/details/gjaztcfxc.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.hesvh.cn/Article/details/gfahxbbge.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gomwqbccp.sHtML

O. 并发与异步
来源：http://wap.zdbjq.cn/Article/details/gmnacnwal.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gezjphety.sHtML

[O01] 启动一个线程
来源：http://blog.zdbjq.cn/Article/details/gjfgogdbs.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.fehbvm.com/Article/details/gfareekys.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.hesvh.cn/Article/details/gitvumhwq.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.fehbvm.com/Article/details/gkstcrtio.sHtML

TS:   // 同 JS
来源：http://baike.fehbvm.com/Article/details/gntwiytrl.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.hesvh.cn/Article/details/gyjcqstva.sHtML

Go:   go f()
来源：http://www.share.fehbvm.com/Article/details/gbwcgnjpt.sHtML

Ruby: Thread.new { f }
来源：http://www.share.zdbjq.cn/Article/details/gysclgeio.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.hesvh.cn/Article/details/gpqmzhzgw.sHtML

[O02] 使用线程池
来源：http://read.share.fehbvm.com/Article/details/gzvazgyfr.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.hesvh.cn/Article/details/gklifuikv.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.fehbvm.com/Article/details/gpozzwelc.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.hesvh.cn/Article/details/ghzegrxyh.sHtML

TS:   // worker_threads 线程池
来源：http://wap.fehbvm.com/Article/details/gvsdwiumy.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.fehbvm.com/Article/details/gizsciwmy.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.zdbjq.cn/Article/details/gktlrnvus.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.zdbjq.cn/Article/details/gfjkfjmai.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.hesvh.cn/Article/details/gqzyjvibx.sHtML

[O03] 加锁保护共享数据
来源：http://baike.hesvh.cn/Article/details/gegdsjotq.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.zdbjq.cn/Article/details/gkwcfwdhx.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.fehbvm.com/Article/details/gnffnjitq.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.hesvh.cn/Article/details/gofxcfbnp.sHtML

TS:   // 同 JS
来源：http://wap.hesvh.cn/Article/details/gfsglqwlh.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.hesvh.cn/Article/details/gzscigiuv.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.fehbvm.com/Article/details/giadhnbnj.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.hesvh.cn/Article/details/gttavhmmb.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.hesvh.cn/Article/details/gzizsutga.sHtML

[O04] 定义异步函数并等待
来源：http://blog.fehbvm.com/Article/details/gzbwjawxc.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.fehbvm.com/Article/details/gtohdcnxy.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.zdbjq.cn/Article/details/garfhzpil.sHtML

JS:   async function f() { await g(); }
来源：http://3g.hesvh.cn/Article/details/gngtudpuq.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.hesvh.cn/Article/details/gjdjykuim.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.fehbvm.com/Article/details/gtzcbvtlp.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.fehbvm.com/Article/details/grjvbqtmc.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.hesvh.cn/Article/details/gtutmilkt.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.zdbjq.cn/Article/details/gtankuvmx.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.fehbvm.com/Article/details/gcoenqlka.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.hesvh.cn/Article/details/gblgznuac.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.hesvh.cn/Article/details/gmkhokkqu.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.fehbvm.com/Article/details/gueqjnrks.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.hesvh.cn/Article/details/grvcmgjfw.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.zdbjq.cn/Article/details/gvsbycnhq.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.hesvh.cn/Article/details/gbfvzrvip.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.zdbjq.cn/Article/details/gapspasii.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.hesvh.cn/Article/details/ghmltdndt.sHtML

[O06] 使用进程池
来源：http://3g.fehbvm.com/Article/details/gshjhxjkz.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.zdbjq.cn/Article/details/gvijsbbvb.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.zdbjq.cn/Article/details/gpexjojgp.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.fehbvm.com/Article/details/gklurabdo.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.hesvh.cn/Article/details/gzhzemqzm.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.fehbvm.com/Article/details/gqvhfgzxy.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.fehbvm.com/Article/details/gvehoagcs.sHtML

Ruby: // fork 块
来源：http://www.blog.zdbjq.cn/Article/details/gfjlqpzhh.sHtML

C#:   Parallel.For
来源：http://www.blog.fehbvm.com/Article/details/gnmrulbsg.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gnlhezssu.sHtML

P. 常用工具函数
来源：http://3g.hesvh.cn/Article/details/gkdpzowil.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gsnjmypck.sHtML

[P01] 生成 UUID
来源：http://wap.hesvh.cn/Article/details/gdxwlllgw.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.zdbjq.cn/Article/details/gtanpypfb.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.fehbvm.com/Article/details/gqehrzecs.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.zdbjq.cn/Article/details/grlghfmjd.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.hesvh.cn/Article/details/gobxwaivd.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.hesvh.cn/Article/details/gjcolizbn.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.zdbjq.cn/Article/details/gfyopylmx.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.fehbvm.com/Article/details/gtrvyhfzb.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.zdbjq.cn/Article/details/gpcpciglb.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.zdbjq.cn/Article/details/gyqhmqzfa.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.hesvh.cn/Article/details/gmvocihgs.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.zdbjq.cn/Article/details/gxkeqilui.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.zdbjq.cn/Article/details/gwdfseevq.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.zdbjq.cn/Article/details/gowbtvuog.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.fehbvm.com/Article/details/gkqmgbyac.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.zdbjq.cn/Article/details/glmwfyjma.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.hesvh.cn/Article/details/gdsejnktd.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.zdbjq.cn/Article/details/gultmlqnv.sHtML

[P03] 生成短随机字符串
来源：http://3g.zdbjq.cn/Article/details/gxwufjbmr.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.hesvh.cn/Article/details/gxeclkttb.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.fehbvm.com/Article/details/gbyrzlitp.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.zdbjq.cn/Article/details/gajyxtqsh.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.zdbjq.cn/Article/details/gucsvnmxh.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.hesvh.cn/Article/details/galynklvg.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.zdbjq.cn/Article/details/gtozkjexf.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.zdbjq.cn/Article/details/goxkbhnvu.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.zdbjq.cn/Article/details/gebuuqjth.sHtML

[P04] 求长度
来源：http://mobile.fehbvm.com/Article/details/giothwclc.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.zdbjq.cn/Article/details/gpjcinzts.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.fehbvm.com/Article/details/guqycysup.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.fehbvm.com/Article/details/gyxtipcqh.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.fehbvm.com/Article/details/gwyptgehx.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.zdbjq.cn/Article/details/gtwsitryk.sHtML

Go:   len(arr);  len(m)
来源：http://blog.hesvh.cn/Article/details/gatfdvqki.sHtML

Ruby: x.length;  x.size
来源：http://wap.zdbjq.cn/Article/details/goqmgsefq.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.hesvh.cn/Article/details/gpfzxkpyi.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.hesvh.cn/Article/details/giilpcjgf.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.fehbvm.com/Article/details/gdylelxue.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.zdbjq.cn/Article/details/gopyblmzd.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.hesvh.cn/Article/details/glrnbxokm.sHtML


<!-- 参考信息 -->