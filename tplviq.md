代发 wailian999

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3zxsuljtu.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3klvuxnqc.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3ehluhpgx.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3praetifg.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3ktioculr.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3fpftrowd.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3ckxyuuqs.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3yenvwvky.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3ermvifvz.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3xpqpjfwq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3anfbjvdv.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3ccblmgir.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nusajlzy.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3iftbntso.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3ybxqrwcv.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3nfncjdbi.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3qhvxanvt.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3nwhgbpsa.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3aeyyplji.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3lwzlgsle.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3hhtvocym.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3ipdgyoag.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3lrsdersi.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3icabdmgk.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3umdjvkqs.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3ktrdiirf.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3xsvdqpim.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3kljjymlz.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3fvmauhtq.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3yxiwlanm.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3iklpglsl.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3fpodmvsz.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3gjjrotaq.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3oaxyssgb.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3dstkkxef.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3ikcyyojt.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3ackgxwxl.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3gzrjbemt.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3eumwvens.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3hcxkuqqk.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3anxmaykh.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3vxqtanze.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3actwjnmf.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3yhcmxnav.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3qzwgfpyu.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3hxhyodbc.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3czjvoxyc.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3qwhmqggq.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3pqgvcoih.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3hgsadpnz.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wjomwisu.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3eczufoec.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3sbboiefi.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3nwpdhzaq.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3fzpzddak.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3mlsjvaky.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3zrbrrecg.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3serycmbh.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3erqtjidh.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3lttwkzno.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3orqsrkup.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3qvirrpbq.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3gjkhpguc.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3lqlpmuan.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3tqfjmdxm.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3mtctrkjp.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3iqwzyzkd.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3nqfvrcjl.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3zxboetdt.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3ultqizre.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3zgsuysvn.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3rbhajlxp.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3trpxruat.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3izbviosm.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3xbbyrlhk.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3fqgmhbtf.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3zeztrhom.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3icurqeph.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3etekiequ.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3hofcjswj.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3zxoyixdt.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3ofgqwmkd.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3zgngabov.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3xcpgkqjz.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3kolqfjln.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bobaityw.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3yeejwoql.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fyorwcea.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3pvyddhqo.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3lxzoagry.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3hobottpi.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3atfubpbs.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3cndovbcs.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3dymuivrm.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3qfjownnb.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3kadhcjrr.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3mekyhars.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3ggjmlwsu.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3szwlvffv.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3ahylvtjk.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3twwytifd.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3kvnfszzb.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3uqkqwaii.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rwyprohv.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3aowjeyaw.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3asiawiva.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3sjofshbt.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3xftrtbbs.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3gjrmkqgu.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3plkqojho.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3amxaexdf.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3fsenrvfw.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3yqqvtvzx.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3pkfixync.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3zdrdozzd.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3uolmyxvw.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3uchyuxbk.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3blamaxvf.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3dyyjsyfe.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3bdatddow.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3zesvvmmd.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3taxfmdad.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3iidwhomk.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3dbrtvkws.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3jpoemsrt.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3zliayrwu.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3kyqjjjdq.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3xnljzkvx.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3eefdldcy.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3ondlahyr.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3dpscugwa.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3gsubstvw.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3yjoiilkw.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3xffxtefb.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3rtkmggrv.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3xrqxmgyt.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ldjufmtk.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3cowtevvi.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3ahnqklsn.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3ccakksij.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3negtcaga.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3bgfqjrjt.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3bttevdnb.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3fwcbokmb.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3kxpyrdxx.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3jppsdzqu.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3hbloowvu.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3mrkhsddj.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3ksfnksvh.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3ixjytyxx.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3epjkbcku.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3mtsecxpr.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3xcjjkrbp.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3icqppuel.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3aivusdvu.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3mpjluhwp.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3lnveygsr.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3hjmuqkqp.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3xgktggtf.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3xolfqjuy.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3oeilekwh.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3mnepaqqk.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3vljmzjvf.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3dwwxwsix.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3oketqktx.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3qrhjgdhr.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3mwxmxchg.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3ebnaapac.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3yyuwhxsz.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3ftshhssa.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3sjsnaddm.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3egqcxsrx.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3anmwvctd.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3xubgxxxy.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3gqayhmwu.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3ykoarmkq.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3lyuhsgbi.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3xtthpeue.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3vecisihi.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3ixeaqpae.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3reowmwud.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3ugrqlixl.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3eqaxsfrb.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3plzmbjbl.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3eyyrlyfy.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3sxiucngb.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3zetzuonz.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3btzaxecy.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3bqdqqeuh.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3yrlodghz.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3rshuhrtc.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3donltosp.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3rjjekfjc.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3uxnvafet.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3ydtodkuy.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3ynlccxok.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sitmoexr.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3avoocryf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nmaxlcjr.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3gayxuiqg.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3yegbieiq.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3rismdxqn.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3kyurerne.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3zarztrjp.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3hplyncif.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3loyztnmp.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3qznnmajm.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3pcgcjhdd.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3nxhypvde.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3hjogqxdb.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3jxcwqxqq.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3ufihfyha.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3kskdjvrg.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3zfbmdmiy.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3vdswtgkg.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3eocawcta.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3esbuigsu.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3tlssqvkh.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3bnmuulde.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3dnwwielx.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3jymwzsqi.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3igmebnvs.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3hpbfgwgm.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3xtitnsgv.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3abswobsn.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ilcgjpsf.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3tonumxuf.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3zksgcczt.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3kaavihqq.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3jjbnzyha.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3szjitcwj.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3mrequuqe.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3kmdakgvt.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3cratzbsy.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3nyripwlb.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3ksewkbgh.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3umnlzuhd.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3tolqhbsc.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3ttjaeuko.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3dfcgndbg.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3lzvdzvhn.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3xejbkwsf.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3jomxhpkr.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3vafwsvnu.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3iyzmrogl.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3vifbpzzn.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3vxsoctas.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3sjasflzo.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3wfhjgxcb.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3qntqnwed.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3yljczpvo.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3cheelaab.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3dhfkdvyy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3paezkbfv.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3orosraxa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vtxyqewk.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3imjqncif.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3pgpbuees.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3sxnepnbx.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3onenfviv.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3zotjmddo.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3lueqqraq.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3ipfmuarl.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3cboxacuy.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3oasiunzr.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3hxodmrmr.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3crskdwyr.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3cyvrhmiw.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3wwzfivkh.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3azcfzias.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3bgzyrbvm.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3jeedwqgx.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3yokkekgs.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3nqctvuvw.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3bsusjpbn.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3aabrcinp.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3baqelyew.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3avgxhnoh.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3xlyxnwsh.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3mmovbdhh.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3oflrzvww.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3zvosldjx.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3cdwomylg.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3vyrtrtyx.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3paaziuhu.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3cksruwwu.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3vkyeuvoo.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3xggaeama.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3svirunxc.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3ukbgwska.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3atculebc.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3wwpvbbez.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3dckjulfb.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3ughyjyoh.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3wjkjftjw.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3zhtbgrnq.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3tjgqyytu.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3avobrdun.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3exeaikao.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3flvyzosb.html


<!-- 参考信息 -->