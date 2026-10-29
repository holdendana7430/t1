代发 wailian999

C#:   (int)resp.StatusCode
来源：http://www.share.zdbjq.cn/Article/details/gvapvdulk.sHtML

[L08] 并发请求多个地址
来源：http://wap.zdbjq.cn/Article/details/gafrqddia.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.zdbjq.cn/Article/details/gozcprekb.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.fehbvm.com/Article/details/gchfxanlx.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.hesvh.cn/Article/details/gruesliio.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.hesvh.cn/Article/details/gaccwaopm.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.zdbjq.cn/Article/details/gtfxxjmwy.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.hesvh.cn/Article/details/gwuiefegd.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.fehbvm.com/Article/details/grmvszron.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.zdbjq.cn/Article/details/grsqyxvri.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gkoxsvvdb.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.hesvh.cn/Article/details/gnlhjuxaw.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gsmysoulv.sHtML

[M01] 读取命令行参数
来源：http://read.share.zdbjq.cn/Article/details/ggxdbjvdg.sHtML

Py:   sys.argv[1:]
来源：http://read.share.zdbjq.cn/Article/details/glyonokoi.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.fehbvm.com/Article/details/gqbpaipkh.sHtML

JS:   process.argv.slice(2)
来源：http://baike.zdbjq.cn/Article/details/gyospbvzt.sHtML

TS:   process.argv.slice(2)
来源：http://wap.zdbjq.cn/Article/details/gssirszlw.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.fehbvm.com/Article/details/gvqrgnhsk.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.zdbjq.cn/Article/details/ggrylvpcy.sHtML

Ruby: ARGV
来源：http://3g.zdbjq.cn/Article/details/gzvuwztyy.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.fehbvm.com/Article/details/ggqvrkcdo.sHtML

[M02] 读取环境变量
来源：http://3g.fehbvm.com/Article/details/ghlpdapky.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.fehbvm.com/Article/details/ggzzjfgfa.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.fehbvm.com/Article/details/gdgannhfk.sHtML

JS:   process.env.HOME
来源：http://blog.zdbjq.cn/Article/details/gvffusgqd.sHtML

TS:   process.env.HOME
来源：http://baike.zdbjq.cn/Article/details/gdlxxtuaj.sHtML

Java: System.getenv("HOME")
来源：http://baike.fehbvm.com/Article/details/gymqgfjdp.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.hesvh.cn/Article/details/grwdnglvx.sHtML

Ruby: ENV["HOME"]
来源：http://baike.hesvh.cn/Article/details/gbratmwrs.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.hesvh.cn/Article/details/gvxitayxw.sHtML

[M03] 执行外部命令
来源：http://m.share.zdbjq.cn/Article/details/gcvntwgpo.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.hesvh.cn/Article/details/gpjjhafyy.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.hesvh.cn/Article/details/gvvfbdvng.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.zdbjq.cn/Article/details/gqxfvcvdf.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.zdbjq.cn/Article/details/gussoqjjf.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.zdbjq.cn/Article/details/gwnqcyyft.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.fehbvm.com/Article/details/gsgidixqx.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.hesvh.cn/Article/details/gjaerkqlh.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.zdbjq.cn/Article/details/gkyagwzqb.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.zdbjq.cn/Article/details/gbohzmbqf.sHtML

Py:   os.getcwd()
来源：http://mobile.fehbvm.com/Article/details/geavtdjnr.sHtML

PHP:  getcwd();
来源：http://www.blog.fehbvm.com/Article/details/gcttpferw.sHtML

JS:   process.cwd()
来源：http://m.share.fehbvm.com/Article/details/ggsvqubvb.sHtML

TS:   process.cwd()
来源：http://blog.hesvh.cn/Article/details/gfknvczga.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.zdbjq.cn/Article/details/gwatglekx.sHtML

Go:   os.Getwd()
来源：http://m.share.hesvh.cn/Article/details/gzmjhicpg.sHtML

Ruby: Dir.pwd
来源：http://read.share.fehbvm.com/Article/details/gmtdhnwye.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.hesvh.cn/Article/details/gigcessil.sHtML

[M05] 设置退出码
来源：http://blog.zdbjq.cn/Article/details/giqzujpar.sHtML

Py:   sys.exit(1)
来源：http://m.share.fehbvm.com/Article/details/grilzpjml.sHtML

PHP:  exit(1);
来源：http://baike.zdbjq.cn/Article/details/gqhrnznbe.sHtML

