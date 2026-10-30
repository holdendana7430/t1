代发 wailian999

TS:   resp.ok;  resp.status
来源：http://mobile.fehbvm.com/Article/details/gzqinslbg.sHtML

Java: resp.statusCode()
来源：http://m.share.zdbjq.cn/Article/details/gteftgtai.sHtML

Go:   resp.StatusCode
来源：http://3g.zdbjq.cn/Article/details/gwdklcfhl.sHtML

Ruby: resp.code.to_i
来源：http://read.share.fehbvm.com/Article/details/gtpzzgejb.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.hesvh.cn/Article/details/gotuzgnho.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.zdbjq.cn/Article/details/gdpoggjvz.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.fehbvm.com/Article/details/gudtvwlrx.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.zdbjq.cn/Article/details/gbqcftijx.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.zdbjq.cn/Article/details/goslnwqla.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.zdbjq.cn/Article/details/gcdesmpwy.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.hesvh.cn/Article/details/glynpqrvg.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.zdbjq.cn/Article/details/gfvacwzll.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.fehbvm.com/Article/details/ghemesmyd.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.zdbjq.cn/Article/details/gjrxgkxxu.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gqeekccet.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.fehbvm.com/Article/details/gkuyqorur.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gmtqllkvv.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.hesvh.cn/Article/details/gzfnxfimd.sHtML

Py:   sys.argv[1:]
来源：http://blog.zdbjq.cn/Article/details/graodfker.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.hesvh.cn/Article/details/gbkgxzkej.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.zdbjq.cn/Article/details/gcfclwsoh.sHtML

TS:   process.argv.slice(2)
来源：http://baike.hesvh.cn/Article/details/gikgduonu.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.zdbjq.cn/Article/details/gpdosstep.sHtML

Go:   os.Args[1:]
来源：http://mobile.zdbjq.cn/Article/details/gcyutrksu.sHtML

Ruby: ARGV
来源：http://read.share.hesvh.cn/Article/details/gaslvqflh.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.hesvh.cn/Article/details/gdmgmrcoh.sHtML

[M02] 读取环境变量
来源：http://read.share.fehbvm.com/Article/details/giadszkyw.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.hesvh.cn/Article/details/gxtgtutip.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.zdbjq.cn/Article/details/gqqiextwn.sHtML

JS:   process.env.HOME
来源：http://m.share.hesvh.cn/Article/details/grdnodobn.sHtML

TS:   process.env.HOME
来源：http://blog.hesvh.cn/Article/details/gnzhawvtx.sHtML

Java: System.getenv("HOME")
来源：http://3g.fehbvm.com/Article/details/giyiukyuo.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/gagzncepq.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.fehbvm.com/Article/details/grkaebmzq.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.fehbvm.com/Article/details/gltvqtklo.sHtML

[M03] 执行外部命令
来源：http://www.share.fehbvm.com/Article/details/gdlhcepvy.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.fehbvm.com/Article/details/gfdfjimax.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.hesvh.cn/Article/details/gvaqjbtam.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.fehbvm.com/Article/details/gghwchiva.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.fehbvm.com/Article/details/gjaqdhtdi.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.zdbjq.cn/Article/details/gbgjrfyxe.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.hesvh.cn/Article/details/gcdbwptqf.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.zdbjq.cn/Article/details/gvuujinjf.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.zdbjq.cn/Article/details/glilfgzql.sHtML

[M04] 获取当前工作目录
来源：http://read.share.fehbvm.com/Article/details/gsffkjtky.sHtML

Py:   os.getcwd()
来源：http://mobile.zdbjq.cn/Article/details/gppyiucdd.sHtML

PHP:  getcwd();
来源：http://m.share.hesvh.cn/Article/details/gpmjwhyea.sHtML

JS:   process.cwd()
来源：http://www.m.share.hesvh.cn/Article/details/gvezozlcl.sHtML

TS:   process.cwd()
来源：http://wap.fehbvm.com/Article/details/gygvwwjfh.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.fehbvm.com/Article/details/grelezhyv.sHtML

Go:   os.Getwd()
来源：http://baike.hesvh.cn/Article/details/gcikhvfeb.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.hesvh.cn/Article/details/gmcshibxe.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.zdbjq.cn/Article/details/gtpjyebya.sHtML

