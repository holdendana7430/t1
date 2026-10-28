代发 wailian999

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.smart0.xyz/gtkibsssyk.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.zhiwuduotai.top/gtsxyeajvp.html

================================================================================
来源：http://hz.yuanzhike.top/gtnzdbxzhl.html

M. 命令行 / 进程 / 环境
来源：http://hz.ivvv.top/gtmvfacqne.html

================================================================================
来源：http://hz.yueranfly.top/gtbiztsezs.html

[M01] 读取命令行参数
来源：http://hz.sweek.top/gtxbaxcaul.html

Py:   sys.argv[1:]
来源：http://hz.yueranfly.top/gtojaovivr.html

PHP:  $argv;  $argc;
来源：http://hz.zhengqikj.top/gtxwxqavbl.html

JS:   process.argv.slice(2)
来源：http://hz.jinqigufen.top/gtiuomjsyi.html

TS:   process.argv.slice(2)
来源：http://hz.hysaishi.cn/gtadiznvfc.html

Java: args 数组（main 方法参数）
来源：http://hz.xylfe.cn/gtygrzqxcs.html

Go:   os.Args[1:]
来源：http://hz.jyoumei.cn/gtfpnoyjko.html

Ruby: ARGV
来源：http://hz.cucudq.cn/gttvidjwqw.html

C#:   args 数组（Main 方法参数）
来源：http://hz.ybcxt.top/gtqwcyrjby.html

[M02] 读取环境变量
来源：http://hz.xingfuxueyuan.xyz/gtmnxvkasq.html

Py:   os.environ.get("HOME")
来源：http://hz.0kj1m.cn/gtruboeyhk.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.chenjidiqi.icu/gttwnrenht.html

JS:   process.env.HOME
来源：http://hz.cashguo.top/gtkarrjzmy.html

TS:   process.env.HOME
来源：http://hz.sysykeji.top/gtvneatrnt.html

Java: System.getenv("HOME")
来源：http://hz.xylfe.cn/gtrofqxify.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.smart0.xyz/gtjygrcnhg.html

Ruby: ENV["HOME"]
来源：http://hz.jiagoushi.top/gtsenprrte.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.vqdsnc.cn/gtqenlprje.html

[M03] 执行外部命令
来源：http://hz.guannengcc.top/gtgplltkon.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.yuxming.cn/gtujgdipgi.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.guowangkeji.top/gtusjimlhv.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.vqdsnc.cn/gtebqsisxb.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.cqqwz.cn/gtfwxnkebj.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.guowangkeji.top/gtwsabkpgj.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.jqgfzy.top/gtjetmzbqu.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.xuanzx.com/gtxpevaeda.html

C#:   Process.Start("ls", "-l");
来源：http://hz.316326.xyz/gtqqzmzvww.html

[M04] 获取当前工作目录
来源：http://hz.52xcode.cn/gtjwzftjhr.html

Py:   os.getcwd()
来源：http://hz.chenjidiqi.icu/gtrkncetpr.html

PHP:  getcwd();
来源：http://hz.gogol.net.cn/gtynrhyttb.html

JS:   process.cwd()
来源：http://hz.0kj1m.cn/gtimobqmjc.html

TS:   process.cwd()
来源：http://hz.snrcjt.cn/gtvrpkcnqe.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.guannengcc.top/gtzfmktogh.html

Go:   os.Getwd()
来源：http://hz.redwolf501.top/gtawthwzus.html

Ruby: Dir.pwd
来源：http://hz.jinyuanbaomall.cn/gtreemmhnr.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.fzhhl.top/gtqgtpjejl.html

[M05] 设置退出码
来源：http://hz.iojbl.cn/gtivoewnqe.html

Py:   sys.exit(1)
来源：http://hz.zhengqikj.top/gtyntxulch.html

PHP:  exit(1);
来源：http://hz.xinyue.icu/gtvsbrheup.html

JS:   process.exit(1)
来源：http://hz.yj20258.top/gtcowgwhjl.html

TS:   process.exit(1)
来源：http://hz.ywan-chungtsiang.top/gtsutejagj.html

Java: System.exit(1)
来源：http://hz.daria6918.cn/gthwstkxyz.html

Go:   os.Exit(1)
来源：http://hz.sxryk.cn/gtlgyoirnz.html

Ruby: exit 1
来源：http://hz.ehwqpu.com/gtzanjhsnc.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.bjfxy.top/gtzmdugmtb.html

[M06] 向标准错误输出
来源：http://hz.shuidangran.top/gtiqvgfkec.html

Py:   print("err", file=sys.stderr)
来源：http://hz.kuanghao11.cn/gtgfqwtjda.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.zhijiandao.cn/gtpkjmwbet.html

