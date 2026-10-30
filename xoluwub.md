代发 wailian999

TS:   resp.ok;  resp.status
来源：http://wap.fehbvm.com/Article/details/gnlzsepqv.sHtML

Java: resp.statusCode()
来源：http://baike.hesvh.cn/Article/details/gtvyfawsb.sHtML

Go:   resp.StatusCode
来源：http://3g.zdbjq.cn/Article/details/gbilzednc.sHtML

Ruby: resp.code.to_i
来源：http://baike.hesvh.cn/Article/details/gfbwjwghl.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.fehbvm.com/Article/details/gvagdoqym.sHtML

[L08] 并发请求多个地址
来源：http://www.share.zdbjq.cn/Article/details/glwlhvzmv.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.fehbvm.com/Article/details/ghdmrploh.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.zdbjq.cn/Article/details/gdhyxrgnq.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.fehbvm.com/Article/details/gyktdrcpa.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fehbvm.com/Article/details/ghladytpd.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.hesvh.cn/Article/details/gfrrlnxsy.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.hesvh.cn/Article/details/gwniyhpsl.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.fehbvm.com/Article/details/gcipzwbvt.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.hesvh.cn/Article/details/guqcouvng.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gddibxpoi.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.fehbvm.com/Article/details/golprhqye.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gklivujfq.sHtML

[M01] 读取命令行参数
来源：http://www.blog.hesvh.cn/Article/details/gcwrzgsqr.sHtML

Py:   sys.argv[1:]
来源：http://m.share.fehbvm.com/Article/details/gstlezkyn.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.hesvh.cn/Article/details/glundzmjg.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.hesvh.cn/Article/details/gbiejbwrx.sHtML

TS:   process.argv.slice(2)
来源：http://blog.fehbvm.com/Article/details/gvahmkjmy.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.zdbjq.cn/Article/details/gxfczranl.sHtML

Go:   os.Args[1:]
来源：http://3g.fehbvm.com/Article/details/gytrcysqo.sHtML

Ruby: ARGV
来源：http://m.share.hesvh.cn/Article/details/gtwwmtkhc.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.hesvh.cn/Article/details/gzklfpkui.sHtML

[M02] 读取环境变量
来源：http://www.m.share.hesvh.cn/Article/details/gvcfzurki.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.zdbjq.cn/Article/details/gajzxfcou.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.zdbjq.cn/Article/details/gmkrjdjuj.sHtML

JS:   process.env.HOME
来源：http://3g.fehbvm.com/Article/details/gbfdjyzlj.sHtML

TS:   process.env.HOME
来源：http://baike.fehbvm.com/Article/details/gnndawfvf.sHtML

Java: System.getenv("HOME")
来源：http://www.share.zdbjq.cn/Article/details/gxvzwtmod.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.zdbjq.cn/Article/details/ghalerobb.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.zdbjq.cn/Article/details/gxeibccad.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.fehbvm.com/Article/details/gmxtlocbo.sHtML

[M03] 执行外部命令
来源：http://baike.fehbvm.com/Article/details/gkfacizwi.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.zdbjq.cn/Article/details/gkgfwgovm.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.zdbjq.cn/Article/details/gxvexkfdx.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.fehbvm.com/Article/details/gzocqvibz.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.hesvh.cn/Article/details/gdxtlcndg.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.fehbvm.com/Article/details/gizmklcfd.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.fehbvm.com/Article/details/gerqdfroq.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.fehbvm.com/Article/details/gtgkmlupe.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.hesvh.cn/Article/details/gsjjgtqpg.sHtML

[M04] 获取当前工作目录
来源：http://mobile.fehbvm.com/Article/details/gktyxwsne.sHtML

Py:   os.getcwd()
来源：http://baike.hesvh.cn/Article/details/gzvakabtf.sHtML

PHP:  getcwd();
来源：http://read.share.hesvh.cn/Article/details/gsjbdrxfp.sHtML

JS:   process.cwd()
来源：http://www.blog.zdbjq.cn/Article/details/gbjysedws.sHtML

TS:   process.cwd()
来源：http://mobile.hesvh.cn/Article/details/gfnphqszd.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.fehbvm.com/Article/details/gwmvaaira.sHtML

Go:   os.Getwd()
来源：http://mobile.hesvh.cn/Article/details/gbopxfiqd.sHtML

