代发 wailian999

JS:   process.argv.slice(2)
来源：http://hz.zhengqikj.top/gtdqpjcjoz.html

TS:   process.argv.slice(2)
来源：http://hz.xuetiantiany.cn/gtnkpvqeuu.html

Java: args 数组（main 方法参数）
来源：http://hz.9152youxi.cn/gtclmkfqgs.html

Go:   os.Args[1:]
来源：http://hz.redwolf501.top/gtcuabjepl.html

Ruby: ARGV
来源：http://hz.zhongyouzk.top/gtnlbccchr.html

C#:   args 数组（Main 方法参数）
来源：http://hz.gaohongyu789.top/gtmmfkxyfs.html

[M02] 读取环境变量
来源：http://hz.daxiang520.top/gtauehueon.html

Py:   os.environ.get("HOME")
来源：http://hz.chenjidiqi.icu/gtexqljmyc.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.cqqwz.cn/gtdzuklpqv.html

JS:   process.env.HOME
来源：http://hz.jqgfzy.top/gtqvwzfybu.html

TS:   process.env.HOME
来源：http://hz.pycfn.com/gtamejmfbt.html

Java: System.getenv("HOME")
来源：http://hz.zhengqikj.top/gtbfuooqfc.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.hywenlv.cn/gtpgxjcxyv.html

Ruby: ENV["HOME"]
来源：http://hz.sweek.top/gtduexndgr.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.shzxlz.cn/gtbkmifpyd.html

[M03] 执行外部命令
来源：http://hz.nwbrower.top/gtjmnstysr.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.yongpay.top/gtvrfrnpua.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.gzhubu.top/gtgdxymhra.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.gogol.net.cn/gtvoeuxelk.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.aizwys.cn/gtallwkhgi.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.aibaodan.cn/gtghbnyfse.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.redwolf501.top/gtcuilxfro.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.gaohongyu789.top/gtfkmyvvwx.html

C#:   Process.Start("ls", "-l");
来源：http://hz.dianchejie.cn/gtjgwbmjcs.html

[M04] 获取当前工作目录
来源：http://hz.yuxming.cn/gtzezeczgm.html

Py:   os.getcwd()
来源：http://hz.sxryk.cn/gtnrcladfl.html

PHP:  getcwd();
来源：http://hz.aibaodan.cn/gtzwtxxkxk.html

JS:   process.cwd()
来源：http://hz.quarkkingdee.top/gtgqctjjkm.html

TS:   process.cwd()
来源：http://hz.zhongyouzk.top/gtaevyxdjq.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.yj202588.top/gtthmvtjqo.html

Go:   os.Getwd()
来源：http://hz.guannengcc.top/gtwfejjajg.html

Ruby: Dir.pwd
来源：http://hz.zycfv.cn/gtlfsaceey.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.sufxvd.cn/gtntwilgre.html

[M05] 设置退出码
来源：http://hz.shzxlz.cn/gtriejoozd.html

Py:   sys.exit(1)
来源：http://hz.quarkkingdee.top/gtldnvxfxa.html

PHP:  exit(1);
来源：http://hz.shzxlz.cn/gtqtbpfrrw.html

JS:   process.exit(1)
来源：http://hz.yj20258888.top/gtefuascli.html

TS:   process.exit(1)
来源：http://hz.hnxiangtu.top/gttpitgqpz.html

Java: System.exit(1)
来源：http://hz.dianchejie.cn/gtonbctsei.html

Go:   os.Exit(1)
来源：http://hz.gogol.net.cn/gtgmltrflx.html

Ruby: exit 1
来源：http://hz.ydzc1.top/gtnclydekl.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.jianghu66.top/gtidrthybq.html

[M06] 向标准错误输出
来源：http://hz.shanyushiyangkeji.top/gtsbprvopq.html

Py:   print("err", file=sys.stderr)
来源：http://hz.yvedp.cn/gtqgbyhaca.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.c1oappe.top/gttpxkzbgl.html

JS:   console.error("err")
来源：http://hz.yvedp.cn/gtkmmibutw.html

TS:   console.error("err")
来源：http://hz.zhoulong.xyz/gtuorjbiza.html

Java: System.err.println("err")
来源：http://hz.yvedp.cn/gtunsbcdov.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.zhaomingkeji.xyz/gtgudfkcxk.html

Ruby: warn "err"
来源：http://hz.mhx1999.top/gtyyfqhvln.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.cheryme.top/gtjzcukknd.html

[M07] 判断是否为主入口
来源：http://hz.shuidangran.top/gtxzaantxn.html

