代发 wailian999

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.quarkkingdee.top/gtqgfryolp.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.kuanghao11.cn/gtxkcywtoq.html

================================================================================
来源：http://hz.sufxvd.cn/gtiaiqjkex.html

M. 命令行 / 进程 / 环境
来源：http://hz.pengpengdd.cyou/gtxaphhngf.html

================================================================================
来源：http://hz.yj20258.top/gtsgdyuprb.html

[M01] 读取命令行参数
来源：http://hz.hammf.cn/gtxugnpiiy.html

Py:   sys.argv[1:]
来源：http://hz.c1oappe.top/gtlcgkjaym.html

PHP:  $argv;  $argc;
来源：http://hz.jinqigufen.top/gtoyvxwmlu.html

JS:   process.argv.slice(2)
来源：http://hz.jyoumei.cn/gtpcojyjkh.html

TS:   process.argv.slice(2)
来源：http://hz.redwolf501.top/gtqolfikhr.html

Java: args 数组（main 方法参数）
来源：http://hz.guowangkeji.top/gtcxcvifmf.html

Go:   os.Args[1:]
来源：http://hz.yvedp.cn/gtnragszma.html

Ruby: ARGV
来源：http://hz.chenzaomai.com/gtvcljeojm.html

C#:   args 数组（Main 方法参数）
来源：http://hz.feifeiyinyue.top/gtjzemmwbs.html

[M02] 读取环境变量
来源：http://hz.xuanzx.com/gteyzcnvlb.html

Py:   os.environ.get("HOME")
来源：http://hz.meibo888.top/gtzdtzeblx.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.yvedp.cn/gtfjwwjkmr.html

JS:   process.env.HOME
来源：http://hz.yonumen.top/gtlxhytvqa.html

TS:   process.env.HOME
来源：http://hz.jyoumei.cn/gtdumobmkk.html

Java: System.getenv("HOME")
来源：http://hz.kuanghao11.cn/gtwuqksxhe.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.snrcjt.cn/gtwrdzidfc.html

Ruby: ENV["HOME"]
来源：http://hz.c1oappe.top/gtajrccmnc.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.vqdsnc.cn/gtyhnqxirp.html

[M03] 执行外部命令
来源：http://hz.bjfxy.top/gtvaoeavti.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.jqgfzy.top/gtgcrgdeow.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.9152youxi.cn/gthznpmuli.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.nwbrower.top/gtfymmjrkf.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.meibo888.top/gtbsqfwnsp.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.zhengqikj.top/gtzvcwqrbs.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.snrcjt.cn/gtffwddybs.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.zdqjudy.top/gtxsgtvlgk.html

C#:   Process.Start("ls", "-l");
来源：http://hz.vqdsnc.cn/gttyduqcjf.html

[M04] 获取当前工作目录
来源：http://hz.c1oappe.top/gtrdzqtjnn.html

Py:   os.getcwd()
来源：http://hz.yvedp.cn/gtzlhtjezk.html

PHP:  getcwd();
来源：http://hz.hnqzz.top/gtcunuwnza.html

JS:   process.cwd()
来源：http://hz.guannengcc.top/gtohdkrhnh.html

TS:   process.cwd()
来源：http://hz.jinqigufen.top/gttwrbhnaa.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.cucudq.cn/gtqsbxoyuu.html

Go:   os.Getwd()
来源：http://hz.sysykeji.top/gtwdnqxpsq.html

Ruby: Dir.pwd
来源：http://hz.yonumen.top/gtrusikofv.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.shanyushiyangtech.top/gthsayxapt.html

[M05] 设置退出码
来源：http://hz.ehwqpu.com/gtpyqbgocb.html

Py:   sys.exit(1)
来源：http://hz.guowangkeji.top/gtcucvozkh.html

PHP:  exit(1);
来源：http://hz.ywan-chungtsiang.top/gtviqougft.html

JS:   process.exit(1)
来源：http://hz.jinqigufen.top/gtlnodukgs.html

TS:   process.exit(1)
来源：http://hz.hywenlv.cn/gtnomoqwzf.html

Java: System.exit(1)
来源：http://hz.zhixingplan.top/gtlmulmqlt.html

Go:   os.Exit(1)
来源：http://hz.chenjidiqi.icu/gtiedewceo.html

Ruby: exit 1
来源：http://hz.guannengcc.top/gtshpuhiim.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.zhaomingkeji.xyz/gtyznqjcag.html

[M06] 向标准错误输出
来源：http://hz.gogol.net.cn/gttbayblnc.html

Py:   print("err", file=sys.stderr)
来源：http://hz.ydjk.org.cn/gtujitxpcm.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.smart0.xyz/gtkqqgumjx.html

