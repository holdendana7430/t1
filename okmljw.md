代发 wailian999

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.jqgfzy.top/gtrqxxtyww.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.jyoumei.cn/gtzyoycvep.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.yj20258888.top/gtsklkhtbv.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.shzxlz.cn/gtovpdtozy.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.jinghuilouyu.cn/gtibciwvvo.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.zdqjudy.top/gtxxzgmdaj.html

================================================================================
来源：http://hz.52xcode.cn/gtnqajyqnn.html

M. 命令行 / 进程 / 环境
来源：http://hz.yj20258888.top/gtmwsmygqi.html

================================================================================
来源：http://hz.zdqjudy.top/gtuqahqznn.html

[M01] 读取命令行参数
来源：http://hz.xziqi.cn/gtigommxkl.html

Py:   sys.argv[1:]
来源：http://hz.mhx1999.top/gtvwmcafpz.html

PHP:  $argv;  $argc;
来源：http://hz.jinqigfzy.top/gtejxrzhyh.html

JS:   process.argv.slice(2)
来源：http://hz.cqqwz.cn/gthnoccuom.html

TS:   process.argv.slice(2)
来源：http://hz.nanxuanxn.top/gtbdamloej.html

Java: args 数组（main 方法参数）
来源：http://hz.chenjidiqi.icu/gtfvxlubro.html

Go:   os.Args[1:]
来源：http://hz.jinqigufen.top/gtrtwjlxrt.html

Ruby: ARGV
来源：http://hz.0kj1m.cn/gtbhhmiegi.html

C#:   args 数组（Main 方法参数）
来源：http://hz.zycfv.cn/gtvivlspep.html

[M02] 读取环境变量
来源：http://hz.dianchejie.cn/gteahindof.html

Py:   os.environ.get("HOME")
来源：http://hz.havefunace.top/gtghcybfsg.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.hnxiangtu.top/gtywvhjhyo.html

JS:   process.env.HOME
来源：http://hz.xziqi.cn/gtpswencju.html

TS:   process.env.HOME
来源：http://hz.316326.xyz/gtysggslsm.html

Java: System.getenv("HOME")
来源：http://hz.cheryme.top/gtikuuvpfd.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.snrcjt.cn/gtyjmncwia.html

Ruby: ENV["HOME"]
来源：http://hz.xuanzx.com/gtufczlcss.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.aizwys.cn/gtwbbgiagt.html

[M03] 执行外部命令
来源：http://hz.zhongyouzk.top/gtgxwofpji.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.yuxming.cn/gtbhidyepo.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.jinqigfzy.top/gtblorqysd.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.jinqigfzy.top/gtktotxngu.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.tanke756.top/gtksvoefeq.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.yuanzhike.top/gtzuupgihf.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.sufxvd.cn/gtdtjfizhg.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.aizwys.cn/gtdcgalbge.html

C#:   Process.Start("ls", "-l");
来源：http://hz.dianchejie.cn/gtbdnyisvl.html

[M04] 获取当前工作目录
来源：http://hz.xingfuxueyuan.xyz/gtdzuguarz.html

Py:   os.getcwd()
来源：http://hz.sysykeji.top/gtexhnbtzu.html

PHP:  getcwd();
来源：http://hz.zhoulong.xyz/gtoleitlkj.html

JS:   process.cwd()
来源：http://hz.jqgfzy.top/gtgbknchgh.html

TS:   process.cwd()
来源：http://hz.nanxuanxn.top/gtwwmzzqrk.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.mhx1999.top/gtjdvdllzw.html

Go:   os.Getwd()
来源：http://hz.dashuyun.cn/gtrgjyahmg.html

Ruby: Dir.pwd
来源：http://hz.yuxming.cn/gtgignpyrk.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.haohaochexian.top/gtgqjqctvu.html

[M05] 设置退出码
来源：http://hz.gotoacloud.top/gtojaqbipi.html

Py:   sys.exit(1)
来源：http://hz.iojbl.cn/gtipvptfhx.html

PHP:  exit(1);
来源：http://hz.zhoulong.xyz/gtfeanfcpu.html

JS:   process.exit(1)
来源：http://hz.zhongyouzk.top/gteqkfvhqn.html

TS:   process.exit(1)
来源：http://hz.c1oappe.top/gtyjbpdujt.html

Java: System.exit(1)
来源：http://hz.zhoulong.xyz/gtcrnkganv.html

Go:   os.Exit(1)
来源：http://hz.jianghu66.top/gtulmyrgud.html

Ruby: exit 1
来源：http://hz.nwbrower.top/gtwpmpgvra.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.jinghuilouyu.cn/gtaeikfhtv.html

