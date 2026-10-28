代发 wailian999

Ruby: ARGV
来源：http://hz.feifeiyinyue.top/gtstfpahmi.html

C#:   args 数组（Main 方法参数）
来源：http://hz.9152youxi.cn/gtgnvqyuxm.html

[M02] 读取环境变量
来源：http://hz.ydzc1.top/gtegvwiniu.html

Py:   os.environ.get("HOME")
来源：http://hz.vqdsnc.cn/gtdukjdtkn.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.mhx1999.top/gtfxabdtdy.html

JS:   process.env.HOME
来源：http://hz.shangyingyoupin.top/gtmxngtksw.html

TS:   process.env.HOME
来源：http://hz.yuxming.cn/gtpiquecid.html

Java: System.getenv("HOME")
来源：http://hz.wangshuangyany.cn/gtymcodoel.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.zhijiandao.cn/gtglfvtxyv.html

Ruby: ENV["HOME"]
来源：http://hz.9152youxi.cn/gtdifbmxlb.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.hnxiangtu.top/gtdcphbvrh.html

[M03] 执行外部命令
来源：http://hz.chenlongwang.top/gtuplfdrph.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.jinghuilouyu.cn/gtsqlqailp.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.xinyue.icu/gtrxqirkoe.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.gogol.net.cn/gtpyylhbte.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.havefunace.top/gtxmxbszwb.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.cqqwz.cn/gtihtuzblx.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.jinqigfzy.top/gtlyndfjnd.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.daria6918.cn/gtmpabnsow.html

C#:   Process.Start("ls", "-l");
来源：http://hz.hammf.cn/gtrpgjkgjn.html

[M04] 获取当前工作目录
来源：http://hz.chenlongwang.top/gtrktnmrqr.html

Py:   os.getcwd()
来源：http://hz.daria6918.cn/gtekofnyez.html

PHP:  getcwd();
来源：http://hz.svipenyu.cn/gtkpzlanqh.html

JS:   process.cwd()
来源：http://hz.hysaishi.cn/gtezwgeldl.html

TS:   process.cwd()
来源：http://hz.jyoumei.cn/gtzgbkovbx.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.birdmap.top/gtjjvmivwv.html

Go:   os.Getwd()
来源：http://hz.hnqzz.top/gtoylfzgrk.html

Ruby: Dir.pwd
来源：http://hz.tianlin.xyz/gtekzgwsnd.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.birdmap.top/gtwgkmucyt.html

[M05] 设置退出码
来源：http://hz.yangfankeji.com/gtrrlzpytp.html

Py:   sys.exit(1)
来源：http://hz.zhoulong.xyz/gtfjkftmvz.html

PHP:  exit(1);
来源：http://hz.dashuyun.cn/gtpbdgwoaw.html

JS:   process.exit(1)
来源：http://hz.gzhubu.top/gttppjthij.html

TS:   process.exit(1)
来源：http://hz.dashuyun.cn/gtixlgnrus.html

Java: System.exit(1)
来源：http://hz.meibo888.top/gtntqxoctp.html

Go:   os.Exit(1)
来源：http://hz.guowangkeji.top/gtckpogkqg.html

Ruby: exit 1
来源：http://hz.zhoulong.xyz/gtnymhfqau.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.nanxinkj.top/gtpuelvxmi.html

[M06] 向标准错误输出
来源：http://hz.snrcjt.cn/gtecgwrnth.html

Py:   print("err", file=sys.stderr)
来源：http://hz.zhiwuduotai.top/gtkfxgnyoi.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.tian-w.cn/gtztyfmuko.html

JS:   console.error("err")
来源：http://hz.fzhhl.top/gtflaumghq.html

TS:   console.error("err")
来源：http://hz.gzhubu.top/gtobkvwnwb.html

Java: System.err.println("err")
来源：http://hz.ybcxt.top/gtiyczoefs.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.shuidangran.top/gtikhxvvbm.html

Ruby: warn "err"
来源：http://hz.chenzaomai.com/gtxsjdhaie.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.zhongyouzk.top/gtziiinppr.html

[M07] 判断是否为主入口
来源：http://hz.tian-w.cn/gtbseskipk.html

Py:   if __name__ == "__main__":
来源：http://hz.zycfv.cn/gtayzqvshn.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.chenzaomai.com/gtbsempvab.html

JS:   require.main === module
来源：http://hz.shuidangran.top/gtgdqkvetw.html

TS:   require.main === module
来源：http://hz.chenlongwang.top/gtbappvnyc.html

Java: public static void main(String[] args)
来源：http://hz.hfpthk.cn/gtbpyabzdg.html

