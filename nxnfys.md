代发 wailian999

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2ozcijgmo.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2rshpaxhk.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2xvhevvsd.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2wvdtynwq.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2mcnexsaz.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2yvmcsicu.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2uevbymuk.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2nobngduk.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2ezdkwoyv.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2pehqsfdp.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2tzchncsq.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2xfqcxdef.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2tocqtnxa.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2ujhrsuas.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2mizvshvw.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2loxycnwe.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2pcrswjqn.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2bnrgeegj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jcexlnqt.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2gtagexbv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vpilorgo.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2emcivokp.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2sfufezfm.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2dhlwtjvm.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2gplfpzaj.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2rhzlkdfp.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2anbqcxpf.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2djfrhywh.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2wnqawkuq.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2huaznhln.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2hgwkpiwz.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2yvujocsa.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2bozerxza.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2ndidgcbq.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2yxsrtzfp.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2amscfajd.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ajokmgtq.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2pwhyhmlo.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2rfqkuwni.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2pbgcjsar.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2bvlhmaxq.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2zsfmvrhu.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2olrhbmeg.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2glqblxah.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2ruslsupe.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2vcgaopdx.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2hkkunepa.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2xvrpeqmq.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2mqdqvrek.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2qqzkvamg.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2vhzqpwdd.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2vquagkbu.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2vbiityov.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2vazfkxgy.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2iytbwnrp.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2bhxbzdev.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2ykcozajn.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2fczksjel.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ukrukqba.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2qgnkgeej.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2fgowgtax.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vzllivgg.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xxxyfcej.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2lpnrtcln.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2tbeithqu.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2ngetvbmk.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2sxwzrvjw.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2zktscyla.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2ekdcjmpd.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2dantblsa.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2efozdxkz.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2yxirfsrf.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2cipfargr.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2rfhnjlrm.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2rqdmpbnz.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2xeshcrxv.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2tutjdrqo.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2lsqxjfhu.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2fltsxpaj.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2cslnqyzi.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2mclrdkre.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2erbgehvu.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2nllqloap.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2brdioirx.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2nakrvurd.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2srzliqld.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2seqykxpv.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2dmncizdv.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2jqhbbvph.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2dtndtmrr.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2ctmeuyqa.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2znbmqnop.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2anivjkca.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wviusflk.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2nlokxejd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lyvckldd.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2zkmiglui.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2jnxtxlrf.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2yquydkbe.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2abagbewf.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2keqwhbbn.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2qyhuumfz.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2stkaaqgb.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2zphjpfow.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2vmxukqmc.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2xotlqlhb.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2qrfpnipr.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2idxlplsb.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2mozuyanh.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2yepffhuv.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2tvbakzxw.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2enpyiqzn.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2hjumxpds.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2jlaouzdi.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2eicwgrci.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2xgiouxml.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2oolbxwbx.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2pmpprolx.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2ubcjpwon.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2rnajnbos.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2lmxagcwu.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2qmyyzabc.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2uraggcfp.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2tgvqppqb.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2vpaxqiww.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2hvykpyke.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2acdljvdj.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2xdntybbo.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2isoboucc.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2lqvifryn.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2cgcztzrk.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2wcdpsmtv.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2ribfrwog.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2xygybssf.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2artzsibk.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2mfqmdeqb.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2pxchkpmw.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2wxaansgj.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2xcjprdxp.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2habvlvzj.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2ljfstuds.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xtvpnqep.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2dmqasrds.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2emwddwde.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2addhebsa.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2lvbjxpmb.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2vfbhfbgk.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2vrpdhrjf.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2qfximrah.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2wirjpwhl.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2szlanvao.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2mijoljtt.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2pjxoccyr.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2behoyoxn.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2iuhjccsw.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2wmquzgos.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2ohvwwgrs.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2dlulsbiw.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2ttehbfuw.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2rjpbzbkg.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2uyzopwpv.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2tgjvtfci.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2bjuhbyma.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2oailmqjb.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2hkeohqme.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2kayquhnr.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2xyclmwpz.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2mhpraltg.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2mhesdrso.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2bigyhyok.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2otlgdmrz.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2szpyxklo.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2gfdxfvwq.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2xfzovfxv.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2mvisddlg.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2bgrnetgt.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2vocchzoy.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2dhyxzsbs.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2uwfxwxvf.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2iacxbnuf.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2vpjtizef.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2vtjlqkea.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2vuextxuw.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2vscfijql.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2luzclxvv.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2svatwusl.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2ujttfajr.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2utdrfexu.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2hjwlthjk.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2ongsscck.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2dwgssigq.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2fccywmpd.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2rwlimook.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2orlairrh.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2ofiqyjjq.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2jmyilavu.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2xzgadftu.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2sjixigzq.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2zlvfnzbi.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2ssrslfdw.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2upfmwbgk.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2urmjoyjp.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2rzmuzlth.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2yohongnm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2htxloytc.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2oqumuldn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xwikqpys.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2xljgwjjy.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2utkvuqdn.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2ngwnyujf.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2jwenenrm.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2jchsktwx.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2ctiqdghu.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2cjojjphe.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2vpinhzsk.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2tzivnvcp.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2nzguzxwz.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2giumefzc.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2gdoefsst.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2mfnceylo.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2eygolyhm.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2ytuuqwym.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2kgpdupms.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2tsrothma.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2bnseqpbt.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2ijmyaqpb.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2kgtnmnfd.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2fkvlykrg.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2mdhjxcfk.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2qytqvlsc.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2hsvvyvoy.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2bnlnfsxg.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2qhmrlngc.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2afbzpunm.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2hwxsjcog.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2orufrpkh.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2jjfagzog.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2sgwwcwrr.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2tzxhcimt.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2imavvziq.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2fxkkzzfq.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2zfshopnc.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2hnfodyfa.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2jnszobyx.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2utsmmyao.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2qunpqewn.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2xynxxkka.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2pzctrjuw.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2lojhgoyo.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2sqtqdfie.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2rvfcjlik.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2wnsbhamg.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2xaxaiuuw.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2mumsgpyh.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2dwvufozk.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2wbqiwncn.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2saszftqp.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2vlevqrmu.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2ampzdjig.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2nompaoow.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2hzweghgc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hoccwfhf.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2fmmwsjzq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mypcdvjn.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2kemklivl.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2lfjqimyz.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2yuophexe.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2pdjnmorx.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2uuoihfqi.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2mqsgajvk.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2ofjdbqdc.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2vflrsvib.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2yztnyeja.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2rmlumzww.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2kggvtkzn.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2vzbynovq.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2rfslihqa.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2hteqaypl.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2fnexnvio.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2lctlxwxr.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fofwpuxf.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2pplvbxen.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2tdsufkdp.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2sdctluwf.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2xzodfwcm.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2nhnejnit.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2wjaapzem.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ykgyfrdy.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2ockmiskw.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2cmaexkog.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2hvpoweiv.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2ekenbbov.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2qggssmsh.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2eouoqbqi.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2vjtixfjw.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2ryewbwpd.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2lsyepnsp.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2fwdpeqnt.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2askekttm.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2kqprtcos.html


<!-- 参考信息 -->