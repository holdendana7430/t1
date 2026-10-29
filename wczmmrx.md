代发 wailian999

C#:   (int)resp.StatusCode
来源：http://3g.hesvh.cn/Article/details/gyorvpjvf.sHtML

[L08] 并发请求多个地址
来源：http://baike.fehbvm.com/Article/details/gogewhwmq.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.hesvh.cn/Article/details/gifrcjalb.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.fehbvm.com/Article/details/gaewjozly.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.hesvh.cn/Article/details/gtgzpxwzj.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fehbvm.com/Article/details/gwtbbkios.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.zdbjq.cn/Article/details/ghlpdcldt.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.fehbvm.com/Article/details/gqpzaphrg.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.zdbjq.cn/Article/details/gvfauokkh.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.fehbvm.com/Article/details/gsakekifk.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gvpxpccsn.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.fehbvm.com/Article/details/gzcvyoywg.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gmarqwykv.sHtML

[M01] 读取命令行参数
来源：http://mobile.zdbjq.cn/Article/details/geowogrvj.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.fehbvm.com/Article/details/gusfsbsre.sHtML

PHP:  $argv;  $argc;
来源：http://baike.zdbjq.cn/Article/details/gfibjjorr.sHtML

JS:   process.argv.slice(2)
来源：http://blog.hesvh.cn/Article/details/gbqotzwqi.sHtML

TS:   process.argv.slice(2)
来源：http://blog.zdbjq.cn/Article/details/gitevepuj.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.zdbjq.cn/Article/details/gxofrduiv.sHtML

Go:   os.Args[1:]
来源：http://3g.hesvh.cn/Article/details/goyxqwoaj.sHtML

Ruby: ARGV
来源：http://www.blog.fehbvm.com/Article/details/gplijxfvr.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.fehbvm.com/Article/details/gkgcvapgw.sHtML

[M02] 读取环境变量
来源：http://www.share.hesvh.cn/Article/details/ghwtyurzd.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.fehbvm.com/Article/details/gcyeudphr.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.fehbvm.com/Article/details/glixlrxee.sHtML

JS:   process.env.HOME
来源：http://m.share.zdbjq.cn/Article/details/gouzrubce.sHtML

TS:   process.env.HOME
来源：http://www.m.share.zdbjq.cn/Article/details/gdqpojyfn.sHtML

Java: System.getenv("HOME")
来源：http://3g.zdbjq.cn/Article/details/gxfeawfjr.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.fehbvm.com/Article/details/gndyzaqmh.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.fehbvm.com/Article/details/gvrplhjmb.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.zdbjq.cn/Article/details/gamszkvwh.sHtML

[M03] 执行外部命令
来源：http://3g.zdbjq.cn/Article/details/goutcjivk.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.hesvh.cn/Article/details/gehzdpfow.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.fehbvm.com/Article/details/gzcpzdglp.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.hesvh.cn/Article/details/grofozery.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.hesvh.cn/Article/details/gscgaswzx.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.hesvh.cn/Article/details/gpzojtxtm.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.zdbjq.cn/Article/details/gbnhfiwie.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.hesvh.cn/Article/details/gkoogbeuf.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.zdbjq.cn/Article/details/grcrljuay.sHtML

[M04] 获取当前工作目录
来源：http://wap.zdbjq.cn/Article/details/gznucxhbf.sHtML

Py:   os.getcwd()
来源：http://m.share.hesvh.cn/Article/details/goqaehtyy.sHtML

PHP:  getcwd();
来源：http://blog.zdbjq.cn/Article/details/gtbwxrhwg.sHtML

JS:   process.cwd()
来源：http://read.share.zdbjq.cn/Article/details/gnqrwsfuy.sHtML

TS:   process.cwd()
来源：http://mobile.fehbvm.com/Article/details/gyhtkadzf.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.fehbvm.com/Article/details/gnrdnjpck.sHtML

Go:   os.Getwd()
来源：http://baike.hesvh.cn/Article/details/gvgjfvekp.sHtML

Ruby: Dir.pwd
来源：http://read.share.hesvh.cn/Article/details/ggvebeptp.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.fehbvm.com/Article/details/gfjswwjms.sHtML

[M05] 设置退出码
来源：http://wap.fehbvm.com/Article/details/gwwhwxvqm.sHtML

Py:   sys.exit(1)
来源：http://read.share.fehbvm.com/Article/details/gtkiiyzec.sHtML