Go:   func main()
来源：http://hz.daxiang520.top/gthyzlbqkl.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.iojbl.cn/gtzlswkzzi.html

C#:   static void Main(string[] args)
来源：http://hz.gaohongyu789.top/gtqgfrwdtp.html

[M08] 获取系统与运行时信息
来源：http://hz.sysykeji.top/gtnqycazlw.html

Py:   platform.system();  platform.python_version()
来源：http://hz.xingfuxueyuan.xyz/gthldxsrmy.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.tian-w.cn/gtvxrcbtqk.html

JS:   process.platform;  process.version
来源：http://hz.jqgfzy.top/gtpuzaugob.html

TS:   process.platform;  process.version
来源：http://hz.mhx1999.top/gtnmjbdpjb.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.0kj1m.cn/gtvcphpgdx.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.gzhubu.top/gtxuqaoywl.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.redwolf501.top/gtchnhfnpj.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.xinyue.icu/gtswipbcxa.html

================================================================================
来源：http://hz.ybcxt.top/gtpezsvclq.html

N. 数据结构与算法
来源：http://hz.hnxiangtu.top/gtcjxbehel.html

================================================================================
来源：http://hz.zhijiandao.cn/gtykobmcmb.html

[N01] 二分查找（有序数组）
来源：http://hz.zhijiandao.cn/gtqrensgpa.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.nanxinkj.top/gtmwrkjzrq.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.jqgufenzy.top/gtuwdlyasu.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.tanke756.top/gtovnwgfki.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.hammf.cn/gtrmaowuzx.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.c1oappe.top/gtmpjliqjj.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.yangfankeji.com/gtfzhpkszu.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.jqgfzy.top/gttpnmexyv.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.xuetiantiany.cn/gtnvxwqodo.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.zhiwuduotai.top/gtrafhlqns.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.tian-w.cn/gtyxbbbxwf.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.jinqigufen.top/gtjbmjpnbb.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.bjfxy.top/gtqlipbebz.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.yuxming.cn/gtsschilry.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.jlsjyb.cn/gtsdqbtllx.html

Go:   slices.Sort(arr)
来源：http://hz.dashuyun.cn/gtndbuvxoi.html

Ruby: arr.sort
来源：http://hz.chenjidiqi.icu/gtkgkbrxzj.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.smart0.xyz/gtwemzzndp.html

[N03] 快速排序（分治示例）
来源：http://hz.tianlin.xyz/gtnzjxegnw.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.redwolf501.top/gtpwalipdt.html

PHP:  // 递归实现，或用 usort
来源：http://hz.zhixingplan.top/gtriksceih.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.zhixingplan.top/gtwgjrkpel.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.pycfn.com/gtdfnawkwn.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.iojbl.cn/gtjpjfvqba.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.feifeiyinyue.top/gtbxbobkoz.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.xuetiantiany.cn/gttdtqrlbg.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.quarkkingdee.top/gtewinwbuj.html

[N04] 斐波那契数列
来源：http://hz.jinghuilouyu.cn/gtgnvfexml.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.jlsjyb.cn/gtbkitniua.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.hnqzz.top/gtfvnxkira.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.daxiang520.top/gtdtvzfacq.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.iojbl.cn/gtsnugqrgw.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.gaohongyu789.top/gtsxkkltqo.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.fengsongda.top/gtyuctezqe.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.hammf.cn/gtaxauroaq.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.xziqi.cn/gtmbgmqdjn.html

[N05] 最大公约数
来源：http://hz.hammf.cn/gtmzlvxqam.html

Py:   math.gcd(a, b)
来源：http://hz.hnxiangtu.top/gtltzxuwnc.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.ehwqpu.com/gtvnctpghp.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.zycfv.cn/gtngdgkxkg.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.cucudq.cn/gtqiqjvlal.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.cqqwz.cn/gtyeqrdqul.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.shuidangran.top/gtghgnyhqf.html

Ruby: a.gcd(b)
来源：http://hz.xziqi.cn/gtagbxjnbq.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.dianchejie.cn/gtexrpnrza.html

[N06] 判断回文字符串
来源：http://hz.mhx1999.top/gtaoewypub.html

Py:   s == s[::-1]
来源：http://hz.ywan-chungtsiang.top/gthsvmczeu.html

PHP:  $s === strrev($s);
来源：http://hz.aibaodan.cn/gteekwfkun.html

JS:   s === [...s].reverse().join("")
来源：http://hz.316326.xyz/gtmeymuqyu.html

