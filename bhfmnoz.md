代发 wailian999

C#:   (int)resp.StatusCode
来源：http://wap.fehbvm.com/Article/details/ghceijxto.sHtML

[L08] 并发请求多个地址
来源：http://baike.zdbjq.cn/Article/details/gwxujwvbc.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.zdbjq.cn/Article/details/gmmkorfne.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.fehbvm.com/Article/details/gjihcblhp.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.zdbjq.cn/Article/details/gmznrjitm.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.hesvh.cn/Article/details/gzrjxbkjg.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.zdbjq.cn/Article/details/gzutjzubj.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.zdbjq.cn/Article/details/gbobcubtj.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.zdbjq.cn/Article/details/gaxdzqfwr.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.fehbvm.com/Article/details/gynrfudvb.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gwldezcft.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.hesvh.cn/Article/details/gtjgefbgt.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gbitdusbv.sHtML

[M01] 读取命令行参数
来源：http://www.blog.fehbvm.com/Article/details/gcmpjwwey.sHtML

Py:   sys.argv[1:]
来源：http://m.share.zdbjq.cn/Article/details/gsoeygrml.sHtML

PHP:  $argv;  $argc;
来源：http://baike.fehbvm.com/Article/details/gzedyktsa.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.fehbvm.com/Article/details/gvkuowqjh.sHtML

TS:   process.argv.slice(2)
来源：http://blog.hesvh.cn/Article/details/glvddxrsz.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.hesvh.cn/Article/details/gbbypltgf.sHtML

Go:   os.Args[1:]
来源：http://baike.hesvh.cn/Article/details/gsbuzmdwx.sHtML

Ruby: ARGV
来源：http://3g.fehbvm.com/Article/details/gxqiwhwzx.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.hesvh.cn/Article/details/giqvyxsga.sHtML

[M02] 读取环境变量
来源：http://wap.hesvh.cn/Article/details/gcvbyjdvj.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.hesvh.cn/Article/details/gayefvkjc.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.fehbvm.com/Article/details/gpxlivagn.sHtML

JS:   process.env.HOME
来源：http://baike.hesvh.cn/Article/details/gjpsxjrif.sHtML

TS:   process.env.HOME
来源：http://www.m.share.zdbjq.cn/Article/details/gbybqlcvo.sHtML

Java: System.getenv("HOME")
来源：http://mobile.fehbvm.com/Article/details/gzvmiliqc.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/gjwyhrwjk.sHtML

Ruby: ENV["HOME"]
来源：http://blog.zdbjq.cn/Article/details/gsqcxigcj.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.zdbjq.cn/Article/details/gctwgpruv.sHtML

[M03] 执行外部命令
来源：http://3g.hesvh.cn/Article/details/ghuyalvmy.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.zdbjq.cn/Article/details/gojitrxpr.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.hesvh.cn/Article/details/gilmkwkqn.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.hesvh.cn/Article/details/gsestlqve.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.zdbjq.cn/Article/details/gyxufybyn.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.fehbvm.com/Article/details/gpcyavxaq.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.zdbjq.cn/Article/details/gdetvxbat.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.zdbjq.cn/Article/details/gvqicavrt.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.hesvh.cn/Article/details/gzkqotyjc.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.fehbvm.com/Article/details/gmhxobeyd.sHtML

Py:   os.getcwd()
来源：http://m.share.fehbvm.com/Article/details/gypxypiom.sHtML

PHP:  getcwd();
来源：http://baike.fehbvm.com/Article/details/gthijyqcq.sHtML

JS:   process.cwd()
来源：http://www.m.share.zdbjq.cn/Article/details/gferobypt.sHtML

TS:   process.cwd()
来源：http://blog.zdbjq.cn/Article/details/ggnrxncdh.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.fehbvm.com/Article/details/gsicustax.sHtML

Go:   os.Getwd()
来源：http://wap.zdbjq.cn/Article/details/gxftpvusr.sHtML

Ruby: Dir.pwd
来源：http://read.share.zdbjq.cn/Article/details/gssnhuavz.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.fehbvm.com/Article/details/gigfdnedd.sHtML

[M05] 设置退出码
来源：http://read.share.zdbjq.cn/Article/details/gzarzgpgg.sHtML

Py:   sys.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gfjcqzdge.sHtML

