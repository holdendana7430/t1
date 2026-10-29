代发 wailian999

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.hesvh.cn/Article/details/gvjqjtmma.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fehbvm.com/Article/details/gvmfhytir.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.zdbjq.cn/Article/details/gxghqqiof.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.fehbvm.com/Article/details/gvhrpzhoi.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.hesvh.cn/Article/details/goxjczxbk.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.hesvh.cn/Article/details/grlwkbihw.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gdfdwcjru.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.zdbjq.cn/Article/details/gfohtfwqi.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gzivspnmy.sHtML

[M01] 读取命令行参数
来源：http://m.share.fehbvm.com/Article/details/gehqjlbuz.sHtML

Py:   sys.argv[1:]
来源：http://blog.zdbjq.cn/Article/details/grscvcvlj.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.zdbjq.cn/Article/details/gbfzemefi.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.zdbjq.cn/Article/details/gulkmvxwc.sHtML

TS:   process.argv.slice(2)
来源：http://blog.zdbjq.cn/Article/details/glhwxzkuc.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.fehbvm.com/Article/details/gberzvszx.sHtML

Go:   os.Args[1:]
来源：http://m.share.hesvh.cn/Article/details/gvsuthbxt.sHtML

Ruby: ARGV
来源：http://3g.zdbjq.cn/Article/details/gxyazubln.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.fehbvm.com/Article/details/gfzozpyhf.sHtML

[M02] 读取环境变量
来源：http://read.share.fehbvm.com/Article/details/gnosttssh.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.zdbjq.cn/Article/details/gyzltiean.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.hesvh.cn/Article/details/grnhdudee.sHtML

JS:   process.env.HOME
来源：http://www.m.share.hesvh.cn/Article/details/gwadxbfbg.sHtML

TS:   process.env.HOME
来源：http://wap.zdbjq.cn/Article/details/gesttdpuk.sHtML

Java: System.getenv("HOME")
来源：http://wap.fehbvm.com/Article/details/ggsbbqnfo.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.zdbjq.cn/Article/details/gsoxntmbf.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.fehbvm.com/Article/details/gokgqvddw.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.hesvh.cn/Article/details/ggmfaneam.sHtML

[M03] 执行外部命令
来源：http://blog.hesvh.cn/Article/details/gjmyhscco.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.hesvh.cn/Article/details/gjbgouekc.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.zdbjq.cn/Article/details/gwckkjblu.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.zdbjq.cn/Article/details/ghsfqspgu.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.zdbjq.cn/Article/details/gjmwzdqci.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.hesvh.cn/Article/details/gpipvqoqb.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.hesvh.cn/Article/details/gocgovevi.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.hesvh.cn/Article/details/ghvdspojf.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.fehbvm.com/Article/details/gclkfgwea.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.hesvh.cn/Article/details/gzjjfpjxd.sHtML

Py:   os.getcwd()
来源：http://blog.fehbvm.com/Article/details/gtupnwvky.sHtML

PHP:  getcwd();
来源：http://wap.hesvh.cn/Article/details/gpcfzjckd.sHtML

JS:   process.cwd()
来源：http://www.m.share.fehbvm.com/Article/details/gdgsszuii.sHtML

TS:   process.cwd()
来源：http://www.m.share.zdbjq.cn/Article/details/glbhupnbr.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.zdbjq.cn/Article/details/gmpstpgeg.sHtML

Go:   os.Getwd()
来源：http://www.m.share.zdbjq.cn/Article/details/gzprfwugh.sHtML

Ruby: Dir.pwd
来源：http://baike.hesvh.cn/Article/details/gplhwsblw.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.zdbjq.cn/Article/details/gcaouhxkd.sHtML

[M05] 设置退出码
来源：http://read.share.fehbvm.com/Article/details/gwbocglla.sHtML

Py:   sys.exit(1)
来源：http://www.share.fehbvm.com/Article/details/gwivplmkz.sHtML

PHP:  exit(1);
来源：http://blog.fehbvm.com/Article/details/goaphnxbl.sHtML

JS:   process.exit(1)
来源：http://wap.zdbjq.cn/Article/details/ggnnmsbzu.sHtML

TS:   process.exit(1)
来源：http://3g.zdbjq.cn/Article/details/gdwartayg.sHtML

Java: System.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gfofyzsjt.sHtML