Py:   if __name__ == "__main__":
来源：http://hz.ydzc1.top/gtfyinbqop.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.jiagoushi.top/gtuiimzbvi.html

JS:   require.main === module
来源：http://hz.zhijiandao.cn/gtartqkcog.html

TS:   require.main === module
来源：http://hz.bjfxy.top/gtkyqkvmqp.html

Java: public static void main(String[] args)
来源：http://hz.yj202588.top/gtoktbueyk.html

Go:   func main()
来源：http://hz.ydzc1.top/gtvpqcbbbn.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.haohaochexian.top/gtfwiihbiv.html

C#:   static void Main(string[] args)
来源：http://hz.guowangkeji.top/gtmrlyjjsh.html

[M08] 获取系统与运行时信息
来源：http://hz.zdqjudy.top/gtoxlhuomz.html

Py:   platform.system();  platform.python_version()
来源：http://hz.ehwqpu.com/gtmajxvgcz.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.wangshuangyany.cn/gtjynhvhzs.html

JS:   process.platform;  process.version
来源：http://hz.zhaomingkeji.xyz/gtqwhkrcmf.html

TS:   process.platform;  process.version
来源：http://hz.cucudq.cn/gthsyjsmey.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.yuxming.cn/gtbylrnlcf.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.xingfuxueyuan.xyz/gtbnxenepp.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.jyoumei.cn/gtwvjehxlz.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.shzxlz.cn/gttoptxxxn.html

================================================================================
来源：http://hz.cheryme.top/gtjfkmetjo.html

N. 数据结构与算法
来源：http://hz.svipenyu.cn/gtwraezklx.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtrkrcwxho.html

[N01] 二分查找（有序数组）
来源：http://hz.jinqigufen.top/gtgcaspyzo.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.jyoumei.cn/gtijsyarrl.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.jqgfzy.top/gtvjzcsgso.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.aibaodan.cn/gthgsbgofu.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.hnqzz.top/gtqyxnskhe.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.gaohongyu789.top/gtqfobrvah.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.sufxvd.cn/gttwauqnou.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.xinyue.icu/gtmujuqyla.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.pycfn.com/gthzpdhifz.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.jinghuilouyu.cn/gtqvnrxqsi.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.yangfankeji.com/gtexvqsugl.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.jianghu66.top/gtufanjtid.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.quarkkingdee.top/gtibnftjoi.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.jiagoushi.top/gtxjuacgbn.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.xuanzx.com/gtxqlxrppa.html

Go:   slices.Sort(arr)
来源：http://hz.smart0.xyz/gtxhkpxjhs.html

Ruby: arr.sort
来源：http://hz.yanxiufei.cn/gtxwchdqus.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.feifeiyinyue.top/gtjfyuavxj.html

[N03] 快速排序（分治示例）
来源：http://hz.zhiwuduotai.top/gtrmavvjgm.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.zhoulong.xyz/gtehmxgboj.html

PHP:  // 递归实现，或用 usort
来源：http://hz.jqgufenzy.top/gtrufdzkim.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.zdqjudy.top/gtcmelpcvh.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.hnxiangtu.top/gthluefhxu.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.cucudq.cn/gtcwavfnjf.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.52xcode.cn/gtcuqfbssy.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.kuanghao11.cn/gtufzielsn.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.sysykeji.top/gtzgtikudl.html

[N04] 斐波那契数列
来源：http://hz.sxryk.cn/gtyrsyoejg.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.shanyushiyangkeji.top/gtvdoafjav.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.daxiang520.top/gtshyrkqdf.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.havefunace.top/gtvowmqifs.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.shanyushiyangkeji.top/gtyljvyjnr.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.jinghuilouyu.cn/gtywebeoza.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.zhongyouzk.top/gtuwktqwgb.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.yvedp.cn/gtmgqbnekm.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.gogol.net.cn/gtzfnkbcqp.html

[N05] 最大公约数
来源：http://hz.0kj1m.cn/gtlzrzttbw.html

Py:   math.gcd(a, b)
来源：http://hz.gogol.net.cn/gtwtpdzwni.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.jinyuanbaomall.cn/gtsqbsaskl.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.yuanzhike.top/gtkvhdjhxn.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.chenzaomai.com/gtfohrnmya.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.yj20258.top/gtvmumsfjz.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.guannengcc.top/gtgkfidoqv.html

Ruby: a.gcd(b)
来源：http://hz.ppjwa.cn/gtmbvpiorv.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.0kj1m.cn/gtlqpqgsyx.html

[N06] 判断回文字符串
来源：http://hz.ppjwa.cn/gtgskathtm.html

