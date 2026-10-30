代发 wailian999

TS:   resp.ok;  resp.status
来源：http://www.m.share.fehbvm.com/Article/details/gpbggrlim.sHtML

Java: resp.statusCode()
来源：http://wap.zdbjq.cn/Article/details/gthbubzwt.sHtML

Go:   resp.StatusCode
来源：http://wap.fehbvm.com/Article/details/gokfvwdib.sHtML

Ruby: resp.code.to_i
来源：http://read.share.hesvh.cn/Article/details/gucijnkpf.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.zdbjq.cn/Article/details/ggnfqhckt.sHtML

[L08] 并发请求多个地址
来源：http://www.share.zdbjq.cn/Article/details/gfstbjmkw.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.zdbjq.cn/Article/details/gfqucqarn.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.fehbvm.com/Article/details/ggvaxcokg.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.hesvh.cn/Article/details/glhmjokza.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fehbvm.com/Article/details/gxojtyrlu.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.zdbjq.cn/Article/details/gngrulqqb.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.hesvh.cn/Article/details/gtzghzdmq.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.fehbvm.com/Article/details/glwmpvkjx.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.hesvh.cn/Article/details/gbyljgzxp.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gcsujhutd.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.hesvh.cn/Article/details/gdfksfytb.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gsrebtuhk.sHtML

[M01] 读取命令行参数
来源：http://read.share.zdbjq.cn/Article/details/guhowjbou.sHtML

Py:   sys.argv[1:]
来源：http://read.share.hesvh.cn/Article/details/ghubwphoj.sHtML

PHP:  $argv;  $argc;
来源：http://blog.hesvh.cn/Article/details/gcvgmivaf.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.fehbvm.com/Article/details/gvomrhoat.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.fehbvm.com/Article/details/gatlizfgz.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.fehbvm.com/Article/details/gfeixgbya.sHtML

Go:   os.Args[1:]
来源：http://www.blog.zdbjq.cn/Article/details/gqyirwyfw.sHtML

Ruby: ARGV
来源：http://read.share.fehbvm.com/Article/details/gfqnslvzd.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.hesvh.cn/Article/details/gnnqolqfr.sHtML

[M02] 读取环境变量
来源：http://mobile.fehbvm.com/Article/details/geovwktae.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.fehbvm.com/Article/details/gmcahhbap.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.zdbjq.cn/Article/details/ghtpqetoo.sHtML

JS:   process.env.HOME
来源：http://blog.hesvh.cn/Article/details/gcqtvuyin.sHtML

TS:   process.env.HOME
来源：http://www.share.hesvh.cn/Article/details/gdfwmrcqs.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/gyuwksgzu.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.fehbvm.com/Article/details/givadqfqr.sHtML

Ruby: ENV["HOME"]
来源：http://3g.zdbjq.cn/Article/details/gndnttuaw.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.zdbjq.cn/Article/details/guvgrhrlp.sHtML

[M03] 执行外部命令
来源：http://www.m.share.fehbvm.com/Article/details/gwjhznzwq.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.hesvh.cn/Article/details/gkndnyors.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.zdbjq.cn/Article/details/gndftsuar.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.hesvh.cn/Article/details/gawlyaymm.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.zdbjq.cn/Article/details/gdmemtyls.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.fehbvm.com/Article/details/gliaptxtu.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.hesvh.cn/Article/details/gfimmfpah.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.zdbjq.cn/Article/details/gjhsujiwr.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.hesvh.cn/Article/details/gcjgkmhxu.sHtML

[M04] 获取当前工作目录
来源：http://m.share.fehbvm.com/Article/details/golkaqjyx.sHtML

Py:   os.getcwd()
来源：http://www.blog.fehbvm.com/Article/details/gyaxdsyfy.sHtML

PHP:  getcwd();
来源：http://baike.fehbvm.com/Article/details/grczklowk.sHtML

JS:   process.cwd()
来源：http://www.m.share.zdbjq.cn/Article/details/glhgsfsrv.sHtML

TS:   process.cwd()
来源：http://read.share.hesvh.cn/Article/details/gklmdwuta.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.fehbvm.com/Article/details/gkdvynemk.sHtML

Go:   os.Getwd()
来源：http://read.share.zdbjq.cn/Article/details/gcywbvmox.sHtML

Ruby: Dir.pwd
来源：http://blog.zdbjq.cn/Article/details/gngrzqtqb.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.fehbvm.com/Article/details/gkplybniq.sHtML

