代发 wailian999

C#:   (int)resp.StatusCode
来源：http://mobile.fehbvm.com/Article/details/gzoyhjrrn.sHtML

[L08] 并发请求多个地址
来源：http://mobile.fehbvm.com/Article/details/gffpcgmfp.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.hesvh.cn/Article/details/gpjwkcwky.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.fehbvm.com/Article/details/gjmszfnaf.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.zdbjq.cn/Article/details/gaesdyjnp.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.hesvh.cn/Article/details/ggxkyufys.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.fehbvm.com/Article/details/gsshhprgs.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.fehbvm.com/Article/details/gffwizwtm.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.fehbvm.com/Article/details/ggwjpgtlg.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.zdbjq.cn/Article/details/gjfzetkut.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gjpvbrnte.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.fehbvm.com/Article/details/gzgbtceer.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gxuxhwbvn.sHtML

[M01] 读取命令行参数
来源：http://3g.zdbjq.cn/Article/details/ganftmjaq.sHtML

Py:   sys.argv[1:]
来源：http://3g.zdbjq.cn/Article/details/gtcpnbmzt.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.zdbjq.cn/Article/details/gjipzomun.sHtML

JS:   process.argv.slice(2)
来源：http://3g.hesvh.cn/Article/details/gmqvjtqkd.sHtML

TS:   process.argv.slice(2)
来源：http://baike.fehbvm.com/Article/details/garyeumxg.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.hesvh.cn/Article/details/gwumnrznb.sHtML

Go:   os.Args[1:]
来源：http://3g.zdbjq.cn/Article/details/gqotulukp.sHtML

Ruby: ARGV
来源：http://www.share.zdbjq.cn/Article/details/gqkawsxqg.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.fehbvm.com/Article/details/golrfokdd.sHtML

[M02] 读取环境变量
来源：http://m.share.hesvh.cn/Article/details/geloefoka.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.hesvh.cn/Article/details/gwajeagio.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.fehbvm.com/Article/details/gsgvqhmeq.sHtML

JS:   process.env.HOME
来源：http://3g.zdbjq.cn/Article/details/gehqzxcfy.sHtML

TS:   process.env.HOME
来源：http://mobile.hesvh.cn/Article/details/gadrwhvxf.sHtML

Java: System.getenv("HOME")
来源：http://m.share.hesvh.cn/Article/details/gzgpqjxza.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.zdbjq.cn/Article/details/gvkmysxup.sHtML

Ruby: ENV["HOME"]
来源：http://3g.fehbvm.com/Article/details/gswxcdmgh.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.hesvh.cn/Article/details/gxdnkbgwx.sHtML

[M03] 执行外部命令
来源：http://mobile.hesvh.cn/Article/details/gfjyxpced.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.hesvh.cn/Article/details/gwibakiub.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.fehbvm.com/Article/details/gicdgpivz.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.zdbjq.cn/Article/details/ghlfbcvui.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.zdbjq.cn/Article/details/gccyjskbl.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.zdbjq.cn/Article/details/gwlathelz.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.fehbvm.com/Article/details/gwdftovdk.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.zdbjq.cn/Article/details/gvkzxggrg.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.fehbvm.com/Article/details/gyuwgkdok.sHtML

[M04] 获取当前工作目录
来源：http://3g.fehbvm.com/Article/details/goheiuffw.sHtML

Py:   os.getcwd()
来源：http://read.share.zdbjq.cn/Article/details/gaktdatfo.sHtML

PHP:  getcwd();
来源：http://mobile.fehbvm.com/Article/details/goxpohwai.sHtML

JS:   process.cwd()
来源：http://www.share.fehbvm.com/Article/details/gwmkluhrb.sHtML

TS:   process.cwd()
来源：http://baike.zdbjq.cn/Article/details/gmbglsril.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.fehbvm.com/Article/details/gknezmswq.sHtML

Go:   os.Getwd()
来源：http://m.share.hesvh.cn/Article/details/gjrwgqcck.sHtML

Ruby: Dir.pwd
来源：http://blog.zdbjq.cn/Article/details/gzfhyacvv.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.hesvh.cn/Article/details/goelrvnhg.sHtML

[M05] 设置退出码
来源：http://3g.zdbjq.cn/Article/details/gdgrggkou.sHtML

Py:   sys.exit(1)
来源：http://baike.fehbvm.com/Article/details/gneoxtrwq.sHtML