Py:   s == s[::-1]
来源：http://hz.guowangkeji.top/gthjzvqnjb.html

PHP:  $s === strrev($s);
来源：http://hz.shanyushiyangtech.top/gthhbxibyp.html

JS:   s === [...s].reverse().join("")
来源：http://hz.guowangkeji.top/gtrhtyfnmj.html

TS:   s === [...s].reverse().join("")
来源：http://hz.jinqigufen.top/gtswfzlocz.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.dianchejie.cn/gtbvfmlrvh.html

Go:   // 双指针从两端比较
来源：http://hz.hysaishi.cn/gtejbfevwi.html

Ruby: s == s.reverse
来源：http://hz.zhijiandao.cn/gtfrzszrki.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.shzxlz.cn/gtqfocfbzb.html

[N07] 两数之和（返回下标）
来源：http://hz.chenzaomai.com/gtocvtaxzr.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.zhaomingkeji.xyz/gtfafcvnrj.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.ybcxt.top/gtoxtkgsee.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.sweek.top/gtomicxdkv.html

TS:   // 手写 Map<string, number>
来源：http://hz.zhengqikj.top/gtamylddsj.html

Java: // 手写 HashMap
来源：http://hz.andypj.xyz/gtxvxewrdb.html

Go:   // 手写 map[int]int
来源：http://hz.sxryk.cn/gtisthfpfm.html

Ruby: // 手写 Hash
来源：http://hz.yangfankeji.com/gtrbnwyugu.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.daria6918.cn/gtjtxwvcde.html

[N08] 生成全排列
来源：http://hz.cheryme.top/gtbjuhgxvl.html

Py:   itertools.permutations(arr)
来源：http://hz.xingfuxueyuan.xyz/gtjwhhocjx.html

PHP:  // 手写递归交换
来源：http://hz.nanxuanxn.top/gtmexgnapy.html

JS:   // 手写回溯递归
来源：http://hz.hysaishi.cn/gtzbaqoxcm.html

TS:   // 手写回溯递归
来源：http://hz.cqqwz.cn/gthllhmnzc.html

Java: // 手写回溯递归
来源：http://hz.wangshuangyany.cn/gtwfmbpzxg.html

Go:   // 手写回溯递归
来源：http://hz.c1oappe.top/gtgcohewjz.html

Ruby: arr.permutation.to_a
来源：http://hz.zhixingplan.top/gtqknggfkl.html

C#:   // 手写回溯递归
来源：http://hz.dianchejie.cn/gtuwhbowmy.html

[N09] 栈与队列
来源：http://hz.52xcode.cn/gtobruujry.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.jlsjyb.cn/gtmwuxygkw.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.zhijiandao.cn/gtbbhxlljg.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.meibo888.top/gtgqaxkdjc.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.zhongyouzk.top/gttvnpamqe.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.cqqwz.cn/gtaktifrhb.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.shangyingyoupin.top/gtxevoxiyy.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.redwolf501.top/gtckbonszb.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.zdqjudy.top/gtibkbryvt.html

[N10] 链表节点定义
来源：http://hz.svipenyu.cn/gtpfzbajhw.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.cashguo.top/gtlubmydah.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.sufxvd.cn/gtedqawdae.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.hysaishi.cn/gtcdrqwovb.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.hammf.cn/gtrxrigthf.html

Java: class Node { int v; Node next; }
来源：http://hz.yj20258.top/gtfalnnoik.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.hammf.cn/gtxownvlge.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.shangyingyoupin.top/gtbnfwwrjw.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.xylfe.cn/gtziizjffa.html

[N11] 二叉树中序遍历
来源：http://hz.zycfv.cn/gteapcwopw.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.jianghu66.top/gtkzffotic.html

PHP:  // 手写递归函数
来源：http://hz.bjfxy.top/gtwkpiyvzf.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.haohaochexian.top/gtkvcvafxy.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.yvedp.cn/gtxfqvyjrf.html

Java: // 手写递归
来源：http://hz.yj202588.top/gtbztcshby.html

Go:   // 手写递归
来源：http://hz.yj20258888.top/gteogeltqu.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.yj20258888.top/gtkjdlusuc.html

C#:   // 手写递归
来源：http://hz.redwolf501.top/gtxrwnfuru.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.ybcxt.top/gtdsfivrev.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.xziqi.cn/gtzfjjklwp.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.cashguo.top/gtytowxfoq.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.yuanzhike.top/gtdnpvwuyb.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.yj202588.top/gtbowqrmpa.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.cashguo.top/gtzqzktqyk.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.tanke756.top/gtfnhyhfte.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.xuanzx.com/gtxwqmchsb.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.sysykeji.top/gtduisbhar.html

