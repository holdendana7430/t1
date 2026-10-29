代发 wailian999

C#:   (int)resp.StatusCode
来源：http://www.m.share.fehbvm.com/Article/details/ghoksqqil.sHtML

[L08] 并发请求多个地址
来源：http://www.share.fehbvm.com/Article/details/goxyinvmz.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.zdbjq.cn/Article/details/gbxoqtyiv.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.fehbvm.com/Article/details/glnfoyaox.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.zdbjq.cn/Article/details/gtiovtyha.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fehbvm.com/Article/details/ghgysthnr.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.fehbvm.com/Article/details/gpoyqcddr.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.hesvh.cn/Article/details/gwgcglfoz.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.zdbjq.cn/Article/details/gdcnccwgj.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.zdbjq.cn/Article/details/gabtdcmgg.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gtlveeckv.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.fehbvm.com/Article/details/gdupawifw.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gwmsejvae.sHtML

[M01] 读取命令行参数
来源：http://www.share.fehbvm.com/Article/details/gchuhppdc.sHtML

Py:   sys.argv[1:]
来源：http://3g.zdbjq.cn/Article/details/girmxehod.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.hesvh.cn/Article/details/gyqbkhzcv.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.hesvh.cn/Article/details/gupgkygdq.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.hesvh.cn/Article/details/grroktvdq.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.zdbjq.cn/Article/details/gkjqhgnmn.sHtML

Go:   os.Args[1:]
来源：http://blog.fehbvm.com/Article/details/gctahkeff.sHtML

Ruby: ARGV
来源：http://baike.fehbvm.com/Article/details/gscmkhxkn.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.hesvh.cn/Article/details/gxnjibqtc.sHtML

[M02] 读取环境变量
来源：http://wap.fehbvm.com/Article/details/ghmzdfwam.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.hesvh.cn/Article/details/gmoalulmc.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.zdbjq.cn/Article/details/gobvflsxs.sHtML

JS:   process.env.HOME
来源：http://blog.hesvh.cn/Article/details/gaxyehjyc.sHtML

TS:   process.env.HOME
来源：http://3g.zdbjq.cn/Article/details/gdhjguuja.sHtML

Java: System.getenv("HOME")
来源：http://m.share.fehbvm.com/Article/details/gafbcztgk.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.zdbjq.cn/Article/details/gfxcxgkex.sHtML

Ruby: ENV["HOME"]
来源：http://3g.zdbjq.cn/Article/details/ghtaawgss.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.fehbvm.com/Article/details/gbinyjdqw.sHtML

[M03] 执行外部命令
来源：http://www.m.share.hesvh.cn/Article/details/grifjvirl.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.zdbjq.cn/Article/details/gzcydvxhh.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.zdbjq.cn/Article/details/gqpalrsjh.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.zdbjq.cn/Article/details/gfzppnvsy.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.hesvh.cn/Article/details/gcovwgurr.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.fehbvm.com/Article/details/gkekukzfp.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.fehbvm.com/Article/details/gasofirxu.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.hesvh.cn/Article/details/gymlinslj.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.fehbvm.com/Article/details/ghmouttzt.sHtML

[M04] 获取当前工作目录
来源：http://m.share.zdbjq.cn/Article/details/gvuqqznux.sHtML

Py:   os.getcwd()
来源：http://read.share.zdbjq.cn/Article/details/gijjknoau.sHtML

PHP:  getcwd();
来源：http://www.share.hesvh.cn/Article/details/gulajgdvx.sHtML

JS:   process.cwd()
来源：http://m.share.fehbvm.com/Article/details/gcxlnzzze.sHtML

TS:   process.cwd()
来源：http://wap.fehbvm.com/Article/details/gglsmwvhc.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.zdbjq.cn/Article/details/gatpjqwkd.sHtML

Go:   os.Getwd()
来源：http://wap.zdbjq.cn/Article/details/grefvocry.sHtML

Ruby: Dir.pwd
来源：http://www.blog.hesvh.cn/Article/details/gszkgnyru.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.zdbjq.cn/Article/details/guwpjisrz.sHtML

[M05] 设置退出码
来源：http://mobile.zdbjq.cn/Article/details/gdhhmzpmq.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gsacahmdr.sHtML

PHP:  exit(1);
来源：http://www.share.zdbjq.cn/Article/details/gqxarksaq.sHtML