JS:   console.error("err")
来源：http://hz.cheryme.top/gtcqkkopmo.html

TS:   console.error("err")
来源：http://hz.ywan-chungtsiang.top/gtuvbqzmcl.html

Java: System.err.println("err")
来源：http://hz.0kj1m.cn/gtoxjciink.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.zdqjudy.top/gtqibktliv.html

Ruby: warn "err"
来源：http://hz.mhx1999.top/gtxtxziynq.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.smart0.xyz/gtwcnvxvka.html

[M07] 判断是否为主入口
来源：http://hz.fzhhl.top/gtbqfedffh.html

Py:   if __name__ == "__main__":
来源：http://hz.jqgfzy.top/gtvfddsngo.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.jinqigfzy.top/gtfjrzvinm.html

JS:   require.main === module
来源：http://hz.pengpengdd.cyou/gtywlylxqz.html

TS:   require.main === module
来源：http://hz.hysaishi.cn/gtrsclcuoo.html

Java: public static void main(String[] args)
来源：http://hz.andypj.xyz/gtkmvjqhtx.html

Go:   func main()
来源：http://hz.dashuyun.cn/gtkzzmvzxe.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.fengsongda.top/gtsytpocka.html

C#:   static void Main(string[] args)
来源：http://hz.ehwqpu.com/gtilvffyyy.html

[M08] 获取系统与运行时信息
来源：http://hz.pengpengdd.cyou/gttjmlwtjt.html

Py:   platform.system();  platform.python_version()
来源：http://hz.havefunace.top/gtsaeqdxgp.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.shzxlz.cn/gtjyxupfja.html

JS:   process.platform;  process.version
来源：http://hz.nanxinkj.top/gtuldzocil.html

TS:   process.platform;  process.version
来源：http://hz.tanke756.top/gtttctbsvw.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.tianlin.xyz/gtcybmnugv.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.svipenyu.cn/gtcxryhxsa.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.yvedp.cn/gtogovmbhp.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.yonumen.top/gthmxqzomr.html

================================================================================
来源：http://hz.zycfv.cn/gtphmmxcrr.html

N. 数据结构与算法
来源：http://hz.aibaodan.cn/gtxswnsqsl.html

================================================================================
来源：http://hz.yvedp.cn/gtlvguexaw.html

[N01] 二分查找（有序数组）
来源：http://hz.xinyue.icu/gtlsfuykze.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.zhengqikj.top/gtkiasyexb.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.jinyuanbaomall.cn/gtfmyumdim.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.xziqi.cn/gttspyqjea.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.snrcjt.cn/gtugnzncwf.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.aizwys.cn/gtcdunnwuu.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.snrcjt.cn/gtostkbsyr.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.hongshengwenyu.top/gtfbbuemoh.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.jyoumei.cn/gtzoepzrwp.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.sufxvd.cn/gtxikmhlig.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.zdqjudy.top/gtitpistie.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.sufxvd.cn/gtybkxwjzr.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.hongshengwenyu.top/gtkyxobcmj.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.yvedp.cn/gtdmcfigvs.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.jinghuilouyu.cn/gttixerbkr.html

Go:   slices.Sort(arr)
来源：http://hz.bjfxy.top/gtfwbtkymi.html

Ruby: arr.sort
来源：http://hz.cdnleiting.top/gtpuglhmgg.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.chenjidiqi.icu/gtgpvsibjc.html

[N03] 快速排序（分治示例）
来源：http://hz.xinyue.icu/gtrunybnbk.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.smart0.xyz/gtmhouplog.html

PHP:  // 递归实现，或用 usort
来源：http://hz.xuetiantiany.cn/gtrlsuszoq.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.ydzc1.top/gtnctuxgug.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.ivvv.top/gtqsxixxjx.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.hywenlv.cn/gtivdxgijm.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.meibo888.top/gtvddtscwp.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.kuanghao11.cn/gtzclvqdhz.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.hysaishi.cn/gtdkvvvanc.html

[N04] 斐波那契数列
来源：http://hz.xuetiantiany.cn/gtrlnnxtaj.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.havefunace.top/gtrtksukgm.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.bjfxy.top/gtgjiwbvuu.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.nwbrower.top/gtehunmtwc.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.fengsongda.top/gtwabfojsg.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.jinqigufen.top/gtvaajhqwu.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.havefunace.top/gtfbxedsls.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.jinghuilouyu.cn/gtfzjwqsqy.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.cqqwz.cn/gtwedqnybu.html

[N05] 最大公约数
来源：http://hz.shanyushiyangkeji.top/gttegqhtex.html