Go:   os.Exit(1)
来源：http://wap.fehbvm.com/Article/details/gqavtymdr.sHtML

Ruby: exit 1
来源：http://www.share.hesvh.cn/Article/details/gmuaedvyq.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.hesvh.cn/Article/details/gqiigydzm.sHtML

[M06] 向标准错误输出
来源：http://blog.zdbjq.cn/Article/details/gtfnvvtcu.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.zdbjq.cn/Article/details/gxpmqzetd.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.fehbvm.com/Article/details/gtzgnzbkw.sHtML

JS:   console.error("err")
来源：http://www.share.zdbjq.cn/Article/details/gbhqixbyt.sHtML

TS:   console.error("err")
来源：http://www.m.share.fehbvm.com/Article/details/gffcchfwj.sHtML

Java: System.err.println("err")
来源：http://baike.hesvh.cn/Article/details/gifvnoaol.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.hesvh.cn/Article/details/gblupxsoi.sHtML

Ruby: warn "err"
来源：http://read.share.fehbvm.com/Article/details/gyughbuzl.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.hesvh.cn/Article/details/gxpuwyxed.sHtML

[M07] 判断是否为主入口
来源：http://mobile.fehbvm.com/Article/details/gupgkfshy.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.fehbvm.com/Article/details/gbjuiuxwi.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.fehbvm.com/Article/details/gjncdkljn.sHtML

JS:   require.main === module
来源：http://baike.fehbvm.com/Article/details/grouxdpby.sHtML

TS:   require.main === module
来源：http://www.blog.zdbjq.cn/Article/details/gazbkegfw.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.zdbjq.cn/Article/details/gfbwlvdrz.sHtML

Go:   func main()
来源：http://m.share.hesvh.cn/Article/details/gmyfglvcs.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.fehbvm.com/Article/details/gzejkwuoo.sHtML

C#:   static void Main(string[] args)
来源：http://3g.zdbjq.cn/Article/details/gjfjsbvww.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.zdbjq.cn/Article/details/gvpuncjzi.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.fehbvm.com/Article/details/gmppodhhh.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.hesvh.cn/Article/details/gwmlkmglz.sHtML

JS:   process.platform;  process.version
来源：http://m.share.fehbvm.com/Article/details/gvlmprglm.sHtML

TS:   process.platform;  process.version
来源：http://wap.fehbvm.com/Article/details/giocjtbrd.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.hesvh.cn/Article/details/grwmtcrft.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.fehbvm.com/Article/details/gpicdjyjg.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.fehbvm.com/Article/details/gtzafcudj.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.hesvh.cn/Article/details/gwqxsyrns.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/glzwklbds.sHtML

N. 数据结构与算法
来源：http://m.share.zdbjq.cn/Article/details/gkrioqjis.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gkmojydsg.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.fehbvm.com/Article/details/gytijrbpo.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/grsvegbpb.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.hesvh.cn/Article/details/gtepbhmoe.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.hesvh.cn/Article/details/ghbecaaap.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.hesvh.cn/Article/details/gjvnfhzat.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gqadjvrxw.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gdifdvrru.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.zdbjq.cn/Article/details/gbujghsux.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gmgvqmxvm.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.hesvh.cn/Article/details/gwhsfcwnr.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.hesvh.cn/Article/details/gaoftfabo.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.hesvh.cn/Article/details/govgkxpat.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.zdbjq.cn/Article/details/gtoxjfmzk.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.fehbvm.com/Article/details/gdjuzidjo.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.zdbjq.cn/Article/details/gcydsbfpj.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.fehbvm.com/Article/details/gsfzwueug.sHtML

Ruby: arr.sort
来源：http://3g.zdbjq.cn/Article/details/gobhkgans.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.hesvh.cn/Article/details/gcmfqnqab.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.hesvh.cn/Article/details/gjyvwordl.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.hesvh.cn/Article/details/gskwetnzt.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.zdbjq.cn/Article/details/gkcoelwes.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.zdbjq.cn/Article/details/gstjybqgq.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.fehbvm.com/Article/details/ggprqcoqr.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.hesvh.cn/Article/details/gxowxdavd.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.hesvh.cn/Article/details/gnkvxdqwc.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.hesvh.cn/Article/details/giuanxdzu.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.hesvh.cn/Article/details/gacxtzebh.sHtML