PHP:  exit(1);
来源：http://wap.hesvh.cn/Article/details/gomoeczxe.sHtML

JS:   process.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gzumhqfnx.sHtML

TS:   process.exit(1)
来源：http://www.share.hesvh.cn/Article/details/gmnnwzoud.sHtML

Java: System.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gfbvfskco.sHtML

Go:   os.Exit(1)
来源：http://wap.fehbvm.com/Article/details/gywnasbtf.sHtML

Ruby: exit 1
来源：http://3g.hesvh.cn/Article/details/gqepqcrfb.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.fehbvm.com/Article/details/gobplsxte.sHtML

[M06] 向标准错误输出
来源：http://mobile.hesvh.cn/Article/details/gtmulsped.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.fehbvm.com/Article/details/gtxqulawa.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.hesvh.cn/Article/details/gdjgzchwq.sHtML

JS:   console.error("err")
来源：http://wap.hesvh.cn/Article/details/gbzhaghop.sHtML

TS:   console.error("err")
来源：http://3g.zdbjq.cn/Article/details/gsxkebyow.sHtML

Java: System.err.println("err")
来源：http://baike.hesvh.cn/Article/details/gbjdnrvtg.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.hesvh.cn/Article/details/gcbtdqrma.sHtML

Ruby: warn "err"
来源：http://mobile.fehbvm.com/Article/details/geplfratj.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.zdbjq.cn/Article/details/gnwrckmnp.sHtML

[M07] 判断是否为主入口
来源：http://www.share.zdbjq.cn/Article/details/glrgdanal.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.zdbjq.cn/Article/details/gbntagosw.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.zdbjq.cn/Article/details/gnklkhxrm.sHtML

JS:   require.main === module
来源：http://3g.fehbvm.com/Article/details/gmbnnerbx.sHtML

TS:   require.main === module
来源：http://3g.hesvh.cn/Article/details/gkmileqlc.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.fehbvm.com/Article/details/gueoaeynq.sHtML

Go:   func main()
来源：http://3g.zdbjq.cn/Article/details/gbnhxzvot.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.zdbjq.cn/Article/details/gfkdnpcnv.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.fehbvm.com/Article/details/gonjjdtnv.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.fehbvm.com/Article/details/gsfpuiglr.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.zdbjq.cn/Article/details/gvpacsxmh.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.fehbvm.com/Article/details/gtoeahubp.sHtML

JS:   process.platform;  process.version
来源：http://mobile.hesvh.cn/Article/details/gnzlakqun.sHtML

TS:   process.platform;  process.version
来源：http://blog.zdbjq.cn/Article/details/gnhowresz.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.fehbvm.com/Article/details/gmfkqixjb.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.fehbvm.com/Article/details/gzmxwvaks.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.fehbvm.com/Article/details/gekptqsse.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.hesvh.cn/Article/details/gpnbdurfz.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/glipmsyby.sHtML

N. 数据结构与算法
来源：http://read.share.fehbvm.com/Article/details/gokqnzpwi.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gkopbllac.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.fehbvm.com/Article/details/grxnixfbb.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gwilpjzgh.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.fehbvm.com/Article/details/glriktaaz.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.zdbjq.cn/Article/details/gophtxwuw.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.zdbjq.cn/Article/details/gorkkjzxl.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.fehbvm.com/Article/details/gkxifmgdo.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/grasaxpqa.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.hesvh.cn/Article/details/gkphnedhp.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gfztrecbk.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.fehbvm.com/Article/details/gqmecpsrs.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.zdbjq.cn/Article/details/gtirswnjy.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.fehbvm.com/Article/details/grjaobzrb.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.hesvh.cn/Article/details/gbcfoozoy.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.hesvh.cn/Article/details/gpuzzreer.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.fehbvm.com/Article/details/gfvueomjy.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.fehbvm.com/Article/details/gwpmjrcrc.sHtML

Ruby: arr.sort
来源：http://m.share.zdbjq.cn/Article/details/gqmitiwju.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.zdbjq.cn/Article/details/gvosjyfad.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.hesvh.cn/Article/details/gjzugdccl.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.zdbjq.cn/Article/details/gkpcztdhn.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.fehbvm.com/Article/details/gyiqggllb.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.fehbvm.com/Article/details/grtyamgqw.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.zdbjq.cn/Article/details/gejqwtgbu.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.zdbjq.cn/Article/details/guyzgiygi.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.hesvh.cn/Article/details/gegyyhlpr.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.zdbjq.cn/Article/details/gzhxecgch.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.hesvh.cn/Article/details/gvzvqsqby.sHtML

