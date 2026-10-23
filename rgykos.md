代发 wailian999

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3lfwatnky.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3lgbepkmw.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3wwzjuuyk.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3duswxgls.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3nlwoisyk.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3iiimnkbq.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3cyrdynws.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3goohhtoz.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3wsqjhybp.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3jqujhxbc.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3ousshlvy.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3ctfygdbb.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ctbnxotf.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3fmqvnzri.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3kgsjpris.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3kdinwfix.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3okgqoeee.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3vokdgjnt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vnlycekw.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3xpyzxcvx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jvmofrbf.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3maznxjkj.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3cgkrhbfn.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3ugahgjlx.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3gzzyuill.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3qvhhsgpt.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3zparaonr.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3stdnmukf.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3uztqekog.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3enkejeyk.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3vdokbvtt.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3qucybglo.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3qndmbgmz.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3clwqctbe.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3wessqumd.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3xrlnaviz.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3wzfobarj.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3pdrkkiob.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3vpvdjggy.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3zlquajdd.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3utyxyjff.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3aylvxupr.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3jxumxriy.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3tzjttqlm.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3ovnlukjd.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3nyczpttf.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3ddbgbsuf.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3hxhtnsin.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3typjjhaz.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3yugpbcmu.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3rtlievid.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3uueltlgu.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3gjxbluva.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3wklmgeak.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3mamymvyp.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3wqdjcsfg.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3kgcqvtlw.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3bwumzciu.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ykjwbmdj.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3aznxyikw.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3pmjnhbnf.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3pbpibbsv.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3lqhgfwld.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3tuyoqdgd.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3yevyewvt.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3oreuxnvb.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3yoxhnouo.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3xyoglcso.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3pzpdslda.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3zrifsvwo.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3fvbfgfoa.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3yuczuxeb.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3dxjdlgub.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3odilahgw.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3yajundze.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3ckccepdh.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3bkghbmtf.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3okrfgtrv.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3qroelbzu.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3bxhquwwp.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3jnoeajyi.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3sfhevetw.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3ogrzsfjf.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3rxcankzm.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3nghoxiba.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3ckldaxlr.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3srvoswbh.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3kaekqoit.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3tzluzivz.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3ukgrtvoy.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3zkqlxnhq.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3tjogytmg.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3dufkxvxo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bzrxpbdw.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3atjfeeaq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xmniisls.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3ttcrqbgl.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3hwpvllni.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3ucqxqzxr.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3ppavjcxu.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3mhdjbyxq.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3fpncuwsh.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3irkjdniu.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3tfzlvlya.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3qqfqikba.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3yridxrcg.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3nxqdbgtg.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3ddrxjrgr.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3tmnljimm.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3fprrofts.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3lzytdyhu.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hsxktavg.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3lxofizqp.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3mzynnakh.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3jboxswft.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3rqwducgu.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3kiyupajn.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3qufnzmsl.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3ngdlkbwc.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3laevtbtp.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3ocjmkpie.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3jtfhxqao.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3yddhxrbj.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3ippmzwpo.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3utwnvyjv.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3tuvpwfbd.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3bdnixseq.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3mzoxecvi.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3zubbupnt.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3erjkwgaw.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3kafwgqdj.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3xpcuesyc.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3retqyuyc.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3bduheffp.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3gexoqnzr.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3kccdcjik.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3sodteenl.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3cmbsibjp.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3nmqhdrco.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3acruoypg.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3gxyeuvfb.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3xxskdrkw.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3xbnhberm.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3yzhotqul.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3acfzneyq.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3eromuqol.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3jwuqkeow.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3dkxdxqdr.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3tzhoiozo.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3dlsfokhr.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3liwytlpz.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3onnnqgws.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3ngmvytpi.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3bnpuahsd.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3rgcaskag.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3petxhhjv.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3oudmnsll.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3qgxucoog.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3thueblev.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3mfxilsqn.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3tsjipwik.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3pmxilxmc.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3gokettzp.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3kgviltyz.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3bgfssfls.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3lbqkkrbf.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3iphiyfab.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3uwfprqbd.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3fxjuwcux.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3nhtufjdw.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3kxmzynbu.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3ggjobdyu.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3jlyevgwx.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3nkbxnoah.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3vxkjysem.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3ahkjwmsi.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3krbcgrfu.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3tcwvajud.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3chliyptf.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3rxtfnrgd.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3qdkvuvvw.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3llhhcjoz.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3iksaokzs.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3cdsxqeag.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3ielkgozb.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3ffrwawfo.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3elvzhonw.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3csodvfrk.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3ioovnvfd.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3srrfncog.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3lxdryfif.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3vitpqqlh.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3tqkdkeok.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3umfuicmg.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3dldwzevb.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3jzpnjuop.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3bbuhknww.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3lpfczfbl.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3qbztvclu.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3phekukmb.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3rgdsyyin.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3uiejynkl.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3uxgiopft.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3ffoxwvgx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bhvukcxa.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3nhcqdkyn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dswbnrbb.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3htnwhlxq.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3jubcmtge.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3paoraryf.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3cdmdrtmd.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3xmyaxkrm.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3iiyrnxdn.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3lmizpmcx.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3vtziybfp.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3ulnlepqs.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3tzhfitgv.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3ndmhzobc.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3wjqadomb.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3nkaqgtea.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3wkgcbdln.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3rsyduhnm.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3wjlbpjzz.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3cseottwu.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3ldxxirno.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3tayhkssw.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3qzdreebt.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3reiodidn.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3htbwpvbt.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3xikftoba.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3vckiujuj.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3mfvgffsc.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3oyyidgix.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ibvmhldf.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3ivxvzdcz.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3zjdcepkq.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3ppuvihqb.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3nlrisnsd.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3rlanglok.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3xrubzksx.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3lxynvdzb.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3mncqnixo.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3aignqqtt.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3xfryvfmo.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3ulrvxmyy.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3pjkutysq.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3zkpuduwe.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3ecmudazq.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3ksfoaykc.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3acjppmct.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3pcozfhqk.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3hbhfgacv.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3kidilkas.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3byzcphsq.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3geqgzcfs.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3bomebqzi.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3xslzsxaa.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3lgngtxbm.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3lyelnowi.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3ljutpqmj.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3obbmofzt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hafnmrns.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3ngqmwuws.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xivputcy.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3mfxlvfsv.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3fkaehcwg.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3hvqlpwfr.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3glaicnbl.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3kvhbvanz.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3nryjrpbx.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3arfhvxaa.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3jjlsacts.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3oueddezz.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3kwleilqo.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3etmoumhh.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3oyhpljrr.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3vszodpiz.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3piedposb.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3qfldivxl.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3gzbxkznc.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gsgxcyie.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3nyelslbu.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3djlswgyg.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3npwhsbgo.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3tqkgaiur.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3gbhzfzqz.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ralihrti.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3cmrbjxgo.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3wnxhuvxq.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3dofrucag.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3jrjlfqni.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3yqpzxfmt.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3zqjvgvuo.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3scexetcz.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3igjxlyjn.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3bmvqfwcl.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3fvjuifgn.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3qsntmaws.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3wfisivko.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3pugallaa.html


<!-- 参考信息 -->