Py:   math.gcd(a, b)
来源：http://hz.xingfuxueyuan.xyz/gtbzjsjujr.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.zhaomingkeji.xyz/gttnlzfkbb.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.yonumen.top/gtpbjnnyed.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.shzxlz.cn/gtbwicxrym.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.zhiwuduotai.top/gtmnqmkvwc.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.guowangkeji.top/gtawxqfwhb.html

Ruby: a.gcd(b)
来源：http://hz.wangdashe.top/gtmtndeoqs.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.hysaishi.cn/gtiinyuaor.html

[N06] 判断回文字符串
来源：http://hz.52xcode.cn/gtcjewwnfo.html

Py:   s == s[::-1]
来源：http://hz.yj20258888.top/gtimafauka.html

PHP:  $s === strrev($s);
来源：http://hz.jyoumei.cn/gtcmwxbgby.html

JS:   s === [...s].reverse().join("")
来源：http://hz.zhoulong.xyz/gtpcqppcap.html

TS:   s === [...s].reverse().join("")
来源：http://hz.jinqigufen.top/gtyrpaonrl.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.hfpthk.cn/gtdevfvwua.html

Go:   // 双指针从两端比较
来源：http://hz.birdmap.top/gtdcotzvik.html

Ruby: s == s.reverse
来源：http://hz.shangyingyoupin.top/gtpycwsnzf.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.jinghuilouyu.cn/gtxecbkvuz.html

[N07] 两数之和（返回下标）
来源：http://hz.meibo888.top/gtuwpjxpts.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.cucudq.cn/gtqpehdtld.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.shanyushiyangkeji.top/gtpswvflfw.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.yonumen.top/gtpvwnfukh.html

TS:   // 手写 Map<string, number>
来源：http://hz.andypj.xyz/gtucntqgvx.html

Java: // 手写 HashMap
来源：http://hz.svipenyu.cn/gthliokzdd.html

Go:   // 手写 map[int]int
来源：http://hz.hongshengwenyu.top/gtrweogeus.html

Ruby: // 手写 Hash
来源：http://hz.vqdsnc.cn/gthdnxppuv.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.daria6918.cn/gttoqkqzom.html

[N08] 生成全排列
来源：http://hz.cdnleiting.top/gtrqbcfekr.html

Py:   itertools.permutations(arr)
来源：http://hz.hnqzz.top/gtetxecthp.html

PHP:  // 手写递归交换
来源：http://hz.daxiang520.top/gttznvhbtu.html

JS:   // 手写回溯递归
来源：http://hz.xinyue.icu/gtoacgpnxk.html

TS:   // 手写回溯递归
来源：http://hz.hongshengwenyu.top/gtohmpqzcf.html

Java: // 手写回溯递归
来源：http://hz.shangyingyoupin.top/gtobofqpch.html

Go:   // 手写回溯递归
来源：http://hz.ywan-chungtsiang.top/gtkciydagf.html

Ruby: arr.permutation.to_a
来源：http://hz.dashuyun.cn/gtbcalumua.html

C#:   // 手写回溯递归
来源：http://hz.cheryme.top/gtruzhfqvq.html

[N09] 栈与队列
来源：http://hz.ybcxt.top/gtoxdmrsvu.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.hywenlv.cn/gtjvopzrgq.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.bjfxy.top/gtsiljxrvr.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.jinqigfzy.top/gtjwayxzer.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.jqgufenzy.top/gtyaeliels.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.redwolf501.top/gtdhyhcgdn.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.andypj.xyz/gtevtekptg.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.jiagoushi.top/gtpldbcifw.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.havefunace.top/gtjijoylmu.html

[N10] 链表节点定义
来源：http://hz.ehwqpu.com/gtbdcwnqom.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.zhengqikj.top/gtbfvcrlex.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.iojbl.cn/gtkketbdnm.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.yuxming.cn/gtkouxdiwg.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.andypj.xyz/gtvxwlkhsv.html

Java: class Node { int v; Node next; }
来源：http://hz.gotoacloud.top/gttglssvjl.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.hnxiangtu.top/gtqvrlqmst.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.jianghu66.top/gtymsnnwzp.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.gaohongyu789.top/gtfpjnpyzb.html

[N11] 二叉树中序遍历
来源：http://hz.nanxinkj.top/gtmpfbosfz.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.chenjidiqi.icu/gtzoeqjapn.html

PHP:  // 手写递归函数
来源：http://hz.yuanzhike.top/gtvrturqtv.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.bjfxy.top/gtpaxftwsq.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.gzhubu.top/gtbwlyyhhf.html