TS:   s === [...s].reverse().join("")
来源：http://hz.nanxinkj.top/gtnvzplplj.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.smart0.xyz/gtpqoyafog.html

Go:   // 双指针从两端比较
来源：http://hz.tianlin.xyz/gtwmsulqkd.html

Ruby: s == s.reverse
来源：http://hz.zhongyouzk.top/gtzpaqyllb.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.hongshengwenyu.top/gtoolkyubt.html

[N07] 两数之和（返回下标）
来源：http://hz.sweek.top/gtfxlaekjx.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.xuetiantiany.cn/gtkvjktzya.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.gotoacloud.top/gtbiwsfleg.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.svipenyu.cn/gtbcccsswn.html

TS:   // 手写 Map<string, number>
来源：http://hz.guowangkeji.top/gtoilwnwtr.html

Java: // 手写 HashMap
来源：http://hz.mhx1999.top/gtmfcmpjvr.html

Go:   // 手写 map[int]int
来源：http://hz.shanyushiyangtech.top/gtyyrmztct.html

Ruby: // 手写 Hash
来源：http://hz.chenjidiqi.icu/gtuhgszemu.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.wangshuangyany.cn/gtuzxhocpe.html

[N08] 生成全排列
来源：http://hz.pengpengdd.cyou/gtxupwuujp.html

Py:   itertools.permutations(arr)
来源：http://hz.jiagoushi.top/gttrwrsgda.html

PHP:  // 手写递归交换
来源：http://hz.yongpay.top/gtkwswzifp.html

JS:   // 手写回溯递归
来源：http://hz.jinqigfzy.top/gtczualvvz.html

TS:   // 手写回溯递归
来源：http://hz.jyoumei.cn/gttjpjpvlv.html

Java: // 手写回溯递归
来源：http://hz.vqdsnc.cn/gtfbcmovuu.html

Go:   // 手写回溯递归
来源：http://hz.jqgufenzy.top/gthxcovmrm.html

Ruby: arr.permutation.to_a
来源：http://hz.xylfe.cn/gtpijimjaq.html

C#:   // 手写回溯递归
来源：http://hz.cdnleiting.top/gtgoehxrrs.html

[N09] 栈与队列
来源：http://hz.jiagoushi.top/gtrsllkaqk.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.hywenlv.cn/gtzruztgxp.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.shanyushiyangtech.top/gtkvkffpws.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.yj20258888.top/gtpdkxohpf.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.jqgfzy.top/gtdfdsalqf.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.zhiwuduotai.top/gtuzgauetg.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.pycfn.com/gtzhszddqm.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.zhoulong.xyz/gtwrrndpuj.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.zhixingplan.top/gtvubvvnfy.html

[N10] 链表节点定义
来源：http://hz.wangshuangyany.cn/gtdonbgskm.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.zdqjudy.top/gtcneclnql.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.sufxvd.cn/gtaiakaezl.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.nanxuanxn.top/gtwhwynzey.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.daxiang520.top/gtlnvszdnh.html

Java: class Node { int v; Node next; }
来源：http://hz.shanyushiyangtech.top/gtetqsieaw.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.cashguo.top/gtvblnupxe.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.ybcxt.top/gtsrknfcvf.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.wangdashe.top/gtcrquiizb.html

[N11] 二叉树中序遍历
来源：http://hz.ehwqpu.com/gtwtbblqto.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.c1oappe.top/gtruqwsfuh.html

PHP:  // 手写递归函数
来源：http://hz.cashguo.top/gtaeozchzf.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.shuidangran.top/gtrqupsteg.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.haohaochexian.top/gtyxpsmmhi.html

Java: // 手写递归
来源：http://hz.pengpengdd.cyou/gtkmfntrbo.html

Go:   // 手写递归
来源：http://hz.cdnleiting.top/gtozutfesw.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.tianlin.xyz/gtklfieksa.html

C#:   // 手写递归
来源：http://hz.yonumen.top/gttautkiiu.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.jinyuanbaomall.cn/gtmvyvfeun.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.dashuyun.cn/gtatrvljjx.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.gogol.net.cn/gtsxnxyhbk.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.shzxlz.cn/gtszfsaatj.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.xuanzx.com/gtsvluwajx.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.jianghu66.top/gteiuqtegc.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.zhiwuduotai.top/gtlhgrjcwj.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.yvedp.cn/gtpderyrzr.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.gogol.net.cn/gtujcdbbit.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtdzkmlenx.html

O. 并发与异步
来源：http://hz.aizwys.cn/gtnsngidjq.html

================================================================================
来源：http://hz.hysaishi.cn/gtlgrmfnyq.html

