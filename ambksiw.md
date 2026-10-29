代发 wailian999

C#:   (int)resp.StatusCode
来源：http://www.share.hesvh.cn/Article/details/gtmbvsywl.sHtML

[L08] 并发请求多个地址
来源：http://www.share.zdbjq.cn/Article/details/gxbnshqus.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.zdbjq.cn/Article/details/goowehsij.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.fehbvm.com/Article/details/gufqynkzx.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fehbvm.com/Article/details/gwzhbndoo.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fehbvm.com/Article/details/gwquxaqac.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.zdbjq.cn/Article/details/gjylwjfpi.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.fehbvm.com/Article/details/gdkwbngdz.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.zdbjq.cn/Article/details/grwjqnnad.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.hesvh.cn/Article/details/guyxbtbfu.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gjkfzroje.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.hesvh.cn/Article/details/gppwfflty.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gfktjkbgp.sHtML

[M01] 读取命令行参数
来源：http://m.share.hesvh.cn/Article/details/gtsdhhcqb.sHtML

Py:   sys.argv[1:]
来源：http://wap.hesvh.cn/Article/details/gtmpywsrl.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.fehbvm.com/Article/details/geuluzmos.sHtML

JS:   process.argv.slice(2)
来源：http://wap.hesvh.cn/Article/details/gzranebml.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.zdbjq.cn/Article/details/gposfvomn.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.fehbvm.com/Article/details/gyauufphp.sHtML

Go:   os.Args[1:]
来源：http://mobile.fehbvm.com/Article/details/gsluloflx.sHtML

Ruby: ARGV
来源：http://baike.hesvh.cn/Article/details/gxcmlsrdt.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.hesvh.cn/Article/details/gntrbmvoq.sHtML

[M02] 读取环境变量
来源：http://www.share.zdbjq.cn/Article/details/gprrvflip.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.fehbvm.com/Article/details/gjhsodqmc.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.hesvh.cn/Article/details/ghbmcuyci.sHtML

JS:   process.env.HOME
来源：http://wap.zdbjq.cn/Article/details/gxvjswtcc.sHtML

TS:   process.env.HOME
来源：http://www.share.fehbvm.com/Article/details/giaabizwr.sHtML

Java: System.getenv("HOME")
来源：http://blog.hesvh.cn/Article/details/gbbbvotvs.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.hesvh.cn/Article/details/gqmedwagq.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.zdbjq.cn/Article/details/guawhwint.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.zdbjq.cn/Article/details/gseycwfbd.sHtML

[M03] 执行外部命令
来源：http://www.blog.fehbvm.com/Article/details/gqndoutdj.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.fehbvm.com/Article/details/gyqscxhqg.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.hesvh.cn/Article/details/gbzobqtct.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.fehbvm.com/Article/details/gbmmzwhqt.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.hesvh.cn/Article/details/gepcalqhj.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.zdbjq.cn/Article/details/gytmenzek.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.fehbvm.com/Article/details/gkpcvqizd.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.fehbvm.com/Article/details/gzivbkysy.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.hesvh.cn/Article/details/gyvvfpppl.sHtML

[M04] 获取当前工作目录
来源：http://blog.hesvh.cn/Article/details/gpglbeodl.sHtML

Py:   os.getcwd()
来源：http://m.share.zdbjq.cn/Article/details/gejvxeoes.sHtML

PHP:  getcwd();
来源：http://www.m.share.zdbjq.cn/Article/details/gqjhgyvke.sHtML

JS:   process.cwd()
来源：http://3g.zdbjq.cn/Article/details/gcsyvcxgs.sHtML

TS:   process.cwd()
来源：http://blog.hesvh.cn/Article/details/gsntydbic.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.fehbvm.com/Article/details/gptvpsgla.sHtML

Go:   os.Getwd()
来源：http://mobile.hesvh.cn/Article/details/gnufyjdhw.sHtML

Ruby: Dir.pwd
来源：http://3g.hesvh.cn/Article/details/gabgezrre.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.fehbvm.com/Article/details/gqlgtlwrp.sHtML

[M05] 设置退出码
来源：http://blog.fehbvm.com/Article/details/glytvctke.sHtML

Py:   sys.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gvwfrdmad.sHtML

PHP:  exit(1);
来源：http://blog.fehbvm.com/Article/details/gvgdkbhiy.sHtML