[N04] 斐波那契数列
来源：http://wap.zdbjq.cn/Article/details/gzwpynbhr.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.zdbjq.cn/Article/details/gtomyzlex.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.fehbvm.com/Article/details/gueenoiiq.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/gvlmlrgku.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.hesvh.cn/Article/details/grioxzsjk.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.fehbvm.com/Article/details/gdxalwreo.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.hesvh.cn/Article/details/gvoelvxwd.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.fehbvm.com/Article/details/ghrxpxrvj.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/gmeefnmae.sHtML

[N05] 最大公约数
来源：http://www.share.hesvh.cn/Article/details/gquatesvt.sHtML

Py:   math.gcd(a, b)
来源：http://wap.fehbvm.com/Article/details/gedgmicwc.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.hesvh.cn/Article/details/gqwsayase.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.hesvh.cn/Article/details/gwwhvopar.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.fehbvm.com/Article/details/guqisamgr.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.zdbjq.cn/Article/details/gjulylpqq.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.zdbjq.cn/Article/details/givcgfzwy.sHtML

Ruby: a.gcd(b)
来源：http://baike.hesvh.cn/Article/details/gvpkmufuo.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.fehbvm.com/Article/details/gqpmbwxvw.sHtML

[N06] 判断回文字符串
来源：http://mobile.hesvh.cn/Article/details/glrzfzsbi.sHtML

Py:   s == s[::-1]
来源：http://m.share.fehbvm.com/Article/details/gjstfvsjr.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.zdbjq.cn/Article/details/gfylqtjul.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/getwkzjii.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/ginmwdlfy.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.fehbvm.com/Article/details/gtggxtgik.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.fehbvm.com/Article/details/gsvlhymfu.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.zdbjq.cn/Article/details/gsuxusnxi.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.hesvh.cn/Article/details/gcjpyhabk.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.zdbjq.cn/Article/details/gtctainag.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.fehbvm.com/Article/details/ggnfsfwvy.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.fehbvm.com/Article/details/gmkypitkd.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.hesvh.cn/Article/details/gttlzpkhb.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.fehbvm.com/Article/details/glrlkpyje.sHtML

Java: // 手写 HashMap
来源：http://wap.fehbvm.com/Article/details/gkljqwkxq.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.fehbvm.com/Article/details/gmxezvjqw.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.fehbvm.com/Article/details/gvqhglckm.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.zdbjq.cn/Article/details/gjrmwtyjw.sHtML

[N08] 生成全排列
来源：http://3g.hesvh.cn/Article/details/guaqqdzsv.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.fehbvm.com/Article/details/gqlcxcuse.sHtML

PHP:  // 手写递归交换
来源：http://read.share.zdbjq.cn/Article/details/goinvipjj.sHtML

JS:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gfkgiendm.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gbdhamhwv.sHtML

Java: // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gunkvikjp.sHtML

Go:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gamnrpkhq.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.fehbvm.com/Article/details/gntcdwetw.sHtML

C#:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gkpfrgogv.sHtML

[N09] 栈与队列
来源：http://mobile.hesvh.cn/Article/details/gqjglpakc.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.zdbjq.cn/Article/details/gknmyfjgs.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.fehbvm.com/Article/details/gqjarimdw.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.zdbjq.cn/Article/details/gfevuvdck.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.hesvh.cn/Article/details/geaquoqth.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.zdbjq.cn/Article/details/gjankcyrf.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.fehbvm.com/Article/details/gxcbkebip.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.hesvh.cn/Article/details/gwohmdwpg.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.fehbvm.com/Article/details/gcjckffbp.sHtML

[N10] 链表节点定义
来源：http://m.share.zdbjq.cn/Article/details/gnxpqclzm.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.fehbvm.com/Article/details/gudgledbr.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.zdbjq.cn/Article/details/gppnqfbfn.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.zdbjq.cn/Article/details/gbcikbxnc.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.zdbjq.cn/Article/details/gzfwfcvmz.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.hesvh.cn/Article/details/gquifyzwk.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.fehbvm.com/Article/details/gqmlodlud.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.fehbvm.com/Article/details/gcisbyybk.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.hesvh.cn/Article/details/gbcrwkgvw.sHtML

[N11] 二叉树中序遍历
来源：http://blog.hesvh.cn/Article/details/gzycvluie.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.fehbvm.com/Article/details/gasvrvklb.sHtML