Java: // 手写递归
来源：http://hz.smart0.xyz/gtfnxkjnqt.html

Go:   // 手写递归
来源：http://hz.chenzaomai.com/gtowjbkpzk.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.zhixingplan.top/gtnljdrvmv.html

C#:   // 手写递归
来源：http://hz.jyoumei.cn/gtgcjyiiaf.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.yj20258888.top/gtiqohcxsh.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.chenjidiqi.icu/gtwiwxthhu.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.gogol.net.cn/gtmlfjoayf.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.yj20258.top/gtpcfzjpwp.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.wangshuangyany.cn/gtdoetluon.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.yuxming.cn/gtaztokjln.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.xingfuxueyuan.xyz/gtlovxksfx.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.nwbrower.top/gtcattkqui.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.nanxinkj.top/gtgalqkybf.html

================================================================================
来源：http://hz.mhx1999.top/gtbboxhxrv.html

O. 并发与异步
来源：http://hz.yj202588.top/gtiapgekaw.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtvmymycap.html

[O01] 启动一个线程
来源：http://hz.yueranfly.top/gtivmejmni.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.zhoulong.xyz/gtbbyxpmbn.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.jinyuanbaomall.cn/gtqckxeqyy.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.guannengcc.top/gtbrjwpmpp.html

TS:   // 同 JS
来源：http://hz.jqgfzy.top/gthaanyety.html

Java: new Thread(() -> f()).start()
来源：http://hz.cheryme.top/gtmtnkxfgz.html

Go:   go f()
来源：http://hz.gotoacloud.top/gtgqwkmjtb.html

Ruby: Thread.new { f }
来源：http://hz.haohaochexian.top/gtahqkiwfh.html

C#:   Task.Run(() => F());
来源：http://hz.9152youxi.cn/gtmpcexpxx.html

[O02] 使用线程池
来源：http://hz.yuanzhike.top/gtrchxeprm.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.52xcode.cn/gtqsvitxlr.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.c1oappe.top/gtltkrflvg.html

JS:   // worker_threads 线程池
来源：http://hz.guannengcc.top/gtebpxdpek.html

TS:   // worker_threads 线程池
来源：http://hz.hongshengwenyu.top/gtgzqftqao.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.hnqzz.top/gtoablhioy.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.yvedp.cn/gtaaqvebch.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.zhengqikj.top/gtetxuixqn.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.gaohongyu789.top/gtywwzgdur.html

[O03] 加锁保护共享数据
来源：http://hz.birdmap.top/gtwrdtrxmv.html

Py:   with lock: shared += 1
来源：http://hz.jinqigufen.top/gtmlbgvenv.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.snrcjt.cn/gtbrqnapcl.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.haohaochexian.top/gtsunqvbui.html

TS:   // 同 JS
来源：http://hz.sweek.top/gtucsjdnof.html

Java: synchronized (this) { shared++; }
来源：http://hz.sysykeji.top/gterrxcujy.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.0kj1m.cn/gtgmadwlru.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.wangshuangyany.cn/gtmqvbjkpu.html

C#:   lock (gate) { shared++; }
来源：http://hz.pycfn.com/gtmnfedbpl.html

[O04] 定义异步函数并等待
来源：http://hz.shangyingyoupin.top/gtbojdgxmy.html

Py:   async def f():⏎    await g()
来源：http://hz.jinqigufen.top/gtxhfwggik.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.wangdashe.top/gtqvblegjh.html

JS:   async function f() { await g(); }
来源：http://hz.tanke756.top/gtslqwqyxh.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.vqdsnc.cn/gtruloenmp.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.andypj.xyz/gthofbsbkx.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.vqdsnc.cn/gtupnciujr.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.aizwys.cn/gtrwxceajm.html

C#:   async Task F() { await G(); }
来源：http://hz.quarkkingdee.top/gtadralomt.html

[O05] 并发执行并等待全部完成
来源：http://hz.chenzaomai.com/gtwwooowaw.html

Py:   asyncio.gather(*tasks)
来源：http://hz.yj202588.top/gtvgxoeybf.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.zdqjudy.top/gtrivvfmhd.html

JS:   await Promise.all(tasks)
来源：http://hz.gotoacloud.top/gtmddhoadu.html

TS:   await Promise.all(tasks)
来源：http://hz.yueranfly.top/gtwxflpjya.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.shanyushiyangkeji.top/gtfyidjbce.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.zhaomingkeji.xyz/gtcmiibhva.html

Ruby: threads.map(&:join)
来源：http://hz.cqqwz.cn/gtaarddwlr.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.316326.xyz/gtxdoacvvc.html