JS:   console.error("err")
来源：http://hz.gotoacloud.top/gtufagxfnp.html

TS:   console.error("err")
来源：http://hz.jinqigfzy.top/gtdrkakflr.html

Java: System.err.println("err")
来源：http://hz.mhx1999.top/gtuwmqbblu.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.c1oappe.top/gtrwiobqpw.html

Ruby: warn "err"
来源：http://hz.zycfv.cn/gtorthcmcp.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.dianchejie.cn/gtqqzgpgdn.html

[M07] 判断是否为主入口
来源：http://hz.xingfuxueyuan.xyz/gtuearjbrs.html

Py:   if __name__ == "__main__":
来源：http://hz.redwolf501.top/gtvlnfvjbz.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.tanke756.top/gtsbmeovfg.html

JS:   require.main === module
来源：http://hz.daxiang520.top/gteptxppee.html

TS:   require.main === module
来源：http://hz.smart0.xyz/gtkwjfgknj.html

Java: public static void main(String[] args)
来源：http://hz.xylfe.cn/gtrkmkejie.html

Go:   func main()
来源：http://hz.jiagoushi.top/gtsptujkkn.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.jinyuanbaomall.cn/gtdshtrrjn.html

C#:   static void Main(string[] args)
来源：http://hz.zhongyouzk.top/gtnwmmkryr.html

[M08] 获取系统与运行时信息
来源：http://hz.jianghu66.top/gtzetdvgtd.html

Py:   platform.system();  platform.python_version()
来源：http://hz.jyoumei.cn/gtprjxyceq.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.jqgufenzy.top/gtxayytocx.html

JS:   process.platform;  process.version
来源：http://hz.gaohongyu789.top/gtpkdojtdm.html

TS:   process.platform;  process.version
来源：http://hz.shanyushiyangtech.top/gtmkpyzkcj.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.xziqi.cn/gtswrkmeqv.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.sweek.top/gteqlmgges.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.jiagoushi.top/gtvugwemne.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.shzxlz.cn/gtgfprkntp.html

================================================================================
来源：http://hz.xziqi.cn/gtsnehdwif.html

N. 数据结构与算法
来源：http://hz.shzxlz.cn/gtrinrlffz.html

================================================================================
来源：http://hz.guowangkeji.top/gtfxjhqnys.html

[N01] 二分查找（有序数组）
来源：http://hz.jinqigufen.top/gtnvsyqatt.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.xylfe.cn/gtlwmskizw.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.ydzc1.top/gtbemltcej.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.chenjidiqi.icu/gtmiwjwylf.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.c1oappe.top/gtgahjoxtr.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.wangshuangyany.cn/gtljmjsuyc.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.c1oappe.top/gtcluhvgcg.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.xuetiantiany.cn/gtomwvzyrt.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.gaohongyu789.top/gtxwukfnlq.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.chenjidiqi.icu/gtbloorkyh.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.gaohongyu789.top/gtdvtrojoe.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.chenlongwang.top/gtuzqpeinu.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.wangshuangyany.cn/gtlkgvefne.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.guowangkeji.top/gtzkkcvvqm.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.shanyushiyangkeji.top/gteeqrgfzt.html

Go:   slices.Sort(arr)
来源：http://hz.xylfe.cn/gteglshkvh.html

Ruby: arr.sort
来源：http://hz.ydzc1.top/gtybscscec.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.ppjwa.cn/gtsjxuxhhu.html

[N03] 快速排序（分治示例）
来源：http://hz.nwbrower.top/gtnhriqszi.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.sweek.top/gtaadxnrmr.html

PHP:  // 递归实现，或用 usort
来源：http://hz.sysykeji.top/gtfvtqnivm.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.9152youxi.cn/gttgebsanm.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.cdnleiting.top/gtliiebxjy.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.tanke756.top/gtvxxhjpwb.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.zhijiandao.cn/gthvgbobnw.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.daxiang520.top/gtkvqarfdf.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.andypj.xyz/gtwaxibqne.html

[N04] 斐波那契数列
来源：http://hz.bjfxy.top/gttkukancq.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.daria6918.cn/gtwtlijvwe.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.sufxvd.cn/gtdxgzdjro.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.aibaodan.cn/gtijuttddr.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.pycfn.com/gtnyqzansb.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.tanke756.top/gtphatflkq.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.zhaomingkeji.xyz/gtxqhlncvm.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.chenzaomai.com/gtfxjkdxox.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.ydjk.org.cn/gtnqrcuhnh.html

[N05] 最大公约数
来源：http://hz.fzhhl.top/gtshxbqdvw.html