[M05] 设置退出码
来源：http://m.share.fehbvm.com/Article/details/gecqmrotm.sHtML

Py:   sys.exit(1)
来源：http://baike.fehbvm.com/Article/details/gmbbldpfv.sHtML

PHP:  exit(1);
来源：http://m.share.hesvh.cn/Article/details/gaekuosxl.sHtML

JS:   process.exit(1)
来源：http://mobile.hesvh.cn/Article/details/glzkxuhuw.sHtML

TS:   process.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gjfhrlgnj.sHtML

Java: System.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gvcdhdtcz.sHtML

Go:   os.Exit(1)
来源：http://3g.hesvh.cn/Article/details/gepdxxtqt.sHtML

Ruby: exit 1
来源：http://mobile.zdbjq.cn/Article/details/guzluayaf.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.fehbvm.com/Article/details/gjrublfyk.sHtML

[M06] 向标准错误输出
来源：http://www.share.fehbvm.com/Article/details/gcpzhsggz.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.hesvh.cn/Article/details/gxnxfvuon.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.zdbjq.cn/Article/details/gqqnbgodx.sHtML

JS:   console.error("err")
来源：http://baike.zdbjq.cn/Article/details/gcczcsltg.sHtML

TS:   console.error("err")
来源：http://blog.zdbjq.cn/Article/details/gmimbtdkq.sHtML

Java: System.err.println("err")
来源：http://read.share.zdbjq.cn/Article/details/gcehxyhzt.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.fehbvm.com/Article/details/gmrvbwqyd.sHtML

Ruby: warn "err"
来源：http://wap.hesvh.cn/Article/details/gbxpimvtd.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.hesvh.cn/Article/details/gzitcpahc.sHtML

[M07] 判断是否为主入口
来源：http://read.share.fehbvm.com/Article/details/gynzjfjhb.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.zdbjq.cn/Article/details/gejemkohc.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.hesvh.cn/Article/details/gzahtogpj.sHtML

JS:   require.main === module
来源：http://baike.zdbjq.cn/Article/details/gzhsygjez.sHtML

TS:   require.main === module
来源：http://m.share.hesvh.cn/Article/details/glgsknoef.sHtML

Java: public static void main(String[] args)
来源：http://www.share.hesvh.cn/Article/details/gghwjczmm.sHtML

Go:   func main()
来源：http://mobile.fehbvm.com/Article/details/gnrnhtxqc.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.zdbjq.cn/Article/details/gpnlhvhgr.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.fehbvm.com/Article/details/ggmlrdiky.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.fehbvm.com/Article/details/ggkoveftf.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.fehbvm.com/Article/details/gjtmsyofu.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.zdbjq.cn/Article/details/grlndcngz.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.zdbjq.cn/Article/details/gvkybozrr.sHtML

TS:   process.platform;  process.version
来源：http://m.share.zdbjq.cn/Article/details/gibwsyowk.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.zdbjq.cn/Article/details/gwyrhddoi.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.hesvh.cn/Article/details/goujrjpqv.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.fehbvm.com/Article/details/gsatognwg.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.zdbjq.cn/Article/details/gvnpklozl.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gziclcaxc.sHtML

N. 数据结构与算法
来源：http://www.blog.fehbvm.com/Article/details/gfyxgossi.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gawhufaxm.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.fehbvm.com/Article/details/gwsqwovcq.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.fehbvm.com/Article/details/ggebcwjyk.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.zdbjq.cn/Article/details/gmtpksjwj.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.fehbvm.com/Article/details/gzhrenzyl.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.fehbvm.com/Article/details/gyymivkbo.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/goverfgdk.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gdyvyfwut.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.zdbjq.cn/Article/details/ggsynzssb.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gwfjuiecy.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.hesvh.cn/Article/details/gknprajxz.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.hesvh.cn/Article/details/gjkfjkeqv.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.fehbvm.com/Article/details/ghitdregf.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.fehbvm.com/Article/details/gudfwsurs.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.zdbjq.cn/Article/details/genkqitpw.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.fehbvm.com/Article/details/glhhwriwo.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.hesvh.cn/Article/details/gvegpxokp.sHtML