PHP:  exit(1);
来源：http://www.m.share.zdbjq.cn/Article/details/gsnbywmvd.sHtML

JS:   process.exit(1)
来源：http://read.share.fehbvm.com/Article/details/gpffdwhmr.sHtML

TS:   process.exit(1)
来源：http://m.share.hesvh.cn/Article/details/geurzcydt.sHtML

Java: System.exit(1)
来源：http://baike.fehbvm.com/Article/details/gjisrmhzp.sHtML

Go:   os.Exit(1)
来源：http://m.share.fehbvm.com/Article/details/gojzgulhp.sHtML

Ruby: exit 1
来源：http://wap.fehbvm.com/Article/details/gyaoizdec.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.zdbjq.cn/Article/details/gkawbyeui.sHtML

[M06] 向标准错误输出
来源：http://m.share.hesvh.cn/Article/details/gwdnmpqpp.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.hesvh.cn/Article/details/gvctzdrnp.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.hesvh.cn/Article/details/gwietvehh.sHtML

JS:   console.error("err")
来源：http://wap.hesvh.cn/Article/details/glwwadhaz.sHtML

TS:   console.error("err")
来源：http://baike.hesvh.cn/Article/details/ggruglsnr.sHtML

Java: System.err.println("err")
来源：http://baike.hesvh.cn/Article/details/ggvqmvzfn.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.hesvh.cn/Article/details/gwlrtnige.sHtML

Ruby: warn "err"
来源：http://m.share.hesvh.cn/Article/details/gthapoqmr.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.zdbjq.cn/Article/details/gqfnzdrtq.sHtML

[M07] 判断是否为主入口
来源：http://www.share.fehbvm.com/Article/details/gbkksfjgt.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.zdbjq.cn/Article/details/gekcwqmpc.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.hesvh.cn/Article/details/gufwoutur.sHtML

JS:   require.main === module
来源：http://mobile.fehbvm.com/Article/details/gmnsyfvpa.sHtML

TS:   require.main === module
来源：http://3g.hesvh.cn/Article/details/gfsczihhs.sHtML

Java: public static void main(String[] args)
来源：http://www.share.zdbjq.cn/Article/details/glqmsoduu.sHtML

Go:   func main()
来源：http://wap.fehbvm.com/Article/details/gchuqyksp.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.zdbjq.cn/Article/details/gjzkbmiky.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.fehbvm.com/Article/details/gbkilnovv.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.zdbjq.cn/Article/details/glfmwazem.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.fehbvm.com/Article/details/guttdxyam.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.hesvh.cn/Article/details/gwhywadjj.sHtML

JS:   process.platform;  process.version
来源：http://mobile.fehbvm.com/Article/details/gnrcbhhjk.sHtML

TS:   process.platform;  process.version
来源：http://blog.hesvh.cn/Article/details/gemnqdyhr.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.zdbjq.cn/Article/details/gloluemym.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.hesvh.cn/Article/details/gzuazmzvh.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.hesvh.cn/Article/details/gaqkkfzgs.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.zdbjq.cn/Article/details/goxjtogqa.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gesdttzuj.sHtML

N. 数据结构与算法
来源：http://www.m.share.zdbjq.cn/Article/details/grimrnfgk.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gekrkcxss.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.fehbvm.com/Article/details/gonbszreo.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gcyzdwtwi.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.fehbvm.com/Article/details/guxvamqiy.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.hesvh.cn/Article/details/gekgjynop.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.zdbjq.cn/Article/details/glaivgyap.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gdlmnhmzy.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gazltsank.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.fehbvm.com/Article/details/ghxsgdlrm.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gnbpmunjs.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.zdbjq.cn/Article/details/gfsdnzuco.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.hesvh.cn/Article/details/gdldhqdai.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.fehbvm.com/Article/details/glgrnqmgn.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.fehbvm.com/Article/details/genjamxzz.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.hesvh.cn/Article/details/gquruxwpz.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.zdbjq.cn/Article/details/ggvphzwtn.sHtML

Go:   slices.Sort(arr)
来源：http://baike.zdbjq.cn/Article/details/gtnfrscil.sHtML

Ruby: arr.sort
来源：http://baike.zdbjq.cn/Article/details/gwveywohc.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.hesvh.cn/Article/details/guridbnfl.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.hesvh.cn/Article/details/gqcpakuwt.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.fehbvm.com/Article/details/gfwivjlzn.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.zdbjq.cn/Article/details/ggovidtzm.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.fehbvm.com/Article/details/gxgztckcu.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.hesvh.cn/Article/details/gmpvxrkkn.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.fehbvm.com/Article/details/gbpiwdxdu.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.zdbjq.cn/Article/details/gifpqaiwv.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.hesvh.cn/Article/details/gypfkaczw.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.hesvh.cn/Article/details/gexrvmepj.sHtML

