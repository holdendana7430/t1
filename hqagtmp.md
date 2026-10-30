代发 wailian999

C#:   (int)resp.StatusCode
来源：http://www.share.zdbjq.cn/Article/details/gkmijhdxv.sHtML

[L08] 并发请求多个地址
来源：http://blog.fehbvm.com/Article/details/golkumrzp.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.fehbvm.com/Article/details/guoallgza.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.zdbjq.cn/Article/details/gnymqgjnd.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.zdbjq.cn/Article/details/ghrtjcdsz.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.zdbjq.cn/Article/details/giytmzdnb.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.zdbjq.cn/Article/details/gwrsskrll.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.fehbvm.com/Article/details/gzkzrkehl.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.hesvh.cn/Article/details/gezdveetz.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.zdbjq.cn/Article/details/gggqxpsoc.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gkpaqhcsa.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.fehbvm.com/Article/details/gtwkakbui.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gykdtwacf.sHtML

[M01] 读取命令行参数
来源：http://www.share.hesvh.cn/Article/details/gbuoistoi.sHtML

Py:   sys.argv[1:]
来源：http://read.share.hesvh.cn/Article/details/gevqlbpxl.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.hesvh.cn/Article/details/gcydwnqpo.sHtML

JS:   process.argv.slice(2)
来源：http://wap.hesvh.cn/Article/details/gestdculf.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.zdbjq.cn/Article/details/gjgboaksh.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.hesvh.cn/Article/details/glaypugtk.sHtML

Go:   os.Args[1:]
来源：http://3g.zdbjq.cn/Article/details/gsiyagnpd.sHtML

Ruby: ARGV
来源：http://read.share.fehbvm.com/Article/details/gxdxdmlvq.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.zdbjq.cn/Article/details/gsvqsbgkx.sHtML

[M02] 读取环境变量
来源：http://mobile.hesvh.cn/Article/details/gthvapdlw.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.hesvh.cn/Article/details/ghuthrutr.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.zdbjq.cn/Article/details/ggxodbrui.sHtML

JS:   process.env.HOME
来源：http://wap.fehbvm.com/Article/details/gjbsgcpds.sHtML

TS:   process.env.HOME
来源：http://www.m.share.zdbjq.cn/Article/details/grhhdozlq.sHtML

Java: System.getenv("HOME")
来源：http://baike.hesvh.cn/Article/details/gzctcgkfp.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.zdbjq.cn/Article/details/gcpcjhepd.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.zdbjq.cn/Article/details/gosiwgijy.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.zdbjq.cn/Article/details/gaerwnftv.sHtML

[M03] 执行外部命令
来源：http://www.share.hesvh.cn/Article/details/gzmkvwkro.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.zdbjq.cn/Article/details/gyjeetavk.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.zdbjq.cn/Article/details/gsihznmkg.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.zdbjq.cn/Article/details/gomkuthku.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.fehbvm.com/Article/details/ggbupypus.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.zdbjq.cn/Article/details/gblcinelg.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.zdbjq.cn/Article/details/gswakyaqj.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.zdbjq.cn/Article/details/gemyujexo.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.hesvh.cn/Article/details/guniwzxnj.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.hesvh.cn/Article/details/gzdkdaquo.sHtML

Py:   os.getcwd()
来源：http://baike.zdbjq.cn/Article/details/gwdraersh.sHtML

PHP:  getcwd();
来源：http://blog.hesvh.cn/Article/details/gtqrhnacv.sHtML

JS:   process.cwd()
来源：http://www.blog.zdbjq.cn/Article/details/gfkytnrcn.sHtML

TS:   process.cwd()
来源：http://read.share.zdbjq.cn/Article/details/gdakvdrvh.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.zdbjq.cn/Article/details/gqgujwgzg.sHtML

Go:   os.Getwd()
来源：http://www.blog.zdbjq.cn/Article/details/gtxvkmswi.sHtML

Ruby: Dir.pwd
来源：http://baike.hesvh.cn/Article/details/grhlrbiqe.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.fehbvm.com/Article/details/gawoyhgfh.sHtML

[M05] 设置退出码
来源：http://blog.hesvh.cn/Article/details/gvefaogth.sHtML

Py:   sys.exit(1)
来源：http://wap.zdbjq.cn/Article/details/gstydpwqu.sHtML

PHP:  exit(1);
来源：http://www.blog.zdbjq.cn/Article/details/gkghkqpkf.sHtML

