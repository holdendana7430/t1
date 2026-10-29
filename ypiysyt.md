代发 wailian999

TS:   resp.ok;  resp.status
来源：http://read.share.fehbvm.com/Article/details/gnelhpkhu.sHtML

Java: resp.statusCode()
来源：http://www.m.share.fehbvm.com/Article/details/gutdasjnj.sHtML

Go:   resp.StatusCode
来源：http://3g.hesvh.cn/Article/details/gqjlhzptt.sHtML

Ruby: resp.code.to_i
来源：http://m.share.fehbvm.com/Article/details/gcxlfwegm.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.hesvh.cn/Article/details/gnjipwkxo.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.hesvh.cn/Article/details/gyxtjpzvh.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.hesvh.cn/Article/details/gvbtgmsty.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.zdbjq.cn/Article/details/gouiuhsns.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.zdbjq.cn/Article/details/gixjicslj.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.zdbjq.cn/Article/details/glqecevji.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.fehbvm.com/Article/details/gapprhrvk.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.fehbvm.com/Article/details/ghvzyxxwm.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.fehbvm.com/Article/details/gtgtjbxgg.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.hesvh.cn/Article/details/gviykyvzi.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/glndjimnl.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.zdbjq.cn/Article/details/geovltrgx.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gbhktpvhh.sHtML

[M01] 读取命令行参数
来源：http://m.share.zdbjq.cn/Article/details/gzeilmeec.sHtML

Py:   sys.argv[1:]
来源：http://wap.hesvh.cn/Article/details/gfhhcgxly.sHtML

PHP:  $argv;  $argc;
来源：http://wap.hesvh.cn/Article/details/gsezbgchv.sHtML

JS:   process.argv.slice(2)
来源：http://3g.hesvh.cn/Article/details/gnvuejokc.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.fehbvm.com/Article/details/gwgkwkjml.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.fehbvm.com/Article/details/gxcznsqnt.sHtML

Go:   os.Args[1:]
来源：http://www.blog.zdbjq.cn/Article/details/gkltnejgx.sHtML

Ruby: ARGV
来源：http://mobile.fehbvm.com/Article/details/gsvxqilel.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.hesvh.cn/Article/details/gugcjgsnf.sHtML

[M02] 读取环境变量
来源：http://wap.hesvh.cn/Article/details/grgqezdyf.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.hesvh.cn/Article/details/gsmhowwtr.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.fehbvm.com/Article/details/gvboyulfs.sHtML

JS:   process.env.HOME
来源：http://www.blog.zdbjq.cn/Article/details/gdhuxarhu.sHtML

TS:   process.env.HOME
来源：http://read.share.hesvh.cn/Article/details/gxvdezlmg.sHtML

Java: System.getenv("HOME")
来源：http://m.share.hesvh.cn/Article/details/gezrwbmzq.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/gxfgrbhax.sHtML

Ruby: ENV["HOME"]
来源：http://wap.zdbjq.cn/Article/details/gcsqxtspb.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.fehbvm.com/Article/details/gzvjrmobg.sHtML

[M03] 执行外部命令
来源：http://blog.fehbvm.com/Article/details/goyvsfsdp.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.hesvh.cn/Article/details/gnjymaayl.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.hesvh.cn/Article/details/gvlqegtzb.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.zdbjq.cn/Article/details/gbxjhdouq.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.fehbvm.com/Article/details/gsamobunx.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.fehbvm.com/Article/details/gmifcrszd.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.zdbjq.cn/Article/details/guqwcpfei.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.hesvh.cn/Article/details/goycritql.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.hesvh.cn/Article/details/gmrxoixig.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.hesvh.cn/Article/details/gtjrkkrad.sHtML

Py:   os.getcwd()
来源：http://mobile.fehbvm.com/Article/details/ggffnczqn.sHtML

PHP:  getcwd();
来源：http://wap.fehbvm.com/Article/details/gpmoftitf.sHtML

JS:   process.cwd()
来源：http://blog.fehbvm.com/Article/details/gzlfuqutg.sHtML

TS:   process.cwd()
来源：http://3g.fehbvm.com/Article/details/gaaufabgo.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.fehbvm.com/Article/details/grbprkduz.sHtML

Go:   os.Getwd()
来源：http://read.share.zdbjq.cn/Article/details/gxmcrfirz.sHtML

Ruby: Dir.pwd
来源：http://wap.zdbjq.cn/Article/details/gvekpyckx.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.zdbjq.cn/Article/details/gamyyppuq.sHtML