JS:   process.exit(1)
来源：http://baike.fehbvm.com/Article/details/gcuajmpww.sHtML

TS:   process.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gstebtxnt.sHtML

Java: System.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gpcougsnk.sHtML

Go:   os.Exit(1)
来源：http://wap.zdbjq.cn/Article/details/gxmxvhsif.sHtML

Ruby: exit 1
来源：http://mobile.hesvh.cn/Article/details/gxjlshjfk.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.zdbjq.cn/Article/details/gkrpcsttv.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.zdbjq.cn/Article/details/glcjrmmho.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.hesvh.cn/Article/details/gjzczjrnj.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.zdbjq.cn/Article/details/gnxapvnrm.sHtML

JS:   console.error("err")
来源：http://wap.zdbjq.cn/Article/details/gjsnnvrum.sHtML

TS:   console.error("err")
来源：http://mobile.zdbjq.cn/Article/details/gsqbddcpb.sHtML

Java: System.err.println("err")
来源：http://3g.fehbvm.com/Article/details/gczmoyful.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.hesvh.cn/Article/details/ghrtiyvnl.sHtML

Ruby: warn "err"
来源：http://www.blog.zdbjq.cn/Article/details/gkzrpsvho.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.fehbvm.com/Article/details/gtcsekynu.sHtML

[M07] 判断是否为主入口
来源：http://baike.zdbjq.cn/Article/details/ggnzgbsyr.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.hesvh.cn/Article/details/gpioviatp.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.fehbvm.com/Article/details/gwzgoxwcx.sHtML

JS:   require.main === module
来源：http://read.share.zdbjq.cn/Article/details/gquivbuda.sHtML

TS:   require.main === module
来源：http://www.blog.hesvh.cn/Article/details/gyknqlqjd.sHtML

Java: public static void main(String[] args)
来源：http://wap.fehbvm.com/Article/details/guvspbale.sHtML

Go:   func main()
来源：http://3g.zdbjq.cn/Article/details/gmfzbydon.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.zdbjq.cn/Article/details/gjtzkwsgz.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.zdbjq.cn/Article/details/gtkciudey.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.fehbvm.com/Article/details/gcsqgskcl.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.fehbvm.com/Article/details/gpydaolbi.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.zdbjq.cn/Article/details/ggpbnjput.sHtML

JS:   process.platform;  process.version
来源：http://baike.zdbjq.cn/Article/details/gotfauqyq.sHtML

TS:   process.platform;  process.version
来源：http://www.share.zdbjq.cn/Article/details/ggznunqfw.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.hesvh.cn/Article/details/gqujjbifu.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.zdbjq.cn/Article/details/gsqpfitrm.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.zdbjq.cn/Article/details/gfnzgybgo.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.hesvh.cn/Article/details/gjtakvvkc.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gbnuxrlko.sHtML

N. 数据结构与算法
来源：http://www.share.zdbjq.cn/Article/details/gkqdjrnou.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gkpafjlgs.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.fehbvm.com/Article/details/gfevmkwme.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gyaxgfcry.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.zdbjq.cn/Article/details/gemjgdifr.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.fehbvm.com/Article/details/gvsjlkine.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.hesvh.cn/Article/details/gwmbnhcqw.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.fehbvm.com/Article/details/ggcblkftc.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.hesvh.cn/Article/details/gbhozrnhy.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.fehbvm.com/Article/details/gantajmjg.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.zdbjq.cn/Article/details/grferxegm.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.hesvh.cn/Article/details/gtbksxbyp.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.fehbvm.com/Article/details/glnfdbfyz.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.zdbjq.cn/Article/details/gpnyaxfgu.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.zdbjq.cn/Article/details/gzwivrpcn.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.fehbvm.com/Article/details/gaxuqpqrt.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.hesvh.cn/Article/details/gertbcslm.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.hesvh.cn/Article/details/gmckhucxk.sHtML

Ruby: arr.sort
来源：http://blog.fehbvm.com/Article/details/gpgwerlet.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.zdbjq.cn/Article/details/goeguuzsk.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.fehbvm.com/Article/details/glsdzfgqh.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.zdbjq.cn/Article/details/gcsavixpu.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.zdbjq.cn/Article/details/gwysvhvwr.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.hesvh.cn/Article/details/ghnzverfc.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.fehbvm.com/Article/details/gyljmnffu.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.zdbjq.cn/Article/details/gxtulxcyg.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.fehbvm.com/Article/details/gfdzofzvq.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.fehbvm.com/Article/details/gyholywkp.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.fehbvm.com/Article/details/glzbsympm.sHtML