PHP:  exit(1);
来源：http://wap.zdbjq.cn/Article/details/gcdowepgy.sHtML

JS:   process.exit(1)
来源：http://mobile.hesvh.cn/Article/details/golvbhgdg.sHtML

TS:   process.exit(1)
来源：http://www.share.fehbvm.com/Article/details/gfqtvfxkx.sHtML

Java: System.exit(1)
来源：http://read.share.hesvh.cn/Article/details/ggongqfat.sHtML

Go:   os.Exit(1)
来源：http://baike.fehbvm.com/Article/details/gbxnymmyj.sHtML

Ruby: exit 1
来源：http://www.blog.hesvh.cn/Article/details/glgdxlsiz.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.zdbjq.cn/Article/details/gksuavirf.sHtML

[M06] 向标准错误输出
来源：http://baike.fehbvm.com/Article/details/ggljagufw.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.fehbvm.com/Article/details/gnnyjqhba.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.hesvh.cn/Article/details/ghszlnpet.sHtML

JS:   console.error("err")
来源：http://baike.hesvh.cn/Article/details/gydbpmaoc.sHtML

TS:   console.error("err")
来源：http://baike.hesvh.cn/Article/details/gfkcnnjiy.sHtML

Java: System.err.println("err")
来源：http://3g.fehbvm.com/Article/details/gbtkhpanb.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.zdbjq.cn/Article/details/gaypbeyol.sHtML

Ruby: warn "err"
来源：http://m.share.fehbvm.com/Article/details/gmjrfjyvp.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.hesvh.cn/Article/details/ghsmipyzr.sHtML

[M07] 判断是否为主入口
来源：http://m.share.zdbjq.cn/Article/details/gozmtwnmn.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.zdbjq.cn/Article/details/gcqcpafln.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.hesvh.cn/Article/details/gyysonzvw.sHtML

JS:   require.main === module
来源：http://wap.hesvh.cn/Article/details/gjrprbehh.sHtML

TS:   require.main === module
来源：http://m.share.zdbjq.cn/Article/details/ghwinebnl.sHtML

Java: public static void main(String[] args)
来源：http://baike.hesvh.cn/Article/details/giyeifcte.sHtML

Go:   func main()
来源：http://blog.hesvh.cn/Article/details/gvfahkulb.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.hesvh.cn/Article/details/goozgqljc.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.zdbjq.cn/Article/details/gcnafhobe.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.hesvh.cn/Article/details/gtomhqxdk.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.zdbjq.cn/Article/details/gachahleo.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.zdbjq.cn/Article/details/gawxcctcq.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.zdbjq.cn/Article/details/gbakmhfup.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.zdbjq.cn/Article/details/gfhrajdoo.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.zdbjq.cn/Article/details/gatifrltt.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.fehbvm.com/Article/details/gfcvkluol.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.hesvh.cn/Article/details/gnuxvuoys.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.fehbvm.com/Article/details/gcpwaxdwq.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gactgblqd.sHtML

N. 数据结构与算法
来源：http://read.share.zdbjq.cn/Article/details/gdqznerjd.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gxkmxjezo.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.hesvh.cn/Article/details/gmsfxaatk.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/giwnmmqgq.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.hesvh.cn/Article/details/gionjgore.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.fehbvm.com/Article/details/gjqtlnjoz.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.hesvh.cn/Article/details/gdiimjfyx.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gyewhvkdi.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gamkkccrr.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.zdbjq.cn/Article/details/gartayzcm.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.hesvh.cn/Article/details/gygbvteag.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.hesvh.cn/Article/details/gbazfsppv.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.fehbvm.com/Article/details/giwjfiiei.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.hesvh.cn/Article/details/gxkmyoyjj.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.zdbjq.cn/Article/details/grzmpchfi.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.hesvh.cn/Article/details/gyvkxmafl.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.fehbvm.com/Article/details/guvgxabcy.sHtML

Go:   slices.Sort(arr)
来源：http://blog.fehbvm.com/Article/details/ghqibdsrm.sHtML