JS:   process.exit(1)
来源：http://m.share.fehbvm.com/Article/details/gtwxhfmpi.sHtML

TS:   process.exit(1)
来源：http://wap.fehbvm.com/Article/details/ghvbajgmp.sHtML

Java: System.exit(1)
来源：http://wap.zdbjq.cn/Article/details/gashqiunq.sHtML

Go:   os.Exit(1)
来源：http://wap.hesvh.cn/Article/details/gtdtdrgrl.sHtML

Ruby: exit 1
来源：http://3g.zdbjq.cn/Article/details/ghhrwioou.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.zdbjq.cn/Article/details/glycyisbo.sHtML

[M06] 向标准错误输出
来源：http://blog.zdbjq.cn/Article/details/gknztmhrr.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.hesvh.cn/Article/details/ggygujbxk.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.hesvh.cn/Article/details/gzmqvghib.sHtML

JS:   console.error("err")
来源：http://wap.zdbjq.cn/Article/details/gfutctvrc.sHtML

TS:   console.error("err")
来源：http://baike.zdbjq.cn/Article/details/gxlavpwwz.sHtML

Java: System.err.println("err")
来源：http://www.blog.fehbvm.com/Article/details/gssdlrggz.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.hesvh.cn/Article/details/gmwwspapo.sHtML

Ruby: warn "err"
来源：http://3g.fehbvm.com/Article/details/gbczfwvzj.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.fehbvm.com/Article/details/gxmundlvj.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.hesvh.cn/Article/details/gzyshysrn.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.zdbjq.cn/Article/details/gzvasbtyt.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.zdbjq.cn/Article/details/gdrwyilzx.sHtML

JS:   require.main === module
来源：http://www.blog.zdbjq.cn/Article/details/gthqqllij.sHtML

TS:   require.main === module
来源：http://blog.hesvh.cn/Article/details/gjhbyoqyb.sHtML

Java: public static void main(String[] args)
来源：http://wap.fehbvm.com/Article/details/ggdpuwpck.sHtML

Go:   func main()
来源：http://blog.fehbvm.com/Article/details/gscpjhftt.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.hesvh.cn/Article/details/gmtwpmgkg.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.hesvh.cn/Article/details/gbcmdzijp.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.zdbjq.cn/Article/details/gkxblvnco.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.zdbjq.cn/Article/details/gcknuaitj.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.fehbvm.com/Article/details/gedksdmly.sHtML

JS:   process.platform;  process.version
来源：http://read.share.fehbvm.com/Article/details/gqyihoghk.sHtML

TS:   process.platform;  process.version
来源：http://baike.zdbjq.cn/Article/details/gubjdlnfy.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.hesvh.cn/Article/details/gsrffnlrm.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.hesvh.cn/Article/details/gllbmcgcx.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.zdbjq.cn/Article/details/gkjrwokwp.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.hesvh.cn/Article/details/gkvyrjtna.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gihnhssam.sHtML

N. 数据结构与算法
来源：http://m.share.zdbjq.cn/Article/details/gpboatnjp.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gjxcaunex.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.fehbvm.com/Article/details/gutxvohsc.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.hesvh.cn/Article/details/gymkqdrdi.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.hesvh.cn/Article/details/gsqsebbog.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.zdbjq.cn/Article/details/gnbxrvipj.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.zdbjq.cn/Article/details/gtswtzdnc.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gngioltjp.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.zdbjq.cn/Article/details/geepxmmci.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.hesvh.cn/Article/details/gviwfzbel.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.fehbvm.com/Article/details/gccrmwvgv.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.hesvh.cn/Article/details/gmfawdzea.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.hesvh.cn/Article/details/gtldqcnwi.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.fehbvm.com/Article/details/gifnulldg.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.zdbjq.cn/Article/details/gwuduabev.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.fehbvm.com/Article/details/gxvbogcqr.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.hesvh.cn/Article/details/gfngrjihg.sHtML

Go:   slices.Sort(arr)
来源：http://wap.zdbjq.cn/Article/details/gwngowzbk.sHtML

Ruby: arr.sort
来源：http://www.share.fehbvm.com/Article/details/gekojlxcl.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.zdbjq.cn/Article/details/gwprizjqd.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.fehbvm.com/Article/details/gftmwktzk.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.hesvh.cn/Article/details/gqcvxbeqi.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.fehbvm.com/Article/details/gpqlvygqo.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.zdbjq.cn/Article/details/gbulygxkl.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.zdbjq.cn/Article/details/gipwakyoa.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.zdbjq.cn/Article/details/gcgtjqixi.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.fehbvm.com/Article/details/gqawpfsjd.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.fehbvm.com/Article/details/gvbvaqese.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.zdbjq.cn/Article/details/gqhjddmrg.sHtML