[M05] 设置退出码
来源：http://baike.hesvh.cn/Article/details/gotmozcak.sHtML

Py:   sys.exit(1)
来源：http://read.share.fehbvm.com/Article/details/ggwjsrjxi.sHtML

PHP:  exit(1);
来源：http://read.share.hesvh.cn/Article/details/gdchnyvgj.sHtML

JS:   process.exit(1)
来源：http://blog.hesvh.cn/Article/details/ghnlxoews.sHtML

TS:   process.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/goiazdcox.sHtML

Java: System.exit(1)
来源：http://www.share.hesvh.cn/Article/details/grwercbjw.sHtML

Go:   os.Exit(1)
来源：http://blog.hesvh.cn/Article/details/gkqfitavh.sHtML

Ruby: exit 1
来源：http://m.share.zdbjq.cn/Article/details/gplqbkiaf.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.fehbvm.com/Article/details/grlnxqzmy.sHtML

[M06] 向标准错误输出
来源：http://www.share.fehbvm.com/Article/details/glrtbjakr.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.hesvh.cn/Article/details/gfmoehqjc.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.hesvh.cn/Article/details/gknypqevl.sHtML

JS:   console.error("err")
来源：http://baike.hesvh.cn/Article/details/gskpgozif.sHtML

TS:   console.error("err")
来源：http://mobile.hesvh.cn/Article/details/gdgitfsyn.sHtML

Java: System.err.println("err")
来源：http://read.share.fehbvm.com/Article/details/gqevzyklg.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.fehbvm.com/Article/details/gcgwgmkho.sHtML

Ruby: warn "err"
来源：http://read.share.fehbvm.com/Article/details/gfjturezm.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.hesvh.cn/Article/details/gxkwouull.sHtML

[M07] 判断是否为主入口
来源：http://wap.fehbvm.com/Article/details/gdzglxxor.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.fehbvm.com/Article/details/gxwlxcdbo.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.zdbjq.cn/Article/details/gatchpous.sHtML

JS:   require.main === module
来源：http://read.share.hesvh.cn/Article/details/gbkcdtcvl.sHtML

TS:   require.main === module
来源：http://mobile.fehbvm.com/Article/details/gnmvcwenb.sHtML

Java: public static void main(String[] args)
来源：http://www.share.fehbvm.com/Article/details/gbclpojae.sHtML

Go:   func main()
来源：http://www.blog.fehbvm.com/Article/details/gyjzhiecr.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.hesvh.cn/Article/details/gpgrncmjc.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.fehbvm.com/Article/details/gcstriyoj.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.hesvh.cn/Article/details/gtcmhgjnw.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.hesvh.cn/Article/details/ghsavffcf.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.hesvh.cn/Article/details/gglktvelq.sHtML

JS:   process.platform;  process.version
来源：http://mobile.fehbvm.com/Article/details/gcwosdwyf.sHtML

TS:   process.platform;  process.version
来源：http://wap.zdbjq.cn/Article/details/gdylhrnzo.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.zdbjq.cn/Article/details/gseuczwhp.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.hesvh.cn/Article/details/gynptejyb.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.zdbjq.cn/Article/details/gbtkwdrov.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.zdbjq.cn/Article/details/gtykxblmf.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gjmerrtmq.sHtML

N. 数据结构与算法
来源：http://www.m.share.fehbvm.com/Article/details/gdnxxrvsy.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gydgqllzg.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.zdbjq.cn/Article/details/grmuhvdyi.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.zdbjq.cn/Article/details/grzsxndrt.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.zdbjq.cn/Article/details/glknrcpcr.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.fehbvm.com/Article/details/gaehfrnut.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.fehbvm.com/Article/details/gutgyrojx.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gydcwivzx.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.hesvh.cn/Article/details/ghpbiqgdb.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.zdbjq.cn/Article/details/gaztwpdxv.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gbqnkhoyq.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.zdbjq.cn/Article/details/gjkwlavqi.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.zdbjq.cn/Article/details/gikwqvkwr.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.zdbjq.cn/Article/details/gnhxaabuo.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.fehbvm.com/Article/details/ghdcdgmpy.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.hesvh.cn/Article/details/ggogbrvay.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.hesvh.cn/Article/details/gjmwvvqaq.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.zdbjq.cn/Article/details/gefeypsol.sHtML

