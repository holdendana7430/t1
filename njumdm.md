代发 wailian999

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2ytbfugol.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2actnsynn.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2pommpyaq.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2vkiyyxtl.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2zwleqowd.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2aexksael.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2bmqtnkyg.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2poshaqfg.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2baoftftg.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2xxdunmmc.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2zlwhwggx.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2blxalmpl.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2gvruefip.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2rfakppyn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2msbyacfa.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2uxoaismi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vbvkezzl.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2rcoqufhk.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2uioixmuk.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2yhnibpdi.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2cjwoelsc.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2uhbihtzm.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2bpjpzpaq.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2momldwjx.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2rawxdczz.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2nrvflfcf.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2mtjutqnm.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2quyvvkxf.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2rtxsooqo.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2mscuolrh.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2vrtnzhen.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2ocbyfika.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2cypbokkr.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2nfnvsaoz.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2evpgmvgm.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2znhvgomk.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2fwuuhfbi.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2xcydmwck.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2twcfebtq.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2qsknsorl.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2ohmkmerr.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2kjvkjqbq.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2uahvkoif.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2rknuamat.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2viawruci.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2foemarhn.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2soxegeyc.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2gglyjcaa.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2xryvelwv.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2kevcssgt.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2wxjhmkde.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2hgejkudb.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2gnsjhpwa.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2lsvwqloy.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2cnsxofgf.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2dlfjjbmb.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2qnhuczlv.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ycsqsdun.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2kgzkahtp.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2yaurjvqc.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2esqmkzpw.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2qzryjacr.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2mvoajpju.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2saxdrcyd.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2mndltqzb.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2qlsvyoxc.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2chzaxeab.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2cwgjxknr.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2oupymlxh.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2kifxperl.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2rtvzloib.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2uswquduw.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2rqefuoki.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2xviroydc.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2netsxynk.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2doynwkyr.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2mwugytsa.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2vothgmer.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2qkunkkbu.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2ccgxwmxl.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2owkceupj.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2pvgphxna.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2rsvksjtd.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2dkxlzzni.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2qqwzqkfk.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2hvxfsrmq.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2espjhgew.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2fobrioyv.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2iidlptgs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jbkmlodu.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2clttxkgj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2klbxwfqb.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2pjopkkbg.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2syfxrptr.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2utecozrg.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2vchakijx.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2jtidtiza.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2txwmialw.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2wktzyhbg.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2cnygntrm.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2hiextbdi.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2mvasluwl.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2zdsomygo.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2nscudfnd.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2tncwtugw.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2gzibohae.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2bdmqzinr.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2halkxqoh.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2kkaosegp.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2wbqwbhus.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2hiqdujbd.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2jfksstxi.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2qrffphjj.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2rmfxhndq.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2yvadsdee.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2wftoctjh.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2ddmmurka.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2jietwzum.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2wuiysceg.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2fpxjstyl.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2jrvtedvj.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2pqnoskbc.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2esmhemqc.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2rczahhke.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2cpathyxm.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2xykezrob.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2kwvyqlqj.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2qthzussi.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2htswtnmb.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2ztvxmxap.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2doglyugh.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2premifrt.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2frpbyybj.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2abkelvmx.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2nrwyfplx.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2hechuxli.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2uzdqvucs.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2dtojdpis.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2gyqbcxla.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2darztfsj.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2rdgtnsoi.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2cnqpftpu.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2dbxrilfe.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2gurpyeop.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2phdwwbya.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2otgjbska.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2eynqoevc.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2zouxwopi.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2sloteopv.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2ymitgyfg.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2zfufcrtw.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2rrddjdma.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2keawlncy.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2abpgzims.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2cxtfyhzr.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2owrquntw.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hxybtxrj.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2ujvhbbvt.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2dwgihjta.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2jvilvxnn.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2hjwcqidn.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2sbwzqdri.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2follgmid.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2mpjxqewb.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2lrgkjhpw.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2thmcahvm.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2ndhopbja.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2korzqfbz.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2uillezmx.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2rsdlnjri.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2qgfimwis.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2rzzuykyq.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2fabstyir.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2qldiqeec.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2evunyjma.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2advtbeuz.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2geafhytd.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2aomryysl.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2btlypmns.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2gzwgtvoh.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2zfyfsarp.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2lbuqnkeb.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2eijpcidp.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2xicfyetn.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2eeqezoiz.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2tgqxylkg.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2gzawjesl.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2pvcopjze.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2wgbsosos.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2ktrukwtb.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2zbgvxvet.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2jffpizey.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2ymxmtrbq.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2fvjcypay.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2gzgbpzxf.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2cnrxgwic.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2npghewmz.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2sudrzztl.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2pfqddvvl.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2azcphroy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mzihdony.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2wwniaeoi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nnhquggs.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2jzmoytgv.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2tprnvoso.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2fteglzqt.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2fjkdshnn.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2znqkltiz.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2ihuhproe.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2edadnmpi.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2seatxbgg.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2nxotsyox.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2pddmqbdd.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2mnoxfwbc.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2qcpcohso.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2gkvefvjm.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2lcjentjb.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2vnbkjezg.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2tuwxczhb.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2ipblcpvr.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2pwcgrmwf.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2ftlvqjrd.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2wudyxydj.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2fjlgsvqp.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2drdqucwp.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2vauovviy.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2dvvfusck.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2fpiokxwg.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2slsxcqvt.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2cawvawel.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2baqsxhhm.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2rtjhcgwd.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2wbzxckak.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qadcqqpv.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zqtdkdud.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2ijqncuyf.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2hnzasjux.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2pklftyql.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2sxkvmfce.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2efteojds.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2moflfkpg.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2dqpbstsw.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2rsdcvdaf.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2xlmrwsen.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2isqwbjpg.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2yxiyzoao.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2xxbfczfc.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2hanobcbl.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2jiremkqb.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2ngemheux.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2orwyueso.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2dfvfszan.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2wlgbfbeu.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2aszqcdfq.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2lkklpyju.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2zlaubgut.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2noyjbtwm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2afxzvham.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2vtarfifn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2urmwifun.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2fkrzxiaa.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2zqhyjpua.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2gzjfmkdy.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2svwdqize.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2ygbpkvrc.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2neqvsauk.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2nlnzyqpu.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2mvlffsod.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2egjqxasw.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2qtycblrr.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2gseqwdqn.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2jkytcjbb.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2rodkgcxo.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2uumsbxca.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2gbprxxqj.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2tfkzhdnk.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2muelysvv.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2qfxladch.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2qdztfxhd.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2smfsrrfa.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2frjqcgbj.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2jsdnjdbu.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2jylfvull.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2gdekglvb.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2jogsmaej.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2ledhappm.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2afpewhjz.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2oprsexle.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2eoekhdda.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2xmbdwuqb.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2yhvsynop.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2wjztgnyd.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2fqnxakpl.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2iqihckqa.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2etlzodff.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2hfhpkflq.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2rnsrarxo.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2jyufynyh.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2mbmujrsc.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2qwvagkjh.html


<!-- 参考信息 -->