[O01] 启动一个线程
来源：http://hz.pengpengdd.cyou/gtkaicktrq.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.ppjwa.cn/gtzhqhbnoq.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.dianchejie.cn/gtzzecpnyx.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.cdnleiting.top/gtwdoktfey.html

TS:   // 同 JS
来源：http://hz.guannengcc.top/gteyvpuvhw.html

Java: new Thread(() -> f()).start()
来源：http://hz.ywan-chungtsiang.top/gtophhsrzf.html

Go:   go f()
来源：http://hz.yuxming.cn/gthzxqtahq.html

Ruby: Thread.new { f }
来源：http://hz.kuanghao11.cn/gtpcwtxzfv.html

C#:   Task.Run(() => F());
来源：http://hz.yvedp.cn/gtuinmzyyh.html

[O02] 使用线程池
来源：http://hz.vqdsnc.cn/gtsbeoaqyf.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.zdqjudy.top/gtfkymkozu.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.xingfuxueyuan.xyz/gtywvfcwsb.html

JS:   // worker_threads 线程池
来源：http://hz.andypj.xyz/gtfzxzwmrz.html

TS:   // worker_threads 线程池
来源：http://hz.sweek.top/gtahggsvye.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.bjfxy.top/gtteanrrdj.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.pengpengdd.cyou/gtklzwyznh.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.zycfv.cn/gtpyfnjsna.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.xuetiantiany.cn/gtywamzkim.html

[O03] 加锁保护共享数据
来源：http://hz.zhiwuduotai.top/gtwydhhwhf.html

Py:   with lock: shared += 1
来源：http://hz.zhengqikj.top/gteyzpfvcc.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.zhiwuduotai.top/gtlgsisvdz.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.haohaochexian.top/gttheeiqad.html

TS:   // 同 JS
来源：http://hz.sweek.top/gtpfbxwbzv.html

Java: synchronized (this) { shared++; }
来源：http://hz.birdmap.top/gtcsmtgweb.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.yonumen.top/gtqitxvtfr.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.smart0.xyz/gtxacwjens.html

C#:   lock (gate) { shared++; }
来源：http://hz.hnxiangtu.top/gtbbofhgkm.html

[O04] 定义异步函数并等待
来源：http://hz.dashuyun.cn/gtgqkbeefr.html

Py:   async def f():⏎    await g()
来源：http://hz.meibo888.top/gtrqblkyod.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.smart0.xyz/gtrlyyyafq.html

JS:   async function f() { await g(); }
来源：http://hz.ydzc1.top/gtgxfsbqot.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.zhoulong.xyz/gtqkvmhakm.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.hywenlv.cn/gtomtqgugu.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.316326.xyz/gtunziqjoi.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.tanke756.top/gtattqhlbh.html

C#:   async Task F() { await G(); }
来源：http://hz.hysaishi.cn/gtvxfhtjjt.html

[O05] 并发执行并等待全部完成
来源：http://hz.fengsongda.top/gtqtdjydto.html

Py:   asyncio.gather(*tasks)
来源：http://hz.hammf.cn/gtoqxqiaiv.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.jinqigufen.top/gtaxigxeij.html

JS:   await Promise.all(tasks)
来源：http://hz.sxryk.cn/gtdgbohidq.html

TS:   await Promise.all(tasks)
来源：http://hz.hnqzz.top/gtzsjsmxxj.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.ydzc1.top/gthruwrimd.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.dashuyun.cn/gtbtffsocz.html

Ruby: threads.map(&:join)
来源：http://hz.tianlin.xyz/gtnpzqmqpx.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.zhaomingkeji.xyz/gtvfnotjgt.html

[O06] 使用进程池
来源：http://hz.52xcode.cn/gtgckfzuhn.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.andypj.xyz/gtkicwcrrc.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.jlsjyb.cn/gtedrwhpar.html

JS:   // child_process / cluster 模块
来源：http://hz.xylfe.cn/gtwhrzrtic.html

TS:   // child_process / cluster 模块
来源：http://hz.shanyushiyangtech.top/gtbdaclqmr.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.gaohongyu789.top/gtqsvhuqux.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.fengsongda.top/gtpvhsdjdw.html

Ruby: // fork 块
来源：http://hz.yangfankeji.com/gtnrhhjusk.html

C#:   Parallel.For
来源：http://hz.hysaishi.cn/gtabtsdype.html

================================================================================
来源：http://hz.iojbl.cn/gtzsitwfqy.html

P. 常用工具函数
来源：http://hz.jiagoushi.top/gtrabnjzfu.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtccuzqqma.html