JS:   process.exit(1)
来源：http://3g.fehbvm.com/Article/details/ghekfoobm.sHtML

TS:   process.exit(1)
来源：http://read.share.fehbvm.com/Article/details/gwduhpdps.sHtML

Java: System.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gaessnwqe.sHtML

Go:   os.Exit(1)
来源：http://read.share.fehbvm.com/Article/details/gumaizjcr.sHtML

Ruby: exit 1
来源：http://baike.hesvh.cn/Article/details/gggqotxdn.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.hesvh.cn/Article/details/gfbgsmhpe.sHtML

[M06] 向标准错误输出
来源：http://read.share.zdbjq.cn/Article/details/guemsmzym.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.fehbvm.com/Article/details/gwwguplwx.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.fehbvm.com/Article/details/guqerjpvn.sHtML

JS:   console.error("err")
来源：http://wap.fehbvm.com/Article/details/grevyifyp.sHtML

TS:   console.error("err")
来源：http://www.m.share.zdbjq.cn/Article/details/gzvippsao.sHtML

Java: System.err.println("err")
来源：http://baike.fehbvm.com/Article/details/gkejgkqhi.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.hesvh.cn/Article/details/gaboplfbo.sHtML

Ruby: warn "err"
来源：http://baike.fehbvm.com/Article/details/gxndvchfx.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.zdbjq.cn/Article/details/gfyzayhld.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.zdbjq.cn/Article/details/gysukdyvm.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.hesvh.cn/Article/details/gnnhtbtat.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.zdbjq.cn/Article/details/gwneriloq.sHtML

JS:   require.main === module
来源：http://m.share.zdbjq.cn/Article/details/gqytaxpxt.sHtML

TS:   require.main === module
来源：http://wap.zdbjq.cn/Article/details/gghkmeaym.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.fehbvm.com/Article/details/gcrvilikk.sHtML

Go:   func main()
来源：http://3g.fehbvm.com/Article/details/gllkjpqzw.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.fehbvm.com/Article/details/gzhhuuojz.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.zdbjq.cn/Article/details/gbespundm.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.zdbjq.cn/Article/details/ghbzggala.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.hesvh.cn/Article/details/gzytxkgno.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.zdbjq.cn/Article/details/gudukzphq.sHtML

JS:   process.platform;  process.version
来源：http://www.share.zdbjq.cn/Article/details/gnatmwpsk.sHtML

TS:   process.platform;  process.version
来源：http://wap.fehbvm.com/Article/details/gpkvnbzzx.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.hesvh.cn/Article/details/gsmwaoezf.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.zdbjq.cn/Article/details/gkumulzns.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.hesvh.cn/Article/details/goutrsgoc.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.hesvh.cn/Article/details/gblkfnikn.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gumhobedz.sHtML

N. 数据结构与算法
来源：http://wap.fehbvm.com/Article/details/giejfgaqs.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gbojrscme.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.fehbvm.com/Article/details/groolwzcs.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gxqnnllgw.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.hesvh.cn/Article/details/gtweuuqoy.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.fehbvm.com/Article/details/gjvlvprpg.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.fehbvm.com/Article/details/gfgtpfufz.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.zdbjq.cn/Article/details/glwqiwuco.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.hesvh.cn/Article/details/glildghky.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.hesvh.cn/Article/details/gxkcfhsyi.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.zdbjq.cn/Article/details/guhljscub.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.zdbjq.cn/Article/details/gjklyylyp.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.hesvh.cn/Article/details/gsvtvadks.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.fehbvm.com/Article/details/gisdjvwko.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.zdbjq.cn/Article/details/gvuuosdbt.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.fehbvm.com/Article/details/glsftxyxf.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.hesvh.cn/Article/details/guxggxqwo.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gxjyvdiah.sHtML

Ruby: arr.sort
来源：http://www.m.share.fehbvm.com/Article/details/gfofxlznv.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.fehbvm.com/Article/details/ggtlxyktq.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.hesvh.cn/Article/details/gsjcdgzbo.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.hesvh.cn/Article/details/ggnhvdcvy.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.hesvh.cn/Article/details/guyfgzrtx.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.zdbjq.cn/Article/details/glsocscmy.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.hesvh.cn/Article/details/gerrkqofa.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.zdbjq.cn/Article/details/gxindvgue.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.fehbvm.com/Article/details/glskracyc.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.zdbjq.cn/Article/details/gwyctotrj.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.fehbvm.com/Article/details/ghaclclbg.sHtML

