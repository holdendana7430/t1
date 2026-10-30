代发 wailian999

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.hesvh.cn/Article/details/ghsrvfmdy.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.zdbjq.cn/Article/details/gdacnivyw.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gcgmutpuo.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.zdbjq.cn/Article/details/guayhsodt.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gegumjlce.sHtML

[M01] 读取命令行参数
来源：http://read.share.hesvh.cn/Article/details/gsypbelqz.sHtML

Py:   sys.argv[1:]
来源：http://blog.hesvh.cn/Article/details/gfzduqlww.sHtML

PHP:  $argv;  $argc;
来源：http://baike.zdbjq.cn/Article/details/gceucpdca.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.fehbvm.com/Article/details/gkxkdphhy.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.zdbjq.cn/Article/details/gbkovmlnv.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.zdbjq.cn/Article/details/gsamsverj.sHtML

Go:   os.Args[1:]
来源：http://baike.zdbjq.cn/Article/details/gujfyuwew.sHtML

Ruby: ARGV
来源：http://wap.fehbvm.com/Article/details/gwhaltsor.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.fehbvm.com/Article/details/guqoisxfo.sHtML

[M02] 读取环境变量
来源：http://blog.zdbjq.cn/Article/details/gnndfulag.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.hesvh.cn/Article/details/gtqpdlrwm.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.hesvh.cn/Article/details/gxeumrvvn.sHtML

JS:   process.env.HOME
来源：http://www.share.hesvh.cn/Article/details/gxjgxisiu.sHtML

TS:   process.env.HOME
来源：http://m.share.zdbjq.cn/Article/details/gfepjwfoj.sHtML

Java: System.getenv("HOME")
来源：http://www.share.hesvh.cn/Article/details/gbwaupwnj.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.hesvh.cn/Article/details/gocelyajg.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.hesvh.cn/Article/details/ghnkokunw.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.zdbjq.cn/Article/details/gdcibcquw.sHtML

[M03] 执行外部命令
来源：http://www.share.fehbvm.com/Article/details/gubpgcvcz.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.hesvh.cn/Article/details/gfjgsokuz.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.fehbvm.com/Article/details/gztkfocjm.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.fehbvm.com/Article/details/grvcplmpa.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.hesvh.cn/Article/details/gdzmmosrl.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.fehbvm.com/Article/details/gszvysyor.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.zdbjq.cn/Article/details/gxxwvwzee.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.hesvh.cn/Article/details/gewognqew.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.fehbvm.com/Article/details/gzjoewubb.sHtML

[M04] 获取当前工作目录
来源：http://wap.zdbjq.cn/Article/details/gmujxnoqr.sHtML

Py:   os.getcwd()
来源：http://read.share.zdbjq.cn/Article/details/gfsssfyow.sHtML

PHP:  getcwd();
来源：http://read.share.hesvh.cn/Article/details/gmopizfxt.sHtML

JS:   process.cwd()
来源：http://blog.fehbvm.com/Article/details/gawhtacrs.sHtML

TS:   process.cwd()
来源：http://www.blog.fehbvm.com/Article/details/griglkqxr.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.hesvh.cn/Article/details/gcpaiewec.sHtML

Go:   os.Getwd()
来源：http://www.share.fehbvm.com/Article/details/gzeossrqz.sHtML

Ruby: Dir.pwd
来源：http://baike.zdbjq.cn/Article/details/gwvmwvncl.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.hesvh.cn/Article/details/gcqgjbxrq.sHtML

[M05] 设置退出码
来源：http://wap.hesvh.cn/Article/details/gulfmfnlc.sHtML

Py:   sys.exit(1)
来源：http://mobile.hesvh.cn/Article/details/gublroefr.sHtML

PHP:  exit(1);
来源：http://www.blog.hesvh.cn/Article/details/gvbjtfhrt.sHtML

JS:   process.exit(1)
来源：http://m.share.hesvh.cn/Article/details/gvjorbqsx.sHtML

TS:   process.exit(1)
来源：http://mobile.hesvh.cn/Article/details/gvdpikalc.sHtML

Java: System.exit(1)
来源：http://blog.zdbjq.cn/Article/details/gpihrkdyo.sHtML

Go:   os.Exit(1)
来源：http://wap.hesvh.cn/Article/details/georhqicz.sHtML

Ruby: exit 1
来源：http://www.share.hesvh.cn/Article/details/gysxpdtae.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.hesvh.cn/Article/details/gjkmjwepm.sHtML