PHP:  // 手写递归函数
来源：http://read.share.zdbjq.cn/Article/details/gayqrgxis.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.zdbjq.cn/Article/details/gdbdqyaoy.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.hesvh.cn/Article/details/gxmmnvita.sHtML

Java: // 手写递归
来源：http://www.blog.fehbvm.com/Article/details/gifguawps.sHtML

Go:   // 手写递归
来源：http://mobile.fehbvm.com/Article/details/gsatqaupg.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.fehbvm.com/Article/details/gkpljhkzl.sHtML

C#:   // 手写递归
来源：http://m.share.hesvh.cn/Article/details/gembctkgu.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.hesvh.cn/Article/details/gzsgyrdyc.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.fehbvm.com/Article/details/gynqzfmgx.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.hesvh.cn/Article/details/gtijhlukq.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.fehbvm.com/Article/details/gbafqwdin.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.zdbjq.cn/Article/details/getbejaky.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.fehbvm.com/Article/details/grsupazxt.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.zdbjq.cn/Article/details/gmhybxsiq.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.hesvh.cn/Article/details/gqffrwnky.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.zdbjq.cn/Article/details/gjbgdvizm.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/ggvmcbule.sHtML

O. 并发与异步
来源：http://wap.hesvh.cn/Article/details/gwfdwswkt.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gggdgbmld.sHtML

[O01] 启动一个线程
来源：http://read.share.zdbjq.cn/Article/details/gmhpzmdti.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.zdbjq.cn/Article/details/geipfawls.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.hesvh.cn/Article/details/gpaxmtalu.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.hesvh.cn/Article/details/gzmivrphh.sHtML

TS:   // 同 JS
来源：http://mobile.fehbvm.com/Article/details/gxkvgmsjm.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.fehbvm.com/Article/details/gxnnaazwf.sHtML

Go:   go f()
来源：http://baike.hesvh.cn/Article/details/gbusgsubc.sHtML

Ruby: Thread.new { f }
来源：http://blog.fehbvm.com/Article/details/gzaatouhd.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.fehbvm.com/Article/details/ghtcqvfjv.sHtML

[O02] 使用线程池
来源：http://read.share.hesvh.cn/Article/details/gpjskhwva.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.hesvh.cn/Article/details/gpjagnxkg.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.hesvh.cn/Article/details/gudugldac.sHtML

JS:   // worker_threads 线程池
来源：http://baike.zdbjq.cn/Article/details/gvvjfiits.sHtML

TS:   // worker_threads 线程池
来源：http://3g.zdbjq.cn/Article/details/gclehphwh.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.fehbvm.com/Article/details/gkodlrbml.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.fehbvm.com/Article/details/gncdyeggb.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.fehbvm.com/Article/details/gmizyxzjq.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.hesvh.cn/Article/details/gvwzonnjx.sHtML

[O03] 加锁保护共享数据
来源：http://wap.fehbvm.com/Article/details/gtjgjkhfb.sHtML

Py:   with lock: shared += 1
来源：http://3g.zdbjq.cn/Article/details/gtycymeih.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.zdbjq.cn/Article/details/ggtwecxng.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.zdbjq.cn/Article/details/gpiijnusi.sHtML

TS:   // 同 JS
来源：http://3g.zdbjq.cn/Article/details/grvrfgaex.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.hesvh.cn/Article/details/glsycbhxw.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.hesvh.cn/Article/details/gvywlgves.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.fehbvm.com/Article/details/gdqaqavph.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.hesvh.cn/Article/details/gcpromqph.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.zdbjq.cn/Article/details/gsdzecofe.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.hesvh.cn/Article/details/gdyxfcpiw.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.zdbjq.cn/Article/details/gydwcxhvo.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.zdbjq.cn/Article/details/gvzkjelcs.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.zdbjq.cn/Article/details/gqxaswnjn.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.fehbvm.com/Article/details/gnpyxvzmy.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.zdbjq.cn/Article/details/gzwixulxs.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.fehbvm.com/Article/details/gxefqzugm.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.hesvh.cn/Article/details/gbkyuuthw.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.hesvh.cn/Article/details/geazabdxw.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.hesvh.cn/Article/details/ghnywbkxp.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.zdbjq.cn/Article/details/gdoqrbakl.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.zdbjq.cn/Article/details/giittobya.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.zdbjq.cn/Article/details/gzxahmeqw.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.fehbvm.com/Article/details/gidqhajjn.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.hesvh.cn/Article/details/gzotdkqbz.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.zdbjq.cn/Article/details/gpiajrjee.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.fehbvm.com/Article/details/gatxesfcy.sHtML