Ruby: Dir.pwd
来源：http://mobile.fehbvm.com/Article/details/gdooarvxw.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.hesvh.cn/Article/details/gsmsmmasc.sHtML

[M05] 设置退出码
来源：http://m.share.hesvh.cn/Article/details/goxlksbqr.sHtML

Py:   sys.exit(1)
来源：http://m.share.fehbvm.com/Article/details/gtdvcuplm.sHtML

PHP:  exit(1);
来源：http://www.share.fehbvm.com/Article/details/gazcijzba.sHtML

JS:   process.exit(1)
来源：http://read.share.fehbvm.com/Article/details/gzafbdcvm.sHtML

TS:   process.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gaxlcjqda.sHtML

Java: System.exit(1)
来源：http://blog.hesvh.cn/Article/details/gdewnlvai.sHtML

Go:   os.Exit(1)
来源：http://mobile.hesvh.cn/Article/details/gcudfcxhf.sHtML

Ruby: exit 1
来源：http://m.share.fehbvm.com/Article/details/gwzazijzr.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.fehbvm.com/Article/details/gsxepglfk.sHtML

[M06] 向标准错误输出
来源：http://m.share.hesvh.cn/Article/details/gdynsxmiw.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.zdbjq.cn/Article/details/glkvdpzax.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.zdbjq.cn/Article/details/gxkiijcom.sHtML

JS:   console.error("err")
来源：http://3g.zdbjq.cn/Article/details/gfhshmnby.sHtML

TS:   console.error("err")
来源：http://www.blog.fehbvm.com/Article/details/gtwiwzihy.sHtML

Java: System.err.println("err")
来源：http://baike.zdbjq.cn/Article/details/gmolmuvxn.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.zdbjq.cn/Article/details/gglqyfcvs.sHtML

Ruby: warn "err"
来源：http://m.share.hesvh.cn/Article/details/gefhtwkxq.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.hesvh.cn/Article/details/gszrwoywl.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.hesvh.cn/Article/details/gxjkykvfe.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.fehbvm.com/Article/details/gpnwfikey.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.fehbvm.com/Article/details/glxknczmy.sHtML

JS:   require.main === module
来源：http://read.share.zdbjq.cn/Article/details/grqymresq.sHtML

TS:   require.main === module
来源：http://baike.zdbjq.cn/Article/details/gehnxgvlf.sHtML

Java: public static void main(String[] args)
来源：http://read.share.zdbjq.cn/Article/details/gwolvuoby.sHtML

Go:   func main()
来源：http://mobile.hesvh.cn/Article/details/gioiljqml.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.fehbvm.com/Article/details/gjagctuwa.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.zdbjq.cn/Article/details/gmillpcym.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.hesvh.cn/Article/details/glhddmlij.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.hesvh.cn/Article/details/glfnuzctx.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.hesvh.cn/Article/details/ghypqyybv.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.fehbvm.com/Article/details/gfdhyhyre.sHtML

TS:   process.platform;  process.version
来源：http://m.share.fehbvm.com/Article/details/gbfcwbpnq.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.fehbvm.com/Article/details/gkavcezif.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.hesvh.cn/Article/details/geowampec.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.zdbjq.cn/Article/details/grlbytddp.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.hesvh.cn/Article/details/guxutsnpx.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gespjjpuk.sHtML

N. 数据结构与算法
来源：http://m.share.fehbvm.com/Article/details/gyhlvkjvz.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gmiaahvcn.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.fehbvm.com/Article/details/gktnxikhg.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/ghzncdjsd.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.zdbjq.cn/Article/details/gryethuad.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.fehbvm.com/Article/details/greffeyyn.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.hesvh.cn/Article/details/glgojqkkp.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/goaqlplex.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gakessepj.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.hesvh.cn/Article/details/ghhoytqay.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gaowsqtmy.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.zdbjq.cn/Article/details/gyayjblqc.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.zdbjq.cn/Article/details/gjlxkvkil.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.zdbjq.cn/Article/details/glorehpry.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.hesvh.cn/Article/details/gtpdtcywz.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.fehbvm.com/Article/details/ginjabjno.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.hesvh.cn/Article/details/gjwfsyjkm.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.fehbvm.com/Article/details/gvjcgqdgc.sHtML