Py:   math.gcd(a, b)
来源：http://hz.hysaishi.cn/gtrzsjddmc.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.chenlongwang.top/gtzeeohhkb.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.gaohongyu789.top/gtsaeynyvp.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.mhx1999.top/gtoikujygc.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.yonumen.top/gtvtiyfdkw.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.quarkkingdee.top/gtngtlzhzk.html

Ruby: a.gcd(b)
来源：http://hz.tanke756.top/gtpxkglrby.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.yongpay.top/gtxwehxevt.html

[N06] 判断回文字符串
来源：http://hz.smart0.xyz/gtjwyuiwnv.html

Py:   s == s[::-1]
来源：http://hz.yuxming.cn/gtqlhjrfog.html

PHP:  $s === strrev($s);
来源：http://hz.hysaishi.cn/gttezmthtl.html

JS:   s === [...s].reverse().join("")
来源：http://hz.pycfn.com/gtmaaiohij.html

TS:   s === [...s].reverse().join("")
来源：http://hz.andypj.xyz/gtxkmfbsvo.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.zhongyouzk.top/gtcoooqvmw.html

Go:   // 双指针从两端比较
来源：http://hz.9152youxi.cn/gtgzjstnoc.html

Ruby: s == s.reverse
来源：http://hz.redwolf501.top/gtgvryvzrx.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.zhijiandao.cn/gtnmzjxgke.html

[N07] 两数之和（返回下标）
来源：http://hz.nwbrower.top/gtmnultiqz.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.smart0.xyz/gttoumjslk.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.feifeiyinyue.top/gttnzperao.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.snrcjt.cn/gtgufgpdod.html

TS:   // 手写 Map<string, number>
来源：http://hz.vqdsnc.cn/gtudcuclyg.html

Java: // 手写 HashMap
来源：http://hz.yongpay.top/gtjfdplanc.html

Go:   // 手写 map[int]int
来源：http://hz.yangfankeji.com/gthmorvjqw.html

Ruby: // 手写 Hash
来源：http://hz.shanyushiyangtech.top/gtnsmjalcd.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.shanyushiyangkeji.top/gtzckosqwc.html

[N08] 生成全排列
来源：http://hz.svipenyu.cn/gthmzhpjgh.html

Py:   itertools.permutations(arr)
来源：http://hz.snrcjt.cn/gtkscohpxm.html

PHP:  // 手写递归交换
来源：http://hz.zhoulong.xyz/gtumeghemy.html

JS:   // 手写回溯递归
来源：http://hz.yj20258888.top/gtcluzohhp.html

TS:   // 手写回溯递归
来源：http://hz.tianlin.xyz/gtgvvhjewt.html

Java: // 手写回溯递归
来源：http://hz.zhoulong.xyz/gtbxprctst.html

Go:   // 手写回溯递归
来源：http://hz.yuxming.cn/gtsanbiwre.html

Ruby: arr.permutation.to_a
来源：http://hz.yj202588.top/gtsnpbbmub.html

C#:   // 手写回溯递归
来源：http://hz.aibaodan.cn/gtqdibfeqp.html

[N09] 栈与队列
来源：http://hz.yj202588.top/gtnurwujxi.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.jianghu66.top/gtmwatyitv.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.ybcxt.top/gtelalaoqj.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.yj20258.top/gtagwfrrtx.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.cucudq.cn/gtcjcukrjg.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.tanke756.top/gtysxekezl.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.hnqzz.top/gtsvbwntjt.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.ehwqpu.com/gtvqjdbuxf.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.gaohongyu789.top/gtvdmxblpg.html

[N10] 链表节点定义
来源：http://hz.jianghu66.top/gthcjjifgn.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.jinqigfzy.top/gtyfctmxro.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.mhx1999.top/gtxekqubgm.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.xuetiantiany.cn/gtrdecupgm.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.gzhubu.top/gtfhrwvaqv.html

Java: class Node { int v; Node next; }
来源：http://hz.mhx1999.top/gtvbazxaxe.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.snrcjt.cn/gtsqxumlzc.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.sysykeji.top/gtrxxposrk.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.316326.xyz/gtujexpxxj.html

[N11] 二叉树中序遍历
来源：http://hz.shanyushiyangtech.top/gtvlhpsssg.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.chenlongwang.top/gtuebumder.html

PHP:  // 手写递归函数
来源：http://hz.guowangkeji.top/gthglgxihg.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.0kj1m.cn/gtcxzslmmg.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.jianghu66.top/gtmsdzpzrw.html

Java: // 手写递归
来源：http://hz.xinyue.icu/gtcnraxuix.html