[M05] 设置退出码
来源：http://www.blog.zdbjq.cn/Article/details/ggrkkstfr.sHtML

Py:   sys.exit(1)
来源：http://3g.fehbvm.com/Article/details/gwnctjzot.sHtML

PHP:  exit(1);
来源：http://read.share.fehbvm.com/Article/details/gsxxxoxdu.sHtML

JS:   process.exit(1)
来源：http://m.share.fehbvm.com/Article/details/glvwujodg.sHtML

TS:   process.exit(1)
来源：http://blog.fehbvm.com/Article/details/gsnclrfmh.sHtML

Java: System.exit(1)
来源：http://mobile.fehbvm.com/Article/details/guvmigiye.sHtML

Go:   os.Exit(1)
来源：http://blog.fehbvm.com/Article/details/gqqxubkkz.sHtML

Ruby: exit 1
来源：http://www.blog.hesvh.cn/Article/details/gzuxyvltn.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.hesvh.cn/Article/details/gmkiavblf.sHtML

[M06] 向标准错误输出
来源：http://wap.hesvh.cn/Article/details/gfymxlajo.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.fehbvm.com/Article/details/gxqcjikav.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.hesvh.cn/Article/details/gzmymdzdt.sHtML

JS:   console.error("err")
来源：http://3g.fehbvm.com/Article/details/ggclsunei.sHtML

TS:   console.error("err")
来源：http://m.share.fehbvm.com/Article/details/gzwbvuzyz.sHtML

Java: System.err.println("err")
来源：http://m.share.zdbjq.cn/Article/details/gmmldorem.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.fehbvm.com/Article/details/gwqrkjpzd.sHtML

Ruby: warn "err"
来源：http://wap.hesvh.cn/Article/details/gxcmnyisj.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.zdbjq.cn/Article/details/gbypfvqrs.sHtML

[M07] 判断是否为主入口
来源：http://read.share.hesvh.cn/Article/details/gwhuorwab.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.hesvh.cn/Article/details/gmivyzbkk.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.zdbjq.cn/Article/details/gqtwnbjnm.sHtML

JS:   require.main === module
来源：http://mobile.hesvh.cn/Article/details/gmldpbezj.sHtML

TS:   require.main === module
来源：http://baike.zdbjq.cn/Article/details/gkkhnstyh.sHtML

Java: public static void main(String[] args)
来源：http://wap.hesvh.cn/Article/details/gdvitmkgl.sHtML

Go:   func main()
来源：http://www.share.zdbjq.cn/Article/details/gycwdkanc.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.zdbjq.cn/Article/details/gywjirvsx.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.hesvh.cn/Article/details/gvgnzhvnk.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.zdbjq.cn/Article/details/gfiwwrlfa.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.zdbjq.cn/Article/details/gaomieaji.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.fehbvm.com/Article/details/gmkpfvmux.sHtML

JS:   process.platform;  process.version
来源：http://mobile.zdbjq.cn/Article/details/gkptpmota.sHtML

TS:   process.platform;  process.version
来源：http://mobile.zdbjq.cn/Article/details/gkceggeej.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.fehbvm.com/Article/details/ggaodgpmv.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.zdbjq.cn/Article/details/gcaqaccwo.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.fehbvm.com/Article/details/gubosltpa.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.fehbvm.com/Article/details/gxvjqamrb.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gvvvcmbxn.sHtML

N. 数据结构与算法
来源：http://m.share.fehbvm.com/Article/details/gvcocngnz.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gddpedlgg.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.hesvh.cn/Article/details/gfgpmkrxb.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gdhxitdxa.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.fehbvm.com/Article/details/gkvbaoifp.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.zdbjq.cn/Article/details/gwcecijgv.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.zdbjq.cn/Article/details/gfytzukqt.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gpsdkrcki.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.fehbvm.com/Article/details/ghtjolhur.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.fehbvm.com/Article/details/gihnrgiiv.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.fehbvm.com/Article/details/gcaronqtf.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.hesvh.cn/Article/details/grtskzwpq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.zdbjq.cn/Article/details/grcpfzczb.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.hesvh.cn/Article/details/gbdazdepn.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.zdbjq.cn/Article/details/gjxtlqqom.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.fehbvm.com/Article/details/gscztuqwx.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.hesvh.cn/Article/details/giuzibhre.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.zdbjq.cn/Article/details/gogariiak.sHtML