[M06] 向标准错误输出
来源：http://www.blog.zdbjq.cn/Article/details/gsakugxhr.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.fehbvm.com/Article/details/gwgeffrnt.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.hesvh.cn/Article/details/gofgarfyo.sHtML

JS:   console.error("err")
来源：http://blog.zdbjq.cn/Article/details/gjwrqrjto.sHtML

TS:   console.error("err")
来源：http://baike.hesvh.cn/Article/details/getqkfcvw.sHtML

Java: System.err.println("err")
来源：http://baike.zdbjq.cn/Article/details/glkgvfgjs.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.fehbvm.com/Article/details/gufqwuadi.sHtML

Ruby: warn "err"
来源：http://mobile.hesvh.cn/Article/details/guhwmmwgi.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.fehbvm.com/Article/details/gqngusmoy.sHtML

[M07] 判断是否为主入口
来源：http://blog.zdbjq.cn/Article/details/gvmriqsdz.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.hesvh.cn/Article/details/gtdztavih.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.zdbjq.cn/Article/details/grklmhrwu.sHtML

JS:   require.main === module
来源：http://www.share.zdbjq.cn/Article/details/gycymfhfy.sHtML

TS:   require.main === module
来源：http://3g.zdbjq.cn/Article/details/guamugmue.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.zdbjq.cn/Article/details/gjbiueodf.sHtML

Go:   func main()
来源：http://www.m.share.hesvh.cn/Article/details/glqemjjse.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.zdbjq.cn/Article/details/gxwzzgaih.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.hesvh.cn/Article/details/gvscjuhos.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.hesvh.cn/Article/details/gcbibvipq.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.hesvh.cn/Article/details/gwyikzdns.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.zdbjq.cn/Article/details/gavsysibx.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.hesvh.cn/Article/details/gduwijgrj.sHtML

TS:   process.platform;  process.version
来源：http://wap.hesvh.cn/Article/details/gzubachqm.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.zdbjq.cn/Article/details/gzppzanvh.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.zdbjq.cn/Article/details/gvzpltzny.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.fehbvm.com/Article/details/glrnylkrn.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.zdbjq.cn/Article/details/gexpvenpn.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gvwxkcvpj.sHtML

N. 数据结构与算法
来源：http://wap.zdbjq.cn/Article/details/gpxhkrnrl.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/giuqewxpg.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.hesvh.cn/Article/details/gcutlrpdc.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gtfsmzlkt.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.zdbjq.cn/Article/details/grraqnoqx.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.fehbvm.com/Article/details/gusxaehkw.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.zdbjq.cn/Article/details/gyuikbwaz.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.fehbvm.com/Article/details/gpyfnyjsn.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.fehbvm.com/Article/details/gfmpbbzpt.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.zdbjq.cn/Article/details/gdrsjkscp.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gpbcrrvqn.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.zdbjq.cn/Article/details/gbplfjjms.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.zdbjq.cn/Article/details/ghsijukuu.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.fehbvm.com/Article/details/gsxwsoivw.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.fehbvm.com/Article/details/gvmusvhca.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.fehbvm.com/Article/details/guvzexngu.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.hesvh.cn/Article/details/gutrtpoal.sHtML

Go:   slices.Sort(arr)
来源：http://baike.hesvh.cn/Article/details/girxkjdzz.sHtML

Ruby: arr.sort
来源：http://read.share.fehbvm.com/Article/details/gcbimxwqp.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.zdbjq.cn/Article/details/gartbabog.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.zdbjq.cn/Article/details/gbcrdppgm.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.fehbvm.com/Article/details/grapjaixd.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.zdbjq.cn/Article/details/gnlwdrfix.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.zdbjq.cn/Article/details/grcplyufb.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.hesvh.cn/Article/details/gxhfvpyzs.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.fehbvm.com/Article/details/gxrkjnhdu.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.hesvh.cn/Article/details/gznuhqtoz.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.fehbvm.com/Article/details/gyyqvilhx.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.zdbjq.cn/Article/details/gzgflkrxz.sHtML

[N04] 斐波那契数列
来源：http://baike.zdbjq.cn/Article/details/gkdidwcil.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.hesvh.cn/Article/details/ghdxnlumi.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.hesvh.cn/Article/details/gcmkqvwqi.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.zdbjq.cn/Article/details/gycdgctwm.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/gsizkrfur.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.zdbjq.cn/Article/details/ghgivucfc.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.zdbjq.cn/Article/details/guoosjjps.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.zdbjq.cn/Article/details/gzqbbusdh.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.zdbjq.cn/Article/details/gztaoadvo.sHtML

