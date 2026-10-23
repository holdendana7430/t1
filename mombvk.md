代发 wailian999

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3dbjmearm.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3evturxnd.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3kverkhga.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3lcolnuqz.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3rmvepqrb.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3folwolvl.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3ycszpcgc.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3ccitawmo.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3selmwnxo.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3aaqnzfod.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3stcmizlw.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3kklnipgv.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3ebgamcum.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3hgkmttqr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cdnkrpgm.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3bslkfime.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qowmjflu.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3oultcjro.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3hlzfvczl.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3bkrzwzhi.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3fwoqssip.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3yfzdavcj.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3bbaljswh.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3jmxbrbmg.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3lmidnahc.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3ppspyqgy.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3nzvemvso.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3qrecdedj.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3ummkcsfa.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3cttrmqyp.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3diisxwmo.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3fhcfsluz.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3gyugywho.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3dyrsbgir.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3agcnggge.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3tdfsnblt.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3mrizkvvh.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3qdlbtwyc.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3kwivyofu.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3yhntwjnx.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3hwqlmsuj.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3wfiljqpe.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3nhhnxmhs.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3lntcggab.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3ixcbznwe.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3rgmjgnel.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3ptafydpw.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3rodllvkv.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3hfxklpks.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3isrudupx.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3rzkhjeop.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3xjthrwqj.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3bnxhscer.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3vpoqkwvb.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3mupulewq.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3ejjfohhl.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3bzizkkqo.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3eskdftgd.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xddlygsg.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3auuejdig.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3fvgfelwi.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3lflkmkfp.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3lkpmmyvl.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3ypdbanqj.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3kxdsilsm.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3whskmhar.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3jitpmqpb.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3gssntifm.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3ngucmsgh.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3dgsgbsrp.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3vqvnjgdp.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3pawedrbb.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3sauqttyb.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3uiujnmin.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3ckkxpscx.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3eyuhdkgz.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3ztfgmwcn.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3qkspawfe.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3xombuxpi.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3txhpypqr.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3cxymdgwx.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3pbcycczi.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3dmauueii.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3udatawbl.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3bqvepviv.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3xzmmakvw.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3xdtuvqdk.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3eeyajuce.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3ipevzfix.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3laqqrntp.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3hsjktpoz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3quujkuep.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3qcbkwuac.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3yiomqgpy.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3tpsbkrbs.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3roaipalg.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3wihawvoo.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ytdumywp.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3pkdeeimt.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3pftdfjwc.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3qfomzdkk.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3tjnwmcek.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3qcpsyvih.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3afqtknxq.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3dslgjrzo.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3mfueobwv.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3orsfkclf.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3zsfhdpcl.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3yievdwsj.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3hwelwbay.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3tgfrdnhl.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3eeuhkdyt.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3pdpzizoh.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3oheuxcad.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3vbygsjjl.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3dpemynwb.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3dcdlapqm.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3jzbprqcj.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3rrnepvzf.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3gwvwjtbp.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3godmyqwb.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3cpgovrja.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3qfeuyhti.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3evzelxkn.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3nqeetyyp.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3zwvwqdrd.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3icprktbw.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3rcnqkrkw.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3riwgpqft.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3kxutyhoi.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3sdkdscyh.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3gyuhmslz.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3gwyaoksb.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3inlswdef.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3iyjfyyke.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3bwlailhs.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3xnlgibyg.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3gltrdvnl.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3junotres.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3fmrmnufr.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3whlpmkwi.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3kojtrmdi.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3oelgvrqn.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3offznlvh.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3nrywtinv.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3ncqpizzl.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3miogkjln.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3ybtbibwy.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3kdzczqbi.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3trdfffnk.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3excoqyes.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3kvholllq.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3ppxpukax.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3muijywfe.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3ttpjtffl.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3nycwmron.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3ewkxxprk.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3vccpllns.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ljglpwjo.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3bzggbuvl.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3erhcrctu.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3gckbmtnp.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3drthhgpj.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ellcyzzn.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3wjnapgph.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3iguatyaw.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3zpjetdwm.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3rppythql.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3mxgujeyc.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3asumuuyl.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3xiwkvskw.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3uqbqbjhp.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3rainovyv.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3afbjuyww.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3fiwiutfa.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3lztfxbng.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3tesncuqm.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3tojgimol.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3logmnjqu.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3rpkonemr.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3ozvybxuh.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3uxeqjptj.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3xzgnostj.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3nqzwcwbu.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3opingtbs.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3ckdxjwds.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3epsunfuj.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3rfozvbsm.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3dnosfaia.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3nngibxne.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3pvxwjpaq.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3oyljsxgt.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3kecdjoyw.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3xjgquics.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3goxullss.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3rcuajwib.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3ovrqnhde.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3vsxwjfxk.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3ypcchomu.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3lsnivbqs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xoucvzxb.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3aaavxbrx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3appufziu.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3hbdhvxzc.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3ocjzgnkh.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3vcwksvcl.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3ofohxklu.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3djxutlmc.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3nodwgmtv.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3vrrcexec.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3khvemxpm.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3ssrpjwcw.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3ixbuzesf.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3rrvgnlvt.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3soqncgok.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3ufvtxqmi.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3vtpfoyuu.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3bvxrkcmq.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3gnhgynif.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3bittvvkb.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3qjsvrujd.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3pyfuomnc.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3alcvryio.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3bdlyewqs.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3qnzgrlbq.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3aulwgich.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3kbddihju.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3gqvmcofq.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3peyzicrj.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3lebiksis.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3mxjdslsv.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3opeoadjc.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3urlvrlgd.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3joswpehj.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3uzzoioue.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3sskhsdvf.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3wxjotkun.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3ydtfjtvg.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3niskozsi.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3ygwvjcdr.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3fsgqqcxv.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3yxzdksgl.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3jqzdqndg.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3sxzznouh.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3xykfolht.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3olizppil.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3ccjohqsp.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3dhvplxzj.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3tjqasolu.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3ageekwrw.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3umkdsozu.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3nosadvgs.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3wnlhftxz.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3zxystgil.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3lmjgbpzi.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3zpzyqqbn.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3bjexybal.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pkttfjdq.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3exysffhf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mqtkyapo.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3eieeghru.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3gmuhmqtj.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3kpqoqiys.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3bphgytsa.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3xajigbwp.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3hlgmwery.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3spkafrja.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3bloodkme.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3mlvueeok.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3kmcbtbwi.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3lvmbqjty.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3cigxiexk.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3nupiyaas.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3nvwbppmj.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3kmuareux.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3ipwtyfcp.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hiztftup.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3xjqdntoe.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3msakcwme.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3vhqbqbrn.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3hfrvugvq.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3nichowqp.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3wtbaligs.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3htqstppz.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3adylbhvx.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3urtgudfc.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3kznzpyms.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3gcbgcvjp.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3dcoclfgo.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3lkwcyoxd.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3jjxkcfjg.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3ndqubvgi.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3zweolhmj.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3qwdnhqcg.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3ibqsxpnv.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3elckwslu.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3adraxpvb.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3wdbnvryh.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3gtvuvhxv.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3zqtjvxts.html


<!-- 参考信息 -->