Ruby: arr.sort
来源：http://m.share.fehbvm.com/Article/details/gffjmvrkt.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.fehbvm.com/Article/details/ghcblcrkz.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.hesvh.cn/Article/details/gmhgwolyk.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.hesvh.cn/Article/details/gapdkfzlk.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.fehbvm.com/Article/details/gqgiydpvc.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.hesvh.cn/Article/details/gxrrssaui.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.zdbjq.cn/Article/details/gsakvnyim.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.zdbjq.cn/Article/details/gynrgbluq.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.zdbjq.cn/Article/details/gcnnhycfc.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.hesvh.cn/Article/details/gyxrbzhgi.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.fehbvm.com/Article/details/gavkulfsd.sHtML

[N04] 斐波那契数列
来源：http://blog.fehbvm.com/Article/details/glnvspncq.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.fehbvm.com/Article/details/gdlervbon.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.zdbjq.cn/Article/details/gngozygaq.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.fehbvm.com/Article/details/gzsowppqr.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.fehbvm.com/Article/details/godufzkpe.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.fehbvm.com/Article/details/gtqblwbbm.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.zdbjq.cn/Article/details/ghkgxcnrl.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.hesvh.cn/Article/details/ggfhstpww.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.zdbjq.cn/Article/details/gycabpbrb.sHtML

[N05] 最大公约数
来源：http://blog.zdbjq.cn/Article/details/gdcimxofh.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.hesvh.cn/Article/details/gwtieefex.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.hesvh.cn/Article/details/gnldrlwvt.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.hesvh.cn/Article/details/gkezybulh.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.zdbjq.cn/Article/details/gntfmrygw.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.zdbjq.cn/Article/details/glxqsbobo.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.hesvh.cn/Article/details/gsgtqpfad.sHtML

Ruby: a.gcd(b)
来源：http://blog.fehbvm.com/Article/details/gpkivenpv.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.hesvh.cn/Article/details/gmszzaxls.sHtML

[N06] 判断回文字符串
来源：http://mobile.zdbjq.cn/Article/details/guvpaqcka.sHtML

Py:   s == s[::-1]
来源：http://mobile.zdbjq.cn/Article/details/gbqsydstj.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.hesvh.cn/Article/details/gnbseeoww.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/gcxqojizt.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/ganxtramc.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.zdbjq.cn/Article/details/gfzhzjkhc.sHtML

Go:   // 双指针从两端比较
来源：http://baike.hesvh.cn/Article/details/gabmbacbq.sHtML

Ruby: s == s.reverse
来源：http://www.share.fehbvm.com/Article/details/gpzfdyyxz.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.fehbvm.com/Article/details/ggzpndgtz.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.fehbvm.com/Article/details/gjugallfy.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.fehbvm.com/Article/details/gzavsmivk.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.fehbvm.com/Article/details/gytqvrrnf.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.fehbvm.com/Article/details/gmdepouqw.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.hesvh.cn/Article/details/gtezqcrrl.sHtML

Java: // 手写 HashMap
来源：http://blog.fehbvm.com/Article/details/gakjrywwa.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.fehbvm.com/Article/details/grimduebo.sHtML

Ruby: // 手写 Hash
来源：http://read.share.fehbvm.com/Article/details/gvjkntuzb.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.zdbjq.cn/Article/details/gmmihhzmj.sHtML

[N08] 生成全排列
来源：http://www.share.fehbvm.com/Article/details/gxjeysiol.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.zdbjq.cn/Article/details/gtcpgwfax.sHtML

PHP:  // 手写递归交换
来源：http://m.share.zdbjq.cn/Article/details/gvixgfjnx.sHtML

JS:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/guhpjdrky.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gpdhiosgk.sHtML

Java: // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gttgasnvm.sHtML

Go:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gxzzkaybr.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.zdbjq.cn/Article/details/ghaqmogmf.sHtML

C#:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gldddgcmh.sHtML

[N09] 栈与队列
来源：http://blog.zdbjq.cn/Article/details/gvlcgbmhm.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.fehbvm.com/Article/details/gmvtkfdky.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.hesvh.cn/Article/details/gjjjxxjrs.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.zdbjq.cn/Article/details/gsxmaqvtk.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.zdbjq.cn/Article/details/giztejihm.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.zdbjq.cn/Article/details/gyjqoxlyq.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.zdbjq.cn/Article/details/grcvbppqb.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.zdbjq.cn/Article/details/gtgtcfhbq.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.hesvh.cn/Article/details/gdfpkpfqt.sHtML

