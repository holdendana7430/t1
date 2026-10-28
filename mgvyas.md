代发 wailian999

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.cdnleiting.top/gtfjxntxwl.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.feifeiyinyue.top/gtxquskhdl.html

================================================================================
来源：http://hz.jqgfzy.top/gtrzvhuzmc.html

M. 命令行 / 进程 / 环境
来源：http://hz.zycfv.cn/gtolnvzvcw.html

================================================================================
来源：http://hz.shzxlz.cn/gtgnebcrcd.html

[M01] 读取命令行参数
来源：http://hz.yueranfly.top/gtftnyrzoc.html

Py:   sys.argv[1:]
来源：http://hz.jlsjyb.cn/gtfonhmbkn.html

PHP:  $argv;  $argc;
来源：http://hz.hysaishi.cn/gtmkdfjanm.html

JS:   process.argv.slice(2)
来源：http://hz.sweek.top/gtqaqvvles.html

TS:   process.argv.slice(2)
来源：http://hz.yonumen.top/gtfppuphxx.html

Java: args 数组（main 方法参数）
来源：http://hz.xuanzx.com/gtlcodomwt.html

Go:   os.Args[1:]
来源：http://hz.fengsongda.top/gtkbmhffsg.html

Ruby: ARGV
来源：http://hz.yj202588.top/gtydaafuzv.html

C#:   args 数组（Main 方法参数）
来源：http://hz.wangshuangyany.cn/gtudodsnuk.html

[M02] 读取环境变量
来源：http://hz.shzxlz.cn/gteokmlukm.html

Py:   os.environ.get("HOME")
来源：http://hz.hnxiangtu.top/gtyxelraky.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.chenlongwang.top/gtsgohmpqg.html

JS:   process.env.HOME
来源：http://hz.sweek.top/gtlgrsebvc.html

TS:   process.env.HOME
来源：http://hz.ehwqpu.com/gthnqyedxe.html

Java: System.getenv("HOME")
来源：http://hz.9152youxi.cn/gtemjrntaf.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.pengpengdd.cyou/gtieexeqqj.html

Ruby: ENV["HOME"]
来源：http://hz.hywenlv.cn/gtbnrmixag.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.zhaomingkeji.xyz/gtdfrfspzb.html

[M03] 执行外部命令
来源：http://hz.birdmap.top/gttqkybrpi.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.shuidangran.top/gtzxinqfvd.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.nanxuanxn.top/gtidcfwwhf.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.dashuyun.cn/gtqxdoiguc.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.aibaodan.cn/gtarpopzwk.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.xuanzx.com/gtiecleniy.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.chenjidiqi.icu/gtrvpminxl.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.hnxiangtu.top/gtkavditqv.html

C#:   Process.Start("ls", "-l");
来源：http://hz.0kj1m.cn/gtwlbezzec.html

[M04] 获取当前工作目录
来源：http://hz.yongpay.top/gtwflhclhk.html

Py:   os.getcwd()
来源：http://hz.pengpengdd.cyou/gtdyqrkrnp.html

PHP:  getcwd();
来源：http://hz.jqgufenzy.top/gtadieeoty.html

JS:   process.cwd()
来源：http://hz.quarkkingdee.top/gtrdbjkgso.html

TS:   process.cwd()
来源：http://hz.smart0.xyz/gtjaerjjrr.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.jinghuilouyu.cn/gtavxxikkg.html

Go:   os.Getwd()
来源：http://hz.xuetiantiany.cn/gtpdcszqtd.html

Ruby: Dir.pwd
来源：http://hz.ybcxt.top/gtwypjdwcd.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.birdmap.top/gtyazxofkt.html

[M05] 设置退出码
来源：http://hz.guannengcc.top/gttswyonbr.html

Py:   sys.exit(1)
来源：http://hz.havefunace.top/gtavbxugmp.html

PHP:  exit(1);
来源：http://hz.gaohongyu789.top/gtfowoijwz.html

JS:   process.exit(1)
来源：http://hz.hfpthk.cn/gtlyrotxhk.html

TS:   process.exit(1)
来源：http://hz.yonumen.top/gtqjdswcpg.html

Java: System.exit(1)
来源：http://hz.yueranfly.top/gtkrpibtdc.html

Go:   os.Exit(1)
来源：http://hz.hammf.cn/gtwqtgisvz.html

Ruby: exit 1
来源：http://hz.sysykeji.top/gtvvsjgrgn.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.ybcxt.top/gtgttkbzcy.html

[M06] 向标准错误输出
来源：http://hz.hongshengwenyu.top/gteoytlfhd.html