JS:   process.exit(1)
来源：http://m.share.hesvh.cn/Article/details/gtpeymmsi.sHtML

TS:   process.exit(1)
来源：http://www.share.hesvh.cn/Article/details/gzsuqpvgm.sHtML

Java: System.exit(1)
来源：http://baike.zdbjq.cn/Article/details/grsqzhpll.sHtML

Go:   os.Exit(1)
来源：http://m.share.hesvh.cn/Article/details/gbwqeeduo.sHtML

Ruby: exit 1
来源：http://read.share.zdbjq.cn/Article/details/gfgfehagi.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.fehbvm.com/Article/details/gebkizlik.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.zdbjq.cn/Article/details/grnqvluhb.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.fehbvm.com/Article/details/gndyjcxfc.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.hesvh.cn/Article/details/gtnkrkxce.sHtML

JS:   console.error("err")
来源：http://m.share.zdbjq.cn/Article/details/gzljcabwd.sHtML

TS:   console.error("err")
来源：http://3g.fehbvm.com/Article/details/gjjmpqcky.sHtML

Java: System.err.println("err")
来源：http://www.share.zdbjq.cn/Article/details/gyhxdhtlu.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.hesvh.cn/Article/details/gxbncadgg.sHtML

Ruby: warn "err"
来源：http://wap.hesvh.cn/Article/details/gwvnabmvy.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.fehbvm.com/Article/details/ghjacnawv.sHtML

[M07] 判断是否为主入口
来源：http://blog.hesvh.cn/Article/details/ggvqmmpdp.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.zdbjq.cn/Article/details/gtexotprh.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.zdbjq.cn/Article/details/gcderfwms.sHtML

JS:   require.main === module
来源：http://mobile.fehbvm.com/Article/details/gofbhgpaq.sHtML

TS:   require.main === module
来源：http://baike.fehbvm.com/Article/details/gqydvscbg.sHtML

Java: public static void main(String[] args)
来源：http://read.share.hesvh.cn/Article/details/gpvlxynww.sHtML

Go:   func main()
来源：http://blog.fehbvm.com/Article/details/gyixufluz.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.fehbvm.com/Article/details/gwmnujlas.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.zdbjq.cn/Article/details/guomxkcpr.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.hesvh.cn/Article/details/ghnpzfkcc.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.hesvh.cn/Article/details/gfhbrpobs.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.zdbjq.cn/Article/details/gmbdlkmtm.sHtML

JS:   process.platform;  process.version
来源：http://3g.fehbvm.com/Article/details/gpsnxppmd.sHtML

TS:   process.platform;  process.version
来源：http://baike.fehbvm.com/Article/details/gnmaqnxbl.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.hesvh.cn/Article/details/gcouerrxl.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.zdbjq.cn/Article/details/gbbsercuf.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.zdbjq.cn/Article/details/gixrlific.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.hesvh.cn/Article/details/gwsflxpmr.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gehwwsxwx.sHtML

N. 数据结构与算法
来源：http://www.share.hesvh.cn/Article/details/gdtvulhsu.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gampwvzto.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.zdbjq.cn/Article/details/gchemnzvo.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gacwifzxu.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.zdbjq.cn/Article/details/guvaocuur.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.zdbjq.cn/Article/details/ggxygkaxg.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.fehbvm.com/Article/details/geiblibwp.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.hesvh.cn/Article/details/ghxvxsvmy.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gxjzmjkoj.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.hesvh.cn/Article/details/gxlpwnyzw.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gdmaimxsu.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.fehbvm.com/Article/details/gbpjtqlro.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.zdbjq.cn/Article/details/gvmlfxola.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.fehbvm.com/Article/details/ghspcxjqs.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.hesvh.cn/Article/details/gmapsgcmq.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.hesvh.cn/Article/details/gwyxuwovs.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.fehbvm.com/Article/details/gfgiejoet.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.zdbjq.cn/Article/details/gamrqwpce.sHtML

Ruby: arr.sort
来源：http://m.share.zdbjq.cn/Article/details/gumcgoytk.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.hesvh.cn/Article/details/gispxhujl.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.zdbjq.cn/Article/details/gbeusnnpm.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.hesvh.cn/Article/details/gfrxxdfuw.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.hesvh.cn/Article/details/giicpyguq.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.zdbjq.cn/Article/details/ggdorjvqn.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.fehbvm.com/Article/details/gjecgmcut.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.hesvh.cn/Article/details/gacvusqwe.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.zdbjq.cn/Article/details/gjmpikbxj.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.zdbjq.cn/Article/details/gelhdzcvl.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.hesvh.cn/Article/details/gwdmjozei.sHtML

