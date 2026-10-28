代发 wailian999

================================================================================
来源：http://hz.0kj1m.cn/gtajflqrfz.html

[M01] 读取命令行参数
来源：http://hz.pengpengdd.cyou/gtefqfgjuq.html

Py:   sys.argv[1:]
来源：http://hz.sxryk.cn/gtivjpgmrm.html

PHP:  $argv;  $argc;
来源：http://hz.jyoumei.cn/gtymfzkzga.html

JS:   process.argv.slice(2)
来源：http://hz.yvedp.cn/gtjxvcwuue.html

TS:   process.argv.slice(2)
来源：http://hz.kuanghao11.cn/gtucnhqbna.html

Java: args 数组（main 方法参数）
来源：http://hz.fengsongda.top/gtrvefrfla.html

Go:   os.Args[1:]
来源：http://hz.ywan-chungtsiang.top/gtfkedukhl.html

Ruby: ARGV
来源：http://hz.shuidangran.top/gtmsdmlxyu.html

C#:   args 数组（Main 方法参数）
来源：http://hz.gzhubu.top/gtzwwxusrq.html

[M02] 读取环境变量
来源：http://hz.gaohongyu789.top/gtgeaddefo.html

Py:   os.environ.get("HOME")
来源：http://hz.hysaishi.cn/gthqhapbaa.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.hywenlv.cn/gtcdstvhei.html

JS:   process.env.HOME
来源：http://hz.bjfxy.top/gtgeeffvna.html

TS:   process.env.HOME
来源：http://hz.zdqjudy.top/gtnphceyil.html

Java: System.getenv("HOME")
来源：http://hz.nanxinkj.top/gtzivvvdzq.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.chenlongwang.top/gttiqhcibs.html

Ruby: ENV["HOME"]
来源：http://hz.meibo888.top/gtnzhxsnbf.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.gogol.net.cn/gtmdpzalmw.html

[M03] 执行外部命令
来源：http://hz.zhixingplan.top/gtotswtqlx.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.haohaochexian.top/gtnrlyfiio.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.zhoulong.xyz/gtrkwnxntk.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.sufxvd.cn/gtbletvmeg.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.xziqi.cn/gtrmtcvogj.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.sxryk.cn/gtnhpqchph.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.jinyuanbaomall.cn/gtahrkaczx.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.hnxiangtu.top/gtqmnxwsvw.html

C#:   Process.Start("ls", "-l");
来源：http://hz.zdqjudy.top/gtbswasefo.html

[M04] 获取当前工作目录
来源：http://hz.sweek.top/gtevuvfbot.html

Py:   os.getcwd()
来源：http://hz.hywenlv.cn/gtuheaqice.html

PHP:  getcwd();
来源：http://hz.iojbl.cn/gtadijlzda.html

JS:   process.cwd()
来源：http://hz.9152youxi.cn/gtkfcgljmu.html

TS:   process.cwd()
来源：http://hz.vqdsnc.cn/gtlfulrznj.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.ppjwa.cn/gtgdbhzyzt.html

Go:   os.Getwd()
来源：http://hz.cheryme.top/gtidhiwjug.html

Ruby: Dir.pwd
来源：http://hz.ppjwa.cn/gtkuxncgba.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.jinqigufen.top/gtuvmuukhz.html

[M05] 设置退出码
来源：http://hz.tianlin.xyz/gtxqyrrdmb.html

Py:   sys.exit(1)
来源：http://hz.nwbrower.top/gtjmbenkak.html

PHP:  exit(1);
来源：http://hz.nanxuanxn.top/gtlxpdrais.html

JS:   process.exit(1)
来源：http://hz.dashuyun.cn/gtrhqyyvfb.html

TS:   process.exit(1)
来源：http://hz.zycfv.cn/gtpspdxyar.html

Java: System.exit(1)
来源：http://hz.chenlongwang.top/gtahezvtcz.html