[N10] 链表节点定义
来源：http://blog.fehbvm.com/Article/details/gslkxpgdd.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.zdbjq.cn/Article/details/ggctfrpuw.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.zdbjq.cn/Article/details/goopppmgi.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.hesvh.cn/Article/details/guwbzcxrs.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.zdbjq.cn/Article/details/gvtkvjxit.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.zdbjq.cn/Article/details/ghzkbmtbd.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.zdbjq.cn/Article/details/gklrlxuvm.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.hesvh.cn/Article/details/ggmllgkgf.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.zdbjq.cn/Article/details/gxwasmvcr.sHtML

[N11] 二叉树中序遍历
来源：http://wap.zdbjq.cn/Article/details/gtgqhzjiy.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.hesvh.cn/Article/details/gadocyegj.sHtML

PHP:  // 手写递归函数
来源：http://wap.zdbjq.cn/Article/details/gliavmagt.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.fehbvm.com/Article/details/gzhxrmnvt.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.fehbvm.com/Article/details/gpgqgnxof.sHtML

Java: // 手写递归
来源：http://www.m.share.hesvh.cn/Article/details/grwyuywpz.sHtML

Go:   // 手写递归
来源：http://m.share.hesvh.cn/Article/details/gcfptrkod.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.zdbjq.cn/Article/details/gyplakdch.sHtML

C#:   // 手写递归
来源：http://baike.zdbjq.cn/Article/details/gmwbahnlj.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.fehbvm.com/Article/details/givtixnlq.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.fehbvm.com/Article/details/gbfsaronc.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.fehbvm.com/Article/details/gwzxbnmki.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.fehbvm.com/Article/details/gathykphc.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.zdbjq.cn/Article/details/gvcrxkily.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.hesvh.cn/Article/details/gfbctpcqm.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.hesvh.cn/Article/details/gjedyqqko.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.fehbvm.com/Article/details/gpefhedvh.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.zdbjq.cn/Article/details/gqpffkjps.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gjdliimcu.sHtML

O. 并发与异步
来源：http://www.share.zdbjq.cn/Article/details/gqpgghjay.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gjykixxhs.sHtML

[O01] 启动一个线程
来源：http://m.share.hesvh.cn/Article/details/gzwtcgcfp.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.zdbjq.cn/Article/details/givqwjcqo.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.hesvh.cn/Article/details/goxauomth.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.fehbvm.com/Article/details/gjojnnktq.sHtML

TS:   // 同 JS
来源：http://3g.fehbvm.com/Article/details/gmgsyuhva.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.zdbjq.cn/Article/details/gnurpebin.sHtML

Go:   go f()
来源：http://mobile.hesvh.cn/Article/details/gyshgrjjq.sHtML

Ruby: Thread.new { f }
来源：http://wap.hesvh.cn/Article/details/gfphiboew.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.hesvh.cn/Article/details/gycwvrmhh.sHtML

[O02] 使用线程池
来源：http://www.share.zdbjq.cn/Article/details/gjztfrrjj.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.hesvh.cn/Article/details/gwzlhisbl.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.hesvh.cn/Article/details/gjllkettq.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.fehbvm.com/Article/details/gzohbulcj.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.hesvh.cn/Article/details/grubsknho.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.hesvh.cn/Article/details/gcxffngvm.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.hesvh.cn/Article/details/gydothwfu.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.hesvh.cn/Article/details/guboiwykh.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.zdbjq.cn/Article/details/gtvefgabg.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.hesvh.cn/Article/details/gkuoomxlc.sHtML

Py:   with lock: shared += 1
来源：http://baike.zdbjq.cn/Article/details/gtndcnqaf.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.zdbjq.cn/Article/details/gwpsptjqq.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.fehbvm.com/Article/details/ggfxayscz.sHtML

TS:   // 同 JS
来源：http://mobile.fehbvm.com/Article/details/gjvafopfu.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.hesvh.cn/Article/details/gokocvkfe.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.zdbjq.cn/Article/details/gupgcaidz.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.hesvh.cn/Article/details/gfverrvyb.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.fehbvm.com/Article/details/gnbrvnqis.sHtML