[N04] 斐波那契数列
来源：http://3g.hesvh.cn/Article/details/gtxkmywri.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.hesvh.cn/Article/details/grplnazbm.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.zdbjq.cn/Article/details/gdufkvwps.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.zdbjq.cn/Article/details/gwrynhklj.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.fehbvm.com/Article/details/grpdgyjhi.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.zdbjq.cn/Article/details/gtwydvkgt.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.fehbvm.com/Article/details/gigswxmuw.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.fehbvm.com/Article/details/gqjosoqps.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.hesvh.cn/Article/details/ggjqfuqam.sHtML

[N05] 最大公约数
来源：http://wap.fehbvm.com/Article/details/gdeadqosb.sHtML

Py:   math.gcd(a, b)
来源：http://3g.fehbvm.com/Article/details/gdviiznvm.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.hesvh.cn/Article/details/gsplttcpk.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.zdbjq.cn/Article/details/gtjmdytxt.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.fehbvm.com/Article/details/gxunpvblw.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.fehbvm.com/Article/details/gvcpkwvsu.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.hesvh.cn/Article/details/gmjbizyqk.sHtML

Ruby: a.gcd(b)
来源：http://wap.zdbjq.cn/Article/details/gszocuglb.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.zdbjq.cn/Article/details/gcacqctdl.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.fehbvm.com/Article/details/ggbnbqfcl.sHtML

Py:   s == s[::-1]
来源：http://wap.zdbjq.cn/Article/details/grhrxsarf.sHtML

PHP:  $s === strrev($s);
来源：http://3g.hesvh.cn/Article/details/gzblrdvar.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/gopcwebvb.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.zdbjq.cn/Article/details/gtsbvzxts.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.zdbjq.cn/Article/details/gwsezlrou.sHtML

Go:   // 双指针从两端比较
来源：http://baike.hesvh.cn/Article/details/gsexierui.sHtML

Ruby: s == s.reverse
来源：http://www.blog.zdbjq.cn/Article/details/getqwxqum.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.fehbvm.com/Article/details/goycdskio.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.fehbvm.com/Article/details/gsmtnhcro.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.fehbvm.com/Article/details/gghmuslxx.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.hesvh.cn/Article/details/gghibsuqx.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.hesvh.cn/Article/details/gyxtlxrui.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.zdbjq.cn/Article/details/giitlqwso.sHtML

Java: // 手写 HashMap
来源：http://blog.zdbjq.cn/Article/details/gpnahsjin.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.fehbvm.com/Article/details/gtyjmyhou.sHtML

Ruby: // 手写 Hash
来源：http://baike.hesvh.cn/Article/details/gwarakmgi.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.hesvh.cn/Article/details/gnwrtljqo.sHtML

[N08] 生成全排列
来源：http://blog.zdbjq.cn/Article/details/gkbxdvuqu.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.fehbvm.com/Article/details/gztwdpdmu.sHtML

PHP:  // 手写递归交换
来源：http://3g.zdbjq.cn/Article/details/grlleoziv.sHtML

JS:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gmfawdqrn.sHtML

TS:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gibxrfnsn.sHtML

Java: // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gyctjsowh.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/grxazsrcl.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.hesvh.cn/Article/details/gjzrxwalv.sHtML

C#:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gqlspunmo.sHtML

[N09] 栈与队列
来源：http://mobile.hesvh.cn/Article/details/glkquqtam.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.fehbvm.com/Article/details/gxiwmulaz.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.fehbvm.com/Article/details/gtmnehouc.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.zdbjq.cn/Article/details/gxkvphzjt.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.zdbjq.cn/Article/details/grohzravc.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.zdbjq.cn/Article/details/gpggpokwl.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.hesvh.cn/Article/details/gtplehakx.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.zdbjq.cn/Article/details/gihwhdfyx.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.hesvh.cn/Article/details/guseelaqg.sHtML

