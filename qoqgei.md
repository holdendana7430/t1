代发 wailian999

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3gljmkbqq.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3tzzskwnb.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3inyykmyy.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3rynfiujx.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3snvdodyy.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3akprjjzk.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3eipwljxj.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3hrjscqsc.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3gevokjkt.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3fzwfnvyt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jebdevhb.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3uihblvjj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bzkdinut.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3otyspkia.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3obctwdtr.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3gthnwctd.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3wwmnmkmk.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3olrvubzb.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3qyvqdcoj.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3vmsjgeri.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3qspogwjp.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3kawrzpuy.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3qqbxwicx.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3vgwpfvgu.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3pnsudwom.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3nbwijcco.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3lhyoyxoe.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3cizeksne.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3jgvpmpfr.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3imfmwbyt.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3hmsicdui.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3nidylgjf.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3oitdwvzv.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3duxdjmgp.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3qvvotrza.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3ujrzbyec.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3igenmvkc.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3gkarzpkf.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3uehtkdbw.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3hjeasxfv.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3egqyoizm.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3dkuxozhp.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3wriqjnqk.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3rzrtinhh.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3fbzcypkj.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3uutukqfs.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3snhqpcdp.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3wxruhqpb.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3wivzfqze.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3ctnbitgl.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xcyrkrcy.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3mvkzzzhd.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qovmcsnl.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3pnmukkry.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3bolvispq.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3bsvdagjn.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3yrfxbuvz.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3kjivlzsr.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3tazljsna.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3rxytpcht.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3ihzhuuns.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ogisnmym.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3lwcryqij.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3makhuakq.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3eezyhtvq.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3gznbqkyo.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3dpwxgvxj.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3sgblmsuc.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3owftzgrp.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3tccpsggc.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3pnvmfpaq.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3qdkvqwkw.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3yxfhlxyt.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3kpztrygz.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3ghyecacv.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3mrkfdmne.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3udcbzzvi.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3rygymars.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3pvopudfd.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3orbbruff.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3vwqkmveh.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3uzhgbbzu.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3jyocpoml.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3zqxktitu.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3mkzaiizb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nefgzwdo.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3hzxrajxt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zzqosbqs.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3rqpynqyr.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3qatitstx.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3paxiwflo.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3txagxhpa.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3ogostkuh.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3pemybpkv.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3nlsomisp.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3btxjnttf.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3oxrxdiql.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3gvevzbnz.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3nzdijqdg.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3tcyytpyt.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3pidktjje.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3axibnhgk.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3cjvrjbbo.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3aphiggby.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3lnqqukky.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3peavxfqb.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3bfbugxji.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3wezestsg.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3fqvromxz.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3ivokkrvv.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3fgubwlph.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3lxzbgtih.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3wxxxwfal.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3wycnmrdk.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3vqngydef.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3howpiwgm.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3wramgjvw.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3iobgspiw.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3ffpkemxn.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3qpcbqfwh.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3vlnvoqjd.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3ieqqnizz.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3tmaffsdy.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3bewtrpdw.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3nthsrpjq.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3bkjquxvz.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3vggetfoe.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3svqzhkus.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3pflokana.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3pesfoott.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3ltrzpaji.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3nsmnkloq.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3hjxhipyr.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wkvtihqa.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3qxbyfaer.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3uljaepgu.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3lrjajlwt.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3syqgomoo.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3kvbqgnfh.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3tnoacjqv.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3gaohtzmn.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3sijomvyt.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3whzfkltm.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3hqflildl.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3gcbsqavx.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3twbvipfd.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3ojuztbcl.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3gmcubdqh.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3xgsfhiww.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3bxehxjlv.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3zyqhvupp.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3milooqpb.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3vzngfaxn.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3xcsjdycu.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3fxvvswbx.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3oqwglfxu.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3wejvkouo.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ypjavoej.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3cwuxnrxo.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3dlrxjpgc.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3lprzpnfo.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3mhqhwpyj.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3ausymglq.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3zpbkqjtn.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3aznhznnh.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3lgybkcej.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3qqlybysj.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3xpzxfjod.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3vbeoghii.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3kvydhpwb.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3vtkileno.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3ggxqnzig.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3eponrprd.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3vlogwqfq.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3fajkxqfc.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3rliephwf.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3rxseiacc.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3ecygowbb.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3dncnufuw.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3dwbwmukf.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3kzumjghp.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3auwzwymx.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3iusjsrnk.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3xgtdaszu.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3wjjuttzp.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3cbifxpvk.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3dyphigmo.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3pfqvgver.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3ygbwsmwn.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3qkgagjow.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3nwgekgql.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3opagulmo.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3tiksgjrg.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3owetfemj.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3mbiretqy.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3pyyzcvjp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ozlrbrmj.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3eonhsbrk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3frpenbuo.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3ehaqfbkq.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3jglmlsho.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3kgwleyux.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3pnwnwvdl.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3pvzbcwuj.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3uzepeflm.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3gucibwkw.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3khdzxdix.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3ooefvkjq.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3afbhhpfn.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3kcccuzhf.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3esrttolo.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3ruhuiqqg.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3zhdlpvis.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3imvhbbdh.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3mwvctepm.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3bikxhwvh.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3sywrhtdv.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3ppstabpk.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3hwpwbqmu.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3xpdanifx.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3eeffbdio.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3snfnufbk.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3xgdeyzyj.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3pverpvkq.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3heotmxmt.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3mrsfmygf.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3uotyhmxw.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3fnguotup.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3ronpgtid.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xtuavlwv.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3hzzitale.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3rvlwacmk.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3spldipkn.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3fvzjhbyw.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3oovvfmxy.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3ftztihwn.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3fzsycnqo.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3xffmmiif.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3wfhxzktl.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3woqpgcbm.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3mogtpqnh.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3trzreari.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3ghvyugdz.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3dvfyipwh.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3rsebbvvj.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3ivheqslb.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3naneawsl.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3liietsxt.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3ceqggpgi.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3flpqizds.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3xrpdcxdv.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3otwegklg.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3lalxuucw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vjqzjgpl.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3maadzylr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sjogdklr.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3jhuueiae.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3clneuvtq.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3qzvqzvaq.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3ieiawgxa.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3zeththbw.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3msfmbcvo.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3xgwedojp.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3rxxjzknv.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3mucdmbcb.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3dvuexlgy.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3nctuczds.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3vknohjyy.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3hsokbmzm.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3jrlkaojb.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3ihztknty.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3dbsbxwov.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qbsfbryh.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3eaxudchg.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jxnjezer.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3uzawampd.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3lyvpexwz.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3urzmkmln.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3nbhkxvam.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3tifiilxr.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3hhugungv.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3rpuhffvr.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3ddkmzbyd.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3wzijudum.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3nmoebhvb.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3leupariq.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3boojishv.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3djnugnxu.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3yulfvbmj.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3nwtwfkqs.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3rxfmmpud.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3puicsnpz.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3bjxurwit.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3ccxkyktq.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3werdzyyq.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3dlxysckm.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3wlcnahfc.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3ciqvqivy.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3kpqrkdwm.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3lkfmbndv.html


<!-- 参考信息 -->