[M06] 向标准错误输出
来源：http://hz.zhoulong.xyz/gtvtdmyufv.html

Py:   print("err", file=sys.stderr)
来源：http://hz.tianlin.xyz/gtsoxqmtmi.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.jianghu66.top/gtiznammnz.html

JS:   console.error("err")
来源：http://hz.quarkkingdee.top/gtratgoixp.html

TS:   console.error("err")
来源：http://hz.yanxiufei.cn/gtxpokpndq.html

Java: System.err.println("err")
来源：http://hz.snrcjt.cn/gtkzseyzav.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.daxiang520.top/gtmrxrnpbz.html

Ruby: warn "err"
来源：http://hz.daria6918.cn/gtnnzebbmn.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.snrcjt.cn/gtdknhfyuk.html

[M07] 判断是否为主入口
来源：http://hz.sxryk.cn/gtdkntlrdr.html

Py:   if __name__ == "__main__":
来源：http://hz.yangfankeji.com/gtyyhcqamo.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.tanke756.top/gtvbldwtds.html

JS:   require.main === module
来源：http://hz.bjfxy.top/gtssbidxik.html

TS:   require.main === module
来源：http://hz.feifeiyinyue.top/gtqddrpswh.html

Java: public static void main(String[] args)
来源：http://hz.havefunace.top/gtgspthgqq.html

Go:   func main()
来源：http://hz.ywan-chungtsiang.top/gtvnrajaou.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.shzxlz.cn/gtsjfmwrvu.html

C#:   static void Main(string[] args)
来源：http://hz.9152youxi.cn/gtytrmptbn.html

[M08] 获取系统与运行时信息
来源：http://hz.xingfuxueyuan.xyz/gtzrrlmpqz.html

Py:   platform.system();  platform.python_version()
来源：http://hz.xylfe.cn/gtovrwfkpc.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.birdmap.top/gtapotiicm.html

JS:   process.platform;  process.version
来源：http://hz.cucudq.cn/gttxxzhemu.html

TS:   process.platform;  process.version
来源：http://hz.hongshengwenyu.top/gtlfnnfisa.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.wangdashe.top/gtgvdnfqii.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.zhoulong.xyz/gtsohnpzhg.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.tian-w.cn/gtpckiyllm.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.jianghu66.top/gtcczzdikg.html

================================================================================
来源：http://hz.shuidangran.top/gtcwckxcxx.html

N. 数据结构与算法
来源：http://hz.fzhhl.top/gtitzjopfv.html

================================================================================
来源：http://hz.vqdsnc.cn/gtlwfvddbp.html

[N01] 二分查找（有序数组）
来源：http://hz.aizwys.cn/gttfodbfew.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.hywenlv.cn/gttpxqnbfx.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.jinqigfzy.top/gtydasqlkj.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.zhongyouzk.top/gtdrhgwptf.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.xuanzx.com/gtjysmrbpw.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.cucudq.cn/gtbapkipfp.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.bjfxy.top/gtsbfbdpwg.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.jqgufenzy.top/gttsxypdrb.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.zhixingplan.top/gtndcczsip.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.cdnleiting.top/gtguzxitzc.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.cashguo.top/gtubwzqtse.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.tianlin.xyz/gtuuyopnaz.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.shanyushiyangtech.top/gtzxfepfyc.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.yangfankeji.com/gtlpgfjxrd.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.nwbrower.top/gtqemeydiz.html

Go:   slices.Sort(arr)
来源：http://hz.sxryk.cn/gtlgzeprmy.html

Ruby: arr.sort
来源：http://hz.chenjidiqi.icu/gtaqtevtgn.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.gogol.net.cn/gtdqiuzlrv.html

[N03] 快速排序（分治示例）
来源：http://hz.hfpthk.cn/gtakkwiesq.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.gaohongyu789.top/gtbjrboiam.html

PHP:  // 递归实现，或用 usort
来源：http://hz.316326.xyz/gtajvbrzhd.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.yongpay.top/gtmmuvfqwa.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.jqgufenzy.top/gtdxobfxjw.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.svipenyu.cn/gtodjcjjoa.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.daria6918.cn/gtqzqwnklx.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.redwolf501.top/gtsjakrdjh.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.ehwqpu.com/gtuwhqdtka.html

[N04] 斐波那契数列
来源：http://hz.cucudq.cn/gtewhszoxq.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.quarkkingdee.top/gtpnvvoigv.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.jlsjyb.cn/gtifzutvky.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.meibo888.top/gtfbsohekz.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.mhx1999.top/gtngvlvoyv.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.yuanzhike.top/gtbttkvszs.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.jinyuanbaomall.cn/gtutbgvyyn.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.jqgfzy.top/gtewzoyszt.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.shangyingyoupin.top/gtbojlyexq.html