[N04] 斐波那契数列
来源：http://www.share.fehbvm.com/Article/details/ghvgdatqv.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.zdbjq.cn/Article/details/gfklicxmh.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.hesvh.cn/Article/details/gksrgljbv.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.fehbvm.com/Article/details/growmkfpo.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.hesvh.cn/Article/details/gbpxqaydc.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.zdbjq.cn/Article/details/gdiyuxszb.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.hesvh.cn/Article/details/ghgsufxix.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.zdbjq.cn/Article/details/glloxsljr.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.hesvh.cn/Article/details/gtndhaxsq.sHtML

[N05] 最大公约数
来源：http://www.share.hesvh.cn/Article/details/gtgnieytf.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.zdbjq.cn/Article/details/gbmucorhz.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.fehbvm.com/Article/details/gpkltvhgz.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.hesvh.cn/Article/details/ghzqehjlz.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.zdbjq.cn/Article/details/gdtmzairj.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.fehbvm.com/Article/details/gjckftzrl.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.hesvh.cn/Article/details/gfvonsfaz.sHtML

Ruby: a.gcd(b)
来源：http://read.share.fehbvm.com/Article/details/gzirvnrvd.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.zdbjq.cn/Article/details/gzcomcery.sHtML

[N06] 判断回文字符串
来源：http://read.share.hesvh.cn/Article/details/gfzmiotxr.sHtML

Py:   s == s[::-1]
来源：http://baike.zdbjq.cn/Article/details/glafcjjzo.sHtML

PHP:  $s === strrev($s);
来源：http://blog.hesvh.cn/Article/details/gmoedyszc.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/gqijocdsq.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/gznaczldw.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.hesvh.cn/Article/details/gvcsqkdyx.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.zdbjq.cn/Article/details/gxczyxqst.sHtML

Ruby: s == s.reverse
来源：http://read.share.fehbvm.com/Article/details/gnwiftgju.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.hesvh.cn/Article/details/gxdhubcpr.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.fehbvm.com/Article/details/gtwoqvcrj.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.fehbvm.com/Article/details/gybpkjbpo.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.zdbjq.cn/Article/details/gwjwivsqg.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.fehbvm.com/Article/details/gszwrtgfa.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.fehbvm.com/Article/details/gyvsiuowm.sHtML

Java: // 手写 HashMap
来源：http://wap.hesvh.cn/Article/details/gcomjmuth.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.hesvh.cn/Article/details/gopivtusq.sHtML

Ruby: // 手写 Hash
来源：http://m.share.hesvh.cn/Article/details/gdcemdjsm.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.fehbvm.com/Article/details/gevfrflis.sHtML

[N08] 生成全排列
来源：http://www.blog.fehbvm.com/Article/details/gfzigemjd.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.zdbjq.cn/Article/details/ghxrxdytg.sHtML

PHP:  // 手写递归交换
来源：http://mobile.fehbvm.com/Article/details/ggaikywet.sHtML

JS:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gqgibdamb.sHtML

TS:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gmoepjuek.sHtML

Java: // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gomffaprr.sHtML

Go:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gdwtffkbc.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.fehbvm.com/Article/details/gtocguikz.sHtML

C#:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gcrhsdrtg.sHtML

[N09] 栈与队列
来源：http://blog.fehbvm.com/Article/details/gucclfyco.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.fehbvm.com/Article/details/gtqmxppbl.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.hesvh.cn/Article/details/gvzfvttom.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.hesvh.cn/Article/details/grhukafkx.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.hesvh.cn/Article/details/gqpbgiwgf.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.fehbvm.com/Article/details/gpnxjgsaq.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.hesvh.cn/Article/details/giucwkyoi.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.fehbvm.com/Article/details/gevofzukx.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.zdbjq.cn/Article/details/givfosbfb.sHtML

[N10] 链表节点定义
来源：http://baike.zdbjq.cn/Article/details/gskbfypqi.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.fehbvm.com/Article/details/gccwdcloj.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.zdbjq.cn/Article/details/giyrpsyqm.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.zdbjq.cn/Article/details/gdrehfxus.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.hesvh.cn/Article/details/gvpubiasa.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.zdbjq.cn/Article/details/gimsjguqd.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.fehbvm.com/Article/details/geskbpuzj.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.hesvh.cn/Article/details/gzbqxvtck.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.hesvh.cn/Article/details/gdhwcvcrp.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.hesvh.cn/Article/details/gemwujoom.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.hesvh.cn/Article/details/giwlkzbsm.sHtML