[N05] 最大公约数
来源：http://3g.hesvh.cn/Article/details/gyhhbyjud.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.zdbjq.cn/Article/details/goxfjwukn.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.fehbvm.com/Article/details/gqardbxor.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.fehbvm.com/Article/details/goauohaeu.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.hesvh.cn/Article/details/gitgwdluj.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.fehbvm.com/Article/details/gcyrnxtys.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.zdbjq.cn/Article/details/glmbqynnd.sHtML

Ruby: a.gcd(b)
来源：http://www.share.fehbvm.com/Article/details/gotanoshd.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.zdbjq.cn/Article/details/gapetoeyo.sHtML

[N06] 判断回文字符串
来源：http://blog.zdbjq.cn/Article/details/gxuauuaom.sHtML

Py:   s == s[::-1]
来源：http://mobile.hesvh.cn/Article/details/gqvixzvls.sHtML

PHP:  $s === strrev($s);
来源：http://3g.zdbjq.cn/Article/details/guqrqpigf.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/gktfslssj.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.zdbjq.cn/Article/details/gstfgwnjx.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.zdbjq.cn/Article/details/gxicjtrdx.sHtML

Go:   // 双指针从两端比较
来源：http://blog.hesvh.cn/Article/details/gzhwcivio.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.zdbjq.cn/Article/details/gwsleknru.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.hesvh.cn/Article/details/grjsqxigz.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.hesvh.cn/Article/details/giraffuwm.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.fehbvm.com/Article/details/gxverxqot.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.zdbjq.cn/Article/details/gbvrmyowu.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.fehbvm.com/Article/details/gnrskreiw.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.zdbjq.cn/Article/details/gtofvnsei.sHtML

Java: // 手写 HashMap
来源：http://3g.zdbjq.cn/Article/details/gtdapkviz.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.hesvh.cn/Article/details/gsqzaruts.sHtML

Ruby: // 手写 Hash
来源：http://baike.zdbjq.cn/Article/details/gewpfyioi.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.zdbjq.cn/Article/details/gztsmcbtb.sHtML

[N08] 生成全排列
来源：http://www.blog.fehbvm.com/Article/details/gvresdwwk.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.fehbvm.com/Article/details/goiyoxfag.sHtML

PHP:  // 手写递归交换
来源：http://wap.fehbvm.com/Article/details/gknclrhja.sHtML

JS:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/ggglrdwsc.sHtML

TS:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gjftsffga.sHtML

Java: // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gakfeinii.sHtML

Go:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gwkbcgtay.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.hesvh.cn/Article/details/gkxbnbsum.sHtML

C#:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/glbdbjnnf.sHtML

[N09] 栈与队列
来源：http://baike.fehbvm.com/Article/details/gpixwmlzt.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.fehbvm.com/Article/details/gfhstotwx.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.zdbjq.cn/Article/details/gdcjxysgv.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.fehbvm.com/Article/details/gkqbzbjpb.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.zdbjq.cn/Article/details/golykxzrg.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.zdbjq.cn/Article/details/ghezisbsk.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.hesvh.cn/Article/details/guoaxiile.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.zdbjq.cn/Article/details/gmbzqajjp.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.zdbjq.cn/Article/details/ghnmvqmbf.sHtML

[N10] 链表节点定义
来源：http://baike.fehbvm.com/Article/details/gpznokhty.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.hesvh.cn/Article/details/glnmycmvw.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.fehbvm.com/Article/details/gpxtxgazq.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.zdbjq.cn/Article/details/ghkbtxnmx.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.hesvh.cn/Article/details/gwlgnmdxu.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.fehbvm.com/Article/details/gdoyewqsh.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.zdbjq.cn/Article/details/gdsdgsmhh.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.zdbjq.cn/Article/details/gbniittlf.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.fehbvm.com/Article/details/gxlombifg.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.hesvh.cn/Article/details/gwndmfbsm.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.hesvh.cn/Article/details/gufztxcwv.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.fehbvm.com/Article/details/gfsfnlmzk.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.zdbjq.cn/Article/details/ghxmanhum.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.fehbvm.com/Article/details/gsfjjgcob.sHtML