[N05] 最大公约数
来源：http://hz.andypj.xyz/gtimyobluy.html

Py:   math.gcd(a, b)
来源：http://hz.cheryme.top/gtrdpqqmsi.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.yangfankeji.com/gtvdrpzgzn.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.ywan-chungtsiang.top/gtlpmtgnfr.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.iojbl.cn/gtlashjemi.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.hysaishi.cn/gthptoqysp.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.ydjk.org.cn/gtdnjqnxwe.html

Ruby: a.gcd(b)
来源：http://hz.xziqi.cn/gtwvpfxfzw.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.yj20258.top/gtzlsbnrve.html

[N06] 判断回文字符串
来源：http://hz.zycfv.cn/gtiquheezc.html

Py:   s == s[::-1]
来源：http://hz.jqgufenzy.top/gtadgjtxgt.html

PHP:  $s === strrev($s);
来源：http://hz.xylfe.cn/gtpzempand.html

JS:   s === [...s].reverse().join("")
来源：http://hz.cucudq.cn/gtucthohas.html

TS:   s === [...s].reverse().join("")
来源：http://hz.hfpthk.cn/gtuptvodjo.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.xinyue.icu/gtodxholvq.html

Go:   // 双指针从两端比较
来源：http://hz.jiagoushi.top/gtrfmicvkq.html

Ruby: s == s.reverse
来源：http://hz.iojbl.cn/gtohhkmhjm.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.chenjidiqi.icu/gtkvorkqnb.html

[N07] 两数之和（返回下标）
来源：http://hz.zhijiandao.cn/gtavlkaebo.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.gotoacloud.top/gtlcqjwgwc.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.sxryk.cn/gtmdtqmrrx.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.hfpthk.cn/gtmngquzzu.html

TS:   // 手写 Map<string, number>
来源：http://hz.tianlin.xyz/gtzapcjfxs.html

Java: // 手写 HashMap
来源：http://hz.snrcjt.cn/gtlnedykvz.html

Go:   // 手写 map[int]int
来源：http://hz.316326.xyz/gtxhzqcgan.html

Ruby: // 手写 Hash
来源：http://hz.shanyushiyangtech.top/gtwvheigqz.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.316326.xyz/gtjxdhsleo.html

[N08] 生成全排列
来源：http://hz.9152youxi.cn/gtjnlqhuoz.html

Py:   itertools.permutations(arr)
来源：http://hz.jlsjyb.cn/gtgkqkmfez.html

PHP:  // 手写递归交换
来源：http://hz.quarkkingdee.top/gtewdbpdof.html

JS:   // 手写回溯递归
来源：http://hz.yangfankeji.com/gtodbggftj.html

TS:   // 手写回溯递归
来源：http://hz.dashuyun.cn/gteuljmmwy.html

Java: // 手写回溯递归
来源：http://hz.hammf.cn/gtvgztvttd.html

Go:   // 手写回溯递归
来源：http://hz.birdmap.top/gtngynoaiu.html

Ruby: arr.permutation.to_a
来源：http://hz.snrcjt.cn/gttugxosmc.html

C#:   // 手写回溯递归
来源：http://hz.jinqigufen.top/gtlaskqxju.html

[N09] 栈与队列
来源：http://hz.pycfn.com/gtvbwecroq.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.zhengqikj.top/gtiggoptzj.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.shangyingyoupin.top/gtocupqore.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.fengsongda.top/gtyqpnhizi.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.jianghu66.top/gtuuwdspgn.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.cucudq.cn/gtebqctvua.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.cheryme.top/gtsupogfro.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.316326.xyz/gtggzifcxt.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.redwolf501.top/gtppytkgui.html

[N10] 链表节点定义
来源：http://hz.hammf.cn/gtvkbblova.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.sxryk.cn/gtrptdhpxb.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.birdmap.top/gtstajwhym.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.yanxiufei.cn/gtelkgetdh.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.sufxvd.cn/gtuabqqfkn.html

Java: class Node { int v; Node next; }
来源：http://hz.gotoacloud.top/gtvioctgbc.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.tian-w.cn/gthjxqogip.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.wangdashe.top/gtauanwnau.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.hammf.cn/gttztmvzmo.html

[N11] 二叉树中序遍历
来源：http://hz.9152youxi.cn/gtclbxtphk.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.jinghuilouyu.cn/gtgwcrkdqp.html