Go:   os.Exit(1)
来源：http://hz.ydjk.org.cn/gtggrtdhxo.html

Ruby: exit 1
来源：http://hz.dashuyun.cn/gtocczlmnl.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.cashguo.top/gtyhlkfdxc.html

[M06] 向标准错误输出
来源：http://hz.snrcjt.cn/gtajfecvrq.html

Py:   print("err", file=sys.stderr)
来源：http://hz.jiagoushi.top/gtgvncdvec.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.xylfe.cn/gtdhuuwpbi.html

JS:   console.error("err")
来源：http://hz.daria6918.cn/gtzyaqvaui.html

TS:   console.error("err")
来源：http://hz.hnxiangtu.top/gtewcmvsve.html

Java: System.err.println("err")
来源：http://hz.yuxming.cn/gtdgqiglam.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.xuanzx.com/gtlkmpwzvi.html

Ruby: warn "err"
来源：http://hz.sufxvd.cn/gtecndqbny.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.tian-w.cn/gtzvlycmys.html

[M07] 判断是否为主入口
来源：http://hz.xuetiantiany.cn/gtmakkbdxq.html

Py:   if __name__ == "__main__":
来源：http://hz.jyoumei.cn/gtyehigwta.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.zhijiandao.cn/gtxntmdwvm.html

JS:   require.main === module
来源：http://hz.cdnleiting.top/gttqsnttal.html

TS:   require.main === module
来源：http://hz.hnxiangtu.top/gtbbhpwdup.html

Java: public static void main(String[] args)
来源：http://hz.cdnleiting.top/gtyqnnmayq.html

Go:   func main()
来源：http://hz.yuxming.cn/gtgiyizkqh.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.yuanzhike.top/gttijdoknq.html

C#:   static void Main(string[] args)
来源：http://hz.fzhhl.top/gtzrwkhecd.html

[M08] 获取系统与运行时信息
来源：http://hz.guowangkeji.top/gtvmuvpuip.html

Py:   platform.system();  platform.python_version()
来源：http://hz.bjfxy.top/gtqdpdnesw.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.ybcxt.top/gtvsganfxo.html

JS:   process.platform;  process.version
来源：http://hz.xylfe.cn/gtnkjkpxxx.html

TS:   process.platform;  process.version
来源：http://hz.yanxiufei.cn/gtvsxzcrtn.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.shangyingyoupin.top/gtspluuabo.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.aizwys.cn/gtxispwxfu.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.zhixingplan.top/gtkscplqyq.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.sufxvd.cn/gtnjhaprqj.html

================================================================================
来源：http://hz.guannengcc.top/gtbquduyfg.html

N. 数据结构与算法
来源：http://hz.jyoumei.cn/gthkssadui.html

================================================================================
来源：http://hz.9152youxi.cn/gtbjawsdwa.html

[N01] 二分查找（有序数组）
来源：http://hz.feifeiyinyue.top/gtbqrcrstr.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.quarkkingdee.top/gtspukewhq.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.cheryme.top/gtwnhnjmlv.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.nanxuanxn.top/gthtsohbnr.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.xylfe.cn/gtnwvstcgp.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.cucudq.cn/gtelrftniz.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.zhoulong.xyz/gtteiikomq.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.9152youxi.cn/gtlzjkgxdk.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.hongshengwenyu.top/gthyfvsahf.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.cucudq.cn/gtxqtigriy.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.zhiwuduotai.top/gtwhcbovvb.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.ywan-chungtsiang.top/gtalsuiruh.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.nanxuanxn.top/gtsrscwnlt.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.mhx1999.top/gtuccewuop.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.fengsongda.top/gtsdefmqeh.html

Go:   slices.Sort(arr)
来源：http://hz.jiagoushi.top/gtyiegkjzx.html

Ruby: arr.sort
来源：http://hz.mhx1999.top/gtmigydgji.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.iojbl.cn/gtvsiohecq.html