[N04] 斐波那契数列
来源：http://wap.fehbvm.com/Article/details/gtsqbmbxf.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.hesvh.cn/Article/details/guvpocpth.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.zdbjq.cn/Article/details/gbkivwbyh.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.fehbvm.com/Article/details/gismdenjv.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.hesvh.cn/Article/details/gwvwvskef.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.zdbjq.cn/Article/details/gbdwbkycy.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.fehbvm.com/Article/details/gfikbcxrp.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.zdbjq.cn/Article/details/gyemspwwx.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.zdbjq.cn/Article/details/gzfmbtrso.sHtML

[N05] 最大公约数
来源：http://mobile.hesvh.cn/Article/details/gwvvmbtun.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.zdbjq.cn/Article/details/gjwqjgjus.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.zdbjq.cn/Article/details/gxgixjlko.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.zdbjq.cn/Article/details/griufezmt.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.zdbjq.cn/Article/details/gvvopbyox.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.fehbvm.com/Article/details/geposejdu.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.hesvh.cn/Article/details/grwguqfco.sHtML

Ruby: a.gcd(b)
来源：http://blog.fehbvm.com/Article/details/gthibsibs.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.fehbvm.com/Article/details/grcpqjbsj.sHtML

[N06] 判断回文字符串
来源：http://m.share.zdbjq.cn/Article/details/gwfhsmrnj.sHtML

Py:   s == s[::-1]
来源：http://blog.fehbvm.com/Article/details/gsyiphgfw.sHtML

PHP:  $s === strrev($s);
来源：http://3g.hesvh.cn/Article/details/gzczpmlva.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/grndyctld.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/gqkpkfbfv.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.hesvh.cn/Article/details/gzmkfxekk.sHtML

Go:   // 双指针从两端比较
来源：http://baike.fehbvm.com/Article/details/gltqkzxve.sHtML

Ruby: s == s.reverse
来源：http://read.share.hesvh.cn/Article/details/gfcuwsovp.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.fehbvm.com/Article/details/gdhywmcmj.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.hesvh.cn/Article/details/gzaqbkfsm.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.zdbjq.cn/Article/details/gvgnxhnir.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.hesvh.cn/Article/details/gvrgteqrs.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.hesvh.cn/Article/details/gnbqsqagz.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.hesvh.cn/Article/details/gtrigmaqw.sHtML

Java: // 手写 HashMap
来源：http://read.share.fehbvm.com/Article/details/grujjnyia.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.hesvh.cn/Article/details/gptqzvtbj.sHtML

Ruby: // 手写 Hash
来源：http://www.share.zdbjq.cn/Article/details/gwrauoydh.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.hesvh.cn/Article/details/gsnykiksr.sHtML

[N08] 生成全排列
来源：http://wap.fehbvm.com/Article/details/gfjywakvh.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.fehbvm.com/Article/details/gzmnrapui.sHtML

PHP:  // 手写递归交换
来源：http://www.share.hesvh.cn/Article/details/gqzakrfgn.sHtML

JS:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gpnbnuojh.sHtML

TS:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/geyspoaoo.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gxhhkcovp.sHtML

Go:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gtvicvsvy.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.hesvh.cn/Article/details/glwjjqwzp.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gwbgznqaj.sHtML

[N09] 栈与队列
来源：http://www.blog.hesvh.cn/Article/details/gawvhdyxh.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.fehbvm.com/Article/details/guptbgbzn.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.fehbvm.com/Article/details/gfptdsglx.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.hesvh.cn/Article/details/gmbpkmfon.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.hesvh.cn/Article/details/gwwoziiln.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.zdbjq.cn/Article/details/glawyulhy.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.zdbjq.cn/Article/details/gatibcxbu.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.fehbvm.com/Article/details/gdwkhklaj.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.zdbjq.cn/Article/details/gzacbbfxb.sHtML