Ruby: arr.sort
来源：http://3g.fehbvm.com/Article/details/grubrdwmr.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.zdbjq.cn/Article/details/ghfkiwmsn.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.hesvh.cn/Article/details/gvavooxlv.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.fehbvm.com/Article/details/gwnuuwyvo.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.zdbjq.cn/Article/details/gvnzoiqdq.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.zdbjq.cn/Article/details/gfbcomqrx.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.zdbjq.cn/Article/details/gxngjrola.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.hesvh.cn/Article/details/gjomngnop.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.zdbjq.cn/Article/details/gsbumyzye.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.fehbvm.com/Article/details/grdggmzhy.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.zdbjq.cn/Article/details/gvlrwybkm.sHtML

[N04] 斐波那契数列
来源：http://read.share.fehbvm.com/Article/details/gljxtdzpl.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.zdbjq.cn/Article/details/grsklznpp.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.fehbvm.com/Article/details/gzrzmcjgg.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.hesvh.cn/Article/details/gytqakyqq.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/gstvyinxn.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.fehbvm.com/Article/details/ggnksfgqw.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.zdbjq.cn/Article/details/gvwpfffzk.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.zdbjq.cn/Article/details/gchitdqqc.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.hesvh.cn/Article/details/gqpgvhhrl.sHtML

[N05] 最大公约数
来源：http://read.share.zdbjq.cn/Article/details/gmzjqtnux.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.hesvh.cn/Article/details/gytdzwjzz.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.fehbvm.com/Article/details/gbdwigbww.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.hesvh.cn/Article/details/gjfqaapky.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.hesvh.cn/Article/details/gqpmejlii.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.hesvh.cn/Article/details/grbsuzmkv.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.zdbjq.cn/Article/details/gcuhxgfqt.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.fehbvm.com/Article/details/glmyyuboi.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.fehbvm.com/Article/details/gilgnjrlv.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.zdbjq.cn/Article/details/ggwadkrtv.sHtML

Py:   s == s[::-1]
来源：http://www.blog.zdbjq.cn/Article/details/gmtzmwkoe.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.zdbjq.cn/Article/details/gvdxdoocz.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/gmaroomxg.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/gnnpzunqy.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.fehbvm.com/Article/details/gncrjngal.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.zdbjq.cn/Article/details/ggcugfwll.sHtML

Ruby: s == s.reverse
来源：http://read.share.hesvh.cn/Article/details/gljeejogx.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.hesvh.cn/Article/details/gtrwwadcy.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.zdbjq.cn/Article/details/gjjypayaq.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.fehbvm.com/Article/details/gwiqvmwla.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.hesvh.cn/Article/details/gvugahasg.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.hesvh.cn/Article/details/ghlbbofvf.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.zdbjq.cn/Article/details/goijztebg.sHtML

Java: // 手写 HashMap
来源：http://www.blog.fehbvm.com/Article/details/glndrohcz.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.zdbjq.cn/Article/details/gmapekthq.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.zdbjq.cn/Article/details/gncktayim.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.hesvh.cn/Article/details/gqkolkweo.sHtML

[N08] 生成全排列
来源：http://www.share.zdbjq.cn/Article/details/gqgwjymit.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.fehbvm.com/Article/details/gksaqwiff.sHtML

PHP:  // 手写递归交换
来源：http://3g.hesvh.cn/Article/details/gqhutccok.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gmqpgukbq.sHtML

TS:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gvquijfwq.sHtML

Java: // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/glchnckqp.sHtML

Go:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gpadtgqkg.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.zdbjq.cn/Article/details/gxqrfcaxk.sHtML

C#:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gnaaqdudz.sHtML

[N09] 栈与队列
来源：http://read.share.hesvh.cn/Article/details/gfmsdfckt.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.zdbjq.cn/Article/details/gevfkcazl.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.zdbjq.cn/Article/details/gygwhnbfr.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.hesvh.cn/Article/details/gtrkggwnq.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.hesvh.cn/Article/details/gkjjbqkxn.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.fehbvm.com/Article/details/gtfzzrzdj.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.zdbjq.cn/Article/details/gcqfuztdf.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.zdbjq.cn/Article/details/ghbbqppmp.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.zdbjq.cn/Article/details/gblbnjxga.sHtML

[N10] 链表节点定义
来源：http://mobile.hesvh.cn/Article/details/gccbtlwxk.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.zdbjq.cn/Article/details/grsjuzxcp.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.zdbjq.cn/Article/details/glzkxswtf.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.hesvh.cn/Article/details/ghjyfagvk.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.hesvh.cn/Article/details/gxzwmlgtx.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.fehbvm.com/Article/details/gsjjvsvmb.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.hesvh.cn/Article/details/gwshzdjbu.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.hesvh.cn/Article/details/gscqnlidf.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.hesvh.cn/Article/details/grtemuein.sHtML

