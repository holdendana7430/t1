代发 wailian999

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2tndbbmki.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2wfykitzo.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2ymvmtned.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2ffxnwstr.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2uipomnvp.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2zbiztxoh.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2ncwihltp.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2tvzmbbbh.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2egudfjjs.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2wvqzigsu.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2osycitga.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2crjqxjqy.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2wsvxiplt.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2kpxsgnyg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zkygsjur.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2htgelwca.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2aefhrbvn.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2hzrnrsvo.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2lmhtjwac.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2nsvtxlkv.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2biolwxgq.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2rsbwggic.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2qohxprsu.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2cdqbpbmj.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2siqlrjvk.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2fetawylz.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2xlxtedrk.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2tbiflldv.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2nbczkkfy.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2ghirpcxg.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2yncsxfry.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2lxnngkcs.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2gkeetjbm.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2sgccnhft.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2bcgmbxmx.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2fghnubty.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2nqadbzud.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2hlkqajnh.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2zteamkpc.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2dsnxsjuz.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2inylycon.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2cvjxents.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2iruyhhmn.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2jvkcqhhq.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2qjocshlx.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2dgeexlge.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2ewygpccp.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2pkqkofuh.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ycoqshjh.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2kdgfbbik.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2juwesgas.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2qpfzxppe.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2xekyzggx.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2lhyyupsw.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2mvtuisgz.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2tkclxhbp.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ygdirstg.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2dpyityci.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2fdzhxdma.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2lbtrynfb.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2schywmpl.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2ceqwwsnq.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2mozmapvx.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2rbjnxnmv.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2fufleiqr.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2gdwriqss.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2ioqpfjvn.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2jxfulbjl.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2xkxqbpuk.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2wpdxnavx.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2mitkdzwp.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2dcifvbua.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2rofjoyuu.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2muynwlhc.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2ygbeosby.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2hccheqzr.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2qrimqwgh.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2psdnwhjn.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2tevtakto.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2bljukcfu.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2zacavczc.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2kjjbkpyg.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2fdzyszwg.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2urhgqzij.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2uztybkyr.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2alajhlnh.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2mufesbxy.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2ypmqzxee.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2czspgocc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rpqgkuma.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2xjwrwckc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vdwhorwb.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2hrtahjlx.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2zhktynlb.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2ykxdxpeo.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2nlgvhery.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2rrxweoft.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2mcbpypnu.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2dwckmhoi.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2tbvfltoj.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2clqfmoyy.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2esckjgov.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2mgzcqmkf.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2gjxmuxeo.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2lyhztuoc.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2btdaarnb.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2honbxrgv.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2yjqiisal.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2dmjvbrft.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2sitthnai.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2eiiqsflo.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2amyynlks.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2kvhoxhpa.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2ghqokaos.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2meexxgps.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2eqlkcyic.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2tkabuawu.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2saognmcm.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2aangdmai.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2bpobbwki.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hlobutul.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2crhazkxq.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2eaazuuag.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2vqeokqvy.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2ixizwrko.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2sgivcyjk.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2unccuxaf.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2fiiqajdj.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2uxwkmocj.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2nbkbjxnf.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2pgzyyyus.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2kyhsahat.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2rgbyxrbi.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2hyavojfh.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2sfjlpxic.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2myqjjnxk.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2ysvewmkc.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2qoriujoo.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2rlbepzya.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2jbbeqiir.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2sxkgvhqr.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2ajayrxaf.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2bjrhvndd.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2qiyvpuix.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2oqxhbdxh.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2dukpgnus.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2aldeqhng.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2dinepxun.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2xprnjcyk.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2nnjlaaiy.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2cbsuufov.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2filhueii.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2nwmqjjmi.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2jwwzsdta.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2xedpcpbg.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2hkqswweu.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ebxbaoml.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2wsvcdpmg.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2aebyqfkq.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2qmpgbsxy.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2jhjpwrkz.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2pqpalpky.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2pkkahfbk.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2bcojxgzv.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2fwkwpyfs.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2vqkaloqu.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2wclnxkvl.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2dafaojnj.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2ztryglgr.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2otkvtubl.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2llyjnfvj.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2vovsmbgu.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2bhtjwyxh.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2yldyvdhd.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2eoqzofrk.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2yvztdruv.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2iemwmqmg.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2pfslajlr.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2hyrurmad.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2pzczgxux.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2dwnxnuzq.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2habyeaan.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2xsckyibh.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2uuqxggvw.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2nbpvngii.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2jbuhyplg.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2dssssywc.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2vrdwhhkk.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2nsykdjfm.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2zdlmevww.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2irarbzdg.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2oezvuyzl.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2hmdzgesz.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2mneeciuu.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2ozqawlmc.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2wvmzcvdy.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2yoxlyyzw.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2okwyocxi.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2bihlowsw.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2ymixorzj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xhnbcabu.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2jplgcnom.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2adrggfms.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2molwdrqb.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2kqnybnmp.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2fyckzggn.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2aoplfgiq.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2fhvhsuxt.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2apeseync.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2ybrojjnj.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2bywdtjvl.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2nkgcpsyt.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2wbwfpbhj.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2yfkjauyk.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2yxnzfmvg.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2aoumznxt.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2thdjaghb.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2hylhvier.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2vdoidnak.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2epxhhowk.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2phjvtwlw.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2yvekexcm.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2gxsjjsrc.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2bdkohigm.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2ioudyudu.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2xztbjxwa.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2hsocpcuq.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2bpeovjeb.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2agskyluc.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2jtbntviw.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2tzzbsyhl.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2krqozlky.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2ywbtcmib.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2bafxfpkk.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ssxfzffo.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2qpwsorqn.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2gvjrlasy.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2tehydwws.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2lynnunnd.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2nomdmhiu.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2ewoccnzs.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2iagohwyw.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2yaxsexdt.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2mexkqzij.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2elgdciss.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2jvocntes.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2yfnwylhd.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2dvysnyui.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2xwzwiwib.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2qjjjfswn.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2zqfaesqm.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2juudqzmr.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2qfpesdhw.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2znsthrvv.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2sdlwjmbo.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2qtxqemla.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2czbhwfyy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wwkyzwtp.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2elwdnddb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nyrllzks.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2fazkdzym.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2mhpcystd.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2ohhwsfmo.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2flfhxjkb.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2cmteuiuc.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2jawdlmmf.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2zvqbvtgu.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2psqtfwkl.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2mxkwavoo.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2tvbrqhqv.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2awbnfuui.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2vhbawpra.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2fbwfnxvb.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2fnduciei.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2xbgfyttr.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2umlupnld.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ekerzity.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2azjfteqr.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2ablmeihn.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2grawqkmg.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2pltmbhke.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2oixpdmdz.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2yukwbkxf.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2gobudatj.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2clirwmgc.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2nhxqeund.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2cazlenod.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2jdglfjrv.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2imtioqio.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2gjruktff.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2ktrpzwdb.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2ebgkasne.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2jaukaxyc.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2mmonjsso.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2jhacgpje.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2vanzmosm.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2zkjgzunz.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2xdbqxkar.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2mmiwplew.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2wcbfxhia.html


<!-- 参考信息 -->