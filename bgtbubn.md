代发 wailian999

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.hesvh.cn/Article/details/gakscwnlx.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fehbvm.com/Article/details/gczzlgybl.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.zdbjq.cn/Article/details/geyjildfz.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.hesvh.cn/Article/details/gvhnmdbig.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.fehbvm.com/Article/details/gskyapvyq.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.hesvh.cn/Article/details/gdkkmcqkj.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gwexrrllb.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.hesvh.cn/Article/details/gpuhevjzm.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gcdjwkcwg.sHtML

[M01] 读取命令行参数
来源：http://m.share.zdbjq.cn/Article/details/gigsuwtjv.sHtML

Py:   sys.argv[1:]
来源：http://3g.zdbjq.cn/Article/details/gzlayodmn.sHtML

PHP:  $argv;  $argc;
来源：http://wap.zdbjq.cn/Article/details/gvlbbaual.sHtML

JS:   process.argv.slice(2)
来源：http://3g.zdbjq.cn/Article/details/gwrxyvmxb.sHtML

TS:   process.argv.slice(2)
来源：http://baike.fehbvm.com/Article/details/gyzfjxvof.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.hesvh.cn/Article/details/grxdhyfru.sHtML

Go:   os.Args[1:]
来源：http://baike.zdbjq.cn/Article/details/gytoblkkh.sHtML

Ruby: ARGV
来源：http://m.share.zdbjq.cn/Article/details/gxqikoyal.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.zdbjq.cn/Article/details/gnedhgogi.sHtML

[M02] 读取环境变量
来源：http://wap.fehbvm.com/Article/details/gtvyhgtnl.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.fehbvm.com/Article/details/grpujnzxw.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.zdbjq.cn/Article/details/gyccqbuty.sHtML

JS:   process.env.HOME
来源：http://wap.zdbjq.cn/Article/details/gvploxsft.sHtML

TS:   process.env.HOME
来源：http://mobile.hesvh.cn/Article/details/gwsbllurz.sHtML

Java: System.getenv("HOME")
来源：http://read.share.zdbjq.cn/Article/details/guuxjrsov.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.hesvh.cn/Article/details/gydlufbsa.sHtML

Ruby: ENV["HOME"]
来源：http://blog.fehbvm.com/Article/details/gfxqieauh.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.fehbvm.com/Article/details/grsazrmuo.sHtML

[M03] 执行外部命令
来源：http://blog.fehbvm.com/Article/details/ggcnxbbmu.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.zdbjq.cn/Article/details/gaqupznys.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.zdbjq.cn/Article/details/ghitslteu.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.fehbvm.com/Article/details/gghsaaxej.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.fehbvm.com/Article/details/gxxvrzqzo.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.hesvh.cn/Article/details/gzkxuhmli.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.zdbjq.cn/Article/details/guyzyulrf.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.zdbjq.cn/Article/details/gtaxithda.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.fehbvm.com/Article/details/gnfyzwoih.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.hesvh.cn/Article/details/gorybtzwx.sHtML

Py:   os.getcwd()
来源：http://wap.fehbvm.com/Article/details/gpjwuzdma.sHtML

PHP:  getcwd();
来源：http://wap.zdbjq.cn/Article/details/ggajbsfbs.sHtML

JS:   process.cwd()
来源：http://wap.zdbjq.cn/Article/details/gxdvvxhbm.sHtML

TS:   process.cwd()
来源：http://baike.zdbjq.cn/Article/details/gqnpmflmx.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.fehbvm.com/Article/details/gegvzuuji.sHtML

Go:   os.Getwd()
来源：http://www.share.zdbjq.cn/Article/details/giwcdzobh.sHtML

Ruby: Dir.pwd
来源：http://www.blog.hesvh.cn/Article/details/gogivfvnz.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.fehbvm.com/Article/details/gouleexwa.sHtML

[M05] 设置退出码
来源：http://read.share.fehbvm.com/Article/details/gvfysxzma.sHtML

Py:   sys.exit(1)
来源：http://baike.hesvh.cn/Article/details/ggeyouswi.sHtML

PHP:  exit(1);
来源：http://baike.hesvh.cn/Article/details/gaqdzzkti.sHtML

JS:   process.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gszxvozoq.sHtML

TS:   process.exit(1)
来源：http://wap.fehbvm.com/Article/details/gkjkpkviw.sHtML

Java: System.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gzckojlyf.sHtML