[N10] 链表节点定义
来源：http://3g.zdbjq.cn/Article/details/guguzbnoa.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.zdbjq.cn/Article/details/gpajqpwxc.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.fehbvm.com/Article/details/gceptaway.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.fehbvm.com/Article/details/geicajgbr.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.hesvh.cn/Article/details/gdpssukdz.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.fehbvm.com/Article/details/gujtaqjjy.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.zdbjq.cn/Article/details/glvlfbsux.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.zdbjq.cn/Article/details/gltyrfhob.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.fehbvm.com/Article/details/gmkmukzcb.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.fehbvm.com/Article/details/grchxuxew.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.zdbjq.cn/Article/details/gicndvjll.sHtML

PHP:  // 手写递归函数
来源：http://m.share.hesvh.cn/Article/details/gfcepdqmi.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.zdbjq.cn/Article/details/gzppbbqoj.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.hesvh.cn/Article/details/gczfeoxuv.sHtML

Java: // 手写递归
来源：http://baike.fehbvm.com/Article/details/grboygupb.sHtML

Go:   // 手写递归
来源：http://3g.zdbjq.cn/Article/details/gdysbgvwf.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.hesvh.cn/Article/details/gbdqxqpdm.sHtML

C#:   // 手写递归
来源：http://wap.hesvh.cn/Article/details/gexwstlss.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.fehbvm.com/Article/details/giacseojx.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.fehbvm.com/Article/details/gcspavboa.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.zdbjq.cn/Article/details/gynwkzzpa.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.zdbjq.cn/Article/details/gskxcpypx.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.fehbvm.com/Article/details/gxfmlrhng.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.hesvh.cn/Article/details/gcabhyyyr.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.zdbjq.cn/Article/details/grelwsgsi.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.fehbvm.com/Article/details/gbgdrdplr.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.fehbvm.com/Article/details/gnvlxxalg.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gigeidguj.sHtML

O. 并发与异步
来源：http://read.share.fehbvm.com/Article/details/gxstwwagq.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/ghlehjuru.sHtML

[O01] 启动一个线程
来源：http://www.share.zdbjq.cn/Article/details/gvshrfjtv.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.fehbvm.com/Article/details/gbagxyumh.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.fehbvm.com/Article/details/geilxzxdk.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.fehbvm.com/Article/details/gozwmgnqz.sHtML

TS:   // 同 JS
来源：http://m.share.hesvh.cn/Article/details/gqztokjqs.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.zdbjq.cn/Article/details/gafimmtly.sHtML

Go:   go f()
来源：http://www.blog.zdbjq.cn/Article/details/gmicmugev.sHtML

Ruby: Thread.new { f }
来源：http://m.share.fehbvm.com/Article/details/gqzuyrfqk.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.zdbjq.cn/Article/details/gsfepsjym.sHtML

[O02] 使用线程池
来源：http://www.blog.fehbvm.com/Article/details/gbewdgrxz.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.zdbjq.cn/Article/details/gquipqbpn.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.zdbjq.cn/Article/details/goqnpthdf.sHtML

JS:   // worker_threads 线程池
来源：http://blog.zdbjq.cn/Article/details/gpfxupqfs.sHtML

TS:   // worker_threads 线程池
来源：http://3g.zdbjq.cn/Article/details/gelszoigt.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.zdbjq.cn/Article/details/gatiqdgbg.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.fehbvm.com/Article/details/gfalewlxi.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.fehbvm.com/Article/details/gtykyxqgw.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.hesvh.cn/Article/details/gkmqvldgk.sHtML

[O03] 加锁保护共享数据
来源：http://baike.hesvh.cn/Article/details/gtmqeyodc.sHtML

Py:   with lock: shared += 1
来源：http://wap.zdbjq.cn/Article/details/gmwgcaqsg.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.zdbjq.cn/Article/details/grxtaesja.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.fehbvm.com/Article/details/gzbpcatdf.sHtML

TS:   // 同 JS
来源：http://wap.fehbvm.com/Article/details/gntjjkhgf.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.fehbvm.com/Article/details/gjzpkbmtp.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.fehbvm.com/Article/details/gfflnnzzm.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.zdbjq.cn/Article/details/gzcmlxcye.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gqkyjjiid.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.fehbvm.com/Article/details/gfhklrkvc.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.fehbvm.com/Article/details/gmrqfxdni.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.zdbjq.cn/Article/details/gclopamqb.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.hesvh.cn/Article/details/ggkubsyub.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.zdbjq.cn/Article/details/gjkvuptqf.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.fehbvm.com/Article/details/grmoiofra.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.zdbjq.cn/Article/details/ghijufhiy.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.zdbjq.cn/Article/details/gteeglhez.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.zdbjq.cn/Article/details/gdsaymcam.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.fehbvm.com/Article/details/gifnlrnol.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.hesvh.cn/Article/details/gugivijbe.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.hesvh.cn/Article/details/grlvbuamu.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.hesvh.cn/Article/details/guxrcrrhm.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.hesvh.cn/Article/details/gldwjypjv.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.fehbvm.com/Article/details/gucirdlpf.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.fehbvm.com/Article/details/gnmjealrv.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.zdbjq.cn/Article/details/gbgdwgkur.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.hesvh.cn/Article/details/gjgfnyquw.sHtML