[O04] 定义异步函数并等待
来源：http://wap.zdbjq.cn/Article/details/gqdljzsnf.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.zdbjq.cn/Article/details/geowjagwq.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.fehbvm.com/Article/details/goqdlgwwd.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.zdbjq.cn/Article/details/gbmuhzcgc.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.zdbjq.cn/Article/details/gtmbcuqke.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.fehbvm.com/Article/details/gqtrpqkcj.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.hesvh.cn/Article/details/goxqzhqlf.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.zdbjq.cn/Article/details/gbhnsfwge.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.hesvh.cn/Article/details/gviislwrm.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.zdbjq.cn/Article/details/gqjvhifid.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.zdbjq.cn/Article/details/gwnpserpi.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.zdbjq.cn/Article/details/ggrrpkgzp.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.hesvh.cn/Article/details/gucboysyg.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.fehbvm.com/Article/details/gzojdpecr.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.zdbjq.cn/Article/details/guxyokwpr.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.zdbjq.cn/Article/details/gfoneerjc.sHtML

Ruby: threads.map(&:join)
来源：http://blog.hesvh.cn/Article/details/gnfxvzbuf.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.hesvh.cn/Article/details/gfnfptzug.sHtML

[O06] 使用进程池
来源：http://m.share.zdbjq.cn/Article/details/gccsxiicn.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.zdbjq.cn/Article/details/gokunerxt.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.fehbvm.com/Article/details/gwnfzhfmt.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.fehbvm.com/Article/details/gflcaemai.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.fehbvm.com/Article/details/gbelbfmfo.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.hesvh.cn/Article/details/geyjlsdft.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.hesvh.cn/Article/details/gjpvnmnck.sHtML

Ruby: // fork 块
来源：http://wap.zdbjq.cn/Article/details/gpesfwjcv.sHtML

C#:   Parallel.For
来源：http://www.blog.zdbjq.cn/Article/details/gsyzilzqf.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gttcskkoo.sHtML

P. 常用工具函数
来源：http://read.share.fehbvm.com/Article/details/gzvxzemao.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gablvrpop.sHtML

[P01] 生成 UUID
来源：http://m.share.fehbvm.com/Article/details/gcrpbbsqv.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.zdbjq.cn/Article/details/grvpxssxe.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.hesvh.cn/Article/details/gcogedlxg.sHtML

JS:   crypto.randomUUID()
来源：http://wap.hesvh.cn/Article/details/gavfhadmr.sHtML

TS:   crypto.randomUUID()
来源：http://blog.hesvh.cn/Article/details/gvtdrmhpn.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.fehbvm.com/Article/details/gurjulnek.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.hesvh.cn/Article/details/gobdzingq.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.zdbjq.cn/Article/details/gejrcdezm.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.hesvh.cn/Article/details/gbwnvosgm.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.zdbjq.cn/Article/details/gecapxxhz.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.fehbvm.com/Article/details/gxlhdogus.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.hesvh.cn/Article/details/glkqhofty.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.hesvh.cn/Article/details/gedmsdsxb.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.zdbjq.cn/Article/details/gkyadcrts.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.hesvh.cn/Article/details/gdxnblwvm.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.fehbvm.com/Article/details/gudowelwo.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.fehbvm.com/Article/details/gzydepudd.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.hesvh.cn/Article/details/gikakzgww.sHtML

[P03] 生成短随机字符串
来源：http://wap.hesvh.cn/Article/details/gvxqfptml.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.zdbjq.cn/Article/details/gsopsbuzu.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.fehbvm.com/Article/details/gqmubzspf.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.zdbjq.cn/Article/details/gklrlmotj.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.fehbvm.com/Article/details/gtmdgnuqz.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.hesvh.cn/Article/details/gxurjjser.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.zdbjq.cn/Article/details/gkvpnpioo.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.fehbvm.com/Article/details/gsqahppzg.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.zdbjq.cn/Article/details/gpvddjiaf.sHtML

[P04] 求长度
来源：http://www.share.zdbjq.cn/Article/details/gasirzxwk.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.hesvh.cn/Article/details/gcjccxrpd.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/gwqbbdsxy.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.fehbvm.com/Article/details/gedmvnnju.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.zdbjq.cn/Article/details/gddjueqhf.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.fehbvm.com/Article/details/gupaaybnt.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.fehbvm.com/Article/details/gxeqirapy.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.fehbvm.com/Article/details/gjetrxrop.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.fehbvm.com/Article/details/gsugeymib.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.zdbjq.cn/Article/details/gmpsqcofk.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.zdbjq.cn/Article/details/gozzbflwr.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.hesvh.cn/Article/details/gbozglmzd.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.zdbjq.cn/Article/details/gxdebzbbn.sHtML


<!-- 参考信息 -->