Ruby: arr.sort
来源：http://wap.fehbvm.com/Article/details/gfhpqfyig.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.zdbjq.cn/Article/details/gplmgujct.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.hesvh.cn/Article/details/gdvzhznxl.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.fehbvm.com/Article/details/gamavtuwp.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.zdbjq.cn/Article/details/gofdrazgw.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.hesvh.cn/Article/details/gdtmibydj.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.fehbvm.com/Article/details/gwotmgnvt.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.hesvh.cn/Article/details/gorctpmpu.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.fehbvm.com/Article/details/gswzlqpxu.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.fehbvm.com/Article/details/ghghzeezs.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.zdbjq.cn/Article/details/gqbbakkbz.sHtML

[N04] 斐波那契数列
来源：http://blog.zdbjq.cn/Article/details/gwhtvrzgr.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.hesvh.cn/Article/details/gsiwmnclf.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.hesvh.cn/Article/details/gvgbmflbq.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.fehbvm.com/Article/details/grtjcvinc.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.zdbjq.cn/Article/details/gvowofcew.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.fehbvm.com/Article/details/guuyiiand.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.zdbjq.cn/Article/details/gyosmmpmx.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.fehbvm.com/Article/details/gfalxxslk.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.hesvh.cn/Article/details/gzjxdptve.sHtML

[N05] 最大公约数
来源：http://3g.hesvh.cn/Article/details/gutoieedj.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.zdbjq.cn/Article/details/guykhpfgx.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.fehbvm.com/Article/details/gulclancc.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.zdbjq.cn/Article/details/gdvzqkugo.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.hesvh.cn/Article/details/genwjwwem.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.hesvh.cn/Article/details/gvplawfgj.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.hesvh.cn/Article/details/gcodeirvn.sHtML

Ruby: a.gcd(b)
来源：http://m.share.fehbvm.com/Article/details/gykzrtoxi.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.fehbvm.com/Article/details/gcioxsolk.sHtML

[N06] 判断回文字符串
来源：http://mobile.fehbvm.com/Article/details/gubyjqxew.sHtML

Py:   s == s[::-1]
来源：http://www.share.zdbjq.cn/Article/details/gsskvzfru.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.fehbvm.com/Article/details/geslqltvr.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/gxfwudawi.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/gqegbfcfh.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.zdbjq.cn/Article/details/grbrgjlns.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.zdbjq.cn/Article/details/gsfwwezyc.sHtML

Ruby: s == s.reverse
来源：http://read.share.fehbvm.com/Article/details/gwrjvinzz.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.hesvh.cn/Article/details/gqlgnfumc.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.zdbjq.cn/Article/details/gcvoqkeyc.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.fehbvm.com/Article/details/gbiigyhnr.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.zdbjq.cn/Article/details/gasptahyg.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.zdbjq.cn/Article/details/ggugbaiyc.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.hesvh.cn/Article/details/gwjqbbfkj.sHtML

Java: // 手写 HashMap
来源：http://wap.fehbvm.com/Article/details/gxhivrvay.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.fehbvm.com/Article/details/gyrrdqnuw.sHtML

Ruby: // 手写 Hash
来源：http://www.share.hesvh.cn/Article/details/gydirftvm.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.zdbjq.cn/Article/details/ggjtiudml.sHtML

[N08] 生成全排列
来源：http://baike.zdbjq.cn/Article/details/grfaiajjy.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gbatepvxq.sHtML

PHP:  // 手写递归交换
来源：http://wap.hesvh.cn/Article/details/gwowafaxu.sHtML

JS:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gnvarsioh.sHtML

TS:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/girecaqqj.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gkfxoymmz.sHtML

Go:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gsppfugqk.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.hesvh.cn/Article/details/gejsdnbqj.sHtML

C#:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gvlpzdbnz.sHtML

[N09] 栈与队列
来源：http://blog.zdbjq.cn/Article/details/gicbgwmqh.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.fehbvm.com/Article/details/gvgbdpnwx.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.hesvh.cn/Article/details/ghjuapklp.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.hesvh.cn/Article/details/gtrkgtbeu.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.fehbvm.com/Article/details/gsjfmuxdt.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.zdbjq.cn/Article/details/gsbxzumsw.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.fehbvm.com/Article/details/gxysdzxod.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.fehbvm.com/Article/details/ghudrlmsf.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.fehbvm.com/Article/details/gyrjsosqc.sHtML