================================================================================
来源：http://hz.birdmap.top/gtlunjfbid.html

O. 并发与异步
来源：http://hz.hysaishi.cn/gtkidsiotk.html

================================================================================
来源：http://hz.yj202588.top/gtxzhrkxab.html

[O01] 启动一个线程
来源：http://hz.cqqwz.cn/gtafdpvglg.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.yonumen.top/gtvjsqttwg.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.daxiang520.top/gtamxvnpfe.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.jiagoushi.top/gtzqxfjqvi.html

TS:   // 同 JS
来源：http://hz.hnxiangtu.top/gtujnihhid.html

Java: new Thread(() -> f()).start()
来源：http://hz.jinqigfzy.top/gtczsgexdw.html

Go:   go f()
来源：http://hz.vqdsnc.cn/gtqgkplldi.html

Ruby: Thread.new { f }
来源：http://hz.sufxvd.cn/gtxejsktvv.html

C#:   Task.Run(() => F());
来源：http://hz.zhoulong.xyz/gtzaydmewf.html

[O02] 使用线程池
来源：http://hz.nanxuanxn.top/gtlozbxjgh.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.guowangkeji.top/gtkncknatk.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.xingfuxueyuan.xyz/gtppowtxap.html

JS:   // worker_threads 线程池
来源：http://hz.shanyushiyangkeji.top/gthfibyshs.html

TS:   // worker_threads 线程池
来源：http://hz.hnqzz.top/gtuvomkhit.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.ybcxt.top/gtqxtlgtfa.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.shanyushiyangtech.top/gtnywnzpgs.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.fengsongda.top/gtiigzrubo.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.yonumen.top/gtrdxasako.html

[O03] 加锁保护共享数据
来源：http://hz.c1oappe.top/gtgcsdjeiq.html

Py:   with lock: shared += 1
来源：http://hz.jinghuilouyu.cn/gtldmrbhmz.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.wangdashe.top/gtngsfxwpw.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.xinyue.icu/gtryfymfuh.html

TS:   // 同 JS
来源：http://hz.yueranfly.top/gtdpdksggz.html

Java: synchronized (this) { shared++; }
来源：http://hz.jqgufenzy.top/gtjowxxftk.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.hnxiangtu.top/gtlughwxuh.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.mhx1999.top/gtdsauhhrc.html

C#:   lock (gate) { shared++; }
来源：http://hz.ydzc1.top/gtfxaqogqa.html

[O04] 定义异步函数并等待
来源：http://hz.birdmap.top/gtrbpmuuaz.html

Py:   async def f():⏎    await g()
来源：http://hz.shanyushiyangtech.top/gtwmxcmqcy.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.hfpthk.cn/gtftcfcttp.html

JS:   async function f() { await g(); }
来源：http://hz.tian-w.cn/gtldeoysql.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.jianghu66.top/gtpeyvtqka.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.zycfv.cn/gtxtdkayyx.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.sufxvd.cn/gtxocyootw.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.redwolf501.top/gtaqthygke.html

C#:   async Task F() { await G(); }
来源：http://hz.sufxvd.cn/gtogtnqaau.html

[O05] 并发执行并等待全部完成
来源：http://hz.yj20258.top/gtjjulsetp.html

Py:   asyncio.gather(*tasks)
来源：http://hz.pengpengdd.cyou/gtmxvsfzvm.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.iojbl.cn/gtcdzhxxts.html

JS:   await Promise.all(tasks)
来源：http://hz.shanyushiyangkeji.top/gtiukitkqn.html

TS:   await Promise.all(tasks)
来源：http://hz.yongpay.top/gtrrczvnvr.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.c1oappe.top/gtyhflsrbh.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.mhx1999.top/gtuurydcpn.html

Ruby: threads.map(&:join)
来源：http://hz.shzxlz.cn/gtujnrqcwz.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.zhengqikj.top/gthbvqihjw.html

[O06] 使用进程池
来源：http://hz.xinyue.icu/gtvjkowzod.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.yueranfly.top/gtvhgpergs.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.daria6918.cn/gtiklbqzxp.html

JS:   // child_process / cluster 模块
来源：http://hz.wangdashe.top/gtvdfaalhp.html

TS:   // child_process / cluster 模块
来源：http://hz.aibaodan.cn/gtnmkjqoql.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.yangfankeji.com/gtnkrabmrl.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.fzhhl.top/gtpaxibzpz.html

Ruby: // fork 块
来源：http://hz.pengpengdd.cyou/gtgoectdui.html