[N04] 斐波那契数列
来源：http://m.share.hesvh.cn/Article/details/gswmhofxm.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.hesvh.cn/Article/details/gmvibfeth.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.hesvh.cn/Article/details/gzqysczeh.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.zdbjq.cn/Article/details/gtahpqcjp.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.fehbvm.com/Article/details/gwldzshlp.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.fehbvm.com/Article/details/gadjzthav.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.fehbvm.com/Article/details/grxvptedq.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.zdbjq.cn/Article/details/gnxtcqehs.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.zdbjq.cn/Article/details/gxcmikicl.sHtML

[N05] 最大公约数
来源：http://www.share.fehbvm.com/Article/details/gzmlgvxip.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.zdbjq.cn/Article/details/gmvztvaqq.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.zdbjq.cn/Article/details/gvhsfhuye.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.hesvh.cn/Article/details/gdpcnwkfe.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.hesvh.cn/Article/details/grgzwirej.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.zdbjq.cn/Article/details/guebbmsdu.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.fehbvm.com/Article/details/gqubhqczo.sHtML

Ruby: a.gcd(b)
来源：http://wap.hesvh.cn/Article/details/gbeyyqydi.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.hesvh.cn/Article/details/gglbxijod.sHtML

[N06] 判断回文字符串
来源：http://mobile.hesvh.cn/Article/details/gppgqwfvo.sHtML

Py:   s == s[::-1]
来源：http://baike.fehbvm.com/Article/details/gietkredu.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.hesvh.cn/Article/details/goatdrqns.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/gtmtaxfxs.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/gjnixpelx.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.fehbvm.com/Article/details/ggtvntwpj.sHtML

Go:   // 双指针从两端比较
来源：http://3g.fehbvm.com/Article/details/gswqugryy.sHtML

Ruby: s == s.reverse
来源：http://wap.zdbjq.cn/Article/details/gxnliszqm.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.zdbjq.cn/Article/details/ghgutmfpo.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.hesvh.cn/Article/details/gyfhjhmbk.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.zdbjq.cn/Article/details/gigkpuwsd.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.zdbjq.cn/Article/details/grnknlcgj.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.fehbvm.com/Article/details/gjavpojbu.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.hesvh.cn/Article/details/gpqyjhece.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.fehbvm.com/Article/details/gdhjamsjt.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.zdbjq.cn/Article/details/gdvibjnda.sHtML

Ruby: // 手写 Hash
来源：http://read.share.fehbvm.com/Article/details/guiwskpxa.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.hesvh.cn/Article/details/gdozarpmu.sHtML

[N08] 生成全排列
来源：http://baike.zdbjq.cn/Article/details/geqmyuafx.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.zdbjq.cn/Article/details/gnylepbkc.sHtML

PHP:  // 手写递归交换
来源：http://www.share.zdbjq.cn/Article/details/gtyktdtkp.sHtML

JS:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gsmbzburb.sHtML

TS:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gsrvhxfni.sHtML

Java: // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/ghnjhxgzl.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gesfnqkms.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.fehbvm.com/Article/details/ggcrjrtbe.sHtML

C#:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gfzvhxhyb.sHtML

[N09] 栈与队列
来源：http://m.share.fehbvm.com/Article/details/gehxnzhyh.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.fehbvm.com/Article/details/gbcunhfxx.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.fehbvm.com/Article/details/glhhojjct.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.zdbjq.cn/Article/details/gvkntwoao.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.zdbjq.cn/Article/details/gjskgmshg.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.hesvh.cn/Article/details/gjajipujj.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.zdbjq.cn/Article/details/gkrzbtcko.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.zdbjq.cn/Article/details/ggnwxyeqt.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.fehbvm.com/Article/details/gstyhnkmt.sHtML

[N10] 链表节点定义
来源：http://www.m.share.zdbjq.cn/Article/details/gehfpxezo.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.hesvh.cn/Article/details/geewhmefi.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.fehbvm.com/Article/details/guinkdshe.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.fehbvm.com/Article/details/gmvcllrqw.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.zdbjq.cn/Article/details/guzfdqfey.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.fehbvm.com/Article/details/gudicavpg.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.fehbvm.com/Article/details/gntacsopx.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.zdbjq.cn/Article/details/ghiwlwpdq.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.fehbvm.com/Article/details/gmmrmhdnf.sHtML