[O06] 使用进程池
来源：http://hz.jinyuanbaomall.cn/gtriqegtyk.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.hammf.cn/gtnoxktxpf.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.shuidangran.top/gtmjnbcxmf.html

JS:   // child_process / cluster 模块
来源：http://hz.hfpthk.cn/gtoiabzvkn.html

TS:   // child_process / cluster 模块
来源：http://hz.shzxlz.cn/gtuzdnvwwu.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.yanxiufei.cn/gtfulihtsq.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.mhx1999.top/gtaoqpecln.html

Ruby: // fork 块
来源：http://hz.316326.xyz/gtwomttmtw.html

C#:   Parallel.For
来源：http://hz.tian-w.cn/gtbcmgvkhm.html

================================================================================
来源：http://hz.kuanghao11.cn/gtugginfqg.html

P. 常用工具函数
来源：http://hz.c1oappe.top/gtyszbbpmc.html

================================================================================
来源：http://hz.yj20258888.top/gtwchuozmw.html

[P01] 生成 UUID
来源：http://hz.hywenlv.cn/gtvahixgsl.html

Py:   str(uuid.uuid4())
来源：http://hz.zhaomingkeji.xyz/gtenfhqjgo.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.dianchejie.cn/gtwrvffloe.html

JS:   crypto.randomUUID()
来源：http://hz.yvedp.cn/gtymxtadja.html

TS:   crypto.randomUUID()
来源：http://hz.gotoacloud.top/gtxbwfztnf.html

Java: UUID.randomUUID().toString()
来源：http://hz.xinyue.icu/gtjhfldyje.html

Go:   // 用 github.com/google/uuid
来源：http://hz.hammf.cn/gtxfzoxhaf.html

Ruby: SecureRandom.uuid
来源：http://hz.nanxinkj.top/gtiwkdfbad.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.gogol.net.cn/gtqbxlcpfy.html

[P02] MD5 / SHA256 摘要
来源：http://hz.yongpay.top/gttjcpyhsx.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.cqqwz.cn/gtqpkyjtjk.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.smart0.xyz/gtqwpzclry.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.meibo888.top/gtslyyytnp.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.iojbl.cn/gtruncptlv.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.cucudq.cn/gtkovohqbv.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.andypj.xyz/gtdymawpjc.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.sufxvd.cn/gtkeheoomf.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.zdqjudy.top/gtntbskofw.html

[P03] 生成短随机字符串
来源：http://hz.bjfxy.top/gtjlepmiuq.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.cashguo.top/gtzdpmposh.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.chenlongwang.top/gtljuwjzug.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.zycfv.cn/gtmgptsluv.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.jyoumei.cn/gtnjndhzbm.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.jinqigfzy.top/gtrphwjitd.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.ydzc1.top/gtuftdqnns.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.chenzaomai.com/gtfxawjigs.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.xziqi.cn/gteakegyod.html

[P04] 求长度
来源：http://hz.svipenyu.cn/gtjmqekgjm.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.jinqigfzy.top/gtpgnwvhsi.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.ehwqpu.com/gtlolzruks.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.tian-w.cn/gtgxusydud.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.yonumen.top/gtdtmiibco.html

Java: list.size();  map.size();  s.length()
来源：http://hz.zhixingplan.top/gtmvnhabjb.html

Go:   len(arr);  len(m)
来源：http://hz.cqqwz.cn/gtmttzevyi.html

Ruby: x.length;  x.size
来源：http://hz.cucudq.cn/gticfpsmqo.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.jinyuanbaomall.cn/gtovsjkapr.html

[P05] 判断两个对象内容是否相等
来源：http://hz.haohaochexian.top/gthyxgwckw.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.cucudq.cn/gtxymdxngp.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.chenlongwang.top/gtaomsadww.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.yj20258.top/gtctspoxlk.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.zhixingplan.top/gtmhgqqxnf.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.yuxming.cn/gtbdmqzzyk.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.wangdashe.top/gtwhdevyqq.html

Ruby: a == b
来源：http://hz.jinqigfzy.top/gtfyujespo.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.ydjk.org.cn/gtvzdpmmrk.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.shanyushiyangtech.top/gtdgyzlfln.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.yj20258.top/gthqnmbozv.html

PHP:  if (empty($x)) {}
来源：http://hz.jqgufenzy.top/gtznamahnu.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.ehwqpu.com/gtteugzfqo.html

TS:   if (x == null) {}
来源：http://hz.wangshuangyany.cn/gtirdwkfti.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.guannengcc.top/gttpelhwlp.html

Go:   if x == nil {}
来源：http://hz.tanke756.top/gtkmdhwyzp.html


<!-- 参考信息 -->