代发 wailian999

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3lccjypsz.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3wpmestyw.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3nqtytkwf.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3weaicusq.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3zwbhywky.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3xurjrojc.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3esgdeiny.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3doljfbgh.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3gwzzgxdu.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3wbwnvoxe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jeszansk.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3vgpnjrvr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kdcemszw.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3nahtumrr.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3sjaqpgnz.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3cajylugu.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3dfjaxbkb.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3qtkqmnnz.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3qwqdhvur.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3qgnwtxmy.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3cntyfmsi.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3guhagtsk.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3prkwyqtm.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3lawhcflb.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3gdiifmfu.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3hhrbvquk.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3zdnnypcy.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3cipdflck.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3pushlvrd.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3mtgmyegx.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3xingiphz.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3qxhykwfc.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3eahdjbwb.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3iqfccygl.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3uwqgtwqs.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3hpfizvyu.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3axfdoxaf.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3jiumxxhb.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3abbmydez.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3ykupiuvq.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3crqljnrp.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3lbgvesor.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3ygzywpgo.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3melgudpt.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3ohsdxmsg.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3lhuupmof.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3qwfdsjcg.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3kqbwcndc.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3ekmrulqc.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3ydhtjutk.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3dztbqaix.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3oaqlbywt.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ygfqhpbs.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3sgwjnkui.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3pgmppitg.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3csaisnuq.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3yxedzxwm.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3googjihh.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3nuybiatq.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3pikuxejm.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3rbxhtvxt.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3sztjcved.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3uirhydos.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3robwqtkg.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3fabjybxz.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3muxtccju.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3qkfdfknx.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3qetvryer.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3yrrdbljf.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3udbvvsbc.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3wlfvqoql.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3xiaixvyz.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3muobhyee.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3bvziomoc.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3oqjajizp.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3olstwncp.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3hprebteo.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3egkyncjv.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3koifcpze.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3ublbeozj.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3iqagmkqr.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3aklwjvpu.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3yamqnudj.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3qmbzgltk.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3mdyqndmh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xhspdidp.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3utpqeixc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bxketoqg.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3yjldllqu.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3zmnwivqh.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3kpsrzdwc.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3cxpggdli.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3vtnkcxak.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3amralias.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3rmlhvkjp.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3jkzpctaz.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3metsvlsf.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3fhxyphjj.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3ckvxcpfs.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3anwqgwwi.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3exlnrmbg.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3wklxdsqg.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3wrafvbdr.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3psenmhwo.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3wbhinpqc.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3gadcukrr.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3oirwwsqs.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3ujiazfcp.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3hikoyrpz.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3tdsvfljl.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3bmsppkrf.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3mvjodaxp.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3gztflaxd.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3fqqnijhs.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3clovsgpg.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3nfehaujq.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3mhnzhrhj.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3klyrxxxk.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3omeyxfzy.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3zhzluskb.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3giziudgb.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3poriacym.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3pmieqlze.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3parvigiv.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3pjrornjg.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3dfhuteez.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3cnpsszdy.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3wozxzgbp.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3fbspzrfs.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3ajqpxzze.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3xdvuyoyo.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3hbozvwtz.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3bqrpwuha.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3aqdpdwxk.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3rwahpkab.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3udahenhn.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3gizqywhp.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3lgsteswa.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3cziftzmm.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3kkiyjsza.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3qlbmoivz.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3jxbpuxuj.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3airotzhk.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3tjyxjgxz.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3kyacjquq.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3mfnfvtcp.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3dvyyzbxi.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3nxaxtvok.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3kopmggvp.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3rgortjaq.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3relohywp.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3nwcogexz.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3czclwyqj.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3uyxwlmpt.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3jgciihxl.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3rheixpqf.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3fygtylgf.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3gevfbful.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3xrcaqkzt.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3qncwijes.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3hpgornao.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3uutjzyzm.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3hxccjxde.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3uvubncmc.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3qdcydqiu.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3alkmcddv.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3adonmlsh.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3ngzbtbrf.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3ddbwgvrf.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3xyjigxbk.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3nruvfpsj.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3awlikrjt.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3yttscsxc.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3ggdgfkaw.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3arnprrkq.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3gqgmhsyc.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3rraeyqin.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3eynxlcmh.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3hrfjhuzz.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3pgmvessr.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3bsycjcgq.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3chqnqqep.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3titphawo.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3wjaaexub.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3kxyohqrx.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3ucgamwhs.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3oebhrzwr.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3vgmguawf.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3eljgmubh.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3txiijzmh.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3jaheywib.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3ofwejvcm.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3gaojmozv.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3tbtbbgtn.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3hyfthesu.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3qebemblm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uhixrend.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3jnoimgui.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mqtcojyv.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3iqtpltaa.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3bipvlttm.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3pmnnnofn.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3gapltohy.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3vlfegmkp.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3dvokjgqt.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3awfbfxtl.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3bgsbpeat.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3ungghtgj.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3thjmnihr.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3wcfxcbmq.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3sbicnqov.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3bnixplyf.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3zpmnvmnw.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3yuhmfwqw.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3jldlpdcl.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3whytidsi.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3cmevklwd.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3bsutfpgw.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3dtqyefmj.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3gmoywrpf.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3ptbuvvlx.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3zgpocrxq.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3fkxraaka.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3oahxkyku.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3djeayrac.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ejqphert.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3zxaiqeyd.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3iwzomfhm.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3pcqhbckm.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3xvacifny.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3dpincria.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3hoyhrisf.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3bcugqkgc.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3pjmtubep.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qfrpjais.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3cxgdormn.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3hhbfxwzd.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3xcxtsbpc.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3ecfzbzhx.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3hhowqjbm.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3arwazdmr.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3molgyclu.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3tpwcrgrc.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3uxzoigbr.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3vyxunngo.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3novvjzrs.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3vybijjxy.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3ggypnbqj.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3tvjczjgs.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3psceyvmf.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3qeafqqqx.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3pipggvil.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3qmczlxsh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3feearbiv.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3dlhjmvbq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vpddxhtp.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3tgvujjya.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3iullrjjj.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3arpbroit.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3gufndfcl.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3owyjlskp.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3nkbdfnxw.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3lzgprqgi.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3wcdhuidq.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3zghiaupd.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3spyiaakw.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3uztgbpkh.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3qgjdnjee.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3hemyzteg.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3aiskvegm.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3rwgrtazm.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3hirbrxar.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3cgypaqhm.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3sdohgqoz.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jvaeizbq.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3cpwaohht.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3wqxvfxxa.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3muunduin.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3snodanrk.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3nxpsvxhu.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3wxuvelks.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3eyjwvxaw.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3pitwjuqh.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3onzfqxkz.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3kqhqlwzi.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3mjivjiod.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3xjfkqhmn.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3bvjpenwr.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3bhnmvrbg.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3grljdcov.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3pngzgaxa.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3rurzbdve.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3omfmrhqe.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3sgfonehr.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3ykxojvlx.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3vhaklvvz.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3ocvqbmru.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3asahbfnk.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3uigtpipf.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3qqfbswlw.html


<!-- 参考信息 -->