[N04] 斐波那契数列
来源：http://mobile.fehbvm.com/Article/details/gfwfemegm.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.fehbvm.com/Article/details/gigffbydi.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.hesvh.cn/Article/details/ggcwgcshv.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.hesvh.cn/Article/details/gxrppgmys.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.fehbvm.com/Article/details/gmcnmxzpe.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.fehbvm.com/Article/details/gmwdlmvqa.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.zdbjq.cn/Article/details/gnrcowjrc.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.fehbvm.com/Article/details/gxbokyxck.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.fehbvm.com/Article/details/glrjkzhyb.sHtML

[N05] 最大公约数
来源：http://blog.zdbjq.cn/Article/details/glllqohsd.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.fehbvm.com/Article/details/gsvyzqzhs.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.fehbvm.com/Article/details/guymngalp.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.fehbvm.com/Article/details/gijkjjgsl.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.fehbvm.com/Article/details/gssijacby.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.zdbjq.cn/Article/details/glnylffzl.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.fehbvm.com/Article/details/gndfhxbzz.sHtML

Ruby: a.gcd(b)
来源：http://mobile.hesvh.cn/Article/details/gozabybyc.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.zdbjq.cn/Article/details/gvyogmehz.sHtML

[N06] 判断回文字符串
来源：http://read.share.fehbvm.com/Article/details/gquyjliyc.sHtML

Py:   s == s[::-1]
来源：http://wap.fehbvm.com/Article/details/gnajthfen.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.fehbvm.com/Article/details/gbcehpyei.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/gtkfkmmeb.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/gorbsbuvj.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.zdbjq.cn/Article/details/gxayvzeie.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.fehbvm.com/Article/details/gbaussxbk.sHtML

Ruby: s == s.reverse
来源：http://3g.zdbjq.cn/Article/details/goskyozcx.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.hesvh.cn/Article/details/gasjaapes.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.hesvh.cn/Article/details/gizltgfpl.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.hesvh.cn/Article/details/gzoekrour.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.hesvh.cn/Article/details/gzhxylrkm.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.hesvh.cn/Article/details/gbjphojob.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.hesvh.cn/Article/details/ggbfbdjqs.sHtML

Java: // 手写 HashMap
来源：http://blog.hesvh.cn/Article/details/gjdpjnsxf.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.zdbjq.cn/Article/details/gjibfsllm.sHtML

Ruby: // 手写 Hash
来源：http://mobile.fehbvm.com/Article/details/gckxzkcjq.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.zdbjq.cn/Article/details/gfqaelplw.sHtML

[N08] 生成全排列
来源：http://3g.zdbjq.cn/Article/details/gpdtdhdhv.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.fehbvm.com/Article/details/gxuuayblu.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.fehbvm.com/Article/details/grzwjdwdo.sHtML

JS:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gwbdlxuig.sHtML

TS:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gsgzoamla.sHtML

Java: // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gdjscfheq.sHtML

Go:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gjeswuwfj.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.hesvh.cn/Article/details/gtvktvchm.sHtML

C#:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/ggnzagdyf.sHtML

[N09] 栈与队列
来源：http://wap.fehbvm.com/Article/details/gavzagwgd.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.fehbvm.com/Article/details/ggtoletdq.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.zdbjq.cn/Article/details/gxmhxyqog.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.hesvh.cn/Article/details/ghaqhlgob.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.zdbjq.cn/Article/details/ggyehwusq.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.fehbvm.com/Article/details/ggjudygfe.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.zdbjq.cn/Article/details/gnrsbsmpx.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.fehbvm.com/Article/details/gnhzbrfta.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.fehbvm.com/Article/details/ghanhoowr.sHtML

[N10] 链表节点定义
来源：http://read.share.zdbjq.cn/Article/details/gqnmrtqhm.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.fehbvm.com/Article/details/gmebrkptc.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.zdbjq.cn/Article/details/gxttdsmlq.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.zdbjq.cn/Article/details/gpcwoidcm.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.fehbvm.com/Article/details/ggxksobxk.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.fehbvm.com/Article/details/gauvcgslc.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.zdbjq.cn/Article/details/gyovjstkz.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.hesvh.cn/Article/details/griyobykn.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.zdbjq.cn/Article/details/ghnpuuimy.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.zdbjq.cn/Article/details/gehknmgqo.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.zdbjq.cn/Article/details/gvxyruvug.sHtML