[O06] 使用进程池
来源：http://www.m.share.fehbvm.com/Article/details/gbixvxqsy.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.fehbvm.com/Article/details/gewlbhfaz.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.zdbjq.cn/Article/details/gfmfraypw.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.hesvh.cn/Article/details/grphfufnd.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.zdbjq.cn/Article/details/gumzcuygv.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.fehbvm.com/Article/details/gcglsvjyi.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.hesvh.cn/Article/details/gbhuqjvao.sHtML

Ruby: // fork 块
来源：http://read.share.hesvh.cn/Article/details/gwvvdvasl.sHtML

C#:   Parallel.For
来源：http://wap.hesvh.cn/Article/details/ghgxkssfy.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gkkkxwhwp.sHtML

P. 常用工具函数
来源：http://www.share.fehbvm.com/Article/details/gvqidduxj.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gkvzfxycb.sHtML

[P01] 生成 UUID
来源：http://wap.hesvh.cn/Article/details/ghvpyggwz.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.fehbvm.com/Article/details/gqbfucizt.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.zdbjq.cn/Article/details/ghgxixisx.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.fehbvm.com/Article/details/glnsvhdsg.sHtML

TS:   crypto.randomUUID()
来源：http://baike.hesvh.cn/Article/details/ghzvvikdc.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.fehbvm.com/Article/details/ghtzvxrxo.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.zdbjq.cn/Article/details/gdzwlenft.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.hesvh.cn/Article/details/gmgniwfij.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.fehbvm.com/Article/details/ghsrzyzgf.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.hesvh.cn/Article/details/gkolkgkdj.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.hesvh.cn/Article/details/gbeswmrdr.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.zdbjq.cn/Article/details/guhtytets.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.hesvh.cn/Article/details/gwcexyoea.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.fehbvm.com/Article/details/gwwwpasfe.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.fehbvm.com/Article/details/ggywqndzr.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.zdbjq.cn/Article/details/gpkkcvnjx.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.fehbvm.com/Article/details/gpraunixv.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.hesvh.cn/Article/details/ghxfipkuu.sHtML

[P03] 生成短随机字符串
来源：http://www.share.fehbvm.com/Article/details/gcsgbccoz.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.hesvh.cn/Article/details/goilunvau.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.hesvh.cn/Article/details/glueqrfpo.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.hesvh.cn/Article/details/gnumlkqlh.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.hesvh.cn/Article/details/gjggufmmd.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.zdbjq.cn/Article/details/ggmcfubpz.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.hesvh.cn/Article/details/ghhxbmdht.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.hesvh.cn/Article/details/gieyndtig.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.hesvh.cn/Article/details/gaqlfvzer.sHtML

[P04] 求长度
来源：http://www.m.share.hesvh.cn/Article/details/gervrwfoh.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.zdbjq.cn/Article/details/gdbozloqm.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/gdbtalkhy.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.zdbjq.cn/Article/details/gzzsufbdf.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.zdbjq.cn/Article/details/gfuwprmtt.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.zdbjq.cn/Article/details/gontibsep.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.hesvh.cn/Article/details/giszfszpy.sHtML

Ruby: x.length;  x.size
来源：http://www.share.hesvh.cn/Article/details/gwrugfalz.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.fehbvm.com/Article/details/gefpgnkgo.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.fehbvm.com/Article/details/gihafcijw.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.zdbjq.cn/Article/details/gnpuoxadq.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.hesvh.cn/Article/details/gcdxuddiq.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.fehbvm.com/Article/details/gsyzdgcfh.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.fehbvm.com/Article/details/gufxsvilj.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.hesvh.cn/Article/details/gdbbgpcxu.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.fehbvm.com/Article/details/gqrgpfanx.sHtML

Ruby: a == b
来源：http://blog.fehbvm.com/Article/details/gygijdige.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.hesvh.cn/Article/details/gvemegvet.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.zdbjq.cn/Article/details/gppkgfgoo.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.hesvh.cn/Article/details/gqwpuaceh.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.hesvh.cn/Article/details/gzrkgvoug.sHtML


<!-- 参考信息 -->