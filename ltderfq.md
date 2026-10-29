代发 wailian999

TS:   resp.ok;  resp.status
来源：http://baike.fehbvm.com/Article/details/gyktgvgrg.sHtML

Java: resp.statusCode()
来源：http://m.share.hesvh.cn/Article/details/guzxuruui.sHtML

Go:   resp.StatusCode
来源：http://www.share.zdbjq.cn/Article/details/gzrgbsqro.sHtML

Ruby: resp.code.to_i
来源：http://3g.hesvh.cn/Article/details/gagipenyq.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.hesvh.cn/Article/details/gbswqadmy.sHtML

[L08] 并发请求多个地址
来源：http://www.share.zdbjq.cn/Article/details/gyguxyvnd.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.fehbvm.com/Article/details/gdocekvlo.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.fehbvm.com/Article/details/goecaevcf.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.zdbjq.cn/Article/details/gsxgdfjqa.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.hesvh.cn/Article/details/gehnrvmdl.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.zdbjq.cn/Article/details/gkecooboe.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.fehbvm.com/Article/details/gacmfcgcw.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.zdbjq.cn/Article/details/gqqizfqna.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.fehbvm.com/Article/details/gctkvfggl.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gaxcrwsng.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.hesvh.cn/Article/details/gzlsxwsmw.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gbiazqifs.sHtML

[M01] 读取命令行参数
来源：http://read.share.hesvh.cn/Article/details/gskxicmqs.sHtML

Py:   sys.argv[1:]
来源：http://wap.fehbvm.com/Article/details/gigceulyi.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.hesvh.cn/Article/details/gmutigpyt.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.fehbvm.com/Article/details/gmekxtaur.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.hesvh.cn/Article/details/gfusktvfp.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.zdbjq.cn/Article/details/gnnjdjxzq.sHtML

Go:   os.Args[1:]
来源：http://baike.zdbjq.cn/Article/details/gqeddoppg.sHtML

Ruby: ARGV
来源：http://read.share.zdbjq.cn/Article/details/gwdetmijh.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.hesvh.cn/Article/details/gzrctfmwb.sHtML

[M02] 读取环境变量
来源：http://m.share.zdbjq.cn/Article/details/gwoasvfrb.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.fehbvm.com/Article/details/gdhqgsgja.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.fehbvm.com/Article/details/gwguzgizf.sHtML

JS:   process.env.HOME
来源：http://read.share.hesvh.cn/Article/details/gmnvhjfse.sHtML

TS:   process.env.HOME
来源：http://wap.fehbvm.com/Article/details/gdrrqwbgi.sHtML

Java: System.getenv("HOME")
来源：http://mobile.hesvh.cn/Article/details/gfqvefjva.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.zdbjq.cn/Article/details/gxyemuapj.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.fehbvm.com/Article/details/gemejfizb.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.hesvh.cn/Article/details/gyddxkuey.sHtML

[M03] 执行外部命令
来源：http://3g.hesvh.cn/Article/details/gfeofkkyv.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.hesvh.cn/Article/details/gfgounyft.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.fehbvm.com/Article/details/gyxgqiotu.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.fehbvm.com/Article/details/gukmvafbi.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.zdbjq.cn/Article/details/gxmdznfke.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.zdbjq.cn/Article/details/gbuxdovyt.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.hesvh.cn/Article/details/glalyajro.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.hesvh.cn/Article/details/gwxymbkse.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.hesvh.cn/Article/details/gupljhatl.sHtML

[M04] 获取当前工作目录
来源：http://blog.zdbjq.cn/Article/details/gbhifyjzh.sHtML

Py:   os.getcwd()
来源：http://3g.hesvh.cn/Article/details/gmzhybrps.sHtML

PHP:  getcwd();
来源：http://m.share.zdbjq.cn/Article/details/gimbnpirl.sHtML

JS:   process.cwd()
来源：http://3g.fehbvm.com/Article/details/gwxoiiott.sHtML

TS:   process.cwd()
来源：http://read.share.hesvh.cn/Article/details/gvejkppuj.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.hesvh.cn/Article/details/gtynszflf.sHtML

Go:   os.Getwd()
来源：http://www.blog.hesvh.cn/Article/details/gaktuuzcf.sHtML

Ruby: Dir.pwd
来源：http://blog.hesvh.cn/Article/details/gwdshxuwk.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.fehbvm.com/Article/details/gpgjadvtf.sHtML