[N03] 快速排序（分治示例）
来源：http://hz.haohaochexian.top/gtxskmisfy.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.nanxinkj.top/gtymqlzzzj.html

PHP:  // 递归实现，或用 usort
来源：http://hz.hysaishi.cn/gtrhaxwiwh.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.jyoumei.cn/gtmzjlsaxi.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.daxiang520.top/gtpydtzxvq.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.shuidangran.top/gtlyltnwup.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.yueranfly.top/gtnhgoaydo.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.shanyushiyangtech.top/gtvlyjansg.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.andypj.xyz/gtsusabajm.html

[N04] 斐波那契数列
来源：http://hz.ivvv.top/gtgiedspjd.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.zhixingplan.top/gtfwscsust.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.ydzc1.top/gtixnaiemw.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.hnxiangtu.top/gtqxsuitop.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.hnqzz.top/gtxsxcjjyy.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.316326.xyz/gtlpobvvmi.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.c1oappe.top/gtwknmkssk.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.shangyingyoupin.top/gtyzvlqipy.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.zhijiandao.cn/gtxptsrzkt.html

[N05] 最大公约数
来源：http://hz.nanxuanxn.top/gtrehwppay.html

Py:   math.gcd(a, b)
来源：http://hz.hywenlv.cn/gtlggjnujj.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.shzxlz.cn/gtbzqaptud.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.haohaochexian.top/gtzmoktsxp.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.gzhubu.top/gtnumupgzs.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.meibo888.top/gtxvzvfrtq.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.mhx1999.top/gtxlhrkspb.html

Ruby: a.gcd(b)
来源：http://hz.wangdashe.top/gtejchenss.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.hongshengwenyu.top/gthozzphmc.html

[N06] 判断回文字符串
来源：http://hz.hongshengwenyu.top/gtxucwfylg.html

Py:   s == s[::-1]
来源：http://hz.shuidangran.top/gtsyqjyzxp.html

PHP:  $s === strrev($s);
来源：http://hz.daxiang520.top/gtfbnlnhvb.html

JS:   s === [...s].reverse().join("")
来源：http://hz.nwbrower.top/gtwkxpugma.html

TS:   s === [...s].reverse().join("")
来源：http://hz.yuanzhike.top/gtmjdcjlvy.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.jyoumei.cn/gtyfmizksx.html

Go:   // 双指针从两端比较
来源：http://hz.shanyushiyangkeji.top/gtxedwrije.html

Ruby: s == s.reverse
来源：http://hz.zycfv.cn/gtmhuefoze.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.shangyingyoupin.top/gtdzbixtjm.html

[N07] 两数之和（返回下标）
来源：http://hz.gotoacloud.top/gtrqeuabjb.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.guowangkeji.top/gtuvnvynnh.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.cqqwz.cn/gtkywluvgo.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.sysykeji.top/gtgavpalyf.html

TS:   // 手写 Map<string, number>
来源：http://hz.daxiang520.top/gttmkruxfo.html

Java: // 手写 HashMap
来源：http://hz.jinyuanbaomall.cn/gtrotylmvi.html

Go:   // 手写 map[int]int
来源：http://hz.wangdashe.top/gtdqziodcp.html

Ruby: // 手写 Hash
来源：http://hz.jyoumei.cn/gtlzlknpfy.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.fengsongda.top/gtvkhyrchv.html

[N08] 生成全排列
来源：http://hz.jianghu66.top/gtacnwpjxc.html

Py:   itertools.permutations(arr)
来源：http://hz.quarkkingdee.top/gtbijbnbft.html

PHP:  // 手写递归交换
来源：http://hz.aibaodan.cn/gtnveljkit.html

JS:   // 手写回溯递归
来源：http://hz.aizwys.cn/gtmlccpsnq.html

TS:   // 手写回溯递归
来源：http://hz.52xcode.cn/gtwpabcxku.html