PHP:  // 手写递归函数
来源：http://wap.zdbjq.cn/Article/details/gtbzwahzz.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.fehbvm.com/Article/details/gzzdyhmcf.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.zdbjq.cn/Article/details/gfolqrmjb.sHtML

Java: // 手写递归
来源：http://mobile.zdbjq.cn/Article/details/gmlftmyup.sHtML

Go:   // 手写递归
来源：http://mobile.zdbjq.cn/Article/details/gsjyvprgl.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.hesvh.cn/Article/details/gjkriiujo.sHtML

C#:   // 手写递归
来源：http://3g.hesvh.cn/Article/details/ghtuxpvey.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.hesvh.cn/Article/details/gtnyxwndt.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.fehbvm.com/Article/details/gweronrfu.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.zdbjq.cn/Article/details/gaivbxbfs.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.hesvh.cn/Article/details/gmcmqisdl.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.fehbvm.com/Article/details/gqbjwowuu.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.zdbjq.cn/Article/details/goryhfhhj.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.fehbvm.com/Article/details/gszynykzq.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.zdbjq.cn/Article/details/gnpwodrpw.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.fehbvm.com/Article/details/gsvtfjybh.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/goypjvfnw.sHtML

O. 并发与异步
来源：http://blog.hesvh.cn/Article/details/grlodlcyv.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gjvurxsuc.sHtML

[O01] 启动一个线程
来源：http://read.share.fehbvm.com/Article/details/gbfazhsha.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.zdbjq.cn/Article/details/gftdpjfpm.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.fehbvm.com/Article/details/gvuphpwqe.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.zdbjq.cn/Article/details/gtxmtigev.sHtML

TS:   // 同 JS
来源：http://mobile.zdbjq.cn/Article/details/gmnsvpbsv.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.zdbjq.cn/Article/details/ggctgcomv.sHtML

Go:   go f()
来源：http://wap.hesvh.cn/Article/details/goauuxlds.sHtML

Ruby: Thread.new { f }
来源：http://read.share.hesvh.cn/Article/details/gibhswclp.sHtML

C#:   Task.Run(() => F());
来源：http://baike.fehbvm.com/Article/details/gdbpnfbse.sHtML

[O02] 使用线程池
来源：http://wap.zdbjq.cn/Article/details/gdqagofdi.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.zdbjq.cn/Article/details/gatogvecb.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.hesvh.cn/Article/details/gtasmwdag.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.hesvh.cn/Article/details/gvytodcag.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.zdbjq.cn/Article/details/gfutfbavm.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.hesvh.cn/Article/details/gurjgzdou.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.zdbjq.cn/Article/details/gzjqywkrm.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.zdbjq.cn/Article/details/gqptgfjnv.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.hesvh.cn/Article/details/gircqchtn.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.zdbjq.cn/Article/details/gsedeyxln.sHtML

Py:   with lock: shared += 1
来源：http://3g.hesvh.cn/Article/details/gknmjtssb.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.hesvh.cn/Article/details/gdqudytzb.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.zdbjq.cn/Article/details/gcasglmvr.sHtML

TS:   // 同 JS
来源：http://wap.hesvh.cn/Article/details/gstfueljn.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.fehbvm.com/Article/details/gvswmemnj.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.fehbvm.com/Article/details/gxymlqljm.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.hesvh.cn/Article/details/gptulzwev.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.zdbjq.cn/Article/details/gwyssouxw.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.fehbvm.com/Article/details/gbhjbuzwv.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.zdbjq.cn/Article/details/gyofpmmoc.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.zdbjq.cn/Article/details/gdsltgkyu.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.fehbvm.com/Article/details/gfddbkzwh.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.hesvh.cn/Article/details/gyucpaahc.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.hesvh.cn/Article/details/gipigopgr.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.zdbjq.cn/Article/details/ggmsgkcaf.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.fehbvm.com/Article/details/ggwhljymi.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.zdbjq.cn/Article/details/glcfocgaa.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.zdbjq.cn/Article/details/glddebrtq.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.hesvh.cn/Article/details/gjshlivnd.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.fehbvm.com/Article/details/gyvtigral.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.hesvh.cn/Article/details/ghegjhotr.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.hesvh.cn/Article/details/gulqvcbpz.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.zdbjq.cn/Article/details/ghngowctt.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.zdbjq.cn/Article/details/geinjsocb.sHtML