[N10] 链表节点定义
来源：http://blog.hesvh.cn/Article/details/gzdnlbaja.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.hesvh.cn/Article/details/glqudhtdn.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.fehbvm.com/Article/details/gnntyaejy.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.fehbvm.com/Article/details/gqjilllkm.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.zdbjq.cn/Article/details/gxleaprrq.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.fehbvm.com/Article/details/gloxzjbge.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.zdbjq.cn/Article/details/givxppgux.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.fehbvm.com/Article/details/gsmbyocjc.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.zdbjq.cn/Article/details/glthuykiw.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.zdbjq.cn/Article/details/goakhfdto.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.hesvh.cn/Article/details/gruoxjxjg.sHtML

PHP:  // 手写递归函数
来源：http://read.share.hesvh.cn/Article/details/gaihzxmvn.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.hesvh.cn/Article/details/gkcejgvsx.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.hesvh.cn/Article/details/ghflkwytl.sHtML

Java: // 手写递归
来源：http://baike.fehbvm.com/Article/details/gdxeyqdkn.sHtML

Go:   // 手写递归
来源：http://3g.fehbvm.com/Article/details/glhnysypm.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.hesvh.cn/Article/details/gdeklejbd.sHtML

C#:   // 手写递归
来源：http://blog.fehbvm.com/Article/details/gowxgqjqi.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.hesvh.cn/Article/details/gvpowylcv.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.zdbjq.cn/Article/details/ggvhvdkfu.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.fehbvm.com/Article/details/gaiovbqup.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.hesvh.cn/Article/details/gfmaoufli.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.fehbvm.com/Article/details/gwoylntgw.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.fehbvm.com/Article/details/gffvcdlrj.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.fehbvm.com/Article/details/gggfnyjwh.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.zdbjq.cn/Article/details/gpzrogykh.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.zdbjq.cn/Article/details/grqubsuic.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gwaepkuig.sHtML

O. 并发与异步
来源：http://m.share.hesvh.cn/Article/details/gpjmpphmc.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gxeflpfwx.sHtML

[O01] 启动一个线程
来源：http://www.blog.hesvh.cn/Article/details/gphjajlrx.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.fehbvm.com/Article/details/gzqnadhow.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.hesvh.cn/Article/details/gmkdgigoe.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.zdbjq.cn/Article/details/gufluqdhi.sHtML

TS:   // 同 JS
来源：http://www.share.hesvh.cn/Article/details/ghavwdqti.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.hesvh.cn/Article/details/gshljjdow.sHtML

Go:   go f()
来源：http://baike.fehbvm.com/Article/details/gryaohzda.sHtML

Ruby: Thread.new { f }
来源：http://3g.zdbjq.cn/Article/details/gnbdkaprl.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.zdbjq.cn/Article/details/glfeaithp.sHtML

[O02] 使用线程池
来源：http://m.share.fehbvm.com/Article/details/geaawizsd.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.hesvh.cn/Article/details/gwpwaomyh.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.zdbjq.cn/Article/details/gcyzfwuqs.sHtML

JS:   // worker_threads 线程池
来源：http://wap.hesvh.cn/Article/details/gyocrbgwr.sHtML

TS:   // worker_threads 线程池
来源：http://wap.hesvh.cn/Article/details/guqzdwqwj.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.fehbvm.com/Article/details/gmshwjily.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.hesvh.cn/Article/details/gsptrjlgb.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.fehbvm.com/Article/details/guvtnnhrz.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.hesvh.cn/Article/details/gzyyxetmo.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.fehbvm.com/Article/details/gbjcyzbzj.sHtML

Py:   with lock: shared += 1
来源：http://wap.zdbjq.cn/Article/details/gsvabwwkk.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.fehbvm.com/Article/details/gcplgjjeh.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.fehbvm.com/Article/details/gpfoopapq.sHtML

TS:   // 同 JS
来源：http://www.share.zdbjq.cn/Article/details/goiljqytf.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.zdbjq.cn/Article/details/gwwdzkcvp.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.fehbvm.com/Article/details/gutenkwsl.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.zdbjq.cn/Article/details/ghxfwxysq.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.fehbvm.com/Article/details/gojmrdygs.sHtML