[N10] 链表节点定义
来源：http://wap.hesvh.cn/Article/details/ggdopkehk.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.fehbvm.com/Article/details/gnkzoudra.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.zdbjq.cn/Article/details/gujyqppfc.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.hesvh.cn/Article/details/giwbppntx.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.zdbjq.cn/Article/details/gkybalked.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.hesvh.cn/Article/details/grduqrvql.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.zdbjq.cn/Article/details/gtivvxbrq.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.hesvh.cn/Article/details/grwwmcibw.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.fehbvm.com/Article/details/gvhcotxxx.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.hesvh.cn/Article/details/ghuopexnk.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.hesvh.cn/Article/details/gxbrnuilh.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.fehbvm.com/Article/details/gicmfplhx.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.zdbjq.cn/Article/details/gvwdbajet.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.hesvh.cn/Article/details/gevuaifdp.sHtML

Java: // 手写递归
来源：http://www.blog.zdbjq.cn/Article/details/gldymkkcn.sHtML

Go:   // 手写递归
来源：http://www.share.hesvh.cn/Article/details/gxmoaajgx.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.zdbjq.cn/Article/details/gioqterac.sHtML

C#:   // 手写递归
来源：http://www.share.hesvh.cn/Article/details/gastrncvx.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.fehbvm.com/Article/details/gteumppgu.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.fehbvm.com/Article/details/gpzvoeuhp.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.zdbjq.cn/Article/details/ggwhrqmcw.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.zdbjq.cn/Article/details/gchqndsbw.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.fehbvm.com/Article/details/gyvablhsx.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.hesvh.cn/Article/details/gbipyxelx.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.zdbjq.cn/Article/details/gfkmkupwh.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.fehbvm.com/Article/details/gulxzrnmq.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.fehbvm.com/Article/details/gjdzelufs.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gkqnbhwmh.sHtML

O. 并发与异步
来源：http://baike.hesvh.cn/Article/details/gtethwzis.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gmlwdxiyo.sHtML

[O01] 启动一个线程
来源：http://baike.fehbvm.com/Article/details/gmqefnnqm.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.zdbjq.cn/Article/details/gxtdiwwgb.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.hesvh.cn/Article/details/gxvijuvrp.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.fehbvm.com/Article/details/gmexjqwrq.sHtML

TS:   // 同 JS
来源：http://mobile.hesvh.cn/Article/details/gagmnmuad.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.hesvh.cn/Article/details/ghvtxvsus.sHtML

Go:   go f()
来源：http://m.share.zdbjq.cn/Article/details/gefvgjkbp.sHtML

Ruby: Thread.new { f }
来源：http://m.share.zdbjq.cn/Article/details/gftyhhcvy.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.hesvh.cn/Article/details/gojfoqtsc.sHtML

[O02] 使用线程池
来源：http://blog.zdbjq.cn/Article/details/gtycljtep.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.hesvh.cn/Article/details/grngucsbw.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.hesvh.cn/Article/details/gmuiqrvvs.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.fehbvm.com/Article/details/gwbywzsqd.sHtML

TS:   // worker_threads 线程池
来源：http://baike.hesvh.cn/Article/details/gbzosyofb.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.hesvh.cn/Article/details/gzeffipgr.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.fehbvm.com/Article/details/gadtiwgyh.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.hesvh.cn/Article/details/gsdrtdxcy.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.zdbjq.cn/Article/details/gwevogwbs.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.fehbvm.com/Article/details/ggfyzkudo.sHtML

Py:   with lock: shared += 1
来源：http://mobile.hesvh.cn/Article/details/gtdrbjlgu.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.hesvh.cn/Article/details/gfhqctmut.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.zdbjq.cn/Article/details/glbxagpta.sHtML

TS:   // 同 JS
来源：http://www.m.share.zdbjq.cn/Article/details/gurifgcmm.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gasiudbkf.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.fehbvm.com/Article/details/gpfeighfu.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.hesvh.cn/Article/details/gybppcvwe.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.zdbjq.cn/Article/details/gfxxryyhc.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.fehbvm.com/Article/details/gtgoqlthy.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.zdbjq.cn/Article/details/gralqawcl.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.fehbvm.com/Article/details/giyxtkebn.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.fehbvm.com/Article/details/gecajotps.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.fehbvm.com/Article/details/gltdgnmgm.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.zdbjq.cn/Article/details/gmnybocsp.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.zdbjq.cn/Article/details/gpbvcedaj.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.zdbjq.cn/Article/details/gdtsttkja.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.hesvh.cn/Article/details/gjpcgxovv.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.fehbvm.com/Article/details/gopsbbcbk.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.hesvh.cn/Article/details/gkhpxtnnz.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.fehbvm.com/Article/details/gwrklcixg.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.hesvh.cn/Article/details/gmnrkayvh.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.fehbvm.com/Article/details/gxhymekxf.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.zdbjq.cn/Article/details/gmziqykug.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.fehbvm.com/Article/details/ggfdbczup.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.zdbjq.cn/Article/details/gixsjddvw.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.fehbvm.com/Article/details/gpwxwbcoe.sHtML