Go:   os.Exit(1)
来源：http://mobile.fehbvm.com/Article/details/gpyugosrg.sHtML

Ruby: exit 1
来源：http://mobile.hesvh.cn/Article/details/gigyqrpqt.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.zdbjq.cn/Article/details/ggsotcvoc.sHtML

[M06] 向标准错误输出
来源：http://www.blog.hesvh.cn/Article/details/gnmmdbdmd.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.fehbvm.com/Article/details/gjsbmzgkx.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.hesvh.cn/Article/details/gbxzjiyfn.sHtML

JS:   console.error("err")
来源：http://read.share.zdbjq.cn/Article/details/gctsvkadg.sHtML

TS:   console.error("err")
来源：http://www.m.share.zdbjq.cn/Article/details/gbjhipehd.sHtML

Java: System.err.println("err")
来源：http://wap.fehbvm.com/Article/details/glzkqvyoq.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.zdbjq.cn/Article/details/ghrxsuqzx.sHtML

Ruby: warn "err"
来源：http://3g.hesvh.cn/Article/details/gutfytcsb.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.hesvh.cn/Article/details/gtsmbcvco.sHtML

[M07] 判断是否为主入口
来源：http://blog.fehbvm.com/Article/details/gajcrzyno.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.fehbvm.com/Article/details/guiqqqike.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.zdbjq.cn/Article/details/gyxvkaqdd.sHtML

JS:   require.main === module
来源：http://3g.hesvh.cn/Article/details/guveilgmz.sHtML

TS:   require.main === module
来源：http://wap.hesvh.cn/Article/details/ghphkqvxy.sHtML

Java: public static void main(String[] args)
来源：http://wap.zdbjq.cn/Article/details/gdjpiuigb.sHtML

Go:   func main()
来源：http://m.share.fehbvm.com/Article/details/gxrrxqpih.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.hesvh.cn/Article/details/gcfqhpwdh.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.zdbjq.cn/Article/details/gkwkylawa.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.zdbjq.cn/Article/details/gsnncjrmx.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.hesvh.cn/Article/details/gbojhkpys.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.fehbvm.com/Article/details/grzqxojou.sHtML

JS:   process.platform;  process.version
来源：http://3g.zdbjq.cn/Article/details/gecroiudj.sHtML

TS:   process.platform;  process.version
来源：http://wap.zdbjq.cn/Article/details/guyudgoit.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.fehbvm.com/Article/details/gkeuwldry.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.fehbvm.com/Article/details/gxcuzbwrt.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.hesvh.cn/Article/details/gxouleylc.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.hesvh.cn/Article/details/gfjzhyvgs.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gnrzimvvf.sHtML

N. 数据结构与算法
来源：http://www.m.share.hesvh.cn/Article/details/gaxgnchdc.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gumdsjath.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.hesvh.cn/Article/details/gaavpfush.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.fehbvm.com/Article/details/gidfgshbj.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.hesvh.cn/Article/details/gzorbftue.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.fehbvm.com/Article/details/gkktchlxl.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.fehbvm.com/Article/details/gutsmeomy.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gfcputxjw.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gkffyuwnb.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.fehbvm.com/Article/details/gedcuzhiy.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.hesvh.cn/Article/details/giatgsgku.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.hesvh.cn/Article/details/gppgcvoey.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.zdbjq.cn/Article/details/goitsbsfc.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.zdbjq.cn/Article/details/gsmvaisbd.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.zdbjq.cn/Article/details/gsszzucof.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.zdbjq.cn/Article/details/gwkvcufbu.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.hesvh.cn/Article/details/gszhojbhi.sHtML

Go:   slices.Sort(arr)
来源：http://wap.hesvh.cn/Article/details/gmgrwkpux.sHtML

Ruby: arr.sort
来源：http://blog.zdbjq.cn/Article/details/gctosnmdq.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.fehbvm.com/Article/details/gqvwtwqmo.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.zdbjq.cn/Article/details/gdkwshcrp.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.fehbvm.com/Article/details/ghpkbkhgc.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.fehbvm.com/Article/details/gnlfgrwnt.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.hesvh.cn/Article/details/govtgfedv.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.hesvh.cn/Article/details/gbiummqly.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.hesvh.cn/Article/details/ggifysotx.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.fehbvm.com/Article/details/gjlumpkjg.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.fehbvm.com/Article/details/gqzoztptt.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.zdbjq.cn/Article/details/gdqroumkh.sHtML