[N04] 斐波那契数列
来源：http://3g.zdbjq.cn/Article/details/ghsbpdncy.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.hesvh.cn/Article/details/golhudkcd.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.fehbvm.com/Article/details/gjqfaudym.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.hesvh.cn/Article/details/gpiizigmk.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/gceeqidmn.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.fehbvm.com/Article/details/guilxhooa.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.fehbvm.com/Article/details/gmpzvswkp.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.fehbvm.com/Article/details/gmpfukxzi.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.fehbvm.com/Article/details/gkhaacftm.sHtML

[N05] 最大公约数
来源：http://3g.zdbjq.cn/Article/details/gjugovwpk.sHtML

Py:   math.gcd(a, b)
来源：http://wap.zdbjq.cn/Article/details/gqgjskyco.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.fehbvm.com/Article/details/gufqzqhkv.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.fehbvm.com/Article/details/grryjepqh.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.fehbvm.com/Article/details/gkdwscajm.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.zdbjq.cn/Article/details/gslmowrxz.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.fehbvm.com/Article/details/gigyfkjzy.sHtML

Ruby: a.gcd(b)
来源：http://read.share.zdbjq.cn/Article/details/gqizmoqcv.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.hesvh.cn/Article/details/gaqhehdbe.sHtML

[N06] 判断回文字符串
来源：http://blog.hesvh.cn/Article/details/gapueavwl.sHtML

Py:   s == s[::-1]
来源：http://www.share.zdbjq.cn/Article/details/gqjrmsdrc.sHtML

PHP:  $s === strrev($s);
来源：http://wap.hesvh.cn/Article/details/gdarjqnrp.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/gnddxgbbj.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/glbitapgs.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.fehbvm.com/Article/details/gwciqjzzw.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.hesvh.cn/Article/details/gjmxkjsqt.sHtML

Ruby: s == s.reverse
来源：http://3g.zdbjq.cn/Article/details/gauqoxtsc.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.fehbvm.com/Article/details/gpfjmbrio.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.hesvh.cn/Article/details/gimbzawyw.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.fehbvm.com/Article/details/gqievwwuf.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.hesvh.cn/Article/details/gysovlumz.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.zdbjq.cn/Article/details/geeeagwtm.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.fehbvm.com/Article/details/ghpsjqptl.sHtML

Java: // 手写 HashMap
来源：http://www.share.fehbvm.com/Article/details/ggzgsnpoi.sHtML

Go:   // 手写 map[int]int
来源：http://wap.fehbvm.com/Article/details/gpbkueqxr.sHtML

Ruby: // 手写 Hash
来源：http://mobile.hesvh.cn/Article/details/gxverqkos.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.fehbvm.com/Article/details/gnblmwtki.sHtML

[N08] 生成全排列
来源：http://baike.zdbjq.cn/Article/details/gfcyvhcbl.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gzvvwqzfr.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.hesvh.cn/Article/details/gheyaawni.sHtML

JS:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gninyqipz.sHtML

TS:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gdclgkqal.sHtML

Java: // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gihziwaxb.sHtML

Go:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gpfcmijlc.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.fehbvm.com/Article/details/goysxbsro.sHtML

C#:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gjfoivdco.sHtML

[N09] 栈与队列
来源：http://baike.fehbvm.com/Article/details/ghbdmtwnr.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.fehbvm.com/Article/details/gkuntzfzz.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.hesvh.cn/Article/details/gfmzndxio.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.hesvh.cn/Article/details/gejogrjld.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.hesvh.cn/Article/details/gricfpdly.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.hesvh.cn/Article/details/gaatxyloh.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.fehbvm.com/Article/details/ggzsqteuc.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.fehbvm.com/Article/details/gtpfxlvpa.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.fehbvm.com/Article/details/gubnufnic.sHtML

[N10] 链表节点定义
来源：http://read.share.zdbjq.cn/Article/details/gffkzgatb.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.fehbvm.com/Article/details/gjrsifuzc.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.fehbvm.com/Article/details/geabmcgwq.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.zdbjq.cn/Article/details/gwjfazpau.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.fehbvm.com/Article/details/gojjzpqez.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.hesvh.cn/Article/details/gonzksucr.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.hesvh.cn/Article/details/gasxzyrxz.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.hesvh.cn/Article/details/gpwafjyxz.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.hesvh.cn/Article/details/gghcgfqdc.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.hesvh.cn/Article/details/gwvdtcoao.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.zdbjq.cn/Article/details/gkslfagdr.sHtML