C#:   Parallel.For
来源：http://hz.ywan-chungtsiang.top/gtpqqnfnii.html

================================================================================
来源：http://hz.ivvv.top/gttkroriml.html

P. 常用工具函数
来源：http://hz.dianchejie.cn/gtfanuzsmq.html

================================================================================
来源：http://hz.yj202588.top/gtnomzuukk.html

[P01] 生成 UUID
来源：http://hz.gzhubu.top/gtmvyjlmqd.html

Py:   str(uuid.uuid4())
来源：http://hz.shzxlz.cn/gtycwpvpvx.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.zhixingplan.top/gtdpyzkyqq.html

JS:   crypto.randomUUID()
来源：http://hz.yongpay.top/gtludjtdpi.html

TS:   crypto.randomUUID()
来源：http://hz.cheryme.top/gtvqkhqfux.html

Java: UUID.randomUUID().toString()
来源：http://hz.xinyue.icu/gtzsrsskiz.html

Go:   // 用 github.com/google/uuid
来源：http://hz.jianghu66.top/gthaktpibg.html

Ruby: SecureRandom.uuid
来源：http://hz.jiagoushi.top/gtotsgowur.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.wangshuangyany.cn/gtuycvonkn.html

[P02] MD5 / SHA256 摘要
来源：http://hz.ydjk.org.cn/gtujlxfxar.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.iojbl.cn/gtkkwppkgg.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.gotoacloud.top/gtvksgnfrr.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.dashuyun.cn/gtbqnuexko.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.hysaishi.cn/gtfkofwebs.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.nanxinkj.top/gtshoweysg.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.xuanzx.com/gtgblzwwev.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.pycfn.com/gthflwumkp.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.shanyushiyangtech.top/gthvrounqa.html

[P03] 生成短随机字符串
来源：http://hz.xylfe.cn/gthgbjfuic.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.yj20258.top/gtfepnwsoi.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.jinqigfzy.top/gttvhkdqmn.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.chenlongwang.top/gtjvreahvn.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.cqqwz.cn/gtywuvurcl.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.hywenlv.cn/gtfiaxcexp.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.zhijiandao.cn/gtlzqxpfrw.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.iojbl.cn/gtgekwcpwq.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.yongpay.top/gtuzyddwkz.html

[P04] 求长度
来源：http://hz.zycfv.cn/gtzeplnmyz.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.mhx1999.top/gtsbzxdltu.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.shanyushiyangkeji.top/gttpvyrein.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.zhoulong.xyz/gtmqeekmko.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.zhongyouzk.top/gtzizagids.html

Java: list.size();  map.size();  s.length()
来源：http://hz.xinyue.icu/gtbcxjwaxn.html

Go:   len(arr);  len(m)
来源：http://hz.zdqjudy.top/gtsqooxgcq.html

Ruby: x.length;  x.size
来源：http://hz.jianghu66.top/gtrwrftlov.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.xingfuxueyuan.xyz/gtathrhmpz.html

[P05] 判断两个对象内容是否相等
来源：http://hz.jqgufenzy.top/gtsbwlxhgk.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.chenjidiqi.icu/gtiomkifme.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.sufxvd.cn/gtieuxayku.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.birdmap.top/gtfqihvdtp.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.ybcxt.top/gtddotacfz.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.svipenyu.cn/gtvkptrxvf.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.pycfn.com/gtrfjsgypy.html

Ruby: a == b
来源：http://hz.xingfuxueyuan.xyz/gtpvuxntqq.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.guowangkeji.top/gtlgkncnay.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.wangdashe.top/gtymcunrxz.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.guowangkeji.top/gtzxrikimd.html

PHP:  if (empty($x)) {}
来源：http://hz.iojbl.cn/gtklqmaazv.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.jlsjyb.cn/gtmcmucqpd.html

TS:   if (x == null) {}
来源：http://hz.zhiwuduotai.top/gtcvisxslc.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.9152youxi.cn/gtsfklatku.html

Go:   if x == nil {}
来源：http://hz.cdnleiting.top/gtfqedryfr.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.vqdsnc.cn/gtyhtcjxeo.html

C#:   if (x is null) {}
来源：http://hz.ivvv.top/gtfxdbofod.html

[P07] 防抖与节流
来源：http://hz.nwbrower.top/gtsbjhssar.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.0kj1m.cn/gtvtukbays.html

PHP:  // 手写时间戳比较
来源：http://hz.jqgfzy.top/gtqwntyxzt.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.bjfxy.top/gtgpssxecj.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.shuidangran.top/gtipofilvp.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.mhx1999.top/gtqprobbgs.html


<!-- 参考信息 -->