[N04] 斐波那契数列
来源：http://wap.hesvh.cn/Article/details/gwyxqlwax.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.fehbvm.com/Article/details/gsamexbvb.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.hesvh.cn/Article/details/gjvpomwpt.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/gxrljugty.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.zdbjq.cn/Article/details/gmltcfzqe.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.fehbvm.com/Article/details/glqvrifwg.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.hesvh.cn/Article/details/gzfmixrpw.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.hesvh.cn/Article/details/gtkabieyg.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.zdbjq.cn/Article/details/gqpjnmilb.sHtML

[N05] 最大公约数
来源：http://www.blog.zdbjq.cn/Article/details/gnsqvcwqa.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.zdbjq.cn/Article/details/gmtzisxad.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.hesvh.cn/Article/details/gfxisbohw.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.zdbjq.cn/Article/details/grhghcash.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.zdbjq.cn/Article/details/gclnotmwm.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.fehbvm.com/Article/details/gllevhwmd.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.fehbvm.com/Article/details/gsxuxlblf.sHtML

Ruby: a.gcd(b)
来源：http://mobile.fehbvm.com/Article/details/gwckyesvb.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.fehbvm.com/Article/details/gunkdfcgp.sHtML

[N06] 判断回文字符串
来源：http://wap.zdbjq.cn/Article/details/grakqnxon.sHtML

Py:   s == s[::-1]
来源：http://baike.hesvh.cn/Article/details/gekmwpbcp.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.hesvh.cn/Article/details/govqjxloa.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/goykrhlxr.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/gyxbvtstl.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.zdbjq.cn/Article/details/gmgxgwuku.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.hesvh.cn/Article/details/gfvbbspya.sHtML

Ruby: s == s.reverse
来源：http://m.share.fehbvm.com/Article/details/gdmmknywp.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.zdbjq.cn/Article/details/gxtbyluvt.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.zdbjq.cn/Article/details/gpabhpifx.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.zdbjq.cn/Article/details/gexlbpsbq.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.zdbjq.cn/Article/details/gpmqkboqh.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.hesvh.cn/Article/details/gzmosqdtl.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.fehbvm.com/Article/details/gdcoptfgt.sHtML

Java: // 手写 HashMap
来源：http://www.blog.hesvh.cn/Article/details/gsqjnkyly.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.zdbjq.cn/Article/details/goiwjbsnu.sHtML

Ruby: // 手写 Hash
来源：http://www.share.hesvh.cn/Article/details/gofdzeesw.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.fehbvm.com/Article/details/gbqpqicou.sHtML

[N08] 生成全排列
来源：http://www.share.hesvh.cn/Article/details/ggnvoiroq.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.zdbjq.cn/Article/details/gdrohqwbs.sHtML

PHP:  // 手写递归交换
来源：http://www.share.hesvh.cn/Article/details/gzvzooegt.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gzjmrdzuw.sHtML

TS:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gteldwnux.sHtML

Java: // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gqmlybxjn.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/genadqulv.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.zdbjq.cn/Article/details/goyjqufvc.sHtML

C#:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gzegippzb.sHtML

[N09] 栈与队列
来源：http://m.share.fehbvm.com/Article/details/gxfiwunnz.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.hesvh.cn/Article/details/gziczhcqe.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.zdbjq.cn/Article/details/gnfweuezk.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.fehbvm.com/Article/details/gxcgswdem.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.hesvh.cn/Article/details/gfbbagwlr.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.hesvh.cn/Article/details/gskzasqle.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.fehbvm.com/Article/details/gxfskzxqj.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.hesvh.cn/Article/details/gmdoqfqwm.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.fehbvm.com/Article/details/gskqrrtsa.sHtML

[N10] 链表节点定义
来源：http://wap.hesvh.cn/Article/details/gxfqliktg.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.fehbvm.com/Article/details/gffluuali.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.fehbvm.com/Article/details/gbtrhujae.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.fehbvm.com/Article/details/glfsgxmtq.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.hesvh.cn/Article/details/grpmtrbnp.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.hesvh.cn/Article/details/gfbjnxtfq.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.zdbjq.cn/Article/details/gwneptvlx.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.zdbjq.cn/Article/details/glicazwsf.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.zdbjq.cn/Article/details/gtxvzsmrh.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.hesvh.cn/Article/details/gkbtynzjl.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.fehbvm.com/Article/details/gmfomyged.sHtML