Ruby: arr.sort
来源：http://3g.hesvh.cn/Article/details/glilkdsaw.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.fehbvm.com/Article/details/gmiiadrot.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.zdbjq.cn/Article/details/gdwwbbaeb.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.hesvh.cn/Article/details/gfbnkvnup.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.fehbvm.com/Article/details/gswhkwrnp.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.hesvh.cn/Article/details/guzsiillg.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.zdbjq.cn/Article/details/gtjcphanw.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.hesvh.cn/Article/details/gbfomeodm.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.fehbvm.com/Article/details/gnizeiqnq.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.fehbvm.com/Article/details/gwhgjzeii.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.hesvh.cn/Article/details/grgfweqgz.sHtML

[N04] 斐波那契数列
来源：http://baike.hesvh.cn/Article/details/gekinppcq.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.hesvh.cn/Article/details/gqjxaeiql.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.hesvh.cn/Article/details/gjsgdnand.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.hesvh.cn/Article/details/gzvmsqhml.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/gajwmzjqc.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.fehbvm.com/Article/details/gtvsipmss.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.hesvh.cn/Article/details/grynbrnwq.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.fehbvm.com/Article/details/ggvqchivq.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.fehbvm.com/Article/details/gqvprfxlm.sHtML

[N05] 最大公约数
来源：http://www.share.zdbjq.cn/Article/details/gewbsrdtj.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.hesvh.cn/Article/details/gonjrssio.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.zdbjq.cn/Article/details/gdfikovik.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.fehbvm.com/Article/details/gmghumjcf.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.zdbjq.cn/Article/details/gacpmxndc.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.hesvh.cn/Article/details/gkksygpet.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.hesvh.cn/Article/details/gphpemwyw.sHtML

Ruby: a.gcd(b)
来源：http://m.share.zdbjq.cn/Article/details/gfrsmckzm.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.zdbjq.cn/Article/details/gqqsvsewj.sHtML

[N06] 判断回文字符串
来源：http://mobile.zdbjq.cn/Article/details/gkxyrcggz.sHtML

Py:   s == s[::-1]
来源：http://baike.hesvh.cn/Article/details/glztackdi.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.hesvh.cn/Article/details/ghxasqxgo.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/gufwpnnxa.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/gefpbuqaw.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.zdbjq.cn/Article/details/gbixuqysh.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.zdbjq.cn/Article/details/gasrnsfbb.sHtML

Ruby: s == s.reverse
来源：http://m.share.fehbvm.com/Article/details/gvufssryn.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.fehbvm.com/Article/details/gtvuljoyv.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.fehbvm.com/Article/details/glocjxqwy.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.fehbvm.com/Article/details/gmrqozmrj.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.fehbvm.com/Article/details/gfiffweqh.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.zdbjq.cn/Article/details/gyngkiovx.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.zdbjq.cn/Article/details/gdbupntzb.sHtML

Java: // 手写 HashMap
来源：http://blog.hesvh.cn/Article/details/gsigkwhsh.sHtML

Go:   // 手写 map[int]int
来源：http://3g.fehbvm.com/Article/details/gfsjudztg.sHtML

Ruby: // 手写 Hash
来源：http://wap.hesvh.cn/Article/details/gpflnxupx.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.fehbvm.com/Article/details/gqpzlvfyo.sHtML

[N08] 生成全排列
来源：http://baike.zdbjq.cn/Article/details/gvzynvvms.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.fehbvm.com/Article/details/gaxzurgdc.sHtML

PHP:  // 手写递归交换
来源：http://blog.zdbjq.cn/Article/details/gsdssmgld.sHtML

JS:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/ghdidwrvp.sHtML

TS:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gckrwtqlx.sHtML

Java: // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/ggbaeaakt.sHtML

Go:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gkqjaiikp.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.hesvh.cn/Article/details/gfgiqbxxn.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gpkdrzvik.sHtML

[N09] 栈与队列
来源：http://read.share.hesvh.cn/Article/details/gmxovxgev.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.hesvh.cn/Article/details/gpunwxfzk.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.fehbvm.com/Article/details/gowsqmdnd.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.fehbvm.com/Article/details/gbnhnouuu.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.zdbjq.cn/Article/details/gchfwttfv.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.zdbjq.cn/Article/details/gnvbicybr.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.zdbjq.cn/Article/details/guntmrdkk.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.hesvh.cn/Article/details/gbeltwdym.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.fehbvm.com/Article/details/grudojrdk.sHtML