Java: // 手写回溯递归
来源：http://hz.ydjk.org.cn/gtlfnhasls.html

Go:   // 手写回溯递归
来源：http://hz.cashguo.top/gtjjuyfqcw.html

Ruby: arr.permutation.to_a
来源：http://hz.sysykeji.top/gtbyzaizmu.html

C#:   // 手写回溯递归
来源：http://hz.gogol.net.cn/gtmzjxzbdy.html

[N09] 栈与队列
来源：http://hz.gaohongyu789.top/gtsglcbhgt.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.aizwys.cn/gtswpdoarp.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.ppjwa.cn/gtzkkefolt.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.pengpengdd.cyou/gtysyaskke.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.tianlin.xyz/gtgjybkywh.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.kuanghao11.cn/gtlmaokzlv.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.yvedp.cn/gtqzmtcrsp.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.c1oappe.top/gtqbdfylvu.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.xuanzx.com/gtbxuttfdx.html

[N10] 链表节点定义
来源：http://hz.tian-w.cn/gtfqgkhzgs.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.chenjidiqi.icu/gtodsgjeub.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.xziqi.cn/gtjrdgeang.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.gzhubu.top/gtuftzuyak.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.vqdsnc.cn/gtkbhgjuas.html

Java: class Node { int v; Node next; }
来源：http://hz.guowangkeji.top/gtscuafczz.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.aizwys.cn/gtqyvtzwuu.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.haohaochexian.top/gtgkryszsr.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.xuetiantiany.cn/gtveuhzylo.html

[N11] 二叉树中序遍历
来源：http://hz.shzxlz.cn/gtxoyuabhi.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.hywenlv.cn/gtwtpvvtcr.html

PHP:  // 手写递归函数
来源：http://hz.hywenlv.cn/gtokjviaoq.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.ivvv.top/gtxghpqdte.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.0kj1m.cn/gtsstxymzu.html

Java: // 手写递归
来源：http://hz.xingfuxueyuan.xyz/gtdikiyizh.html

Go:   // 手写递归
来源：http://hz.hysaishi.cn/gtrkofanew.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.shanyushiyangkeji.top/gtlzbcscle.html

C#:   // 手写递归
来源：http://hz.jqgufenzy.top/gtlhslwpeq.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.aizwys.cn/gtdlntsyww.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.tian-w.cn/gtqovvshfg.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.vqdsnc.cn/gtzipidvrf.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.tian-w.cn/gtgbrkwzlj.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.ivvv.top/gtjsejpmyv.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.guannengcc.top/gtulsnhmri.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.cqqwz.cn/gtudieqkxs.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.zhengqikj.top/gtjotjhlfs.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.chenzaomai.com/gtqqywoqvf.html

================================================================================
来源：http://hz.chenjidiqi.icu/gttzujyojs.html

O. 并发与异步
来源：http://hz.jqgufenzy.top/gtsobfnxmn.html

================================================================================
来源：http://hz.yanxiufei.cn/gtxqhlttvg.html

[O01] 启动一个线程
来源：http://hz.shanyushiyangtech.top/gtaradtnfk.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.sysykeji.top/gtvbssggig.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.shzxlz.cn/gtiapukkcg.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.smart0.xyz/gtznemznzn.html

TS:   // 同 JS
来源：http://hz.vqdsnc.cn/gttvtnhnhu.html

Java: new Thread(() -> f()).start()
来源：http://hz.jqgufenzy.top/gthxlwphys.html

Go:   go f()
来源：http://hz.yj202588.top/gtzuxkilcz.html

Ruby: Thread.new { f }
来源：http://hz.yueranfly.top/gtlryvvtdx.html

C#:   Task.Run(() => F());
来源：http://hz.gotoacloud.top/gtamqyixhh.html