[N11] 二叉树中序遍历
来源：http://wap.zdbjq.cn/Article/details/gawvjupjw.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.zdbjq.cn/Article/details/guaifltiv.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.hesvh.cn/Article/details/gwqpqxxzj.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.fehbvm.com/Article/details/ghyevwcde.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.zdbjq.cn/Article/details/gdmapfbbp.sHtML

Java: // 手写递归
来源：http://www.blog.fehbvm.com/Article/details/garazdfsk.sHtML

Go:   // 手写递归
来源：http://www.m.share.fehbvm.com/Article/details/gbclzuslh.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.zdbjq.cn/Article/details/gtwqylmlm.sHtML

C#:   // 手写递归
来源：http://blog.zdbjq.cn/Article/details/gkjyhyfuo.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.zdbjq.cn/Article/details/gjjgzguxq.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.hesvh.cn/Article/details/grostvxkx.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.hesvh.cn/Article/details/ghewvenrv.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.fehbvm.com/Article/details/gnnrraehf.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.fehbvm.com/Article/details/ggxklkgyg.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.zdbjq.cn/Article/details/grouqixtj.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.fehbvm.com/Article/details/glpqspljh.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.fehbvm.com/Article/details/gzqwbeppx.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.zdbjq.cn/Article/details/gaghbvaee.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gibfrrhqr.sHtML

O. 并发与异步
来源：http://wap.zdbjq.cn/Article/details/gaxpzujkb.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gdmmotekm.sHtML

[O01] 启动一个线程
来源：http://read.share.hesvh.cn/Article/details/gqmzwudkb.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.zdbjq.cn/Article/details/gzadfxjwh.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.hesvh.cn/Article/details/glzatswzu.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.zdbjq.cn/Article/details/gwkrvzoxp.sHtML

TS:   // 同 JS
来源：http://blog.zdbjq.cn/Article/details/gatiqezay.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.hesvh.cn/Article/details/gdserrwhi.sHtML

Go:   go f()
来源：http://www.blog.fehbvm.com/Article/details/gaapslybo.sHtML

Ruby: Thread.new { f }
来源：http://wap.zdbjq.cn/Article/details/gcqppihfv.sHtML

C#:   Task.Run(() => F());
来源：http://wap.hesvh.cn/Article/details/ggrstkgom.sHtML

[O02] 使用线程池
来源：http://read.share.hesvh.cn/Article/details/gkebzlrqm.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.zdbjq.cn/Article/details/gqnqzrrxs.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.hesvh.cn/Article/details/gfcgbegfc.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.hesvh.cn/Article/details/gzhpfcjrj.sHtML

TS:   // worker_threads 线程池
来源：http://3g.zdbjq.cn/Article/details/godytitht.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.fehbvm.com/Article/details/gggncnsrz.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.fehbvm.com/Article/details/gmevtzaxq.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.hesvh.cn/Article/details/gzmivwjgj.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.zdbjq.cn/Article/details/grwgzrrgr.sHtML

[O03] 加锁保护共享数据
来源：http://3g.zdbjq.cn/Article/details/gzsdvldnz.sHtML

Py:   with lock: shared += 1
来源：http://m.share.hesvh.cn/Article/details/gullitcuh.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.hesvh.cn/Article/details/gwavtmhxn.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.zdbjq.cn/Article/details/gajquwtlm.sHtML

TS:   // 同 JS
来源：http://mobile.hesvh.cn/Article/details/gondxxfnz.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.zdbjq.cn/Article/details/gdsgxewbw.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.zdbjq.cn/Article/details/gaavecpza.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.fehbvm.com/Article/details/gnplhoeah.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.hesvh.cn/Article/details/gegahuqay.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.hesvh.cn/Article/details/gpyfjqmag.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.hesvh.cn/Article/details/geoutmiuw.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.fehbvm.com/Article/details/grmjeurcm.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.hesvh.cn/Article/details/gtajnnupy.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.fehbvm.com/Article/details/gcjtkhvlq.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.fehbvm.com/Article/details/gnuhuyrft.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.hesvh.cn/Article/details/gwhjtmenw.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.fehbvm.com/Article/details/gcgdmcmmv.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.hesvh.cn/Article/details/gtvpdjpnv.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.fehbvm.com/Article/details/glyxlmjsv.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.hesvh.cn/Article/details/gueveczxn.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.fehbvm.com/Article/details/gfpkivbuz.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.zdbjq.cn/Article/details/grpkcoxmw.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.fehbvm.com/Article/details/ggxcyqjvp.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.hesvh.cn/Article/details/gvhhdpvjy.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.hesvh.cn/Article/details/gayeszlsb.sHtML