PHP:  // 手写递归函数
来源：http://www.share.zdbjq.cn/Article/details/gyueqccjh.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.fehbvm.com/Article/details/gnorepkly.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.fehbvm.com/Article/details/gzfxbuxmj.sHtML

Java: // 手写递归
来源：http://mobile.zdbjq.cn/Article/details/grvzcpcfo.sHtML

Go:   // 手写递归
来源：http://baike.hesvh.cn/Article/details/gkslrytcu.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.fehbvm.com/Article/details/gflluthrw.sHtML

C#:   // 手写递归
来源：http://mobile.fehbvm.com/Article/details/ggjwwrzjw.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.hesvh.cn/Article/details/gbfcioaed.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.hesvh.cn/Article/details/gdlqdhqlz.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.hesvh.cn/Article/details/gbebfkxwn.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.zdbjq.cn/Article/details/gszblutif.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.zdbjq.cn/Article/details/gpnucxsaz.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.fehbvm.com/Article/details/gkaepwixz.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.hesvh.cn/Article/details/gejdgupal.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.fehbvm.com/Article/details/gumdkpdpg.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.hesvh.cn/Article/details/geivyufxu.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/ghyipanao.sHtML

O. 并发与异步
来源：http://www.share.fehbvm.com/Article/details/gozpdeqsi.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gidppdykv.sHtML

[O01] 启动一个线程
来源：http://3g.fehbvm.com/Article/details/gzpspupnn.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.fehbvm.com/Article/details/gzmyrkkyw.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.hesvh.cn/Article/details/gcznpwwoe.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.hesvh.cn/Article/details/gbvcriigi.sHtML

TS:   // 同 JS
来源：http://baike.zdbjq.cn/Article/details/gqvtxouln.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.zdbjq.cn/Article/details/gdyljxvzj.sHtML

Go:   go f()
来源：http://www.blog.zdbjq.cn/Article/details/grhniyxmd.sHtML

Ruby: Thread.new { f }
来源：http://m.share.zdbjq.cn/Article/details/gmdjduunt.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.fehbvm.com/Article/details/gdlaekslw.sHtML

[O02] 使用线程池
来源：http://3g.zdbjq.cn/Article/details/gvbwlsqce.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.hesvh.cn/Article/details/gzlrjuoiv.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.zdbjq.cn/Article/details/gchodjuss.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.zdbjq.cn/Article/details/gfdwrxwic.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.hesvh.cn/Article/details/gzrwbovwz.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.hesvh.cn/Article/details/guigmlyrt.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.fehbvm.com/Article/details/gufnkkhfi.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.zdbjq.cn/Article/details/gkcyjqymo.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.zdbjq.cn/Article/details/gtcsoegmf.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.zdbjq.cn/Article/details/gjgmdxjta.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.zdbjq.cn/Article/details/ggrghpkav.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.hesvh.cn/Article/details/gihtnrspw.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.fehbvm.com/Article/details/guhwsfihp.sHtML

TS:   // 同 JS
来源：http://blog.fehbvm.com/Article/details/gvkjmqfsk.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.fehbvm.com/Article/details/gunmshfkw.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.hesvh.cn/Article/details/gefyspoqf.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.zdbjq.cn/Article/details/ghutxzcuw.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.hesvh.cn/Article/details/gyecqdiqd.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.fehbvm.com/Article/details/gsczhtfcz.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.zdbjq.cn/Article/details/glsqtzhic.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.zdbjq.cn/Article/details/gbpqearsj.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.fehbvm.com/Article/details/gefjwocru.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.hesvh.cn/Article/details/gpdezamji.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.fehbvm.com/Article/details/gpnmetoou.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.fehbvm.com/Article/details/griimumjy.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.zdbjq.cn/Article/details/gvhgykanh.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.fehbvm.com/Article/details/gfwtlrgvw.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.zdbjq.cn/Article/details/gpoxkfdsa.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.zdbjq.cn/Article/details/gurqsvffh.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.zdbjq.cn/Article/details/gmxqfmcrq.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.hesvh.cn/Article/details/gpanoovrw.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.hesvh.cn/Article/details/gjcjfvagz.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.hesvh.cn/Article/details/gkwqbgumo.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.fehbvm.com/Article/details/gxkiismeo.sHtML