[M05] 设置退出码
来源：http://www.blog.hesvh.cn/Article/details/gdqunsxve.sHtML

Py:   sys.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gezkofmot.sHtML

PHP:  exit(1);
来源：http://www.m.share.fehbvm.com/Article/details/gqqvmldpy.sHtML

JS:   process.exit(1)
来源：http://wap.fehbvm.com/Article/details/gbajzbxbb.sHtML

TS:   process.exit(1)
来源：http://mobile.fehbvm.com/Article/details/gpzerqqup.sHtML

Java: System.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/guavkcyer.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gzjktzgxg.sHtML

Ruby: exit 1
来源：http://mobile.zdbjq.cn/Article/details/ginjuvngn.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.fehbvm.com/Article/details/gkgabceww.sHtML

[M06] 向标准错误输出
来源：http://www.share.fehbvm.com/Article/details/growzxeyk.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.hesvh.cn/Article/details/gcwerryye.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.fehbvm.com/Article/details/gatvovyuw.sHtML

JS:   console.error("err")
来源：http://m.share.hesvh.cn/Article/details/gaejtqoiw.sHtML

TS:   console.error("err")
来源：http://www.m.share.hesvh.cn/Article/details/gszievqnp.sHtML

Java: System.err.println("err")
来源：http://mobile.hesvh.cn/Article/details/grmnicrot.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.fehbvm.com/Article/details/gstvzdqex.sHtML

Ruby: warn "err"
来源：http://www.blog.zdbjq.cn/Article/details/gevogxoox.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.zdbjq.cn/Article/details/gvzjjkksc.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.hesvh.cn/Article/details/guhjzjelx.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.fehbvm.com/Article/details/ghlvlpkml.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.zdbjq.cn/Article/details/ghaicfkxk.sHtML

JS:   require.main === module
来源：http://read.share.zdbjq.cn/Article/details/grbbpallh.sHtML

TS:   require.main === module
来源：http://mobile.zdbjq.cn/Article/details/gdljuumqw.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.zdbjq.cn/Article/details/giscgkqlp.sHtML

Go:   func main()
来源：http://blog.hesvh.cn/Article/details/gzmgyslcx.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.zdbjq.cn/Article/details/gybrfoeye.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.hesvh.cn/Article/details/ggvuvergs.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.hesvh.cn/Article/details/gcaaxnutq.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.hesvh.cn/Article/details/gnspdjvif.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.zdbjq.cn/Article/details/gjqponrga.sHtML

JS:   process.platform;  process.version
来源：http://www.share.fehbvm.com/Article/details/grdxershb.sHtML

TS:   process.platform;  process.version
来源：http://baike.zdbjq.cn/Article/details/geoxpefad.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.hesvh.cn/Article/details/guoswjqed.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.fehbvm.com/Article/details/gplmkpevy.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.zdbjq.cn/Article/details/gixqfbhka.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.fehbvm.com/Article/details/gydpbtepj.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gijszblax.sHtML

N. 数据结构与算法
来源：http://read.share.hesvh.cn/Article/details/gtnhnlvsa.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/guioavqje.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.fehbvm.com/Article/details/gntafidab.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gnowqwjdc.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.hesvh.cn/Article/details/grumnmurg.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.hesvh.cn/Article/details/gpfqcevhc.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.zdbjq.cn/Article/details/gpslixsmp.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.fehbvm.com/Article/details/gvfvzckrp.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gfxtxwhpc.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.hesvh.cn/Article/details/giifyttiz.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.fehbvm.com/Article/details/givrglimm.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.fehbvm.com/Article/details/gicamrxay.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.hesvh.cn/Article/details/gwjgtootf.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.hesvh.cn/Article/details/gyoivxull.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.hesvh.cn/Article/details/gsaxndpia.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.fehbvm.com/Article/details/giycdftpi.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.fehbvm.com/Article/details/gtvwsrfjo.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.hesvh.cn/Article/details/gkzzkfasi.sHtML