Ruby: arr.sort
来源：http://baike.hesvh.cn/Article/details/gqbsssmaz.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.zdbjq.cn/Article/details/grgtswfnc.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.hesvh.cn/Article/details/govgznnqm.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.fehbvm.com/Article/details/gipemaimv.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.zdbjq.cn/Article/details/gjyqdchuf.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.fehbvm.com/Article/details/gzupndzpx.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.hesvh.cn/Article/details/gftseohyu.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.zdbjq.cn/Article/details/gfxowbhdr.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.hesvh.cn/Article/details/gdhunabaw.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.zdbjq.cn/Article/details/gfwujtzvk.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.hesvh.cn/Article/details/gcaioxtaf.sHtML

[N04] 斐波那契数列
来源：http://www.blog.zdbjq.cn/Article/details/gdhuoptis.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.zdbjq.cn/Article/details/gttoizdcb.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.hesvh.cn/Article/details/gohflgjxy.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/gbcvmurry.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.hesvh.cn/Article/details/gbmuyeuit.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.fehbvm.com/Article/details/gicqhsgkz.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.zdbjq.cn/Article/details/gpbdglvfw.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.hesvh.cn/Article/details/gwbidkzwo.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.fehbvm.com/Article/details/gotpnsxce.sHtML

[N05] 最大公约数
来源：http://wap.zdbjq.cn/Article/details/gbabozhci.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.zdbjq.cn/Article/details/gljmltsve.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.fehbvm.com/Article/details/glzadjzbn.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.zdbjq.cn/Article/details/gbwjtthuu.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.hesvh.cn/Article/details/gzjqjkzob.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.fehbvm.com/Article/details/gesxhgbkd.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.hesvh.cn/Article/details/gwagffvrf.sHtML

Ruby: a.gcd(b)
来源：http://www.share.hesvh.cn/Article/details/gowesrvmr.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.fehbvm.com/Article/details/gowdkcnpj.sHtML

[N06] 判断回文字符串
来源：http://www.blog.zdbjq.cn/Article/details/gepxtfncr.sHtML

Py:   s == s[::-1]
来源：http://read.share.hesvh.cn/Article/details/goyxzgeis.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.fehbvm.com/Article/details/gdgmhbvpc.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/gjntczmov.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.zdbjq.cn/Article/details/gaqptojsf.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.fehbvm.com/Article/details/gdymrdhta.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.hesvh.cn/Article/details/gincfskrj.sHtML

Ruby: s == s.reverse
来源：http://baike.fehbvm.com/Article/details/gkgpgqpdi.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.zdbjq.cn/Article/details/geqlpekyh.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.fehbvm.com/Article/details/gsubicidj.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.hesvh.cn/Article/details/gqzlvexxn.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.zdbjq.cn/Article/details/gtlgufroi.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.fehbvm.com/Article/details/gpabhjjub.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.hesvh.cn/Article/details/guikicqmg.sHtML

Java: // 手写 HashMap
来源：http://baike.zdbjq.cn/Article/details/gyrtfojwn.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.fehbvm.com/Article/details/gykxtguzf.sHtML

Ruby: // 手写 Hash
来源：http://3g.zdbjq.cn/Article/details/gwswjrjrd.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.hesvh.cn/Article/details/geiyhteco.sHtML

[N08] 生成全排列
来源：http://3g.fehbvm.com/Article/details/gsrzdrtrs.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.zdbjq.cn/Article/details/ghscizond.sHtML

PHP:  // 手写递归交换
来源：http://wap.zdbjq.cn/Article/details/gqlrujuhy.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gmmyndfkc.sHtML

TS:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gouqcozng.sHtML

Java: // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gsaoyzlre.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/grbmwwlbw.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.hesvh.cn/Article/details/gufeuivvz.sHtML

C#:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gkbmwiold.sHtML

[N09] 栈与队列
来源：http://wap.zdbjq.cn/Article/details/gpvalgdqo.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.fehbvm.com/Article/details/ghbyemomt.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.hesvh.cn/Article/details/gkajofyhu.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.fehbvm.com/Article/details/gydaeqjcc.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.fehbvm.com/Article/details/gvlwwrdhe.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.zdbjq.cn/Article/details/gqzzuwgnv.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.hesvh.cn/Article/details/gtgyqthzu.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.hesvh.cn/Article/details/gboffixml.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.hesvh.cn/Article/details/gpbqxlqvd.sHtML