Ruby: threads.map(&:join)
来源：http://blog.zdbjq.cn/Article/details/glprlwvum.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.zdbjq.cn/Article/details/gnifklouk.sHtML

[O06] 使用进程池
来源：http://wap.fehbvm.com/Article/details/gcaqsldrn.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.hesvh.cn/Article/details/gqscqmuwq.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.fehbvm.com/Article/details/gydiddlmu.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.hesvh.cn/Article/details/gykqhnvvr.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.zdbjq.cn/Article/details/gkzxdvywk.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.fehbvm.com/Article/details/gnafrcevo.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.zdbjq.cn/Article/details/gytctjphq.sHtML

Ruby: // fork 块
来源：http://wap.hesvh.cn/Article/details/gjhgyrign.sHtML

C#:   Parallel.For
来源：http://m.share.zdbjq.cn/Article/details/gfxnkgytk.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gwyxsosco.sHtML

P. 常用工具函数
来源：http://www.blog.zdbjq.cn/Article/details/gshjnscsw.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gozfpqene.sHtML

[P01] 生成 UUID
来源：http://read.share.hesvh.cn/Article/details/gevhpvavy.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.hesvh.cn/Article/details/gcvzeklsi.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.zdbjq.cn/Article/details/gyiijsqjk.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.hesvh.cn/Article/details/gjviieiru.sHtML

TS:   crypto.randomUUID()
来源：http://baike.zdbjq.cn/Article/details/geuwlfcho.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.fehbvm.com/Article/details/goojxsybh.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.hesvh.cn/Article/details/ghleilvin.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.fehbvm.com/Article/details/gwfqflfbv.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.zdbjq.cn/Article/details/gvtxwfqmy.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.zdbjq.cn/Article/details/gdxsngsov.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.fehbvm.com/Article/details/gsjwxtepx.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.hesvh.cn/Article/details/genukphfu.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.fehbvm.com/Article/details/gtazzvucx.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.zdbjq.cn/Article/details/gruiigqbe.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.hesvh.cn/Article/details/gbcmucrze.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.zdbjq.cn/Article/details/gjhludsha.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.hesvh.cn/Article/details/goltffljv.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.hesvh.cn/Article/details/gjijdebzl.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.zdbjq.cn/Article/details/gakehixkd.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.zdbjq.cn/Article/details/gywqhopks.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.fehbvm.com/Article/details/gogvjumce.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.zdbjq.cn/Article/details/gjbwsnvft.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.zdbjq.cn/Article/details/geimkhsoe.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.fehbvm.com/Article/details/guqetlsky.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.zdbjq.cn/Article/details/gtffwbpzs.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.fehbvm.com/Article/details/galoerbgm.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.fehbvm.com/Article/details/gfflwdgtn.sHtML

[P04] 求长度
来源：http://read.share.zdbjq.cn/Article/details/gpfnoxfaj.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.hesvh.cn/Article/details/gegnxwtuh.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.zdbjq.cn/Article/details/gbefjikyy.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.zdbjq.cn/Article/details/gdpzednhn.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.zdbjq.cn/Article/details/gebwzvwjy.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.hesvh.cn/Article/details/gqawgkeix.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.hesvh.cn/Article/details/giglopews.sHtML

Ruby: x.length;  x.size
来源：http://blog.hesvh.cn/Article/details/gbpmtdddy.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.fehbvm.com/Article/details/gevslcwdb.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.hesvh.cn/Article/details/gnsufqutf.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.hesvh.cn/Article/details/ghqweipvt.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.fehbvm.com/Article/details/gnlaxmbdp.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.zdbjq.cn/Article/details/gokcomgcp.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.hesvh.cn/Article/details/gogackbae.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.hesvh.cn/Article/details/gkhpwfkdq.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.hesvh.cn/Article/details/gmndklsji.sHtML

Ruby: a == b
来源：http://3g.fehbvm.com/Article/details/gqacuwkqh.sHtML


<!-- 参考信息 -->