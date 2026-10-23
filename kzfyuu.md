代发 wailian999

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3hofomrib.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3ttoaocuc.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3atidlcqu.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3ofmjbiri.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3cqzrlxxn.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3vlrymstl.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3lqpyltny.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3qjoatjwn.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3yeasjatx.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3rzzocejr.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3voayqgee.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3jlbdterr.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ggrsqruj.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3fqcgyynl.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3llntmvcl.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3wuxyespf.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3qwjzrdue.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3ajuzgxbx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gempvegh.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3gzoudizy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fmwzsfiw.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3nbpwxbny.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3yfziwfrv.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3uunmlvjh.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3pohrtjfs.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3kwjhgggo.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3iwyemclk.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3whpltoel.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3vkxgnzhi.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3ttcpbomn.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3rjgatxmg.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3efjedgqf.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3nppktpxl.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3crsluxus.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3hrssogzk.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3wbgthyab.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3wbsjflhv.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3lbqrjebz.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3ruyjsbwr.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3jotcqonc.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3kshurpso.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3khmfiovl.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3weclgocy.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3ahmjkfct.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3rhzbqbeh.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3pyejzfxq.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3mrccuqmt.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3zxzgidca.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3adzacqkm.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3xszvggpp.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3rsiosjnf.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3fpkkksvr.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3vwdthcgw.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3zcpkvbqu.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3qfbnmqlr.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3tqwnsvnr.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3wonqcrap.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3fbkzgbci.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3fltrqqzx.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3sziuwdlh.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3hvklztty.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3fwslnieh.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3tmuoeouk.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3evjppifz.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3fcxoyhvo.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3utqkymwk.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3gmizmixs.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3lkgzprlr.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3qrrbqwny.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3htplpaoa.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3ohhwrlnn.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3bszxqhjn.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3rliqtdse.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3htjkgpin.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3uojrqflw.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3bezkxndr.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3rcrgqefx.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3hbsppakc.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3xotiwmek.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3iqhwuflz.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3kmxcboyb.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3mtwmwgbe.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3zkimrcwu.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3qydbycqy.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3vbqatdte.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3rqgeisuy.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3fpeoqvws.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3epknttyh.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3xclciqbu.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3wzwzsrlj.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3kgoxbbvy.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3bewlpykw.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3cgshjwah.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vwtlggfh.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3dislbjya.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jtuotbbd.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3dvxcndrq.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3elnupsrq.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3pjapgdlc.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3zrtdegpm.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3sqlyszum.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3qlnrvxla.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3xbepdwuc.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3zhproiph.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3atwibsin.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3tfmdmzbm.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3obgqhmtb.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3ibbroxbz.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3xrbyfiru.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3rxtpsann.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3cdzqjban.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3moshvzgv.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3acyhcosl.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3logrvysb.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3nmppdlje.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3qmbatqzj.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3wywlcvkz.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3mnkyqvsf.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3sxaqxmcv.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3cytqblvd.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3sbqhsmrd.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3gsczmops.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3ufglezaw.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3vozgllfq.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3dbennenp.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3advzfvtt.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3tjcqhvby.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3oiznrhqv.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3hxdvqbfg.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3xuicklwy.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3axngyktx.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ujuxcrhi.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3ztkruxag.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3rdnvbcpg.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3seknlsmz.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3mssqnzgw.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3efobjzbw.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3bcrxadsm.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3ezmziivo.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3bzbiuvnu.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3pylcstmm.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3okftujwl.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3bmmieohc.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3zccrreld.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3dfgxzmtm.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3otynymhb.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3jvsncrau.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3hjsfufak.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3equxmpqz.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3oweqltgl.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3khciigjy.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3ezopqjno.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3lmikfcwg.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3ijfpqlvo.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3uustmpxm.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3wmetezrh.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3vtpfmynb.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3bygpkndw.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3ougojmpj.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3qxolvluc.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zdnealnd.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3rflrzhoz.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ofgnlgxm.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3gelxeaya.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3lvbztfbx.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3empinpaf.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3rwbnxpgr.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3akdqnkqb.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3ualpqpfk.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3lizlrfle.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3ymptnjuu.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3knrfvcru.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3lzjhwkra.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3ccfyapbg.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3fmarznka.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3dswjqwim.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3zwnnphqm.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3ghnvylts.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3noqesfcw.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3dwgtvhbj.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3hhinwyck.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3umeshjlc.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3sanlkyqu.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3uhablcwm.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3qulcbrik.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3tyodfbbn.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3ujduwurc.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3ewghzyjq.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3cxyftfla.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3svmjzrmd.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3dyrziant.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3jqhjtwpr.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3flgpxozi.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3gnzwytte.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3lstguytq.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3dnaoccev.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3mdukgcca.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3klmuisfh.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3ivzrjcjb.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3vjorebgi.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3lptvsire.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3lsjmgibl.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3hqhtvfyr.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3tbrtkano.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tyikbday.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3xnxhdsre.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ygvwbyeo.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3pytcgmid.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3qqmrpxpk.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3jnsjhreu.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3nklaphgm.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3nnsnrbuq.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3dyussjzs.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3ooagavee.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3nclpprey.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3ajgsexmg.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3uldyfruq.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3atkiztmp.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3qaxegcai.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3nqzfxfjt.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3wirlriqe.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3oiyzoaul.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3doxctluk.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3eqiwocph.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3vnvomtal.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3xommtdcz.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3xbgzeips.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3gftcsfti.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3mweipyfv.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3vzqvwuot.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3eqyouxdh.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3zgjmigqo.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3vgdbghjj.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3xjeftiip.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3rksgmeyc.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3zjllbamh.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3zzjecmje.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3hzomjytj.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3ebjcamwk.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3yxitsdcg.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3xvjkajnx.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3ceihalbj.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3hdctkymy.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3nlypyxde.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3ukiatpdq.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3nxoayxhz.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3tvmyltnp.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3imqygzho.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3sripjhsl.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3rpukszdd.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3swjlfxoo.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3dhfntdur.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3jvgingiu.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3abggjiyz.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3gqrbxcxv.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3seewnubu.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3ampmfmbf.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3dmwjdslj.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3stcrulbu.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3dlxwwwtf.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3oiicsaib.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tawjhzrg.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3eosuekzr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3svlkehqy.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3rzmqwuiz.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3qqrnzhgy.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3vtmjfnty.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3knxjofmn.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3kmqcgbpt.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3paxnpklr.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3uetpexjj.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3ebywculo.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3jnpgpadt.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3fsghhoyh.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3uvgcrqen.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ssqpgamh.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3rjknfqqo.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3mitxtmzx.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3loywbmbr.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3xibvvkck.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3csjwkegr.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3xbmnkudz.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3utlxsbfw.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3emrxweil.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3cibcmlje.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3iwmaouzp.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3bfmygtpu.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3fuvliert.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3dqqgjedd.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3erefsvqi.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3umuanpxh.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3ibopdwhs.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3kxpzijtr.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3antkbqwz.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3zhbojgin.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3qejuzqrz.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3quhlhqzk.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3vjfluhuv.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3pmagkjie.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3pmpvdqiq.html


<!-- 参考信息 -->