Py:   print("err", file=sys.stderr)
来源：http://hz.9152youxi.cn/gtytyxacgj.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.yvedp.cn/gtdaxnbxvk.html

JS:   console.error("err")
来源：http://hz.jiagoushi.top/gtrjudvcxc.html

TS:   console.error("err")
来源：http://hz.gaohongyu789.top/gtqbmacwmi.html

Java: System.err.println("err")
来源：http://hz.zhaomingkeji.xyz/gtkpifsjbc.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.havefunace.top/gtnwqqodsc.html

Ruby: warn "err"
来源：http://hz.nanxinkj.top/gthwqlralh.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.aibaodan.cn/gtuphypagz.html

[M07] 判断是否为主入口
来源：http://hz.yuanzhike.top/gtlxakrqzy.html

Py:   if __name__ == "__main__":
来源：http://hz.ydjk.org.cn/gtpxntzmvn.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.0kj1m.cn/gtlebmulhd.html

JS:   require.main === module
来源：http://hz.0kj1m.cn/gtdrvwntzz.html

TS:   require.main === module
来源：http://hz.yanxiufei.cn/gtxsiqocep.html

Java: public static void main(String[] args)
来源：http://hz.yuanzhike.top/gtvpptqhpr.html

Go:   func main()
来源：http://hz.hnxiangtu.top/gtjtmshthk.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.yuanzhike.top/gtwphvkruk.html

C#:   static void Main(string[] args)
来源：http://hz.0kj1m.cn/gtfkqwipbb.html

[M08] 获取系统与运行时信息
来源：http://hz.meibo888.top/gtwmdybbjs.html

Py:   platform.system();  platform.python_version()
来源：http://hz.feifeiyinyue.top/gtovlygoqf.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.zhixingplan.top/gtpsxrddij.html

JS:   process.platform;  process.version
来源：http://hz.yangfankeji.com/gtmbcwiozw.html

TS:   process.platform;  process.version
来源：http://hz.sxryk.cn/gtkethwpvt.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.havefunace.top/gtzsqpggag.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.jlsjyb.cn/gtcfwxkxsx.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.nanxuanxn.top/gtchyhakib.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.snrcjt.cn/gtxshiuqja.html

================================================================================
来源：http://hz.snrcjt.cn/gtmozituzk.html

N. 数据结构与算法
来源：http://hz.smart0.xyz/gtsrhujukv.html

================================================================================
来源：http://hz.nwbrower.top/gtnvhfgtnm.html

[N01] 二分查找（有序数组）
来源：http://hz.ywan-chungtsiang.top/gtrbqqiikr.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.nwbrower.top/gtybtqfaqf.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.ybcxt.top/gtmzrcscau.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.jinqigufen.top/gtcqkjwmkk.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.chenlongwang.top/gtsvubrlhw.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.ehwqpu.com/gtvuugohoo.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.0kj1m.cn/gtvydtqbuk.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.yuanzhike.top/gtminolxhx.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.ydjk.org.cn/gthvttkjhz.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.ivvv.top/gtybwqblqm.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.cqqwz.cn/gtauoexkwk.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.redwolf501.top/gtykyotmjs.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.hnqzz.top/gtkbzxnpbk.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.svipenyu.cn/gtbrjakses.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.hnxiangtu.top/gtwmbcnvhl.html

Go:   slices.Sort(arr)
来源：http://hz.jqgufenzy.top/gtlyakharu.html

Ruby: arr.sort
来源：http://hz.xziqi.cn/gtrnpdqich.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.hysaishi.cn/gtgnsikyjl.html

[N03] 快速排序（分治示例）
来源：http://hz.nwbrower.top/gtsfgbtnit.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.nanxuanxn.top/gtgnygrwjw.html

PHP:  // 递归实现，或用 usort
来源：http://hz.havefunace.top/gtcmmazaxv.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.yj20258888.top/gtdqulyowa.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.redwolf501.top/gtuuyjhicn.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.xziqi.cn/gtqpyeictc.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.hywenlv.cn/gtqhazslxd.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.ywan-chungtsiang.top/gtehfxomfk.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.xziqi.cn/gtganxvgqj.html

[N04] 斐波那契数列
来源：http://hz.cqqwz.cn/gtqkojbsfy.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.fengsongda.top/gtwxvyzscb.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.cucudq.cn/gtfbmkvlef.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.jinqigufen.top/gtillqvzib.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.cucudq.cn/gtuozrsnue.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.xuanzx.com/gtitorrbhl.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.ehwqpu.com/gtbtksnepx.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.ywan-chungtsiang.top/gtabkzoaur.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.nanxuanxn.top/gtfynbgnqy.html