[P01] 生成 UUID
来源：http://hz.cheryme.top/gttbbzsnpj.html

Py:   str(uuid.uuid4())
来源：http://hz.hysaishi.cn/gtbsxvyzrb.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.ywan-chungtsiang.top/gtmqthebld.html

JS:   crypto.randomUUID()
来源：http://hz.jqgfzy.top/gtvxhtyfqq.html

TS:   crypto.randomUUID()
来源：http://hz.yj202588.top/gtozfbhmds.html

Java: UUID.randomUUID().toString()
来源：http://hz.ivvv.top/gtnfofxhku.html

Go:   // 用 github.com/google/uuid
来源：http://hz.birdmap.top/gtdzkddpzs.html

Ruby: SecureRandom.uuid
来源：http://hz.hnxiangtu.top/gthvyspenj.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.tianlin.xyz/gtjhqskaql.html

[P02] MD5 / SHA256 摘要
来源：http://hz.sysykeji.top/gtfsljfega.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.c1oappe.top/gtklnnqjes.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.zdqjudy.top/gtlzlnjjvl.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.zhixingplan.top/gtfymrlxdu.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.hfpthk.cn/gtjsupsbvw.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.0kj1m.cn/gtuviflyvw.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.ehwqpu.com/gtlhyysady.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.pengpengdd.cyou/gtetlxeshb.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.yuanzhike.top/gtrpolcbra.html

[P03] 生成短随机字符串
来源：http://hz.jinghuilouyu.cn/gtqsnhdeho.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.hysaishi.cn/gtvhuyqjat.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.jinqigufen.top/gttwnizvda.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.yonumen.top/gtuwajrovu.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.mhx1999.top/gtsfmvzuho.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.chenjidiqi.icu/gtwnjqcezq.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.yuanzhike.top/gtriinouck.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.jianghu66.top/gtisjwmrcb.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.gaohongyu789.top/gtsikepfqp.html

[P04] 求长度
来源：http://hz.yj20258888.top/gtrjvznhop.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.zhiwuduotai.top/gtdvamhafe.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.zycfv.cn/gtlprgldam.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.yuanzhike.top/gtmlbscokp.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.jlsjyb.cn/gthpvkgjnc.html

Java: list.size();  map.size();  s.length()
来源：http://hz.ydzc1.top/gtmsrxojde.html

Go:   len(arr);  len(m)
来源：http://hz.sweek.top/gtbwcpkxus.html

Ruby: x.length;  x.size
来源：http://hz.sysykeji.top/gtgafiuxsc.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.hnxiangtu.top/gticxdujdo.html

[P05] 判断两个对象内容是否相等
来源：http://hz.zhaomingkeji.xyz/gtpiwoceqj.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.svipenyu.cn/gtxurrlntv.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.hysaishi.cn/gtgjwgfgkj.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.snrcjt.cn/gtljxarzih.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.daxiang520.top/gttrtqqbqf.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.zhiwuduotai.top/gthqjmwfvb.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.zhoulong.xyz/gtqhaxxkrg.html

Ruby: a == b
来源：http://hz.aizwys.cn/gtqwwosxmi.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.ppjwa.cn/gtupdxbbyr.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.52xcode.cn/gtufdyuknj.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.yuxming.cn/gtifapotap.html

PHP:  if (empty($x)) {}
来源：http://hz.cashguo.top/gtvebnzoji.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.xziqi.cn/gtcvrvsxww.html

TS:   if (x == null) {}
来源：http://hz.jinghuilouyu.cn/gtxausrxoh.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.cheryme.top/gtdlnwbipu.html

Go:   if x == nil {}
来源：http://hz.zhixingplan.top/gtqxlndtlh.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.redwolf501.top/gtonlzzdto.html

C#:   if (x is null) {}
来源：http://hz.fengsongda.top/gtevivsvws.html

[P07] 防抖与节流
来源：http://hz.gzhubu.top/gtxcgtwoua.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.jlsjyb.cn/gtjvxlnczn.html

PHP:  // 手写时间戳比较
来源：http://hz.hfpthk.cn/gtsaxcdoxo.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.aizwys.cn/gtmzacqgwh.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.ydjk.org.cn/gtrjgcjfpd.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.andypj.xyz/gtukavkaah.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.chenjidiqi.icu/gtbkosoofx.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.cashguo.top/gtoxzbkadg.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.yvedp.cn/gtuzwqhuac.html

[P08] 处理浮点精度问题
来源：http://hz.shanyushiyangkeji.top/gtxkkweilq.html


<!-- 参考信息 -->