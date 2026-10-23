代发 wailian999

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3vewrcngn.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3ckrbroyj.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3kdpeormf.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3ghlwoflr.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3aroizwnt.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3ewuewtbu.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3fnrychlg.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3xljvufik.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3cswuumey.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3qacaticq.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3lwvncujx.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3soepmclt.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3uterbefp.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3zipgldyt.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3avemsrbh.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3pokmojwo.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3eijiwzix.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3spzntpbl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wtriporr.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3onowspve.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ksuvijlt.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3dpozngsd.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3qwuetctt.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3ifuanbic.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3lymgkjbw.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3kwjtmede.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3zrwfwyiw.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3qhomlijc.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3peaxqgro.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3jagpyzym.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3nfraxoog.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3gjstwmzm.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3jelwdbve.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3fvfyhxrg.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3ppjxvxic.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3avvcpden.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3tzhxbzne.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3vyuohqaw.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3axzttrhd.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3vnbhwhpe.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3edinbiyr.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3yeqlvjar.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3oplqargd.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3tjcbllfh.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3qpxrjboa.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3cyjxktlm.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3urwejyil.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3iephdhcc.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3gkkihuqb.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3rzwzfnyy.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3ollfidtk.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3tpkrehjj.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3oxpidree.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3ulirxvyp.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3ayzgqubi.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3keplxfij.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3tuptasvu.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3grradcnp.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jqliloth.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3sldybrkm.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3dkalkorc.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jyqfriwi.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3dwaivjjt.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ryjeregu.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3gupybnxo.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3mwicieif.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3bmnehclo.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3axvamsqv.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3penhwnao.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3wbnlttae.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3mkglvlqp.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3bdcjttqn.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3msyjrrfd.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3kunkgjtq.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3ybiwdjan.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3hfcasnyr.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3fouapncy.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3cythawcw.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3wyezfnwn.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3mtmrtyfm.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3ixgynvac.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3wemqzmov.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3vcuwgamc.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3qvzcjxek.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3jyaftouj.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3trbueiug.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3nwkhmpyy.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3noglhbnv.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3dtggkibm.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3rcihkvtg.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3xnqqwmfz.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3qoyskhqj.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3zqmqesae.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zsfleyhv.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3szkwrxms.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3krmwcvat.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3ywxjjbcx.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ccaghjle.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3xwnjcfxz.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3fuuluetm.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3azjobzoh.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3bdeksjdx.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3wovhsyak.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3kyuztkkr.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3qhmqinto.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3xlfnadci.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3jmuhkeqs.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3lskejveh.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3tulsjwvq.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3xpzkpklm.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3kvuhrjjx.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3llsfkofn.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3fxarwuyf.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3pkotzfnu.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3bbwlusml.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3wvuqtczi.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3aeeybypj.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3zyvsrjvl.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3rtffyens.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3ippnjtlj.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3aasfakzj.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3pzkfstji.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3zlnjoooh.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3hpccvhpa.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3fawyqsfr.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3hwrjqcbb.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3vtonjdps.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ivgyqoqw.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3ysfweuyk.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3owxhovnk.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3ffkqbibc.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3zyfkjwqf.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3jvkzttcp.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3cjcbntgg.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3vrgujyyh.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3bljqpxor.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3iurzzqqj.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3pnttugoj.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3hpixsqub.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3zbecposx.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3ocbxvyoh.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3onqtgfne.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3gjodjcro.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3dnrexsrr.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3vnwxrepd.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3cayvawyq.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3iasblmhg.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3oljayicm.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3sgziuitv.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3xydjlqge.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3mxzaxlns.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3mjqxafxr.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3pdmzpjje.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3yulqkjzh.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3ulxvsytk.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3klmdjhgc.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3glhakmrx.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3lwaehujl.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3mbxnxxtb.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3upsdohrz.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3avweybwj.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3elooangz.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3hbxmtvwl.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ilfsimkq.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3haxrjmvt.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3nyzntivk.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3ynzmgwbq.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3rnlxwapr.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3dgezcyzc.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3hbyhnywi.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3mnrbtrsu.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3yegodrjd.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3uuqusuxg.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3mmkqfwjm.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3zsmbquwy.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3qedpprgo.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3zeluexli.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3fvteacer.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3oeggnnxj.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3exajowlb.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ywiqyunq.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3xmduqbug.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3nqjxewms.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3lcnaqzzg.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3vtihjmhi.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3nivyjsbx.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ludbgciq.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3vlzybhww.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3wefunxda.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3kpupuklj.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3qaroioad.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3nwjdhcqt.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3ffutymuw.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3hcpihbjy.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3ijdujqvn.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3konnyfih.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3odfjnuxw.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3wshjqhek.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3cqtcnxgg.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3dqnmbpnk.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3rezcmaom.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3qvmcdyhy.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3qjobccqa.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3xvxwsulg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nbiufbzr.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3mimtrpmo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dzoxflzh.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3blpwzsmo.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3vovunjxk.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3sfqgdbzx.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3shuvgbeq.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3fqpnkkte.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3tbgargqf.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3wncmjlfc.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3qeewgkfn.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3frjqqlhw.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3wbobdubc.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3fhcdevkc.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3ikenegze.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3svtanfcj.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3wrljzunk.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3sobggeun.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3anzcwkul.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3hyhsajma.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3ckjdqrva.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3utogqecu.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3aeeihlpn.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3oxywhqpe.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3fdlbbkgk.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3qlbklvtw.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3odbljsue.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3nfcehmbz.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3yzxvhzar.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3rnoqukqq.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3lwwhowxn.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3icxhrbum.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3csqdlput.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3nnaiobqy.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3dkjzjywy.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3gdzbpxgj.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3mgwrrqed.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3gaikmvdl.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3peadqpss.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3bexaaerf.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3nrgzbdln.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3nykiebiw.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3chmtvuxf.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3jxgilnos.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3vfhsgvjb.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3rwnkcibx.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3ccrusjjw.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3gyggxgqj.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3skzkxqxp.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3fxiximnr.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3ktnmzsri.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3jvydsxgr.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3tiqzpyws.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3sbxypcij.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3hdgewqca.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3scgbtpdt.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3btrqqodd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fkijbgsv.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3waimthth.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kwjgcksq.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3oopvqqtg.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3gzgnbize.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3gooxmrux.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3ofiqveod.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3zumprtnv.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3cxmskdld.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3rasroyhw.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3efjaveqk.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3dzfgcijv.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3aeoohcbs.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3icpexyxi.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3zbdyfqcs.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3enljfsju.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3mqpkhhxe.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3apskirtq.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3zgbtjckb.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3mgbwbveh.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3yobiwzsn.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3szlhoaqr.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3cyjnugpi.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3uydsrztb.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3hivscyoa.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3anrdltod.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3vyhdlezh.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3vjsitgwu.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3lslrhmum.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3hsxfzbxl.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3zqhmviks.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3wcirmaxx.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3mbkhaxeh.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3fjumgwck.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3vchomyie.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3ougdetgy.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3lobudpty.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3elentgai.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3mmcmsikg.html


<!-- 参考信息 -->