[N05] 最大公约数
来源：http://hz.wangdashe.top/gtokfgahfq.html

Py:   math.gcd(a, b)
来源：http://hz.yuxming.cn/gtkpyfjujp.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.hnqzz.top/gtvwlmofnr.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.yj20258.top/gtajsnbjnc.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.ehwqpu.com/gtztbscudd.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.shzxlz.cn/gtzrkuyciy.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.c1oappe.top/gttqicwurn.html

Ruby: a.gcd(b)
来源：http://hz.nwbrower.top/gtihcbanxn.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.xinyue.icu/gtmeendwhx.html

[N06] 判断回文字符串
来源：http://hz.wangdashe.top/gtynoswkbh.html

Py:   s == s[::-1]
来源：http://hz.bjfxy.top/gtdkvwmfbz.html

PHP:  $s === strrev($s);
来源：http://hz.aibaodan.cn/gtabzuugwx.html

JS:   s === [...s].reverse().join("")
来源：http://hz.ivvv.top/gthglgaxdz.html

TS:   s === [...s].reverse().join("")
来源：http://hz.shuidangran.top/gtifjjqesb.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.zhiwuduotai.top/gtpuddebsf.html

Go:   // 双指针从两端比较
来源：http://hz.jinqigfzy.top/gtpcqiepyx.html

Ruby: s == s.reverse
来源：http://hz.svipenyu.cn/gtexmndzqx.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.yj202588.top/gtciadwjzd.html

[N07] 两数之和（返回下标）
来源：http://hz.mhx1999.top/gtrndmevqx.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.chenjidiqi.icu/gtfkisdzmb.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.xuanzx.com/gturwqggzn.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.jianghu66.top/gtmixkpytb.html

TS:   // 手写 Map<string, number>
来源：http://hz.tanke756.top/gtuzmvhewp.html

Java: // 手写 HashMap
来源：http://hz.jianghu66.top/gtpeuwqucu.html

Go:   // 手写 map[int]int
来源：http://hz.xziqi.cn/gtskxdwrty.html

Ruby: // 手写 Hash
来源：http://hz.hysaishi.cn/gtwsgihbjd.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.nanxuanxn.top/gttmbgjdcy.html

[N08] 生成全排列
来源：http://hz.xuetiantiany.cn/gtjbfpimqu.html

Py:   itertools.permutations(arr)
来源：http://hz.svipenyu.cn/gtfivjptcb.html

PHP:  // 手写递归交换
来源：http://hz.zhiwuduotai.top/gtubipbfyj.html

JS:   // 手写回溯递归
来源：http://hz.316326.xyz/gtybijzwli.html

TS:   // 手写回溯递归
来源：http://hz.yangfankeji.com/gttchpuiqz.html

Java: // 手写回溯递归
来源：http://hz.hywenlv.cn/gtosglyrvz.html

Go:   // 手写回溯递归
来源：http://hz.yongpay.top/gtupzwvoet.html

Ruby: arr.permutation.to_a
来源：http://hz.yj202588.top/gtdslepego.html

C#:   // 手写回溯递归
来源：http://hz.yj20258888.top/gtrhywgpud.html

[N09] 栈与队列
来源：http://hz.tian-w.cn/gtbfsahdaj.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.nanxuanxn.top/gtppbspfeg.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.cucudq.cn/gtiyrfbsry.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.xuanzx.com/gttafjbnfj.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.zhijiandao.cn/gtvrykybnl.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.jinqigufen.top/gttrkxaouh.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.xylfe.cn/gtdkgbdofu.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.c1oappe.top/gttfmcostz.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.aizwys.cn/gtwynidlwt.html

[N10] 链表节点定义
来源：http://hz.shanyushiyangkeji.top/gtipveskvq.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.ehwqpu.com/gtprwyqxtd.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.xuetiantiany.cn/gtzciwquno.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.cqqwz.cn/gtixmguxdz.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.zhiwuduotai.top/gtpaagmxpp.html

Java: class Node { int v; Node next; }
来源：http://hz.vqdsnc.cn/gtmjtxpwrs.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.jqgfzy.top/gtheozzmla.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.yuanzhike.top/gtrcukihvf.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.sxryk.cn/gtwrtamnwd.html

[N11] 二叉树中序遍历
来源：http://hz.cashguo.top/gtladanjyr.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.iojbl.cn/gtmkodkyxz.html

PHP:  // 手写递归函数
来源：http://hz.sxryk.cn/gtjfpzsxxf.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.svipenyu.cn/gtowcjxgfj.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.shanyushiyangkeji.top/gtnpqgdfvz.html

Java: // 手写递归
来源：http://hz.yongpay.top/gtaryqalbq.html