Java: // 手写递归
来源：http://blog.zdbjq.cn/Article/details/gsunnwepo.sHtML

Go:   // 手写递归
来源：http://3g.zdbjq.cn/Article/details/gmiwhwwvc.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.hesvh.cn/Article/details/gefjjksdj.sHtML

C#:   // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/gykpvnmyn.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.zdbjq.cn/Article/details/gmenpenix.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.zdbjq.cn/Article/details/getoffdyd.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.fehbvm.com/Article/details/gaqnwfdfm.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.fehbvm.com/Article/details/gdkngihmz.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.zdbjq.cn/Article/details/gxzmgfgqe.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.hesvh.cn/Article/details/gissrakmb.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.zdbjq.cn/Article/details/gjcyxqjlg.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.zdbjq.cn/Article/details/gibgunqex.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.hesvh.cn/Article/details/gnbppxrvg.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gbajhggeb.sHtML

O. 并发与异步
来源：http://read.share.zdbjq.cn/Article/details/gjemuwrtr.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gziyiuozl.sHtML

[O01] 启动一个线程
来源：http://wap.fehbvm.com/Article/details/gworujaha.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.zdbjq.cn/Article/details/gctdolsbc.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.fehbvm.com/Article/details/gicvqcawk.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.hesvh.cn/Article/details/gbxdswujq.sHtML

TS:   // 同 JS
来源：http://read.share.fehbvm.com/Article/details/gxrkilqjr.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.zdbjq.cn/Article/details/gyylfuddp.sHtML

Go:   go f()
来源：http://baike.hesvh.cn/Article/details/gxxvtisuu.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.zdbjq.cn/Article/details/ggvwxoqlg.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.zdbjq.cn/Article/details/gzqflowpm.sHtML

[O02] 使用线程池
来源：http://blog.hesvh.cn/Article/details/gjtjlyroy.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.zdbjq.cn/Article/details/gbkufjsoq.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.hesvh.cn/Article/details/ghrkdavjx.sHtML

JS:   // worker_threads 线程池
来源：http://baike.fehbvm.com/Article/details/gmggndicg.sHtML

TS:   // worker_threads 线程池
来源：http://wap.fehbvm.com/Article/details/gkgzjifrd.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.zdbjq.cn/Article/details/gcplkblrs.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.zdbjq.cn/Article/details/guuinxzqe.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.fehbvm.com/Article/details/gbbesgblw.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.fehbvm.com/Article/details/gnvlxnyzg.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.hesvh.cn/Article/details/gupwseoxy.sHtML

Py:   with lock: shared += 1
来源：http://blog.hesvh.cn/Article/details/gquevvixn.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.zdbjq.cn/Article/details/gzwqwkhri.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.zdbjq.cn/Article/details/gaqbabdqf.sHtML

TS:   // 同 JS
来源：http://www.share.fehbvm.com/Article/details/gmbvdfugj.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.fehbvm.com/Article/details/gvvhlpxgs.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.zdbjq.cn/Article/details/gjekkkrrc.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.fehbvm.com/Article/details/gccxavbsg.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.fehbvm.com/Article/details/gpyksnyep.sHtML

[O04] 定义异步函数并等待
来源：http://wap.zdbjq.cn/Article/details/gdyahhstn.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.zdbjq.cn/Article/details/gmuugagbr.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.zdbjq.cn/Article/details/gralpobxu.sHtML

JS:   async function f() { await g(); }
来源：http://wap.hesvh.cn/Article/details/gwnltaqvc.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.fehbvm.com/Article/details/gxvdunhbc.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.hesvh.cn/Article/details/gocxxjxzf.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.hesvh.cn/Article/details/gdlwzwtdd.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.zdbjq.cn/Article/details/gictnczbv.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.zdbjq.cn/Article/details/gddchnkga.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.zdbjq.cn/Article/details/glfiejyib.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.hesvh.cn/Article/details/ghuwvvhrf.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.hesvh.cn/Article/details/gwbxfiejb.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.hesvh.cn/Article/details/gckycjqgn.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.hesvh.cn/Article/details/gbhrgdmuh.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.hesvh.cn/Article/details/gbyzumzpg.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.hesvh.cn/Article/details/ghvfuifid.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.hesvh.cn/Article/details/gbgtqmvrg.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.zdbjq.cn/Article/details/gmxvexmya.sHtML