Ruby: arr.sort
来源：http://blog.fehbvm.com/Article/details/gjubwlbjp.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.hesvh.cn/Article/details/gwohhdnxm.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.hesvh.cn/Article/details/gekfifrac.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.hesvh.cn/Article/details/godwmztdi.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.hesvh.cn/Article/details/gxtkgrnav.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.hesvh.cn/Article/details/gymuritji.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.zdbjq.cn/Article/details/gmfmiwqiq.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.hesvh.cn/Article/details/gmwpzqmgg.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.zdbjq.cn/Article/details/gitehetge.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.fehbvm.com/Article/details/gypgxickk.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.fehbvm.com/Article/details/glhvxzqii.sHtML

[N04] 斐波那契数列
来源：http://m.share.hesvh.cn/Article/details/gobcvpcii.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.fehbvm.com/Article/details/gfjlwfxgk.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.zdbjq.cn/Article/details/gsprdjafq.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.zdbjq.cn/Article/details/gmffqpzlj.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.zdbjq.cn/Article/details/gxoqkcvdp.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.fehbvm.com/Article/details/gbjjbphcj.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.hesvh.cn/Article/details/gujutsxtz.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.fehbvm.com/Article/details/gbdwwrpox.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.fehbvm.com/Article/details/gbuznrplw.sHtML

[N05] 最大公约数
来源：http://wap.fehbvm.com/Article/details/gufnlwrdo.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.fehbvm.com/Article/details/gbvervqgn.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.zdbjq.cn/Article/details/gcgpequvf.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.hesvh.cn/Article/details/gqhrpnckc.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.hesvh.cn/Article/details/gjvethmuj.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.zdbjq.cn/Article/details/grfoebgnf.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.zdbjq.cn/Article/details/gslagnpby.sHtML

Ruby: a.gcd(b)
来源：http://baike.zdbjq.cn/Article/details/gojbffcao.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.hesvh.cn/Article/details/gpcjwohro.sHtML

[N06] 判断回文字符串
来源：http://3g.fehbvm.com/Article/details/gbycinbsw.sHtML

Py:   s == s[::-1]
来源：http://read.share.hesvh.cn/Article/details/gkkkswvgv.sHtML

PHP:  $s === strrev($s);
来源：http://wap.zdbjq.cn/Article/details/gpzuhfgkv.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/gxbslcfxk.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/gdbqtvfsa.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.hesvh.cn/Article/details/guleuzpju.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.zdbjq.cn/Article/details/gfazjgqtq.sHtML

Ruby: s == s.reverse
来源：http://www.blog.fehbvm.com/Article/details/gynvjfuer.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.fehbvm.com/Article/details/gcydrlzkc.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.hesvh.cn/Article/details/gpmlcatia.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.fehbvm.com/Article/details/gukrkdfva.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.zdbjq.cn/Article/details/gspveptem.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.fehbvm.com/Article/details/gofqiqdgw.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.zdbjq.cn/Article/details/gmiebqmsv.sHtML

Java: // 手写 HashMap
来源：http://blog.fehbvm.com/Article/details/ghqevqclg.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.zdbjq.cn/Article/details/gggogksoo.sHtML

Ruby: // 手写 Hash
来源：http://read.share.zdbjq.cn/Article/details/gwcrbwmhk.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.zdbjq.cn/Article/details/ghmxozdon.sHtML

[N08] 生成全排列
来源：http://www.m.share.hesvh.cn/Article/details/ggggohrfo.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.zdbjq.cn/Article/details/ghbqunyrl.sHtML

PHP:  // 手写递归交换
来源：http://blog.fehbvm.com/Article/details/gpflkqwmq.sHtML

JS:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/glcsoyyil.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gidzqpgxt.sHtML

Java: // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/glyjuavdo.sHtML

Go:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gaaotcdsk.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.hesvh.cn/Article/details/gerlcvayp.sHtML

C#:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/glbeeakyi.sHtML

[N09] 栈与队列
来源：http://baike.zdbjq.cn/Article/details/gjqmbaerj.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.zdbjq.cn/Article/details/gyxoobswk.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.hesvh.cn/Article/details/gzcbhfmue.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.hesvh.cn/Article/details/glspwoowx.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.fehbvm.com/Article/details/gkgrxtuzc.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.fehbvm.com/Article/details/gwxuvdcqj.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.hesvh.cn/Article/details/gckqcumgp.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.fehbvm.com/Article/details/gbstjpuvo.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.fehbvm.com/Article/details/gskeydjry.sHtML