Go:   // 手写递归
来源：http://hz.jinyuanbaomall.cn/gtoigxmrqg.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.nwbrower.top/gtijxvdoto.html

C#:   // 手写递归
来源：http://hz.chenzaomai.com/gttcaakgpd.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.smart0.xyz/gtnkmwrpme.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.smart0.xyz/gtmhnjbzva.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.xylfe.cn/gtujvmbhla.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.smart0.xyz/gtqivcrntk.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.pycfn.com/gtrarydnds.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.dianchejie.cn/gtlvgurljk.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.smart0.xyz/gtcuymjjvh.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.quarkkingdee.top/gthdesyqpq.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.iojbl.cn/gtxcufriml.html

================================================================================
来源：http://hz.nwbrower.top/gtyfelfezo.html

O. 并发与异步
来源：http://hz.nanxuanxn.top/gtpqqkqike.html

================================================================================
来源：http://hz.9152youxi.cn/gtcaswxxbu.html

[O01] 启动一个线程
来源：http://hz.quarkkingdee.top/gtezdfcttp.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.yj20258.top/gthpiguckc.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.316326.xyz/gtlbvmgrox.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.cashguo.top/gtyviejjxh.html

TS:   // 同 JS
来源：http://hz.9152youxi.cn/gtliiechha.html

Java: new Thread(() -> f()).start()
来源：http://hz.aizwys.cn/gtwfpkfrvg.html

Go:   go f()
来源：http://hz.smart0.xyz/gtdycqdiit.html

Ruby: Thread.new { f }
来源：http://hz.fzhhl.top/gtnbyweidt.html

C#:   Task.Run(() => F());
来源：http://hz.gogol.net.cn/gtvcliwidi.html

[O02] 使用线程池
来源：http://hz.tian-w.cn/gtqvefvohb.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.bjfxy.top/gtdzoiqxdc.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.tian-w.cn/gtspbtzpkh.html

JS:   // worker_threads 线程池
来源：http://hz.zhaomingkeji.xyz/gtckxdxfha.html

TS:   // worker_threads 线程池
来源：http://hz.hnqzz.top/gtzdxpyjvp.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.zhijiandao.cn/gtjlrowfua.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.shanyushiyangkeji.top/gtsakpsloi.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.316326.xyz/gtoqtdnxax.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.yvedp.cn/gtrprqrijt.html

[O03] 加锁保护共享数据
来源：http://hz.ehwqpu.com/gtaxniuolm.html

Py:   with lock: shared += 1
来源：http://hz.haohaochexian.top/gtadfhsqph.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.sweek.top/gtwiwxvqsj.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.chenzaomai.com/gtkkkakuin.html

TS:   // 同 JS
来源：http://hz.hammf.cn/gtyxbacijh.html

Java: synchronized (this) { shared++; }
来源：http://hz.sufxvd.cn/gtzrldozio.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.gogol.net.cn/gtyegkfkbm.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.shanyushiyangtech.top/gtnmkitgrw.html

C#:   lock (gate) { shared++; }
来源：http://hz.zhaomingkeji.xyz/gtohenktbd.html

[O04] 定义异步函数并等待
来源：http://hz.shuidangran.top/gtubzoaybk.html

Py:   async def f():⏎    await g()
来源：http://hz.guowangkeji.top/gtmoffmsoy.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.xuetiantiany.cn/gthuaorrnz.html

JS:   async function f() { await g(); }
来源：http://hz.jianghu66.top/gtzhisohcr.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.cucudq.cn/gtzcodtfcx.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.yj202588.top/gtcemliats.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.9152youxi.cn/gtrlqtlpry.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.guowangkeji.top/gtvauvjrrm.html

C#:   async Task F() { await G(); }
来源：http://hz.haohaochexian.top/gtwjlbikdr.html

[O05] 并发执行并等待全部完成
来源：http://hz.sysykeji.top/gtiavxkogx.html

Py:   asyncio.gather(*tasks)
来源：http://hz.cashguo.top/gtgyutxojn.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.yuanzhike.top/gteqyqayxg.html

JS:   await Promise.all(tasks)
来源：http://hz.svipenyu.cn/gtvhtfowmw.html

TS:   await Promise.all(tasks)
来源：http://hz.chenjidiqi.icu/gtwbhcemij.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.feifeiyinyue.top/gtlmgxnzbk.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.fzhhl.top/gtlaxdkcuz.html

Ruby: threads.map(&:join)
来源：http://hz.hammf.cn/gthyqkaqau.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.cqqwz.cn/gtwvkanhyr.html

