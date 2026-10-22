代发 wailian999

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2ceefdgxn.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2vavmwgji.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2oliszldr.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2szcdntqx.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2edkfipyt.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2jxshudak.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2pbijayjl.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2siyiwqxf.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2osixebql.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2lxocrntu.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2kfewyhry.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2uypjpiuj.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2yqcokeea.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2wnaaryep.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2whptpoiy.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2hskfrrgs.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2evwiqiec.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2exviuqjb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ptwhckrc.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2jtassdxa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kuolkbst.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2nolvqjua.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2hmzlulbd.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2visdoyfh.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2szvobjwq.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2kzgkxwql.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2jnlwcuwf.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2emblbayn.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2ncqwbtcp.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2alwxmgll.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2cwqbmhuu.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2fyoxagtg.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2dkmxjqba.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2qogsftzo.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2frvfktcm.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2oujvzvmk.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2wittjjsa.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2agkcvkrq.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2pcvknqrr.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2avbuhzpm.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2wffreixg.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2yrjecctd.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2xjlxpftt.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2vwtxzsfb.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2ciizhvpi.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2wtmkqnfs.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2roxhscri.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2lcmlwzye.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2qkgoefhg.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2svtmeltm.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2nrxsjjiw.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2dvlrokzj.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2lfryishd.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2hoasxlvr.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2nlhlcrwn.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2uvhukeox.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2eedkwsnv.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2jrxjfprs.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2osqocrsn.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2bzypwqkv.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2mftqcwog.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2noapeldb.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2cvjzsdwa.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xdrhejnv.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2tbthnicm.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2mcuwcape.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2vfiodraz.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2fenfvhpj.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2lrnkzgix.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2hgoupwnx.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2ecxooqrf.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2zuuazrgm.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2iboelbpt.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2grparlxn.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2smvaquhm.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2ypvqbkba.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2yjgkvnmb.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2qgalwgah.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2modrebgz.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2urrmdoxa.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2dkdinjyg.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2wuiaeabr.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2ppnyfcmc.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2cjwzdzyl.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2tojjolud.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2gmemktmm.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2hytepvlk.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2yhrigypd.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2tmvcrrti.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2uksmiank.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2tkxkmhai.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2qsavffzo.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2rorsnnfj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bjybitlw.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2zkcmydch.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vkqjdwet.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2nopcxczh.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2udlfdozm.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2gjgzulbe.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2kjzigyku.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2aobmopxn.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2cgsrhtrg.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ljvcxror.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2nfouyapi.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2kdiflbvp.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2yfjucggf.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2aubytqci.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2owgvxikk.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2ztvgauvs.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2gdmctlnr.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2dmtmkakc.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vefzmeuo.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2jlnfdycb.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2aizmyzps.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2zpkswxuj.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2csooxmnc.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2jijwrule.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2xjkpsikx.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2yajawdeh.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2gcewxwxp.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2eosngxmb.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2qouknxlm.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2hdqrmqwm.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2jbvnslcb.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2sguvayys.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2pjztwons.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2wansbkbf.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2jexecfnr.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2ecfodjmy.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2tgbhqyym.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2kycpdgdu.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2hwrayugj.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2qtdnawey.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2skxkohmk.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2dgoedwhz.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2wzwzumny.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2snbdgthq.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2kzfktcmr.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2bmvscjva.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ffioiyoe.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2ygdghsfk.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2tukfoxsa.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2kzmhlywu.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2lxyrnrtu.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2zgsxzgqb.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2lvhgtyne.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2ikkujxee.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2agxxqfje.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2frjiscoo.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2ebtgplgv.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2ownqnfkm.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2rqojzimx.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2dsfbnlrn.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2bsiwacig.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2iohgfroh.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2yuollots.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2pftsrkws.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2vvdcilfk.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2tjzlszjv.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2lufslzoe.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2hdipmvlo.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2xfwqrsnq.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2wcfoxlte.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2tnpzkqml.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2twgwgkwu.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2pklfnrdo.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2apkeabgj.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2yaewllia.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2pdpaotyj.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2ovgsrcky.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2ncsiqbff.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2uiqicvlu.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2jjbrkuru.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2ssrxwlaj.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2hopbbyvd.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2esfjeise.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2sgyzioae.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2jaybhxia.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2zfeifipe.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2iwazeeok.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2zfxgnvai.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2pbymjdrl.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2actrffis.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2ujlcombo.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2hcmmunkt.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2aplfeqbp.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2oeutzqtd.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2ujhqepfo.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2jtmaxrwe.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2blonjwfe.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2jgynaxzv.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2yzhawzzu.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2zuypjunx.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2aeqrupje.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2wpzilcmb.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2nfhrrfxf.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2lhxuzxjc.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2kopdcbhi.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2dqktmgdg.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2lulvtvka.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2uliofboo.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2rwhnsnch.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2injxwzhw.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2nzwoofgj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2slbxjxzu.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2wweqhccw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vkxxpkvk.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2opvzayra.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2rmqhdfmj.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2tuqfonew.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2xztphjhc.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2kmeamypj.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2jdgnattn.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2ahkkxznr.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2wixidlps.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2lmdynfsi.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2vfystqwz.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2mxiqgzbs.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2nvmchngi.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2jezmgzqz.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2xhbmmfzg.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2fhfsuztf.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2dhkrvrqo.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2tzdpeqcs.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2ottpjjrq.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2ulcqudvr.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2naidcplz.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2ifpqwzvk.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2fltjdynq.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2iokobvvl.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2ntcenwyx.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2gooikdbj.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2gnandphi.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2izxarpuo.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2leseyjsx.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2mznuqvep.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2fawaaabc.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2anddliwz.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2fqrfvfet.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2odvjzvar.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2lvviawxc.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2byrhmrid.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2waoiknet.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2rgdfihga.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2hturqqfl.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2bglrfsnb.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2eixltrks.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2zmmoynhq.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2bvaljpqj.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2yhgqkqqd.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2sugegexo.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2scafpevf.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2bjznijgb.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2hgrppfhe.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2wrmlpahh.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2elbpcepj.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2crtzxrnm.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2vziqaswf.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2inrlhxqy.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2drtznkay.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2wkncsksx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wmwzfdpc.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2alauuqgw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2riebbfnm.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2uyzcecfx.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2hydcqxum.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2hksxrpic.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2obpksxlj.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2oyhmrwdm.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2witjdfnm.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2psojzeyz.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2fzuyhxzm.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2yjyhhgfl.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2vckzhpdt.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2hekvwoot.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2ngpyqgjl.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2aenbwsso.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2kkxcwcxe.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2utpiktoh.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2hgtxxijr.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2ouizbini.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2qjzgmznm.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2nskwxrfj.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2awacxbvc.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2owkbrghy.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2mjilkstd.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2nllwqpei.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2xyuqcrqc.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2kkbxerdk.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2euszrmtw.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2jluanwea.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2hqvzwobp.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2obqhhelg.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2mbhhanvo.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2uafajaka.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2omhutrde.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2crywhsyp.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2deeodqip.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2hzmbjbwj.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2zllncybn.html


<!-- 参考信息 -->