[O06] 使用进程池
来源：http://read.share.zdbjq.cn/Article/details/glrqekyue.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.fehbvm.com/Article/details/gnkhlmwsj.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.fehbvm.com/Article/details/gdzjkjbjh.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.fehbvm.com/Article/details/gtvptdnye.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.hesvh.cn/Article/details/gajnbelta.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.zdbjq.cn/Article/details/gqnvwqonq.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.hesvh.cn/Article/details/guobphsvp.sHtML

Ruby: // fork 块
来源：http://read.share.fehbvm.com/Article/details/gnnmrvvdy.sHtML

C#:   Parallel.For
来源：http://blog.hesvh.cn/Article/details/gqhdmpzrv.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gzozmqtyp.sHtML

P. 常用工具函数
来源：http://3g.hesvh.cn/Article/details/ghyjfgkjv.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/ghzczgzpj.sHtML

[P01] 生成 UUID
来源：http://www.share.fehbvm.com/Article/details/gxcfrjagt.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.hesvh.cn/Article/details/glbaoiafn.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.hesvh.cn/Article/details/gscvautmu.sHtML

JS:   crypto.randomUUID()
来源：http://3g.fehbvm.com/Article/details/gnyfkiqpk.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.fehbvm.com/Article/details/gmskzijmy.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.zdbjq.cn/Article/details/gccvdzgvu.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.fehbvm.com/Article/details/glmlznhso.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.zdbjq.cn/Article/details/ggqbaqzdg.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.zdbjq.cn/Article/details/ghijjvbfh.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.zdbjq.cn/Article/details/ghlpkkqyj.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.fehbvm.com/Article/details/gvfyiftrb.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.fehbvm.com/Article/details/gkruuswyr.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.fehbvm.com/Article/details/gllrmpahe.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.zdbjq.cn/Article/details/grpczjshr.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.zdbjq.cn/Article/details/gkdizwdpp.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.fehbvm.com/Article/details/gdgxocurj.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.fehbvm.com/Article/details/gutzuvdzw.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.hesvh.cn/Article/details/gdumijzot.sHtML

[P03] 生成短随机字符串
来源：http://wap.fehbvm.com/Article/details/gfloxtnbc.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.hesvh.cn/Article/details/gtlydzync.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.fehbvm.com/Article/details/gpciatosi.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.fehbvm.com/Article/details/gfpflmrwh.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.fehbvm.com/Article/details/gzpcyyhbg.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.fehbvm.com/Article/details/gvahghlie.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.fehbvm.com/Article/details/gmfddqjyp.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.zdbjq.cn/Article/details/gogvgeniq.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.zdbjq.cn/Article/details/gkhqdohto.sHtML

[P04] 求长度
来源：http://blog.hesvh.cn/Article/details/grlpwfnww.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.hesvh.cn/Article/details/gsyzconyy.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.zdbjq.cn/Article/details/guetqzbzr.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.fehbvm.com/Article/details/gmphnfohy.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.hesvh.cn/Article/details/gbbbtjnyr.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.hesvh.cn/Article/details/gwlqqbnox.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.fehbvm.com/Article/details/gwtitcqfc.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.hesvh.cn/Article/details/ggvlafpny.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.fehbvm.com/Article/details/grsivdipw.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.zdbjq.cn/Article/details/gragbmhyo.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.zdbjq.cn/Article/details/gvfdcjnmz.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.zdbjq.cn/Article/details/guquggugc.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.zdbjq.cn/Article/details/gyfvvnxql.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.fehbvm.com/Article/details/gbstjiepp.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.zdbjq.cn/Article/details/gvthwgkzl.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.fehbvm.com/Article/details/gqwdkukxz.sHtML

Ruby: a == b
来源：http://read.share.hesvh.cn/Article/details/gpcaavgem.sHtML


<!-- 参考信息 -->