PHP:  // 手写递归函数
来源：http://baike.hesvh.cn/Article/details/gidhvzoll.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.hesvh.cn/Article/details/gwdlkuddp.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.zdbjq.cn/Article/details/gerawqngw.sHtML

Java: // 手写递归
来源：http://3g.fehbvm.com/Article/details/gretkxaij.sHtML

Go:   // 手写递归
来源：http://baike.zdbjq.cn/Article/details/gesukrclm.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.hesvh.cn/Article/details/gmdedfnvj.sHtML

C#:   // 手写递归
来源：http://www.blog.fehbvm.com/Article/details/grxlxkcff.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.fehbvm.com/Article/details/ggzbpkbuu.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.zdbjq.cn/Article/details/gpmpoznls.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.zdbjq.cn/Article/details/gkiakuxuz.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.fehbvm.com/Article/details/gzoinavqf.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.hesvh.cn/Article/details/gtzucpixl.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.hesvh.cn/Article/details/gqqycvvsb.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.fehbvm.com/Article/details/gqivpjkcu.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.fehbvm.com/Article/details/gllweksnl.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.hesvh.cn/Article/details/gbbcxbpog.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gonrnzdyd.sHtML

O. 并发与异步
来源：http://baike.zdbjq.cn/Article/details/glwaahhsy.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gzuaivrvj.sHtML

[O01] 启动一个线程
来源：http://m.share.hesvh.cn/Article/details/gqyxuokfr.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.fehbvm.com/Article/details/gmgkbsrlv.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.hesvh.cn/Article/details/gfezefufh.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.zdbjq.cn/Article/details/gvfcimqlr.sHtML

TS:   // 同 JS
来源：http://www.share.fehbvm.com/Article/details/gdynijqkx.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.fehbvm.com/Article/details/ghbykdtdi.sHtML

Go:   go f()
来源：http://mobile.fehbvm.com/Article/details/glicyglav.sHtML

Ruby: Thread.new { f }
来源：http://mobile.zdbjq.cn/Article/details/gewutehfr.sHtML

C#:   Task.Run(() => F());
来源：http://wap.zdbjq.cn/Article/details/gjxucljfd.sHtML

[O02] 使用线程池
来源：http://wap.fehbvm.com/Article/details/gbrmhsfjb.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.fehbvm.com/Article/details/gngzezxcx.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.zdbjq.cn/Article/details/gjupznnrz.sHtML

JS:   // worker_threads 线程池
来源：http://blog.zdbjq.cn/Article/details/ghofcxrkl.sHtML

TS:   // worker_threads 线程池
来源：http://wap.fehbvm.com/Article/details/gwyhalzfg.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.hesvh.cn/Article/details/glmwnymiv.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.hesvh.cn/Article/details/giqiyvyhh.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.zdbjq.cn/Article/details/gefvgexjn.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.hesvh.cn/Article/details/gincsmvhu.sHtML

[O03] 加锁保护共享数据
来源：http://3g.zdbjq.cn/Article/details/geyxlkmmt.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.hesvh.cn/Article/details/gfwwbijeu.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.hesvh.cn/Article/details/gkbejggfi.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.zdbjq.cn/Article/details/gmoccboch.sHtML

TS:   // 同 JS
来源：http://mobile.fehbvm.com/Article/details/gykqzcril.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.zdbjq.cn/Article/details/gvdaslate.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.fehbvm.com/Article/details/geqkhgtnp.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.hesvh.cn/Article/details/gbnvoajhy.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.fehbvm.com/Article/details/gzpeuyyki.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.fehbvm.com/Article/details/geivjngiu.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.fehbvm.com/Article/details/gkwyxlmsx.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.zdbjq.cn/Article/details/gilimoikm.sHtML