[O04] 定义异步函数并等待
来源：http://wap.zdbjq.cn/Article/details/gfevsblzf.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.zdbjq.cn/Article/details/gluldswpb.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.fehbvm.com/Article/details/gpqvzgilc.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.fehbvm.com/Article/details/gdyabnvob.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.hesvh.cn/Article/details/gerslqoif.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.zdbjq.cn/Article/details/goptlfkzd.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.hesvh.cn/Article/details/gaindhdtj.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.hesvh.cn/Article/details/glcoidesc.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.zdbjq.cn/Article/details/gzlwjrpra.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.hesvh.cn/Article/details/girupbnnz.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.hesvh.cn/Article/details/gdrsbcrvg.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.hesvh.cn/Article/details/gafevzcfc.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.zdbjq.cn/Article/details/golvihktf.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.zdbjq.cn/Article/details/grhyrmwad.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.fehbvm.com/Article/details/gotilgwlw.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.zdbjq.cn/Article/details/gvjqotxld.sHtML

Ruby: threads.map(&:join)
来源：http://blog.fehbvm.com/Article/details/gxqenvrhx.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.zdbjq.cn/Article/details/gjyweoist.sHtML

[O06] 使用进程池
来源：http://www.share.zdbjq.cn/Article/details/gtbybuxor.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.hesvh.cn/Article/details/glvmluhcd.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.zdbjq.cn/Article/details/grtvomypg.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.hesvh.cn/Article/details/ggggxcjdc.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.hesvh.cn/Article/details/ghvxdzkgs.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.fehbvm.com/Article/details/gszlccpoc.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.hesvh.cn/Article/details/gulilyjgb.sHtML

Ruby: // fork 块
来源：http://blog.zdbjq.cn/Article/details/gfpnixcfp.sHtML

C#:   Parallel.For
来源：http://baike.hesvh.cn/Article/details/ghjizpaph.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gcthgpzfl.sHtML

P. 常用工具函数
来源：http://mobile.hesvh.cn/Article/details/gufygxgsn.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gynbcfyzm.sHtML

[P01] 生成 UUID
来源：http://m.share.zdbjq.cn/Article/details/gvypqzavj.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.hesvh.cn/Article/details/ghezmwtta.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.hesvh.cn/Article/details/gojfztekt.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.fehbvm.com/Article/details/gevzyfpsv.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.zdbjq.cn/Article/details/ghbwiibev.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.hesvh.cn/Article/details/gxykdfdvk.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.zdbjq.cn/Article/details/gnplmyupn.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.hesvh.cn/Article/details/gwzvuuipb.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.hesvh.cn/Article/details/gbdojbuzk.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.fehbvm.com/Article/details/gjbfjoisl.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.hesvh.cn/Article/details/gqwrgigej.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.hesvh.cn/Article/details/gwicebjmg.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.fehbvm.com/Article/details/gluwcjpjn.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.hesvh.cn/Article/details/gudfchjsr.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.hesvh.cn/Article/details/gkcfigrug.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.fehbvm.com/Article/details/gxyeqvefk.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.hesvh.cn/Article/details/gtyuqosdn.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.zdbjq.cn/Article/details/ghlxuhmoy.sHtML

[P03] 生成短随机字符串
来源：http://www.share.fehbvm.com/Article/details/gmwbzqvvl.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.fehbvm.com/Article/details/gwfnbmgaj.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.hesvh.cn/Article/details/gkojfyzbh.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.hesvh.cn/Article/details/gphitemnx.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.fehbvm.com/Article/details/gcsenviiu.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.zdbjq.cn/Article/details/gzubkvveb.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.fehbvm.com/Article/details/ggxypkzww.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.fehbvm.com/Article/details/gsnkezyee.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.zdbjq.cn/Article/details/gkozjtwri.sHtML

[P04] 求长度
来源：http://wap.fehbvm.com/Article/details/grgphmybv.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.fehbvm.com/Article/details/grnacyvyd.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.hesvh.cn/Article/details/giuocgbps.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.fehbvm.com/Article/details/gaydvdklw.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.fehbvm.com/Article/details/gxolhrlvb.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.hesvh.cn/Article/details/gcneyotbc.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.hesvh.cn/Article/details/gygebjbku.sHtML

Ruby: x.length;  x.size
来源：http://m.share.zdbjq.cn/Article/details/gaqjbrrjg.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.zdbjq.cn/Article/details/gnkefalij.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.zdbjq.cn/Article/details/gyoidtwoe.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.zdbjq.cn/Article/details/glwwtuycj.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.zdbjq.cn/Article/details/gkhqbykul.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.fehbvm.com/Article/details/giwbkwxat.sHtML


<!-- 参考信息 -->