[O02] 使用线程池
来源：http://hz.vqdsnc.cn/gtydvmyvhu.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.shangyingyoupin.top/gtnnfnzngg.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.jinyuanbaomall.cn/gtbetkfmdx.html

JS:   // worker_threads 线程池
来源：http://hz.c1oappe.top/gtbxwkpban.html

TS:   // worker_threads 线程池
来源：http://hz.smart0.xyz/gtgkxpfogc.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.jiagoushi.top/gtvrofibfd.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.shzxlz.cn/gtjmkmedeu.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.gotoacloud.top/gtfeyaadoo.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.yangfankeji.com/gtmkatauis.html

[O03] 加锁保护共享数据
来源：http://hz.iojbl.cn/gtrifvgbgh.html

Py:   with lock: shared += 1
来源：http://hz.pengpengdd.cyou/gtrztymibo.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.fengsongda.top/gthyiyncvl.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.yanxiufei.cn/gtzdhvdpzk.html

TS:   // 同 JS
来源：http://hz.zhaomingkeji.xyz/gtvzwjwqlm.html

Java: synchronized (this) { shared++; }
来源：http://hz.quarkkingdee.top/gtquawpyup.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.sxryk.cn/gtufuraxzy.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.tian-w.cn/gtttcpxvug.html

C#:   lock (gate) { shared++; }
来源：http://hz.svipenyu.cn/gtohrafbpl.html

[O04] 定义异步函数并等待
来源：http://hz.cashguo.top/gtyqlsmqli.html

Py:   async def f():⏎    await g()
来源：http://hz.hnxiangtu.top/gtmhlrxcwi.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.zhongyouzk.top/gtlhmvhtlk.html

JS:   async function f() { await g(); }
来源：http://hz.fzhhl.top/gttyjddxim.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.jyoumei.cn/gtaugijlvr.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.ehwqpu.com/gtcqilipmx.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.sufxvd.cn/gtqiojdkdm.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.ppjwa.cn/gtuxruxeda.html

C#:   async Task F() { await G(); }
来源：http://hz.daxiang520.top/gthbhptjkx.html

[O05] 并发执行并等待全部完成
来源：http://hz.pycfn.com/gtdjflgijl.html

Py:   asyncio.gather(*tasks)
来源：http://hz.xinyue.icu/gtkyzmqmnq.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.xinyue.icu/gtrqtngbho.html

JS:   await Promise.all(tasks)
来源：http://hz.gotoacloud.top/gtuvjdieub.html

TS:   await Promise.all(tasks)
来源：http://hz.guowangkeji.top/gtczykpoxe.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.52xcode.cn/gtzsznxuud.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.yj202588.top/gtmbgewzon.html

Ruby: threads.map(&:join)
来源：http://hz.sxryk.cn/gtbkxingih.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.dianchejie.cn/gtcgeifogt.html

[O06] 使用进程池
来源：http://hz.ppjwa.cn/gtteovxnst.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.daria6918.cn/gtsjugzksd.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.pengpengdd.cyou/gtbuurdvkr.html

JS:   // child_process / cluster 模块
来源：http://hz.guannengcc.top/gtlckfyjci.html

TS:   // child_process / cluster 模块
来源：http://hz.jqgfzy.top/gtrkgufglu.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.zhixingplan.top/gtglzygjax.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.cqqwz.cn/gtklotzsis.html

Ruby: // fork 块
来源：http://hz.hammf.cn/gthruajdxk.html

C#:   Parallel.For
来源：http://hz.snrcjt.cn/gtzgnetegf.html

================================================================================
来源：http://hz.zhijiandao.cn/gtcarjrvez.html

P. 常用工具函数
来源：http://hz.sysykeji.top/gtmcwekmaj.html

================================================================================
来源：http://hz.jinqigfzy.top/gtfqosuqzv.html

[P01] 生成 UUID
来源：http://hz.chenlongwang.top/gtmcrejgqf.html