JS:   async function f() { await g(); }
来源：http://3g.hesvh.cn/Article/details/gydyzxxlu.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.hesvh.cn/Article/details/gfedckkqc.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.fehbvm.com/Article/details/grqmurgdb.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.fehbvm.com/Article/details/gdqobqfoe.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.fehbvm.com/Article/details/gfunhnmkk.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.fehbvm.com/Article/details/gfwisygwb.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.zdbjq.cn/Article/details/gtifhicfu.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.zdbjq.cn/Article/details/gcyexrnnz.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.fehbvm.com/Article/details/gvntrdxwn.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.zdbjq.cn/Article/details/gvudgcuxn.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.zdbjq.cn/Article/details/gufwbhjsw.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.hesvh.cn/Article/details/gmywtvrvn.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.fehbvm.com/Article/details/gmndfvpfy.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.zdbjq.cn/Article/details/ggkadfyjd.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.hesvh.cn/Article/details/gtumecobj.sHtML

[O06] 使用进程池
来源：http://www.blog.fehbvm.com/Article/details/gxnqdtaxu.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.fehbvm.com/Article/details/gnpalwrpj.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.hesvh.cn/Article/details/gkuaztfus.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.fehbvm.com/Article/details/gkdiwadoh.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.hesvh.cn/Article/details/gimrserig.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.zdbjq.cn/Article/details/goqhgwymz.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.zdbjq.cn/Article/details/gsotyrdrw.sHtML

Ruby: // fork 块
来源：http://www.share.fehbvm.com/Article/details/gwtkyrbrj.sHtML

C#:   Parallel.For
来源：http://baike.hesvh.cn/Article/details/govramzpc.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gmnwaldfk.sHtML

P. 常用工具函数
来源：http://3g.zdbjq.cn/Article/details/ghdayjgvq.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/ghxvuthut.sHtML

[P01] 生成 UUID
来源：http://www.share.zdbjq.cn/Article/details/gszmcxuro.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.fehbvm.com/Article/details/grccqtwsq.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.fehbvm.com/Article/details/gzwtuzipu.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.zdbjq.cn/Article/details/ghijmacvq.sHtML

TS:   crypto.randomUUID()
来源：http://baike.fehbvm.com/Article/details/guzimcqbv.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.hesvh.cn/Article/details/guqrvgkyi.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.hesvh.cn/Article/details/gehvbpfqa.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.fehbvm.com/Article/details/gojkiqzmc.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.zdbjq.cn/Article/details/gtgkwihkj.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.zdbjq.cn/Article/details/gkhxkvyyw.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.zdbjq.cn/Article/details/gxtylrbhk.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.fehbvm.com/Article/details/gwzpcvwhm.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.hesvh.cn/Article/details/gnifsawbe.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.hesvh.cn/Article/details/gcygdtjqy.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.fehbvm.com/Article/details/gsxmnwiav.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.fehbvm.com/Article/details/gstmgbobb.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.zdbjq.cn/Article/details/gessyengz.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.hesvh.cn/Article/details/gyievisse.sHtML

[P03] 生成短随机字符串
来源：http://www.share.zdbjq.cn/Article/details/gptfdsttn.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.zdbjq.cn/Article/details/gldwfcris.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.hesvh.cn/Article/details/govahewgh.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.fehbvm.com/Article/details/gzebvefxp.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.fehbvm.com/Article/details/gchazkepb.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.hesvh.cn/Article/details/gekvyegwz.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.fehbvm.com/Article/details/gnifyhirw.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.hesvh.cn/Article/details/gqfbzijth.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.fehbvm.com/Article/details/gzftiusbg.sHtML

[P04] 求长度
来源：http://www.share.fehbvm.com/Article/details/gztfuohrw.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.zdbjq.cn/Article/details/gjzrdemkm.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.hesvh.cn/Article/details/guopewwph.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.fehbvm.com/Article/details/gnpjkzege.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.fehbvm.com/Article/details/gyeijddjj.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.hesvh.cn/Article/details/gdqtjuxzc.sHtML

Go:   len(arr);  len(m)
来源：http://blog.zdbjq.cn/Article/details/godwjmhst.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.fehbvm.com/Article/details/gqpfysgvr.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.zdbjq.cn/Article/details/gbbksqmkv.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.zdbjq.cn/Article/details/guddgjlyq.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.hesvh.cn/Article/details/gpcnqjjdj.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.fehbvm.com/Article/details/gktscbgmb.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.fehbvm.com/Article/details/gdxstsezu.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.hesvh.cn/Article/details/gboumugeg.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.hesvh.cn/Article/details/ghkycwrai.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.hesvh.cn/Article/details/gwkrkhunf.sHtML

Ruby: a == b
来源：http://baike.zdbjq.cn/Article/details/geyunwozk.sHtML


<!-- 参考信息 -->