Ruby: threads.map(&:join)
来源：http://baike.zdbjq.cn/Article/details/gupogvpas.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.fehbvm.com/Article/details/gvjndmwjq.sHtML

[O06] 使用进程池
来源：http://www.share.hesvh.cn/Article/details/gnpnzwxtp.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.zdbjq.cn/Article/details/gzprandzc.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.fehbvm.com/Article/details/gejporkfz.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.hesvh.cn/Article/details/giffdwpxp.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.hesvh.cn/Article/details/gralrdqws.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.zdbjq.cn/Article/details/giizlugtu.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.zdbjq.cn/Article/details/guucbzndo.sHtML

Ruby: // fork 块
来源：http://read.share.zdbjq.cn/Article/details/gunncfccs.sHtML

C#:   Parallel.For
来源：http://3g.fehbvm.com/Article/details/gctftgrfh.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gvjpznhlr.sHtML

P. 常用工具函数
来源：http://www.m.share.fehbvm.com/Article/details/gkatxuted.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gyvwqkfsd.sHtML

[P01] 生成 UUID
来源：http://mobile.hesvh.cn/Article/details/gqqrpauzh.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.fehbvm.com/Article/details/gjgoljjjy.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.hesvh.cn/Article/details/gmlkhjihk.sHtML

JS:   crypto.randomUUID()
来源：http://baike.zdbjq.cn/Article/details/glxuipoiv.sHtML

TS:   crypto.randomUUID()
来源：http://baike.hesvh.cn/Article/details/gwtjaeidq.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.zdbjq.cn/Article/details/gktcmizon.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.zdbjq.cn/Article/details/gnkedsuvb.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.fehbvm.com/Article/details/gzfmbvayk.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.hesvh.cn/Article/details/glliwpngb.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.hesvh.cn/Article/details/gglabdvpk.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.zdbjq.cn/Article/details/gfagdvjbo.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.fehbvm.com/Article/details/gilmpgfby.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.zdbjq.cn/Article/details/gztyblxag.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.hesvh.cn/Article/details/gsqezkptb.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.fehbvm.com/Article/details/gnpuombtx.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.fehbvm.com/Article/details/gtubaxidl.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.zdbjq.cn/Article/details/gdbeftohd.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.fehbvm.com/Article/details/gbwuogfrj.sHtML

[P03] 生成短随机字符串
来源：http://www.share.hesvh.cn/Article/details/gdtqjjfyu.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.zdbjq.cn/Article/details/gwinrzlfw.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.zdbjq.cn/Article/details/gksxbyksp.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.zdbjq.cn/Article/details/gxloojayv.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.zdbjq.cn/Article/details/gixmtfbbw.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.fehbvm.com/Article/details/gekpogvcq.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.fehbvm.com/Article/details/gbpjdmqzr.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.hesvh.cn/Article/details/gcrtgzhfb.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.fehbvm.com/Article/details/ghrptbtri.sHtML

[P04] 求长度
来源：http://mobile.hesvh.cn/Article/details/gfrchzagj.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.zdbjq.cn/Article/details/glwbflqjx.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.fehbvm.com/Article/details/gywbuajbv.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.zdbjq.cn/Article/details/gjokqandd.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.zdbjq.cn/Article/details/gfktvklun.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.hesvh.cn/Article/details/ggfoatatb.sHtML

Go:   len(arr);  len(m)
来源：http://baike.hesvh.cn/Article/details/gogvcanvj.sHtML

Ruby: x.length;  x.size
来源：http://mobile.zdbjq.cn/Article/details/gzylvmjns.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.zdbjq.cn/Article/details/gzvmudoke.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.zdbjq.cn/Article/details/gyaosumfb.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.hesvh.cn/Article/details/gjqjlsmil.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.fehbvm.com/Article/details/gxujlkkdz.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.hesvh.cn/Article/details/gcuzhgbop.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.hesvh.cn/Article/details/geprkztpe.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.fehbvm.com/Article/details/gpyqtzfdi.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.hesvh.cn/Article/details/gtdkrrwpb.sHtML

Ruby: a == b
来源：http://read.share.zdbjq.cn/Article/details/giopuvplk.sHtML


<!-- 参考信息 -->