[O06] 使用进程池
来源：http://hz.yj20258.top/gtsburuhll.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.guannengcc.top/gtcswlxhzy.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.ppjwa.cn/gtvcbodeyk.html

JS:   // child_process / cluster 模块
来源：http://hz.sweek.top/gtovjdyoal.html

TS:   // child_process / cluster 模块
来源：http://hz.tianlin.xyz/gtdtqvhlxf.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.feifeiyinyue.top/gtarykxdwm.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.hywenlv.cn/gthafqpxre.html

Ruby: // fork 块
来源：http://hz.0kj1m.cn/gtvafnsriz.html

C#:   Parallel.For
来源：http://hz.c1oappe.top/gthisxpkkz.html

================================================================================
来源：http://hz.sweek.top/gtdtnsvykf.html

P. 常用工具函数
来源：http://hz.hammf.cn/gtisseieof.html

================================================================================
来源：http://hz.yuanzhike.top/gtlynxjtdm.html

[P01] 生成 UUID
来源：http://hz.xylfe.cn/gtikwxlfwo.html

Py:   str(uuid.uuid4())
来源：http://hz.svipenyu.cn/gtdagiopbd.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.jinqigfzy.top/gtzylrfuri.html

JS:   crypto.randomUUID()
来源：http://hz.gotoacloud.top/gtmlmpqrlr.html

TS:   crypto.randomUUID()
来源：http://hz.snrcjt.cn/gtjaqfuwho.html

Java: UUID.randomUUID().toString()
来源：http://hz.meibo888.top/gttwgaljdy.html

Go:   // 用 github.com/google/uuid
来源：http://hz.feifeiyinyue.top/gtzvlpmfce.html

Ruby: SecureRandom.uuid
来源：http://hz.pengpengdd.cyou/gtcrkohomw.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.meibo888.top/gtpobdtujk.html

[P02] MD5 / SHA256 摘要
来源：http://hz.chenjidiqi.icu/gtismmjjcz.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.chenjidiqi.icu/gtcdddhkxo.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.tianlin.xyz/gtgpzwbbvd.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.zhiwuduotai.top/gtqwjplnlu.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.chenlongwang.top/gthuoxezqt.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.shanyushiyangkeji.top/gtmisfstnq.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.dianchejie.cn/gtkxpcevth.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.hammf.cn/gtbcsupker.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.hammf.cn/gtvvffzhlq.html

[P03] 生成短随机字符串
来源：http://hz.sxryk.cn/gtxwlkhpef.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.tanke756.top/gtptrisuxx.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.haohaochexian.top/gtnjedgnve.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.yj202588.top/gtctnbuvvj.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.gogol.net.cn/gtymfzhphg.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.haohaochexian.top/gtcueenqop.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.yueranfly.top/gttbbqaqya.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.gaohongyu789.top/gtpudkbpce.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.aizwys.cn/gtqspumjhp.html

[P04] 求长度
来源：http://hz.zhiwuduotai.top/gtgnjxzmky.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.kuanghao11.cn/gtcsrwknen.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.gogol.net.cn/gtopihhiey.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.fengsongda.top/gtkhurphny.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.haohaochexian.top/gtqcieliec.html

Java: list.size();  map.size();  s.length()
来源：http://hz.jinqigufen.top/gtzruzhmzn.html

Go:   len(arr);  len(m)
来源：http://hz.yj20258888.top/gtzkmqybmn.html

Ruby: x.length;  x.size
来源：http://hz.0kj1m.cn/gtzihfaahe.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.tanke756.top/gtsvzvnvrx.html

[P05] 判断两个对象内容是否相等
来源：http://hz.guannengcc.top/gtxfxperzk.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.jinghuilouyu.cn/gthwrqvrhn.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.jinghuilouyu.cn/gtbizzevxu.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.sweek.top/gtjezgxnpi.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.andypj.xyz/gtbjrjsihw.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.jqgfzy.top/gtewutztqv.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.daxiang520.top/gtfqrptlms.html

Ruby: a == b
来源：http://hz.hysaishi.cn/gtxjkryfwv.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.nwbrower.top/gtihmglkmq.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.chenlongwang.top/gtivipowdb.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.zhaomingkeji.xyz/gtgugcwyjo.html

PHP:  if (empty($x)) {}
来源：http://hz.snrcjt.cn/gtfdswdxov.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.zdqjudy.top/gtncdlzfun.html

TS:   if (x == null) {}
来源：http://hz.andypj.xyz/gtbnzapwhu.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.dashuyun.cn/gtwoyqkoyq.html

Go:   if x == nil {}
来源：http://hz.xinyue.icu/gttdbobljl.html


<!-- 参考信息 -->