PHP:  // 手写递归函数
来源：http://hz.xingfuxueyuan.xyz/gtegvkyxqs.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.tianlin.xyz/gtqdusfogb.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.sweek.top/gtocmhcvdc.html

Java: // 手写递归
来源：http://hz.0kj1m.cn/gtldaqdlzo.html

Go:   // 手写递归
来源：http://hz.yj20258.top/gtbxgsbfka.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.sweek.top/gtyqjjnzid.html

C#:   // 手写递归
来源：http://hz.ehwqpu.com/gtovmtiyzm.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.zhiwuduotai.top/gtqfwrvpyk.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.sxryk.cn/gtnuyiefhv.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.tianlin.xyz/gtmbqxfsuw.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.cashguo.top/gtzqunsyjf.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.yanxiufei.cn/gtfxibjpno.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.yangfankeji.com/gtmwqkcgzp.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.chenzaomai.com/gtcfpuqswb.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.xinyue.icu/gtefzdmmzi.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.ehwqpu.com/gtjtpdgvga.html

================================================================================
来源：http://hz.zhongyouzk.top/gtovxwmjnd.html

O. 并发与异步
来源：http://hz.andypj.xyz/gttrwapmxg.html

================================================================================
来源：http://hz.jiagoushi.top/gtflquvtci.html

[O01] 启动一个线程
来源：http://hz.iojbl.cn/gtrtmycxet.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.bjfxy.top/gtrdjgojsr.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.0kj1m.cn/gtrqcdbwrp.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.shanyushiyangtech.top/gthllgntsv.html

TS:   // 同 JS
来源：http://hz.iojbl.cn/gtgztdbtew.html

Java: new Thread(() -> f()).start()
来源：http://hz.meibo888.top/gtmzrmyvfo.html

Go:   go f()
来源：http://hz.gogol.net.cn/gtnzsapwqv.html

Ruby: Thread.new { f }
来源：http://hz.shzxlz.cn/gtrpzrdhfg.html

C#:   Task.Run(() => F());
来源：http://hz.shanyushiyangtech.top/gtjcayzvdu.html

[O02] 使用线程池
来源：http://hz.ehwqpu.com/gtwgoirfay.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.yonumen.top/gtiirsqswg.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.wangdashe.top/gteokrdnle.html

JS:   // worker_threads 线程池
来源：http://hz.yj202588.top/gtmfoelfhs.html

TS:   // worker_threads 线程池
来源：http://hz.cdnleiting.top/gtobrccbdu.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.zhijiandao.cn/gtigsqarhe.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.dashuyun.cn/gtudgvmiei.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.jqgufenzy.top/gtqwxtwyih.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.zhongyouzk.top/gtrmbgicmz.html

[O03] 加锁保护共享数据
来源：http://hz.tanke756.top/gtqrjsnpxb.html

Py:   with lock: shared += 1
来源：http://hz.yj20258888.top/gtxemqhskk.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.feifeiyinyue.top/gtyrpqnebn.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.shuidangran.top/gtngvdlzpl.html

TS:   // 同 JS
来源：http://hz.yuanzhike.top/gtpwawywij.html

Java: synchronized (this) { shared++; }
来源：http://hz.cashguo.top/gtxzsjkouh.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.wangshuangyany.cn/gtdghuumyo.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.yvedp.cn/gtblpwqwoz.html

C#:   lock (gate) { shared++; }
来源：http://hz.svipenyu.cn/gtalxpogom.html

[O04] 定义异步函数并等待
来源：http://hz.jyoumei.cn/gtzbmumarc.html

Py:   async def f():⏎    await g()
来源：http://hz.jinghuilouyu.cn/gttbltsvon.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.nwbrower.top/gtkkwtylux.html

JS:   async function f() { await g(); }
来源：http://hz.feifeiyinyue.top/gtfvjxosfv.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.zhiwuduotai.top/gtftealbuy.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.yonumen.top/gtdrnqigma.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.hammf.cn/gtwxciqjjr.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.fengsongda.top/gtqnkbkaxy.html

C#:   async Task F() { await G(); }
来源：http://hz.nwbrower.top/gtqtibptwb.html

[O05] 并发执行并等待全部完成
来源：http://hz.zhijiandao.cn/gtffasgwcn.html

Py:   asyncio.gather(*tasks)
来源：http://hz.yj202588.top/gtupsbmyph.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.yj20258888.top/gtusbxfifn.html

JS:   await Promise.all(tasks)
来源：http://hz.jlsjyb.cn/gtugynsmsn.html

TS:   await Promise.all(tasks)
来源：http://hz.yuanzhike.top/gtetnctkuy.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.nanxuanxn.top/gtrtqyuqib.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.hnxiangtu.top/gtnwygqhjt.html