Py:   str(uuid.uuid4())
来源：http://hz.shzxlz.cn/gtxdhmkavh.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.fzhhl.top/gtrlvtjcqw.html

JS:   crypto.randomUUID()
来源：http://hz.quarkkingdee.top/gtruwbrnhh.html

TS:   crypto.randomUUID()
来源：http://hz.haohaochexian.top/gtghqbjxib.html

Java: UUID.randomUUID().toString()
来源：http://hz.jinqigfzy.top/gtqzqtxzmx.html

Go:   // 用 github.com/google/uuid
来源：http://hz.guannengcc.top/gtuovkryow.html

Ruby: SecureRandom.uuid
来源：http://hz.nwbrower.top/gtmqwgnakd.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.9152youxi.cn/gtguovebez.html

[P02] MD5 / SHA256 摘要
来源：http://hz.gzhubu.top/gtskfwylto.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.snrcjt.cn/gtkoyrhsyo.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.zhaomingkeji.xyz/gtrykokgga.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.gaohongyu789.top/gtdphaxjvm.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.jinqigufen.top/gtabgglabi.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.jqgufenzy.top/gtqgxvonsn.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.c1oappe.top/gtswcpeecr.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.zycfv.cn/gtcjvsemzb.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.birdmap.top/gteqcgyyhc.html

[P03] 生成短随机字符串
来源：http://hz.yj202588.top/gtzaedrkcc.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.havefunace.top/gtkvakoaox.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.yj202588.top/gtxmlaurcd.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.pycfn.com/gtbbowotpf.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.hnqzz.top/gtihekvuaz.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.svipenyu.cn/gtrvyrwzkn.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.bjfxy.top/gtfzqjxttf.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.gogol.net.cn/gtdnddnmca.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.jinghuilouyu.cn/gtgwaytvod.html

[P04] 求长度
来源：http://hz.dashuyun.cn/gtvfuctxzr.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.xziqi.cn/gtkjtmscix.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.xingfuxueyuan.xyz/gtsseblhoi.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.yuxming.cn/gtewlizgbt.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.yj20258888.top/gtrrtyqyhn.html

Java: list.size();  map.size();  s.length()
来源：http://hz.cdnleiting.top/gtxfvygmwy.html

Go:   len(arr);  len(m)
来源：http://hz.yanxiufei.cn/gtgpgzksvb.html

Ruby: x.length;  x.size
来源：http://hz.tanke756.top/gtsxgeaqyt.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.yj20258.top/gtqnnxmlge.html

[P05] 判断两个对象内容是否相等
来源：http://hz.ywan-chungtsiang.top/gtnbsswlnv.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.chenzaomai.com/gtvhiwxdjc.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.pycfn.com/gtpoipbwjx.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.havefunace.top/gtqgzetpwu.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.yongpay.top/gtnpmnoaps.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.yangfankeji.com/gthsigbzyx.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.guowangkeji.top/gtyfrylezf.html

Ruby: a == b
来源：http://hz.yueranfly.top/gtyyhbsumv.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.zhijiandao.cn/gtvxjscacf.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.pycfn.com/gtwedtabwg.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.yj20258.top/gtoxrnigac.html

PHP:  if (empty($x)) {}
来源：http://hz.feifeiyinyue.top/gtwuwahvjo.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.jinqigfzy.top/gttwpbivmv.html

TS:   if (x == null) {}
来源：http://hz.jyoumei.cn/gtrazzekbr.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.ppjwa.cn/gtoesudepu.html

Go:   if x == nil {}
来源：http://hz.havefunace.top/gtxjasswgi.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.pengpengdd.cyou/gtnemnnqfm.html

C#:   if (x is null) {}
来源：http://hz.wangshuangyany.cn/gtmaarrtcy.html

[P07] 防抖与节流
来源：http://hz.ydzc1.top/gtoycsheku.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.yuanzhike.top/gtmgxlplsw.html


<!-- 参考信息 -->