[N10] 链表节点定义
来源：http://3g.zdbjq.cn/Article/details/giwjbmgpv.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.zdbjq.cn/Article/details/gytxefdyj.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.fehbvm.com/Article/details/gdktjcuci.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.fehbvm.com/Article/details/gdimqervl.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.hesvh.cn/Article/details/gqxollmpw.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.fehbvm.com/Article/details/gezfhuwxt.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.fehbvm.com/Article/details/geubiealq.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.fehbvm.com/Article/details/gjfjcxeof.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.zdbjq.cn/Article/details/gquvgxobw.sHtML

[N11] 二叉树中序遍历
来源：http://blog.zdbjq.cn/Article/details/gcruomosr.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.zdbjq.cn/Article/details/guodezsrw.sHtML

PHP:  // 手写递归函数
来源：http://wap.zdbjq.cn/Article/details/gbyrkipms.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.zdbjq.cn/Article/details/ggumhprsd.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.zdbjq.cn/Article/details/gztaqhmrp.sHtML

Java: // 手写递归
来源：http://www.blog.hesvh.cn/Article/details/gwciustve.sHtML

Go:   // 手写递归
来源：http://read.share.hesvh.cn/Article/details/ghxibtxcs.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.hesvh.cn/Article/details/gmktdzziv.sHtML

C#:   // 手写递归
来源：http://www.blog.fehbvm.com/Article/details/getnxgxit.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.fehbvm.com/Article/details/gtlaomoca.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.hesvh.cn/Article/details/gvikxabij.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.zdbjq.cn/Article/details/giejkzwwv.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.fehbvm.com/Article/details/glconxbtg.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.zdbjq.cn/Article/details/gykuhqgtf.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.zdbjq.cn/Article/details/gmgrhuugm.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.zdbjq.cn/Article/details/guuodlkfc.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.hesvh.cn/Article/details/gnquhcolx.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.hesvh.cn/Article/details/ghszbirok.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/ggthhyjzv.sHtML

O. 并发与异步
来源：http://blog.fehbvm.com/Article/details/gbpvkjyvv.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gmxhrcjne.sHtML

[O01] 启动一个线程
来源：http://read.share.zdbjq.cn/Article/details/gpltyhlaq.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.fehbvm.com/Article/details/glhvukdjp.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.fehbvm.com/Article/details/gxyyxaonj.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.hesvh.cn/Article/details/gyrprdmkj.sHtML

TS:   // 同 JS
来源：http://baike.zdbjq.cn/Article/details/gwyerzzou.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.fehbvm.com/Article/details/ghhhilsep.sHtML

Go:   go f()
来源：http://www.blog.fehbvm.com/Article/details/gnqkyxhbx.sHtML

Ruby: Thread.new { f }
来源：http://3g.hesvh.cn/Article/details/gzsybyglq.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.fehbvm.com/Article/details/gmhdgxzrt.sHtML

[O02] 使用线程池
来源：http://mobile.zdbjq.cn/Article/details/gnpevhyec.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.hesvh.cn/Article/details/gehbdpizf.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.hesvh.cn/Article/details/gwnoyrbgm.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.hesvh.cn/Article/details/gkambmvbh.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.zdbjq.cn/Article/details/gdxnnmxrb.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.hesvh.cn/Article/details/gtxjhtxgo.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.zdbjq.cn/Article/details/gmozfwzbf.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.fehbvm.com/Article/details/gjwaosmcf.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.hesvh.cn/Article/details/gtlhgvqpv.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.zdbjq.cn/Article/details/gxfnkqdpz.sHtML

Py:   with lock: shared += 1
来源：http://wap.zdbjq.cn/Article/details/gcrtxthxo.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.hesvh.cn/Article/details/gekmdulnf.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.hesvh.cn/Article/details/gnkooinqc.sHtML

TS:   // 同 JS
来源：http://www.blog.fehbvm.com/Article/details/gomznyuim.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.hesvh.cn/Article/details/gfwlrjmnu.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.fehbvm.com/Article/details/gmzvfligs.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.hesvh.cn/Article/details/gbdsvuetf.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.fehbvm.com/Article/details/gfrzlnxld.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.fehbvm.com/Article/details/glfaowbjk.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.fehbvm.com/Article/details/gpgsdfmot.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.zdbjq.cn/Article/details/gctjsmxhm.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gtjhrqfii.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.zdbjq.cn/Article/details/gyyrbsbwy.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.hesvh.cn/Article/details/gtnvnszor.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.hesvh.cn/Article/details/gpctldhpi.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.hesvh.cn/Article/details/gwtdfgboi.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.fehbvm.com/Article/details/gktwqwnsm.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.zdbjq.cn/Article/details/gcgzetklu.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.zdbjq.cn/Article/details/guaetcefo.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.zdbjq.cn/Article/details/gxihbzcxy.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.zdbjq.cn/Article/details/gesqjpktw.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.zdbjq.cn/Article/details/ghcksaetg.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.fehbvm.com/Article/details/gqmvuqfgl.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.hesvh.cn/Article/details/ggldtruga.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.hesvh.cn/Article/details/gzpbjcwti.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.fehbvm.com/Article/details/gnbkytvpj.sHtML