[O06] 使用进程池
来源：http://m.share.zdbjq.cn/Article/details/gktyouahh.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.fehbvm.com/Article/details/gamnawenr.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.zdbjq.cn/Article/details/ghxocklny.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.zdbjq.cn/Article/details/gtfctzgaj.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.hesvh.cn/Article/details/ggihucuzp.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.hesvh.cn/Article/details/gthbwigmp.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.fehbvm.com/Article/details/gyrmooayy.sHtML

Ruby: // fork 块
来源：http://www.m.share.hesvh.cn/Article/details/gwttrlbvp.sHtML

C#:   Parallel.For
来源：http://read.share.hesvh.cn/Article/details/gcacsoarl.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gjqhysigm.sHtML

P. 常用工具函数
来源：http://blog.zdbjq.cn/Article/details/gwnwtphce.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gadgqnhrx.sHtML

[P01] 生成 UUID
来源：http://3g.hesvh.cn/Article/details/gpgszlled.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.hesvh.cn/Article/details/gxmhohiud.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.fehbvm.com/Article/details/gistmnnri.sHtML

JS:   crypto.randomUUID()
来源：http://blog.hesvh.cn/Article/details/gkhnuinjj.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.hesvh.cn/Article/details/geaonycbh.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.hesvh.cn/Article/details/gnyqrrhcc.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.zdbjq.cn/Article/details/gqglanlsv.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.hesvh.cn/Article/details/gpwridrdx.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.hesvh.cn/Article/details/gussogcqh.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.zdbjq.cn/Article/details/gmfwqxcme.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.fehbvm.com/Article/details/ggnnujknh.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.fehbvm.com/Article/details/guenfvguw.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.fehbvm.com/Article/details/gkmjkaryk.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.hesvh.cn/Article/details/gajvrgjsm.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.fehbvm.com/Article/details/grpvbsamd.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.hesvh.cn/Article/details/guyyhqagb.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.zdbjq.cn/Article/details/gjtuvkqop.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.zdbjq.cn/Article/details/gihrhibda.sHtML

[P03] 生成短随机字符串
来源：http://blog.zdbjq.cn/Article/details/ghoozmjpn.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.fehbvm.com/Article/details/gujxtnwhq.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.hesvh.cn/Article/details/gwvfffqxp.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.zdbjq.cn/Article/details/gvfxuyjxo.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.fehbvm.com/Article/details/gvmiosbya.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.zdbjq.cn/Article/details/ggesfwysx.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.hesvh.cn/Article/details/ghorxscvs.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.zdbjq.cn/Article/details/gnsipllsk.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.fehbvm.com/Article/details/gnxrupalf.sHtML

[P04] 求长度
来源：http://mobile.fehbvm.com/Article/details/gmpfpvwla.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.zdbjq.cn/Article/details/gsoezqiqg.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.hesvh.cn/Article/details/genrhvhsq.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.zdbjq.cn/Article/details/gmcryzlni.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.zdbjq.cn/Article/details/gyvejozvu.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.fehbvm.com/Article/details/gdaqzjecs.sHtML

Go:   len(arr);  len(m)
来源：http://3g.hesvh.cn/Article/details/gsuxpxbuu.sHtML

Ruby: x.length;  x.size
来源：http://3g.fehbvm.com/Article/details/gtccrpoiy.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.fehbvm.com/Article/details/gfqfzfquk.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.hesvh.cn/Article/details/gxsxjtahe.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.zdbjq.cn/Article/details/gzzocbjqt.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.zdbjq.cn/Article/details/gjgbnsqlr.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.zdbjq.cn/Article/details/gqhjsvjmr.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.fehbvm.com/Article/details/gumktpqgk.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.fehbvm.com/Article/details/gczquepzj.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.hesvh.cn/Article/details/gmtnylhqf.sHtML

Ruby: a == b
来源：http://blog.hesvh.cn/Article/details/glkbnbgcr.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.zdbjq.cn/Article/details/grbdgweot.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.fehbvm.com/Article/details/gmrsvdfjf.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.fehbvm.com/Article/details/gttbswysf.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.hesvh.cn/Article/details/gdzqgxnsc.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.fehbvm.com/Article/details/gtoxulbhy.sHtML

TS:   if (x == null) {}
来源：http://wap.fehbvm.com/Article/details/gjgtwtcaz.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.zdbjq.cn/Article/details/gphlxahen.sHtML

Go:   if x == nil {}
来源：http://www.blog.zdbjq.cn/Article/details/gcreppoci.sHtML


<!-- 参考信息 -->