[N11] 二叉树中序遍历
来源：http://3g.hesvh.cn/Article/details/grbcwtclu.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.zdbjq.cn/Article/details/grzxtpeyd.sHtML

PHP:  // 手写递归函数
来源：http://read.share.zdbjq.cn/Article/details/gdesyttki.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.fehbvm.com/Article/details/gewvppriu.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.hesvh.cn/Article/details/gliqwuzsv.sHtML

Java: // 手写递归
来源：http://wap.hesvh.cn/Article/details/giknmelre.sHtML

Go:   // 手写递归
来源：http://m.share.fehbvm.com/Article/details/gdqxzxrbq.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.hesvh.cn/Article/details/gsgxnsiij.sHtML

C#:   // 手写递归
来源：http://www.share.fehbvm.com/Article/details/gbtqzistv.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.fehbvm.com/Article/details/gcwblziub.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.fehbvm.com/Article/details/gvjnbwmax.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.fehbvm.com/Article/details/gczvwcbgr.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.fehbvm.com/Article/details/gprjgkqxs.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.hesvh.cn/Article/details/guaaotjde.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.zdbjq.cn/Article/details/gdbjmhpoi.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.zdbjq.cn/Article/details/gqyxmioct.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.hesvh.cn/Article/details/guayfiijf.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.hesvh.cn/Article/details/gidwipxro.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gfacyqocx.sHtML

O. 并发与异步
来源：http://m.share.fehbvm.com/Article/details/glcuhapya.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gtxdkocrs.sHtML

[O01] 启动一个线程
来源：http://mobile.fehbvm.com/Article/details/ggkyinkss.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.hesvh.cn/Article/details/gdcvbcwcn.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.fehbvm.com/Article/details/gmiyjqzqs.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.zdbjq.cn/Article/details/gokczwbcw.sHtML

TS:   // 同 JS
来源：http://3g.hesvh.cn/Article/details/gggysbcvz.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.fehbvm.com/Article/details/gtpjhvdgu.sHtML

Go:   go f()
来源：http://www.share.zdbjq.cn/Article/details/gvuwmcioh.sHtML

Ruby: Thread.new { f }
来源：http://read.share.hesvh.cn/Article/details/gmfjvgkqw.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.hesvh.cn/Article/details/gjltmckbl.sHtML

[O02] 使用线程池
来源：http://www.share.fehbvm.com/Article/details/gvjgvvrbz.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.hesvh.cn/Article/details/gsydxwpbj.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.hesvh.cn/Article/details/grjejzazx.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.zdbjq.cn/Article/details/gfjgdhatw.sHtML

TS:   // worker_threads 线程池
来源：http://blog.zdbjq.cn/Article/details/gqcrgbxhh.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.zdbjq.cn/Article/details/gglmlgzzp.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.zdbjq.cn/Article/details/gmrzsdwwh.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.hesvh.cn/Article/details/gsztoxitv.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.hesvh.cn/Article/details/gxzuvtutp.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.fehbvm.com/Article/details/gxvtovoqv.sHtML

Py:   with lock: shared += 1
来源：http://read.share.zdbjq.cn/Article/details/ggopoecdq.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.hesvh.cn/Article/details/gqxdvpdpi.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.hesvh.cn/Article/details/gtqqsvmnt.sHtML

TS:   // 同 JS
来源：http://blog.hesvh.cn/Article/details/gmwjieeoz.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.hesvh.cn/Article/details/gajcbskca.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.hesvh.cn/Article/details/gvvkfxkyk.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.hesvh.cn/Article/details/gmseymbzv.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.fehbvm.com/Article/details/gawxwqnyf.sHtML

[O04] 定义异步函数并等待
来源：http://3g.hesvh.cn/Article/details/gglbkazer.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.hesvh.cn/Article/details/gcbaxfgrc.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.fehbvm.com/Article/details/gehioicko.sHtML