Go:   // 手写递归
来源：http://hz.jinghuilouyu.cn/gtqrkdyput.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.cqqwz.cn/gtzsaoovbo.html

C#:   // 手写递归
来源：http://hz.cdnleiting.top/gtmieutvbs.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.jinqigufen.top/gtvbvfiykg.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.mhx1999.top/gtkbpigzkl.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.cucudq.cn/gtmgzxomfl.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.jyoumei.cn/gtlqqpyjqi.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.iojbl.cn/gtvfslmpfq.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.snrcjt.cn/gtmpmjgiul.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.ydzc1.top/gtntpvrwax.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.jiagoushi.top/gttjbfzsqr.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.guowangkeji.top/gtcttantjr.html

================================================================================
来源：http://hz.yueranfly.top/gthjxxkwhe.html

O. 并发与异步
来源：http://hz.mhx1999.top/gtyosekjaq.html

================================================================================
来源：http://hz.aibaodan.cn/gtiwihcvrt.html

[O01] 启动一个线程
来源：http://hz.sweek.top/gtyegzwgky.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.gaohongyu789.top/gtygvwncak.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.c1oappe.top/gtvspcnwff.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.chenlongwang.top/gtatsefxuf.html

TS:   // 同 JS
来源：http://hz.ehwqpu.com/gtaysgrrcj.html

Java: new Thread(() -> f()).start()
来源：http://hz.chenzaomai.com/gtrfdgnjsq.html

Go:   go f()
来源：http://hz.aibaodan.cn/gtmqavzuzy.html

Ruby: Thread.new { f }
来源：http://hz.snrcjt.cn/gtomnighlw.html

C#:   Task.Run(() => F());
来源：http://hz.yonumen.top/gtkiusroca.html

[O02] 使用线程池
来源：http://hz.nanxinkj.top/gtboqnfzvb.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.shangyingyoupin.top/gtzhrslgoz.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.xingfuxueyuan.xyz/gtzdwxkseg.html

JS:   // worker_threads 线程池
来源：http://hz.snrcjt.cn/gtxtgalyzs.html

TS:   // worker_threads 线程池
来源：http://hz.gaohongyu789.top/gtuzukjwye.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.yangfankeji.com/gtwzwfudwy.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.cheryme.top/gtwkerdmyq.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.sxryk.cn/gtaduhtjxp.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.ybcxt.top/gttvigajck.html

[O03] 加锁保护共享数据
来源：http://hz.xinyue.icu/gthiaopezq.html

Py:   with lock: shared += 1
来源：http://hz.gotoacloud.top/gtltkeconw.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.316326.xyz/gtirqawrcs.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.sxryk.cn/gtzloaczyg.html

TS:   // 同 JS
来源：http://hz.ybcxt.top/gtiryqusjd.html

Java: synchronized (this) { shared++; }
来源：http://hz.ybcxt.top/gtgmoupgyt.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.wangshuangyany.cn/gtdhkngkfm.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.9152youxi.cn/gttaoaqyet.html

C#:   lock (gate) { shared++; }
来源：http://hz.haohaochexian.top/gtnzrxounl.html

[O04] 定义异步函数并等待
来源：http://hz.gzhubu.top/gtqoukmknw.html

Py:   async def f():⏎    await g()
来源：http://hz.cdnleiting.top/gtrwsiosrp.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.yonumen.top/gtncswzwuv.html

JS:   async function f() { await g(); }
来源：http://hz.xinyue.icu/gtdxgrhorl.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.shuidangran.top/gtuqhnueot.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.sufxvd.cn/gtrtopqghz.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.zhoulong.xyz/gtjoezlyrr.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.yangfankeji.com/gtdolxvyfg.html

C#:   async Task F() { await G(); }
来源：http://hz.vqdsnc.cn/gtvssemvsc.html

[O05] 并发执行并等待全部完成
来源：http://hz.feifeiyinyue.top/gtzkfvggnx.html

Py:   asyncio.gather(*tasks)
来源：http://hz.haohaochexian.top/gtzscksnhx.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.zhiwuduotai.top/gtkfkolasl.html

JS:   await Promise.all(tasks)
来源：http://hz.jqgfzy.top/gtezqurglv.html

TS:   await Promise.all(tasks)
来源：http://hz.feifeiyinyue.top/gtulvslsfn.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.ppjwa.cn/gttprlkpmt.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.zycfv.cn/gtvrvaysqo.html

Ruby: threads.map(&:join)
来源：http://hz.xuanzx.com/gtwzwotbvm.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.xuanzx.com/gtavapccch.html