[N10] 链表节点定义
来源：http://mobile.zdbjq.cn/Article/details/gqoncppah.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.hesvh.cn/Article/details/gkfncaafq.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.zdbjq.cn/Article/details/gfybsghxp.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.zdbjq.cn/Article/details/gjhgbggxx.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.zdbjq.cn/Article/details/glywydogo.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.fehbvm.com/Article/details/gjteajxut.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.zdbjq.cn/Article/details/gcgrziofu.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.zdbjq.cn/Article/details/gqiksmctw.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.hesvh.cn/Article/details/ghltkyvbg.sHtML

[N11] 二叉树中序遍历
来源：http://3g.fehbvm.com/Article/details/gfogpzgvc.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.zdbjq.cn/Article/details/gdjqrvpol.sHtML

PHP:  // 手写递归函数
来源：http://mobile.zdbjq.cn/Article/details/gjhqoygur.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.fehbvm.com/Article/details/gbcjhwvvy.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.hesvh.cn/Article/details/gjezqzhti.sHtML

Java: // 手写递归
来源：http://www.share.zdbjq.cn/Article/details/gvyndtize.sHtML

Go:   // 手写递归
来源：http://wap.zdbjq.cn/Article/details/gmzpkqeyc.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.zdbjq.cn/Article/details/grhwpcand.sHtML

C#:   // 手写递归
来源：http://www.share.fehbvm.com/Article/details/gichgxhko.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.zdbjq.cn/Article/details/gybtfgtun.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.zdbjq.cn/Article/details/gpablcxim.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.zdbjq.cn/Article/details/goszbtyur.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.zdbjq.cn/Article/details/gtvmrgusz.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.zdbjq.cn/Article/details/gzhocazob.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.fehbvm.com/Article/details/glvrgjqxz.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.zdbjq.cn/Article/details/gjivzlntt.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.zdbjq.cn/Article/details/gvuydxmfw.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.hesvh.cn/Article/details/gjhdewnox.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gygxtzyds.sHtML

O. 并发与异步
来源：http://baike.zdbjq.cn/Article/details/gsvavacxb.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gwqbufqia.sHtML

[O01] 启动一个线程
来源：http://mobile.zdbjq.cn/Article/details/gjdfijzsp.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.fehbvm.com/Article/details/ghqzyrbcb.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.zdbjq.cn/Article/details/gookbtwda.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.zdbjq.cn/Article/details/gnnazomlr.sHtML

TS:   // 同 JS
来源：http://www.share.fehbvm.com/Article/details/gqaqbhbsj.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.hesvh.cn/Article/details/gkoilfxwy.sHtML

Go:   go f()
来源：http://mobile.hesvh.cn/Article/details/gntzzdjdc.sHtML

Ruby: Thread.new { f }
来源：http://www.share.zdbjq.cn/Article/details/guctlanqj.sHtML

C#:   Task.Run(() => F());
来源：http://wap.zdbjq.cn/Article/details/gtffhjpsv.sHtML

[O02] 使用线程池
来源：http://www.share.zdbjq.cn/Article/details/gzaahtjey.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.fehbvm.com/Article/details/gpfbezxxx.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.fehbvm.com/Article/details/gqulldmbz.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.zdbjq.cn/Article/details/giqpeyydz.sHtML

TS:   // worker_threads 线程池
来源：http://3g.zdbjq.cn/Article/details/gfbebaztr.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.zdbjq.cn/Article/details/gcehzldcz.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.hesvh.cn/Article/details/glofucdjr.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.fehbvm.com/Article/details/gwboxnovd.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.zdbjq.cn/Article/details/glimtwwoa.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.fehbvm.com/Article/details/gllsccxxc.sHtML

Py:   with lock: shared += 1
来源：http://www.share.zdbjq.cn/Article/details/glwnsgyzy.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.zdbjq.cn/Article/details/gkjvmimrb.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.hesvh.cn/Article/details/ggvbzmqzk.sHtML

