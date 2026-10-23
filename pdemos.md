代发 wailian999

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3ojgveghw.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3cwypgidb.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3rgrzjvpd.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3ppeqdzop.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3vbmxjcew.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3srvyrbuz.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3benuzgsy.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3gwjznjsu.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3fikkpnvx.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3cjykbwiy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mosiyanw.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3ohsdercx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tmkkwdqs.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3xxtmkhtk.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3ravdimio.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3ljwgaofz.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3nzhzxunt.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3pvjkdtuf.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3gotibcoz.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3eudwkigo.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3tlrwnozv.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3uoskxdxx.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3ququfnsp.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3wvmtiehv.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3djpjtrdg.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3uaapztgj.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3qwmjenvu.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3pgqjhwif.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3hazcmluo.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3eeqstzvz.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3zlzyeqgl.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3bijxyjnq.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3uxhaqbdt.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3xpoyufif.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3rdjpbgcj.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3jsguiuaz.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3dltsirof.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3kuyapqku.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3dhibojbr.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3jpuxxvus.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3svhrmqbz.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3qboptshk.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3ipodryko.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3asiuqrmg.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3occjppur.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3cnlntvlg.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3rjxmerxr.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3exuigzns.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3olauiytv.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3okjkgmcu.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3sxexcrpc.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3sbpgsmvg.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3kexacbrt.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3mdinlvjo.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3xtmsnkvb.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jvymhwok.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3mgpdvifz.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3xgyeqbiv.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3rrzdljum.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3ysshyppt.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3arjzbcal.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3yxcofebv.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3xlhpstjj.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3nzrzvfpx.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3vqxgpeon.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3yradcddt.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3tmzmqmrb.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3svjhjipy.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3lcnevpnr.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3wbartujs.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3zjmhsrxt.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3tdetpyhu.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3jsebfwre.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3pnozfzzs.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3jyqjiahz.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3axcstjxb.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3nhocsvcy.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3zqpbbwvw.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3gphypsjb.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3orkqfslb.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3quatnktl.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3mlasvcxe.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3vuhmpzjt.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3gdahyefx.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3qsqgxrid.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fykklrvi.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3mlvsdtgf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zeknsdqg.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3qkfybckm.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3uaeoodch.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3kawmwxsl.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3ivahmfmb.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3okmffuyo.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3bmdpggyw.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3rouewvpo.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3irfboval.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3qexqsgmo.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3hjtkvmlu.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3mzfmxabh.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3zqwagvbh.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3pcgnfpxd.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3vzchanbz.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3uxdruyar.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3urjnqgkg.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3jwmzgtgz.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3qjcsamoi.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3jblmtdwo.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3gqfvxbwq.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3lsqvejku.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3ziquwqkl.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3zwkusysg.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3tcoazrrh.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3hrsfilsd.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3kumyijtd.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3ybrdnwxo.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3sbyioypt.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3omsogfan.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3mlgncbwk.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3clvdyuzw.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3nnnzwefr.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3akqmwshx.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3dclnqpwx.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3bvkmtijp.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3utdjuqer.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3blowuukr.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3qduqpxgh.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3ziwjmomp.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3ohnmwyvf.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3gfclxoan.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3rmypvpoa.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3gexapjth.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3xknmvbue.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3oczumobw.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3vvxiklaa.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3lyyiapjl.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3yltebjtq.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3qormbhqk.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3oezschuy.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3pycwqyaq.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3igwvkvcb.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3rbfqgjpk.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3demvspaq.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3ngjroxuq.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3srtnoqmk.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3cdiqkpzm.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3mixzlwuu.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3owpuyoys.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3ylslgxhk.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3bnbbovlk.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3tcyshnwu.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3froysgww.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3rnyprvqu.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dxenluuz.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3okpgfylw.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3pungivac.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3nqwwbbow.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ymedmxvg.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3mpzxgxnr.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3nxatwdpo.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3pawatjto.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3fdiaesko.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3oyquamjg.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3vflbmige.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3qyksoemy.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3ypimkufd.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3tprsncjl.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3pxokhvcj.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3bfdeuscn.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3ybspbhvx.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3fbjvawqz.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3tqewwvvn.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3nedzdnwt.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3iblftepl.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3dbdvysmw.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3narrgnsw.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3dkjfcrqs.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3aktoimcu.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3mchxqzmg.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3ajowlykv.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3npypjace.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3wpiddgrg.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3cakeksot.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3chcazezi.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3nytacgvr.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3clszaxwx.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3unkndihl.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3yiafafxd.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3danoekcr.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3zlwunzlo.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3dgouuqdy.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3anuifmoz.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3zhaqgmsg.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3jfmbdpel.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3bzsyfzmz.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3ajoyakpw.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3joxgpfid.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qcukqgte.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3ksgufzss.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fyqecmtz.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3rmhbhcyb.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3ymerjxbo.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3tpxegevn.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3sgchofwd.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3hnttnadx.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3lsomkrrj.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3uswbftac.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3oerdotlf.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3oxyntthb.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3ofjqkbbu.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3zepvewok.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3pjbechiy.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3gfptndvx.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3emrkivwr.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3qvknoghi.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3mtmzzsgn.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3lwusqnur.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3xozshqtp.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3mczfvrvk.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3yffcsrpt.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3kmyyntgl.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3iavthhbs.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3uolxfxta.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3vbmlrbtg.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3qfgkxrbe.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3avepcylh.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3vqcodtsb.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3yuivhvck.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3csbojflu.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3vailfvqq.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3rbenrtau.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3xdbdblli.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3bcdedtty.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3vtmqhhwi.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3lkqbctik.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3fkygkuia.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3kefsqiio.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3lrbfrozj.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3mkxbmfij.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3anegxlkf.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3vvkhnlwj.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3gxnbkzlt.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3klhsfumb.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3ujkmartc.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3ookkfvrv.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3sjppnwix.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3kyzwrfms.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3aemgmxuo.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3qpbtkjss.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3rviybjuz.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3xitoruvd.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3tqzeycvu.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3kfgtswnc.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3ltvtmwhv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zejpozrf.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3gzdfuvdy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ddsbgxju.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3nminuzdv.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3mhzfagol.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3rgtqfbvc.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3hapgodqw.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3kvhuihjc.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3hpqqcwpa.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3dvacfsyf.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3jkxmijov.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3tfkjsiat.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3luaacbtf.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3rquyplsg.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3xmagzcyb.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3mmwnijsp.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3hwwzywvd.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3qilzfzfw.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3buiysvol.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3tphrpdrq.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3yaztmqqd.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vgqonphh.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3dprtivsy.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3suluxotc.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3rufjsknp.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3eswnbkna.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3ejbinckj.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3wcbfdgsv.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3rjhtiznk.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3wddfacim.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3ifcujcak.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3oznxojlm.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3uqzqgfju.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3ctbzqaqz.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3ftdlzoju.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3jkhzsvzq.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3jgeunvsq.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3qiabahec.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3clbrqfox.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3tqnblyyh.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3vfdvhayv.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3fkarutlv.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3nulezhdf.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3zyavbbcy.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3txnpxbqu.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3lefbvemg.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3dvnelute.html


<!-- 参考信息 -->