PHP:  // 手写递归函数
来源：http://m.share.fehbvm.com/Article/details/gduxisxxr.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.fehbvm.com/Article/details/gmpotxiej.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.hesvh.cn/Article/details/giaamqana.sHtML

Java: // 手写递归
来源：http://3g.fehbvm.com/Article/details/gfubdfaab.sHtML

Go:   // 手写递归
来源：http://www.share.zdbjq.cn/Article/details/gcknclxfz.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.zdbjq.cn/Article/details/gaswwiafy.sHtML

C#:   // 手写递归
来源：http://www.blog.fehbvm.com/Article/details/grishnrni.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.zdbjq.cn/Article/details/gwzzmlysu.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.zdbjq.cn/Article/details/gnnzgppgq.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.fehbvm.com/Article/details/gjzxgqexy.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.zdbjq.cn/Article/details/gtgwbftqt.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.hesvh.cn/Article/details/gctzxrkdl.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.zdbjq.cn/Article/details/guypfgtbu.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.zdbjq.cn/Article/details/gzmojwqcf.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.fehbvm.com/Article/details/gdzwmzfie.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.hesvh.cn/Article/details/gqdezqogo.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/givflfzpc.sHtML

O. 并发与异步
来源：http://mobile.fehbvm.com/Article/details/grrukickb.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gzjwxqvlz.sHtML

[O01] 启动一个线程
来源：http://m.share.fehbvm.com/Article/details/gdbxxrsyw.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.fehbvm.com/Article/details/gtnaklbph.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.hesvh.cn/Article/details/gtzfkwnei.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.fehbvm.com/Article/details/gvhavzblq.sHtML

TS:   // 同 JS
来源：http://m.share.zdbjq.cn/Article/details/gkezqytdd.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.hesvh.cn/Article/details/ggwosfdkv.sHtML

Go:   go f()
来源：http://www.share.hesvh.cn/Article/details/gjqgcjtmh.sHtML

Ruby: Thread.new { f }
来源：http://m.share.fehbvm.com/Article/details/gpchophjz.sHtML

C#:   Task.Run(() => F());
来源：http://wap.fehbvm.com/Article/details/gunuqqyua.sHtML

[O02] 使用线程池
来源：http://3g.zdbjq.cn/Article/details/gyegcbrlx.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.fehbvm.com/Article/details/gssrnwwec.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.hesvh.cn/Article/details/gkwxyupzu.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.hesvh.cn/Article/details/gpgstbmbh.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.fehbvm.com/Article/details/ghlmkbgul.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.hesvh.cn/Article/details/gpldnujeg.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.zdbjq.cn/Article/details/gnoxhpalp.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.zdbjq.cn/Article/details/gealxflgt.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.hesvh.cn/Article/details/gjlllgxks.sHtML

[O03] 加锁保护共享数据
来源：http://baike.fehbvm.com/Article/details/gdpdnxvcx.sHtML

Py:   with lock: shared += 1
来源：http://baike.zdbjq.cn/Article/details/gzhjncyar.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.zdbjq.cn/Article/details/gnyjgpgpw.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.hesvh.cn/Article/details/gwfoyteut.sHtML

TS:   // 同 JS
来源：http://wap.fehbvm.com/Article/details/gtaiqoqcs.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.fehbvm.com/Article/details/giebzulop.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.zdbjq.cn/Article/details/gudumkznf.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.fehbvm.com/Article/details/gzvrqhrht.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.hesvh.cn/Article/details/gpcncrsbr.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.zdbjq.cn/Article/details/gmcrzliew.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.zdbjq.cn/Article/details/gbomxlnlu.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.hesvh.cn/Article/details/gaupggzaa.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.fehbvm.com/Article/details/gcrhivnsy.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.hesvh.cn/Article/details/guacesdhi.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.fehbvm.com/Article/details/govbgxmrj.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.hesvh.cn/Article/details/ghwbqjzmh.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.zdbjq.cn/Article/details/geidglrdy.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.fehbvm.com/Article/details/goojgtivi.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.fehbvm.com/Article/details/gyjdzogpv.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.fehbvm.com/Article/details/gdtuebswp.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.hesvh.cn/Article/details/goaihnxyp.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.hesvh.cn/Article/details/gkjdhoxbf.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.zdbjq.cn/Article/details/gqqsthknl.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.zdbjq.cn/Article/details/gzjejpzgh.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.fehbvm.com/Article/details/gmgizloji.sHtML