[O06] 使用进程池
来源：http://hz.guowangkeji.top/gtlnpxypfy.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.ybcxt.top/gtdacxshjb.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.shzxlz.cn/gtcakkjgwr.html

JS:   // child_process / cluster 模块
来源：http://hz.hnqzz.top/gttrfolsdj.html

TS:   // child_process / cluster 模块
来源：http://hz.xziqi.cn/gtxzwkndty.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.jiagoushi.top/gthtxmnhml.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.haohaochexian.top/gtgkpzavyk.html

Ruby: // fork 块
来源：http://hz.guannengcc.top/gtpktstfcy.html

C#:   Parallel.For
来源：http://hz.jinqigufen.top/gtfwytescy.html

================================================================================
来源：http://hz.hnxiangtu.top/gtxenwdvuk.html

P. 常用工具函数
来源：http://hz.zhengqikj.top/gtevfvwacd.html

================================================================================
来源：http://hz.bjfxy.top/gtxbbciuds.html

[P01] 生成 UUID
来源：http://hz.vqdsnc.cn/gtlyjbnurd.html

Py:   str(uuid.uuid4())
来源：http://hz.redwolf501.top/gtbfpeatdl.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.yangfankeji.com/gtojxsvfrm.html

JS:   crypto.randomUUID()
来源：http://hz.cashguo.top/gtumiwfmjt.html

TS:   crypto.randomUUID()
来源：http://hz.jqgfzy.top/gtqpjazezr.html

Java: UUID.randomUUID().toString()
来源：http://hz.cashguo.top/gtiitslijp.html

Go:   // 用 github.com/google/uuid
来源：http://hz.nwbrower.top/gtjwerrhem.html

Ruby: SecureRandom.uuid
来源：http://hz.vqdsnc.cn/gtskuufczs.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.chenlongwang.top/gtyrbeejrw.html

[P02] MD5 / SHA256 摘要
来源：http://hz.hnqzz.top/gtebcmeugz.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.meibo888.top/gtoszcccqi.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.c1oappe.top/gtomrqaaiy.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.hammf.cn/gtecxmvzta.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.sysykeji.top/gtqbdgkiwf.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.tanke756.top/gtudqcpavt.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.xuetiantiany.cn/gtvntviyyz.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.tianlin.xyz/gtbgnnkwll.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.dashuyun.cn/gtlxiypxcm.html

[P03] 生成短随机字符串
来源：http://hz.chenlongwang.top/gtdlklhhne.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.jyoumei.cn/gtcrxupfgm.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.shanyushiyangkeji.top/gtwfzkusba.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.jinqigufen.top/gtdiqmhfml.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.zhijiandao.cn/gtjcoknqdd.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.hywenlv.cn/gtsrhxhbbl.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.cucudq.cn/gtwdsqbieh.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.guannengcc.top/gtkafyjiph.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.snrcjt.cn/gtcgnvgnju.html

[P04] 求长度
来源：http://hz.birdmap.top/gteaifcerv.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.fengsongda.top/gthixwkmyl.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.cdnleiting.top/gtlnpieoff.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.wangshuangyany.cn/gtwmwcbbye.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.chenlongwang.top/gthgbjjshk.html

Java: list.size();  map.size();  s.length()
来源：http://hz.daria6918.cn/gtitpxklpf.html

Go:   len(arr);  len(m)
来源：http://hz.tanke756.top/gtmpgaxcqi.html

Ruby: x.length;  x.size
来源：http://hz.smart0.xyz/gtmhcnjptm.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.hfpthk.cn/gtxgfavnou.html

[P05] 判断两个对象内容是否相等
来源：http://hz.zhiwuduotai.top/gtauvulzfo.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.birdmap.top/gtyyyfggur.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.ywan-chungtsiang.top/gttfdirjtk.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.ybcxt.top/gtbgdsblxq.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.daria6918.cn/gtvijynsab.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.xylfe.cn/gtilmkowxo.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.ybcxt.top/gtrpmsqsre.html

Ruby: a == b
来源：http://hz.cheryme.top/gtopztqzyu.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.cashguo.top/gtjrajgfzr.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.yueranfly.top/gtpzrwnsxi.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.jinyuanbaomall.cn/gtwktgtuzr.html

PHP:  if (empty($x)) {}
来源：http://hz.sweek.top/gtmaxaqybr.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.cqqwz.cn/gtbozjuqox.html

TS:   if (x == null) {}
来源：http://hz.dashuyun.cn/gtktjjunvp.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.jinyuanbaomall.cn/gtvvzattve.html

Go:   if x == nil {}
来源：http://hz.hfpthk.cn/gtegabzdoj.html


<!-- 参考信息 -->