Ruby: threads.map(&:join)
来源：http://hz.xuetiantiany.cn/gtimybfami.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.jinghuilouyu.cn/gtpinzjbvs.html

[O06] 使用进程池
来源：http://hz.feifeiyinyue.top/gtaatkwouc.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.mhx1999.top/gtcikyyhge.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.cashguo.top/gtyjuhlull.html

JS:   // child_process / cluster 模块
来源：http://hz.ppjwa.cn/gtbpurohlc.html

TS:   // child_process / cluster 模块
来源：http://hz.dianchejie.cn/gtiwqovcsa.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.aibaodan.cn/gtyqoycoyo.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.iojbl.cn/gtxewxzhwc.html

Ruby: // fork 块
来源：http://hz.ppjwa.cn/gtorijrcpx.html

C#:   Parallel.For
来源：http://hz.0kj1m.cn/gtxofpjlpv.html

================================================================================
来源：http://hz.fzhhl.top/gtdtuwzlis.html

P. 常用工具函数
来源：http://hz.wangshuangyany.cn/gtlircyolf.html

================================================================================
来源：http://hz.chenzaomai.com/gtlrhhxdmh.html

[P01] 生成 UUID
来源：http://hz.xinyue.icu/gttnmwuuxo.html

Py:   str(uuid.uuid4())
来源：http://hz.jqgfzy.top/gtyagyokwr.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.shanyushiyangtech.top/gtoodjoyhq.html

JS:   crypto.randomUUID()
来源：http://hz.vqdsnc.cn/gtzprdrren.html

TS:   crypto.randomUUID()
来源：http://hz.zhengqikj.top/gtokrhmthp.html

Java: UUID.randomUUID().toString()
来源：http://hz.jinyuanbaomall.cn/gtjecxdmep.html

Go:   // 用 github.com/google/uuid
来源：http://hz.svipenyu.cn/gtojmhidxe.html

Ruby: SecureRandom.uuid
来源：http://hz.jinqigfzy.top/gtigonystg.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.hnxiangtu.top/gtxyaynvka.html

[P02] MD5 / SHA256 摘要
来源：http://hz.sysykeji.top/gtvqslhbpl.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.zhaomingkeji.xyz/gtleckqcvx.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.hywenlv.cn/gtfjbgtwlw.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.chenlongwang.top/gtxphrluea.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.chenjidiqi.icu/gtbplkvijo.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.fzhhl.top/gtksekqnjt.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.zhiwuduotai.top/gtcpqztgdt.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.svipenyu.cn/gtqbzkpblc.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.wangshuangyany.cn/gtotaotvcd.html

[P03] 生成短随机字符串
来源：http://hz.smart0.xyz/gtsdgrhely.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.shanyushiyangkeji.top/gtmzrhdfdg.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.hongshengwenyu.top/gtfqkagosp.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.9152youxi.cn/gtpekcbllk.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.meibo888.top/gtaegrwcjp.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.ivvv.top/gtdalkmsvd.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.shanyushiyangkeji.top/gtparbpxvj.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.ywan-chungtsiang.top/gtckqdppws.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.smart0.xyz/gtswyuoszs.html

[P04] 求长度
来源：http://hz.9152youxi.cn/gtckiccbib.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.svipenyu.cn/gtuhlnskzu.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.daria6918.cn/gtaekmyiew.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.guannengcc.top/gtcuiehsku.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.zhijiandao.cn/gtxqctmwrc.html

Java: list.size();  map.size();  s.length()
来源：http://hz.cqqwz.cn/gttlkhezau.html

Go:   len(arr);  len(m)
来源：http://hz.dianchejie.cn/gtwkjuvmql.html

Ruby: x.length;  x.size
来源：http://hz.zhengqikj.top/gtgjeazhrd.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.jqgufenzy.top/gtfprvwmsf.html

[P05] 判断两个对象内容是否相等
来源：http://hz.xuetiantiany.cn/gttprgfyuk.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.sweek.top/gtcsgvxhsk.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.ehwqpu.com/gtlveddczy.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.yonumen.top/gtdpwfynei.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.sweek.top/gtnndwddsw.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.jinqigufen.top/gtumdfkmhg.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.zycfv.cn/gtsqbdzinf.html

Ruby: a == b
来源：http://hz.9152youxi.cn/gtwjmbwbvw.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.cdnleiting.top/gtrmtyxrfv.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.cucudq.cn/gtnodtzgni.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.daxiang520.top/gtrfxussor.html

PHP:  if (empty($x)) {}
来源：http://hz.yuanzhike.top/gtfqbirwjs.html


<!-- 参考信息 -->