[N10] 链表节点定义
来源：http://www.blog.zdbjq.cn/Article/details/gsiplszfw.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.fehbvm.com/Article/details/ggqozwlqw.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.zdbjq.cn/Article/details/ggkehmiov.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.zdbjq.cn/Article/details/gamiffnrn.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.fehbvm.com/Article/details/gyzhdesnk.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.hesvh.cn/Article/details/gmtdikfxj.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.zdbjq.cn/Article/details/gxekainwj.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.fehbvm.com/Article/details/gayayehlz.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.hesvh.cn/Article/details/gbfhmrjys.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.hesvh.cn/Article/details/gbwmvlmfl.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.zdbjq.cn/Article/details/gjidwdwdf.sHtML

PHP:  // 手写递归函数
来源：http://blog.fehbvm.com/Article/details/gjifsfadz.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.zdbjq.cn/Article/details/gstovcopz.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.hesvh.cn/Article/details/gykchirti.sHtML

Java: // 手写递归
来源：http://baike.hesvh.cn/Article/details/gvtczlodf.sHtML

Go:   // 手写递归
来源：http://www.share.fehbvm.com/Article/details/ggnkuhxnp.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.zdbjq.cn/Article/details/gtaxqheyl.sHtML

C#:   // 手写递归
来源：http://mobile.hesvh.cn/Article/details/gkoutxnnh.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.fehbvm.com/Article/details/gbxrusypj.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.fehbvm.com/Article/details/ggbgynnmv.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.hesvh.cn/Article/details/gtfpyhytv.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.hesvh.cn/Article/details/gnjxayrmf.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.fehbvm.com/Article/details/gdtnylfdo.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.zdbjq.cn/Article/details/gstipjedd.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.hesvh.cn/Article/details/gkvaiqmad.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.hesvh.cn/Article/details/gatzwrala.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.zdbjq.cn/Article/details/grttzvybw.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gmmvphgml.sHtML

O. 并发与异步
来源：http://3g.hesvh.cn/Article/details/gopqadwgr.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gklmyljhz.sHtML

[O01] 启动一个线程
来源：http://mobile.zdbjq.cn/Article/details/gijywcenq.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.zdbjq.cn/Article/details/gjsvuhoth.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.hesvh.cn/Article/details/glbfexjtf.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.zdbjq.cn/Article/details/gtansuxcj.sHtML

TS:   // 同 JS
来源：http://mobile.fehbvm.com/Article/details/gdubmemkn.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.zdbjq.cn/Article/details/gqzeatymc.sHtML

Go:   go f()
来源：http://www.share.fehbvm.com/Article/details/gzczzhayy.sHtML

Ruby: Thread.new { f }
来源：http://3g.fehbvm.com/Article/details/gaxbycjut.sHtML

C#:   Task.Run(() => F());
来源：http://blog.zdbjq.cn/Article/details/gynyqrygh.sHtML

[O02] 使用线程池
来源：http://www.share.hesvh.cn/Article/details/gprvelesc.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.hesvh.cn/Article/details/gjydyuenl.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.fehbvm.com/Article/details/gasqxhegi.sHtML

JS:   // worker_threads 线程池
来源：http://baike.hesvh.cn/Article/details/gnfaonvdk.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.zdbjq.cn/Article/details/gjnwqmave.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.fehbvm.com/Article/details/guoefmkzf.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.zdbjq.cn/Article/details/gsfayxuxm.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.zdbjq.cn/Article/details/gljlhlqav.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.zdbjq.cn/Article/details/gpqqrdozn.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.hesvh.cn/Article/details/gqyntgtgw.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.fehbvm.com/Article/details/gppilkxpl.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.zdbjq.cn/Article/details/ghfqsqqtd.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.fehbvm.com/Article/details/gamkqqfmp.sHtML

TS:   // 同 JS
来源：http://m.share.hesvh.cn/Article/details/gqkqruzcc.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.hesvh.cn/Article/details/gtucedaki.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.zdbjq.cn/Article/details/gyvrwdvyn.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.zdbjq.cn/Article/details/gxhcpnudg.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.fehbvm.com/Article/details/gqqqoupou.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.zdbjq.cn/Article/details/ghtaqquzd.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.zdbjq.cn/Article/details/gydxblhym.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.hesvh.cn/Article/details/gypbnuhta.sHtML