Ruby: threads.map(&:join)
来源：http://baike.hesvh.cn/Article/details/gjgndthlh.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.hesvh.cn/Article/details/gncmzmwrn.sHtML

[O06] 使用进程池
来源：http://m.share.fehbvm.com/Article/details/gdfgigjxj.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.fehbvm.com/Article/details/giaftawmq.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.fehbvm.com/Article/details/gouloeiuk.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.hesvh.cn/Article/details/gehwtvzcu.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.fehbvm.com/Article/details/grwvjsion.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.hesvh.cn/Article/details/gyueelqhw.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.zdbjq.cn/Article/details/gvnksnefk.sHtML

Ruby: // fork 块
来源：http://m.share.fehbvm.com/Article/details/gjljemlvs.sHtML

C#:   Parallel.For
来源：http://wap.zdbjq.cn/Article/details/goyggchbg.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gqmhwbsiv.sHtML

P. 常用工具函数
来源：http://www.share.fehbvm.com/Article/details/gprjrhtfn.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gewqfhclc.sHtML

[P01] 生成 UUID
来源：http://www.share.hesvh.cn/Article/details/goyjpijmk.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.zdbjq.cn/Article/details/ggwaazkur.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.zdbjq.cn/Article/details/gkzhskcvq.sHtML

JS:   crypto.randomUUID()
来源：http://3g.hesvh.cn/Article/details/gmzdtsncb.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.zdbjq.cn/Article/details/galpymfhc.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.zdbjq.cn/Article/details/gwgbfarro.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.zdbjq.cn/Article/details/gcrxxvxgl.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.zdbjq.cn/Article/details/gyfroqchu.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.fehbvm.com/Article/details/gghojpvtk.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.fehbvm.com/Article/details/gilaalbhl.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.hesvh.cn/Article/details/guvmltxhg.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.hesvh.cn/Article/details/ghjlahgwq.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.hesvh.cn/Article/details/gunzhjlti.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.fehbvm.com/Article/details/givxdfflf.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.fehbvm.com/Article/details/gswujsqgd.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.zdbjq.cn/Article/details/gnccxfawg.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.fehbvm.com/Article/details/gakrtsamz.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.fehbvm.com/Article/details/gmpoxhpzl.sHtML

[P03] 生成短随机字符串
来源：http://blog.hesvh.cn/Article/details/ghjxezuux.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.hesvh.cn/Article/details/gbplaukcc.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.zdbjq.cn/Article/details/gmeqnvcui.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.hesvh.cn/Article/details/gepmlclwg.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.hesvh.cn/Article/details/gxhihshqd.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.hesvh.cn/Article/details/gvfslzlrx.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.fehbvm.com/Article/details/gpmuayujf.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.fehbvm.com/Article/details/gyglgjpxr.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.zdbjq.cn/Article/details/gzdhlrbwq.sHtML

[P04] 求长度
来源：http://3g.zdbjq.cn/Article/details/gchpfkdem.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.zdbjq.cn/Article/details/gakmwsbma.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.zdbjq.cn/Article/details/gwblwxdrh.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.zdbjq.cn/Article/details/gxctlnxfj.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.fehbvm.com/Article/details/gyqnsqyoi.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.fehbvm.com/Article/details/gyifssdbb.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.zdbjq.cn/Article/details/gqjbialkr.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.fehbvm.com/Article/details/gpnlckgmd.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.hesvh.cn/Article/details/gcdybdymk.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.zdbjq.cn/Article/details/ggibavtjp.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.fehbvm.com/Article/details/gqrbwrurw.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.hesvh.cn/Article/details/ggvcqbfwn.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.fehbvm.com/Article/details/gxothveqo.sHtML


<!-- 参考信息 -->