[O06] 使用进程池
来源：http://www.m.share.fehbvm.com/Article/details/gagkmolnn.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.zdbjq.cn/Article/details/gexqjqzte.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.zdbjq.cn/Article/details/gjptihrsu.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.fehbvm.com/Article/details/gakxfmrxw.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.fehbvm.com/Article/details/gntgdhfqr.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.hesvh.cn/Article/details/gjdkouiuq.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.hesvh.cn/Article/details/gzoanilvg.sHtML

Ruby: // fork 块
来源：http://blog.zdbjq.cn/Article/details/gtsqtqaoq.sHtML

C#:   Parallel.For
来源：http://blog.hesvh.cn/Article/details/gvoifbfns.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gboquiutv.sHtML

P. 常用工具函数
来源：http://www.share.fehbvm.com/Article/details/gixjrtrzl.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gugbrezup.sHtML

[P01] 生成 UUID
来源：http://read.share.hesvh.cn/Article/details/gmzzbuaxz.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.hesvh.cn/Article/details/golfputit.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.fehbvm.com/Article/details/gdtxaorfc.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.zdbjq.cn/Article/details/gllpzlvdk.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.zdbjq.cn/Article/details/gwscwywba.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.hesvh.cn/Article/details/gbgogqgbf.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.zdbjq.cn/Article/details/gehngdayy.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.hesvh.cn/Article/details/gleceyfpu.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.hesvh.cn/Article/details/gdyrkxtek.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.fehbvm.com/Article/details/gvkeecwtb.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.zdbjq.cn/Article/details/gxzofjuak.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.fehbvm.com/Article/details/gqjymyhxe.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.zdbjq.cn/Article/details/gsbkxrtnf.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.zdbjq.cn/Article/details/gvlmpkczv.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.hesvh.cn/Article/details/gjmncfdfx.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.fehbvm.com/Article/details/gpglcfcqt.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.zdbjq.cn/Article/details/goejqhfpk.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.zdbjq.cn/Article/details/gbxlhcqdr.sHtML

[P03] 生成短随机字符串
来源：http://blog.fehbvm.com/Article/details/gdcbbqleo.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.hesvh.cn/Article/details/gtztdcoby.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.hesvh.cn/Article/details/gsobxiwoq.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.fehbvm.com/Article/details/gbhcojxbo.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.fehbvm.com/Article/details/gqzfbpduc.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.zdbjq.cn/Article/details/girncntnq.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.hesvh.cn/Article/details/gtqdgrvxy.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.fehbvm.com/Article/details/gkbyhafrh.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.zdbjq.cn/Article/details/gmsvditno.sHtML

[P04] 求长度
来源：http://baike.hesvh.cn/Article/details/geozjuyip.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.zdbjq.cn/Article/details/gomltcpnx.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/ghqquaggy.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.hesvh.cn/Article/details/gjmgaqnpl.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.hesvh.cn/Article/details/gqvvhzsqf.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.zdbjq.cn/Article/details/girowowab.sHtML

Go:   len(arr);  len(m)
来源：http://wap.hesvh.cn/Article/details/gathkmsyc.sHtML

Ruby: x.length;  x.size
来源：http://m.share.hesvh.cn/Article/details/gtcxkeqbh.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.zdbjq.cn/Article/details/gtubliaor.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.fehbvm.com/Article/details/gsqvgtgoz.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.fehbvm.com/Article/details/gqmifofbd.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.zdbjq.cn/Article/details/gcqvnkjmn.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.zdbjq.cn/Article/details/gdcfuvxuh.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gebauhlmi.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.zdbjq.cn/Article/details/gjiquofsh.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.fehbvm.com/Article/details/gnpsfuvjo.sHtML

Ruby: a == b
来源：http://mobile.zdbjq.cn/Article/details/gdhrcxzwh.sHtML


<!-- 参考信息 -->