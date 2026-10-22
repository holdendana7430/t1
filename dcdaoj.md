代发 wailian999

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2atpbzybd.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2vyqfnfmq.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2wefbpjlm.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2ymqumubp.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2fxkzhccu.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2atknzxdz.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2fspgtbze.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2rujicksk.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2yblvyemw.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2ggcgmuia.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wvctysnq.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2mwurlzug.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2klczgqql.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2okhxnmnz.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2awojycdh.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2uaayudbi.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2rahnhhfr.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2vmcxsaly.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2rkyurxns.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2lnvjcyay.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2dwjzrvxf.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2gccaozno.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2pofolxvw.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2qjeqqmjw.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2amjopmyc.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2sbwtmzgk.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2ucxsuowx.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2votbtqpt.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ipqihgdo.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2cqzdluhd.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2cznftknj.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2srwvcmoj.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2czvpekhd.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2kfbtzwwq.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2levuvllw.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2tcsywbmy.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2ohbiekof.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2jlrdjtjs.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2nuukmpmd.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2onvqjtoy.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2tlaubdhx.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2dlfzmmax.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2qxprvhbx.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2idaiilap.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2fuaoqebd.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2stfvijje.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2ewlgjimb.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2sqrnxtgu.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2usfnlxwa.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2dsoffeef.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2euqnylvw.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2ktsdceiv.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2geokcvvi.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ntulupml.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xnhfcuic.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2uqygsoyu.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2mufievah.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2dzpaykdv.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2vwvqsech.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2zpktumid.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2kzvkxkvi.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2fpiskkft.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2yvnbmvlg.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2gqapiwen.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2odbnrdto.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2psxqeyml.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2bpcgvujo.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2dnmvvpim.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2pxikimok.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2khjsgeci.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2xgpdilgr.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2mvbobcis.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2euvdvpco.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2uyflnict.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2gplrsinb.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2pcssslvb.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2ayprskno.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2mbomkgud.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2bkvqliaq.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2qdqvlyxn.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2chlterfs.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2upnmecqo.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2pzoqkcut.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2hmpymnxq.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2fzdkpkqk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sjmahwxq.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2yxaxzbow.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2plvnwnhx.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2rrfwumus.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2udqkmpem.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2mjmwknon.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2tjnkkwcg.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2elqvcskn.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2zfhneynd.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2oavvqisy.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2bcxnjwvc.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2dkkudqgx.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2pyxxloun.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2vflujwfc.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2ukeybuuy.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2irzmkrtg.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2crghgugd.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2ofcllgyj.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2ldteiobo.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2faazqoks.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2byisopsd.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2ghjjiwqu.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2eoclnykt.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2xszhgbti.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2agvqdcil.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2krkdzpru.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2fdyatnyu.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2ssrvjdbp.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2jcexpjxs.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2engqcfdp.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2vnuydjwi.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2dqznxryh.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2vgjfrwne.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2rzcyhnwv.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2cojhxzeo.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2vsxmnoey.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2qjcebyzz.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2daarvnci.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2wymoaesx.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2njrbwhxu.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2vwissdfq.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2pzybwlkr.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2kchzbbrh.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2hbwlizey.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2imnhfobo.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2npaarpkv.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2jimhlujg.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2fgblwpjx.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2inufdbuq.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2qrltpdyd.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2zzbaqnda.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2pulhbrqt.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2nlejsvlt.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2ujovtzfx.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2tyrjfrqv.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2dcuejvkj.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2cwouvjfj.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2ugmuhoss.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2tlfmbuwr.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2krmgetpr.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2jfksucta.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2rvogmasr.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2dknmfhxz.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2cxlafviq.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2bfellkxg.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2ormhmzre.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2tdqqbmxl.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2kvpnmkgh.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2emabgspq.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2oaaiehpk.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2dctbejkv.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2vkvgsvtc.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ddchcrwd.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2wvmchvpd.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ndtxylae.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2xkxejosd.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2zhdztoqf.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2pznxadij.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2pffvgmzz.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2crvrnntj.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2qdybqgoc.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2jdfxjcsl.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2azixsqvf.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2lhnjdsfx.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2jshljahe.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2jwebyszy.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2blurehcp.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2eciheibf.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2wkssrlwn.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2rtqjktgi.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2fwdhotey.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2ihqnkvgs.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2lfizaqpp.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2vilmispo.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2jwwaebyl.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2gksofhgs.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2ufmxcasj.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2mbgwznlb.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2srwxliog.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2tensnqoy.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2srodyavv.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2ttplgbwg.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2xlgvmjvb.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2lixqzsxr.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2wyttfrkr.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2pmgjdxds.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2paaarwql.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2pvzsdyve.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2fuporxam.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2sivfwwlu.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2pufwhtyx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vyguwftl.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2gbebterh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2asvqjlib.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2mutgvqil.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2ocqunxus.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2ktkozctz.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2kjrezxwa.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2vtegjmyd.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2ogtvtsgt.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2iwrbbtvv.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2qglofqan.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2mepbhvly.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2vyqyndqp.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2uyiyesxp.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2wcdyygpo.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2twjuekcl.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2rvvqjwyu.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2zyqruqjj.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2fffrkjdz.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2pncybmvq.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2lpqxienk.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2juhtupqr.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2nccyteqr.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2ngmqrejr.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2dhoqtond.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2iujucfly.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ffylozux.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2zgcyhqrz.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2klskncrs.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2kyljvfjh.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2iomdoyqy.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2abumlprj.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2ecvrwnxl.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2ebomisky.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2lojhzoca.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2wbfytrea.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2rhnydsav.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2yauwecli.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2lfkgjbew.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2zvbphhux.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2ugvmxktn.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2vistqexa.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2mqgbzcnu.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2qjlcfdiz.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2yvrjfphw.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2irdzcchl.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2yvgcffua.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2llvkkmlk.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2jqyvfvdo.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2fkkmfbuv.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2jerpggyx.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2nuepnoyq.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2dipxfvsi.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2sewrbqtj.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2eneuhvcj.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2zoekjtkf.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2gnkuhhrh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wiwatkts.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2ojiikzsl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zxboiywl.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2golbhguo.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2iigshmbh.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2dibrretv.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2slxiflvy.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2zotcrwlf.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2phfhxvuf.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2jarkdqxt.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2mkhjrjcr.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2bssmmjfe.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2cbdouhle.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2swnqwsbd.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2hfyaoemc.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2isvovomz.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2gvczvdqe.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2ejkbtgqb.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2eyfaoesa.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2ewsroill.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2qfqxxpou.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2pkzcvtia.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2oavxljlx.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2yegwjpwh.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ihljnnlb.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2yeapuerh.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2amwtfaib.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2waabotqk.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2fzaufpyh.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2ejgazplr.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2qckfbikq.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2koujfsns.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2cufnlysr.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2osqbyhoq.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2fbzeyocr.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2lxdspuqs.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2znqircyz.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2evdjniyl.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2rmkmecme.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2rcaqwsro.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2luhsefwy.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2duedjwnb.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2iyfxymyz.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2jetnayuy.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2jzinyrui.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2zwtivdiy.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2sradsfwy.html


<!-- 参考信息 -->