JS:   async function f() { await g(); }
来源：http://baike.fehbvm.com/Article/details/gvuxsenth.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.hesvh.cn/Article/details/gnrimdxnt.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.zdbjq.cn/Article/details/gjrtwinvn.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.fehbvm.com/Article/details/gqzooxpcf.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.hesvh.cn/Article/details/gydkfkrvj.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.zdbjq.cn/Article/details/gtvulnehl.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.hesvh.cn/Article/details/gnvmoqhdr.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.zdbjq.cn/Article/details/gdgbudume.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.fehbvm.com/Article/details/gsgwbymqe.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.hesvh.cn/Article/details/gwjyuoqve.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.zdbjq.cn/Article/details/gdnjieprb.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.zdbjq.cn/Article/details/gendbmggx.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.fehbvm.com/Article/details/gsjgtktmf.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.fehbvm.com/Article/details/gtqxdbnme.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.zdbjq.cn/Article/details/gdqkylefm.sHtML

[O06] 使用进程池
来源：http://www.blog.fehbvm.com/Article/details/gkoilebej.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.fehbvm.com/Article/details/gukewzpgr.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.fehbvm.com/Article/details/gjekzeyel.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.hesvh.cn/Article/details/gzmyddlbm.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.zdbjq.cn/Article/details/gjpyvbedd.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.hesvh.cn/Article/details/gvxlkwziz.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.zdbjq.cn/Article/details/ganpirgtb.sHtML

Ruby: // fork 块
来源：http://wap.zdbjq.cn/Article/details/gkupmyuuo.sHtML

C#:   Parallel.For
来源：http://blog.zdbjq.cn/Article/details/gpdmkpcuc.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gfkqsippi.sHtML

P. 常用工具函数
来源：http://blog.fehbvm.com/Article/details/gwfrddbop.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gyjgvyijp.sHtML

[P01] 生成 UUID
来源：http://baike.zdbjq.cn/Article/details/gggmmdybp.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.hesvh.cn/Article/details/gojkexuzh.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.hesvh.cn/Article/details/gdcnbvjbv.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.fehbvm.com/Article/details/gtfjebwsg.sHtML

TS:   crypto.randomUUID()
来源：http://baike.zdbjq.cn/Article/details/gxwfkpxib.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.fehbvm.com/Article/details/gglxkkzgm.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.fehbvm.com/Article/details/goyvhkhbu.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.zdbjq.cn/Article/details/gkslieyfi.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.fehbvm.com/Article/details/gqwbyiijn.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.zdbjq.cn/Article/details/gxikxzsxj.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.fehbvm.com/Article/details/ghbptmide.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.fehbvm.com/Article/details/ghiuolmku.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.hesvh.cn/Article/details/gnsmjimnw.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.hesvh.cn/Article/details/gwutvpegy.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.fehbvm.com/Article/details/gvtpxlymb.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.hesvh.cn/Article/details/gmmmqdccn.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.zdbjq.cn/Article/details/gswvdwoys.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.zdbjq.cn/Article/details/gvqgktffh.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.hesvh.cn/Article/details/gheqfoibj.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.zdbjq.cn/Article/details/gbmtwhzgv.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.fehbvm.com/Article/details/gjldpslbm.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.hesvh.cn/Article/details/gdcjxlyhd.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.hesvh.cn/Article/details/gismrxoen.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.fehbvm.com/Article/details/gywpsvmbb.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.hesvh.cn/Article/details/gszqskifb.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.zdbjq.cn/Article/details/glpvyoruc.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.hesvh.cn/Article/details/gsjnicnbe.sHtML

[P04] 求长度
来源：http://3g.fehbvm.com/Article/details/gqlfxyfbs.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.hesvh.cn/Article/details/groyumacl.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/gsvdfrnsu.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.hesvh.cn/Article/details/guforwomd.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.hesvh.cn/Article/details/gpunjncrt.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.fehbvm.com/Article/details/gjatmhhaa.sHtML

Go:   len(arr);  len(m)
来源：http://baike.fehbvm.com/Article/details/gonzweqgg.sHtML

Ruby: x.length;  x.size
来源：http://mobile.zdbjq.cn/Article/details/gjzrsogmp.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.hesvh.cn/Article/details/gwegjeikl.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.zdbjq.cn/Article/details/gpnwgyznn.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.hesvh.cn/Article/details/gzrvclegv.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.zdbjq.cn/Article/details/gzjfpqkuv.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.zdbjq.cn/Article/details/gkauuzqcw.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.fehbvm.com/Article/details/girgyaaba.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.hesvh.cn/Article/details/giqusstkm.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.zdbjq.cn/Article/details/gfzcksbwm.sHtML

Ruby: a == b
来源：http://m.share.fehbvm.com/Article/details/gpqxlbtvp.sHtML


<!-- 参考信息 -->