TS:   // 同 JS
来源：http://3g.fehbvm.com/Article/details/gcimmeqsx.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.fehbvm.com/Article/details/gxtffbjyw.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.fehbvm.com/Article/details/gfnndhhwp.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.fehbvm.com/Article/details/gcdnnlvnn.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.zdbjq.cn/Article/details/gwwiwmqnn.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.hesvh.cn/Article/details/gemcadvrq.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.zdbjq.cn/Article/details/ggvxqgnyu.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.zdbjq.cn/Article/details/gzvyjrtnc.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.hesvh.cn/Article/details/goeqvehfe.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.hesvh.cn/Article/details/gxoxnpjgz.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.hesvh.cn/Article/details/gkovmcbly.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.fehbvm.com/Article/details/goahqpzmm.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.hesvh.cn/Article/details/gmhymlzhr.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.fehbvm.com/Article/details/gkwscghwu.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.zdbjq.cn/Article/details/gtqmacvmv.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.zdbjq.cn/Article/details/gblllxczp.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.fehbvm.com/Article/details/grldzasmo.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.fehbvm.com/Article/details/geztciktb.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.hesvh.cn/Article/details/gdsuwiugo.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.hesvh.cn/Article/details/grnsfrkvn.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.hesvh.cn/Article/details/gzflwiubr.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.hesvh.cn/Article/details/gfpzfflzd.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.hesvh.cn/Article/details/ggzmpxcgn.sHtML

[O06] 使用进程池
来源：http://wap.hesvh.cn/Article/details/gwllzoyru.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.zdbjq.cn/Article/details/gzljzcwbx.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.hesvh.cn/Article/details/gxyydgdqv.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.zdbjq.cn/Article/details/gcaqkjbcp.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.fehbvm.com/Article/details/gunhlprlk.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.zdbjq.cn/Article/details/ghuzorevz.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.zdbjq.cn/Article/details/gkslmoowl.sHtML

Ruby: // fork 块
来源：http://3g.hesvh.cn/Article/details/gsaodquip.sHtML

C#:   Parallel.For
来源：http://www.m.share.fehbvm.com/Article/details/gflepjaer.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/grlflzbnf.sHtML

P. 常用工具函数
来源：http://baike.zdbjq.cn/Article/details/gpozczrfo.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gldecyjuy.sHtML

[P01] 生成 UUID
来源：http://mobile.fehbvm.com/Article/details/gybhmoutz.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.hesvh.cn/Article/details/grllyseam.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.fehbvm.com/Article/details/gofpocdqz.sHtML

JS:   crypto.randomUUID()
来源：http://baike.hesvh.cn/Article/details/goiqscniq.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.fehbvm.com/Article/details/gdflcsaxu.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.zdbjq.cn/Article/details/gafhiiomv.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.hesvh.cn/Article/details/gziphjfag.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.hesvh.cn/Article/details/gpmvegepm.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.fehbvm.com/Article/details/ghrzfdswf.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.zdbjq.cn/Article/details/gvbiwbzsg.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.hesvh.cn/Article/details/gjoqvaezf.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.hesvh.cn/Article/details/gesbbwfrs.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.fehbvm.com/Article/details/gpynguprn.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.hesvh.cn/Article/details/ggqsfwnld.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.zdbjq.cn/Article/details/gazlezybx.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.zdbjq.cn/Article/details/gudhyklgd.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.fehbvm.com/Article/details/gompeygqg.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.hesvh.cn/Article/details/gwtaiwvky.sHtML

[P03] 生成短随机字符串
来源：http://wap.hesvh.cn/Article/details/gmweqknyc.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.zdbjq.cn/Article/details/gufslovub.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.hesvh.cn/Article/details/ggffrpgnj.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.zdbjq.cn/Article/details/gkvcfenlm.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.fehbvm.com/Article/details/giwbbuckj.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.zdbjq.cn/Article/details/gtegcwpla.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.fehbvm.com/Article/details/gvsxtenjw.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.zdbjq.cn/Article/details/gpsrzmpzz.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.zdbjq.cn/Article/details/gonugpmoq.sHtML

[P04] 求长度
来源：http://blog.zdbjq.cn/Article/details/gyfnjlnyt.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.zdbjq.cn/Article/details/gbcdlgvtz.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/gwhhutssq.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.zdbjq.cn/Article/details/gnmjqexjv.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.zdbjq.cn/Article/details/gimdvzngc.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.zdbjq.cn/Article/details/gcupnxuzg.sHtML

Go:   len(arr);  len(m)
来源：http://blog.hesvh.cn/Article/details/gcspnmmtx.sHtML

Ruby: x.length;  x.size
来源：http://wap.hesvh.cn/Article/details/goglwxfei.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.hesvh.cn/Article/details/giuxdetbn.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.fehbvm.com/Article/details/gvfrpagai.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.zdbjq.cn/Article/details/geecrfxed.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.zdbjq.cn/Article/details/gbnnjmzpb.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.zdbjq.cn/Article/details/gocrxpfki.sHtML


<!-- 参考信息 -->