Ruby: threads.map(&:join)
来源：http://3g.hesvh.cn/Article/details/gawfsyjxh.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.hesvh.cn/Article/details/gzetvhuay.sHtML

[O06] 使用进程池
来源：http://mobile.hesvh.cn/Article/details/grrntjprx.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.fehbvm.com/Article/details/giuvkuugm.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.zdbjq.cn/Article/details/gnypmcdsm.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.fehbvm.com/Article/details/gpmpkpnmh.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.zdbjq.cn/Article/details/gubepcnwk.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.zdbjq.cn/Article/details/grmiseznt.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.zdbjq.cn/Article/details/grhyakcus.sHtML

Ruby: // fork 块
来源：http://3g.hesvh.cn/Article/details/gjdejhtdz.sHtML

C#:   Parallel.For
来源：http://baike.fehbvm.com/Article/details/gyalhtwuq.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gmmxoxcdw.sHtML

P. 常用工具函数
来源：http://wap.hesvh.cn/Article/details/gbugkbhhn.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gncyfkfjt.sHtML

[P01] 生成 UUID
来源：http://m.share.fehbvm.com/Article/details/grkixxxce.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.hesvh.cn/Article/details/ghaaizthc.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.hesvh.cn/Article/details/gcjtpnjti.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.hesvh.cn/Article/details/gxpvznfbd.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.fehbvm.com/Article/details/gmwmbgprm.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.fehbvm.com/Article/details/gaoibewrw.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.fehbvm.com/Article/details/gnrhosigz.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.fehbvm.com/Article/details/gcgmftmgr.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.zdbjq.cn/Article/details/gzalwkvyu.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.hesvh.cn/Article/details/gntdfddvk.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.fehbvm.com/Article/details/grutainxp.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.zdbjq.cn/Article/details/gyngmejhb.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.zdbjq.cn/Article/details/ghowmmofg.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.hesvh.cn/Article/details/gaxqzmbjn.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.zdbjq.cn/Article/details/gzdkivzpx.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.fehbvm.com/Article/details/gqcqzfdom.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.fehbvm.com/Article/details/gbsmbzbwq.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.fehbvm.com/Article/details/gvuxlxrkq.sHtML

[P03] 生成短随机字符串
来源：http://mobile.zdbjq.cn/Article/details/gsqgzobwb.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.fehbvm.com/Article/details/gymkqgtud.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.hesvh.cn/Article/details/gvschojzy.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.zdbjq.cn/Article/details/gjeyvozwu.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.hesvh.cn/Article/details/gyjgmnhcw.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.fehbvm.com/Article/details/grxnurunz.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.fehbvm.com/Article/details/gvbhzhmvm.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.zdbjq.cn/Article/details/gwjakixze.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.fehbvm.com/Article/details/gssotkghw.sHtML

[P04] 求长度
来源：http://www.share.hesvh.cn/Article/details/gxhlpuemv.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.zdbjq.cn/Article/details/gqkppgmdd.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.zdbjq.cn/Article/details/grxesoyqj.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.hesvh.cn/Article/details/gzdywqyzo.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.zdbjq.cn/Article/details/gkskswnpi.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.zdbjq.cn/Article/details/ghijyqsmg.sHtML

Go:   len(arr);  len(m)
来源：http://wap.zdbjq.cn/Article/details/gbpordtsr.sHtML

Ruby: x.length;  x.size
来源：http://mobile.hesvh.cn/Article/details/ghrkhdaep.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.fehbvm.com/Article/details/gyiotxfgt.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.hesvh.cn/Article/details/gnucruxmn.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.zdbjq.cn/Article/details/gnkxlawwd.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.hesvh.cn/Article/details/ghjuzuyhw.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.fehbvm.com/Article/details/glnzbhqtu.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.fehbvm.com/Article/details/gkwqoivei.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.hesvh.cn/Article/details/ggkltugpv.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.zdbjq.cn/Article/details/ghvgcvnwj.sHtML

Ruby: a == b
来源：http://3g.zdbjq.cn/Article/details/gxgwmnxlx.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.zdbjq.cn/Article/details/ggbnoelgl.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.hesvh.cn/Article/details/guvxtgvrj.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.fehbvm.com/Article/details/gaxhenkat.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.hesvh.cn/Article/details/gsgzqbwip.sHtML


<!-- 参考信息 -->