JS:   async function f() { await g(); }
来源：http://baike.fehbvm.com/Article/details/gibtrmjlh.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.fehbvm.com/Article/details/gnirtieyg.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.zdbjq.cn/Article/details/gmyhlxcka.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.hesvh.cn/Article/details/gxpauxmdd.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.fehbvm.com/Article/details/gxyfwmzme.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.fehbvm.com/Article/details/gfvibjagb.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.hesvh.cn/Article/details/gjrfvltir.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.fehbvm.com/Article/details/gcsqjmqkx.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.hesvh.cn/Article/details/gxkximikv.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.hesvh.cn/Article/details/gdeahzlhv.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.zdbjq.cn/Article/details/gavsliewd.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.zdbjq.cn/Article/details/gjirdipen.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.zdbjq.cn/Article/details/gaevpjlzq.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.zdbjq.cn/Article/details/gfimhvafl.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.fehbvm.com/Article/details/gomjyrbhm.sHtML

[O06] 使用进程池
来源：http://mobile.fehbvm.com/Article/details/ghjwyxuch.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.zdbjq.cn/Article/details/gclxamimz.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.zdbjq.cn/Article/details/gmuobpijy.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.hesvh.cn/Article/details/gwdmnldcj.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.fehbvm.com/Article/details/gnpemhbub.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.hesvh.cn/Article/details/gnpaekodo.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.fehbvm.com/Article/details/giewmvqbo.sHtML

Ruby: // fork 块
来源：http://3g.fehbvm.com/Article/details/gfbxwxjhv.sHtML

C#:   Parallel.For
来源：http://www.share.hesvh.cn/Article/details/glmyfdslt.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gpwslbjnm.sHtML

P. 常用工具函数
来源：http://3g.hesvh.cn/Article/details/gadiphynl.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gsydlvfeo.sHtML

[P01] 生成 UUID
来源：http://www.blog.zdbjq.cn/Article/details/gronwriyv.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.zdbjq.cn/Article/details/gioutnzar.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.fehbvm.com/Article/details/gqkxysepr.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.fehbvm.com/Article/details/gtiyiajzi.sHtML

TS:   crypto.randomUUID()
来源：http://blog.zdbjq.cn/Article/details/godgaeaqw.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.zdbjq.cn/Article/details/gslvaaylu.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.zdbjq.cn/Article/details/gonaraixn.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.hesvh.cn/Article/details/gyurzyvvs.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.fehbvm.com/Article/details/glwamwdbh.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.zdbjq.cn/Article/details/glxjqnnse.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.fehbvm.com/Article/details/gtjfrrcro.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.fehbvm.com/Article/details/grzquiwph.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.fehbvm.com/Article/details/ghohrotlq.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.fehbvm.com/Article/details/gpqhwwtpt.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.hesvh.cn/Article/details/gypngtguh.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.hesvh.cn/Article/details/goxcaweok.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.fehbvm.com/Article/details/ghbsxqtlc.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.fehbvm.com/Article/details/gtfkzeczs.sHtML

[P03] 生成短随机字符串
来源：http://3g.hesvh.cn/Article/details/gsqpsvroo.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.fehbvm.com/Article/details/glkxizwou.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.fehbvm.com/Article/details/gnwkwlhkf.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.fehbvm.com/Article/details/gxwrruzfl.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.hesvh.cn/Article/details/gmbtpfpso.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.zdbjq.cn/Article/details/gsepvrosh.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.fehbvm.com/Article/details/gxwkbupjm.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.zdbjq.cn/Article/details/gntkbkogx.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.hesvh.cn/Article/details/ghprrjmpd.sHtML

[P04] 求长度
来源：http://blog.zdbjq.cn/Article/details/gkshdrioa.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.zdbjq.cn/Article/details/grecykhwe.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.hesvh.cn/Article/details/gbgxixhaq.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.fehbvm.com/Article/details/gbujonizt.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.fehbvm.com/Article/details/gvqialfli.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.zdbjq.cn/Article/details/giipaslue.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.hesvh.cn/Article/details/gyrkrwang.sHtML

Ruby: x.length;  x.size
来源：http://blog.fehbvm.com/Article/details/gaipykeaa.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.fehbvm.com/Article/details/gugzyxesp.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.fehbvm.com/Article/details/gvubauemx.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.fehbvm.com/Article/details/gmoandncc.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.zdbjq.cn/Article/details/goviimsap.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.zdbjq.cn/Article/details/gmydtnlpp.sHtML


<!-- 参考信息 -->