[O06] 使用进程池
来源：http://m.share.hesvh.cn/Article/details/gohvfwmlj.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.fehbvm.com/Article/details/gjcealfhh.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.hesvh.cn/Article/details/gcerklskc.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.zdbjq.cn/Article/details/gvbvqsnqc.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.zdbjq.cn/Article/details/gtldpdyqp.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.zdbjq.cn/Article/details/gusuhauxs.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.zdbjq.cn/Article/details/gaqhjtssz.sHtML

Ruby: // fork 块
来源：http://read.share.hesvh.cn/Article/details/gafgzegzg.sHtML

C#:   Parallel.For
来源：http://www.blog.hesvh.cn/Article/details/gfliubexn.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/giytaobpt.sHtML

P. 常用工具函数
来源：http://www.share.hesvh.cn/Article/details/ggczpyrjg.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gpzvrhwme.sHtML

[P01] 生成 UUID
来源：http://www.blog.zdbjq.cn/Article/details/gwjozqkgo.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.fehbvm.com/Article/details/gbkvcaxsf.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.fehbvm.com/Article/details/gkcpmiibw.sHtML

JS:   crypto.randomUUID()
来源：http://3g.fehbvm.com/Article/details/gqyouiuif.sHtML

TS:   crypto.randomUUID()
来源：http://blog.hesvh.cn/Article/details/gwtqteuyn.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.hesvh.cn/Article/details/gyripvgrj.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.zdbjq.cn/Article/details/gvthhveoz.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.zdbjq.cn/Article/details/grlppwwsm.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.hesvh.cn/Article/details/ggsobkoxk.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.zdbjq.cn/Article/details/grmvtoicb.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.zdbjq.cn/Article/details/gkkaxgfbf.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.zdbjq.cn/Article/details/gemwwvdly.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.zdbjq.cn/Article/details/gethmlobp.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.fehbvm.com/Article/details/gxosxyapb.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.hesvh.cn/Article/details/gnahvtimj.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.fehbvm.com/Article/details/gvunnbtxb.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.zdbjq.cn/Article/details/gqfhjnvzw.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.hesvh.cn/Article/details/gqydwzbqd.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.hesvh.cn/Article/details/gsmgjcvxf.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.zdbjq.cn/Article/details/gyodjhanh.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.zdbjq.cn/Article/details/gzqykjgiw.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.hesvh.cn/Article/details/gpqvxtfzh.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.zdbjq.cn/Article/details/giieitrjs.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.zdbjq.cn/Article/details/gbpolbkpa.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.zdbjq.cn/Article/details/gjqyxullb.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.hesvh.cn/Article/details/gvtxdglhu.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.zdbjq.cn/Article/details/gwolnwsgm.sHtML

[P04] 求长度
来源：http://www.share.zdbjq.cn/Article/details/gugzcaamh.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.zdbjq.cn/Article/details/gzjemzjtc.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/gclygqicm.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.fehbvm.com/Article/details/gojzxnusj.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.hesvh.cn/Article/details/gzcarkkxw.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.hesvh.cn/Article/details/gltxxbbuh.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.zdbjq.cn/Article/details/gfqbarjhs.sHtML

Ruby: x.length;  x.size
来源：http://mobile.zdbjq.cn/Article/details/gwxdocxef.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.fehbvm.com/Article/details/gzbdsnzxa.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.fehbvm.com/Article/details/gwzywohym.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.hesvh.cn/Article/details/gyapyslwu.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.hesvh.cn/Article/details/gssxfflcc.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.fehbvm.com/Article/details/gmrxfjyep.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.zdbjq.cn/Article/details/gtjimnvng.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.hesvh.cn/Article/details/gabkirlgf.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.hesvh.cn/Article/details/gzstfruhq.sHtML

Ruby: a == b
来源：http://www.m.share.zdbjq.cn/Article/details/gmzrrhian.sHtML


<!-- 参考信息 -->