代发 wailian999

Ruby: ARGV
来源：http://hz.hnqzz.top/gtkdmpgoam.html

C#:   args 数组（Main 方法参数）
来源：http://hz.cucudq.cn/gtgqxsblrn.html

[M02] 读取环境变量
来源：http://hz.zhaomingkeji.xyz/gtmeanegcv.html

Py:   os.environ.get("HOME")
来源：http://hz.hysaishi.cn/gtptovnwne.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.sweek.top/gtiavpbfan.html

JS:   process.env.HOME
来源：http://hz.havefunace.top/gtxjigxxde.html

TS:   process.env.HOME
来源：http://hz.ehwqpu.com/gtaldzlane.html

Java: System.getenv("HOME")
来源：http://hz.pycfn.com/gtzdvwakdv.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.zhixingplan.top/gtuniyeoef.html

Ruby: ENV["HOME"]
来源：http://hz.cucudq.cn/gtiuugsntb.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.c1oappe.top/gtbcpuweee.html

[M03] 执行外部命令
来源：http://hz.cdnleiting.top/gtrrhyngjz.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.xuanzx.com/gtxhazndmf.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.guannengcc.top/gtqpgyrwbp.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.0kj1m.cn/gtvjcfbxns.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.ivvv.top/gtviykqheg.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.yj20258888.top/gtfeepelpc.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.tian-w.cn/gtpxtvzwqc.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.yj20258.top/gtgztpkckr.html

C#:   Process.Start("ls", "-l");
来源：http://hz.yuanzhike.top/gtvhpslugo.html

[M04] 获取当前工作目录
来源：http://hz.316326.xyz/gthwafygsr.html

Py:   os.getcwd()
来源：http://hz.smart0.xyz/gtvrgtfqut.html

PHP:  getcwd();
来源：http://hz.smart0.xyz/gtavhdpioz.html

JS:   process.cwd()
来源：http://hz.hongshengwenyu.top/gtzcblwcfz.html

TS:   process.cwd()
来源：http://hz.ywan-chungtsiang.top/gtvuprneju.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.fzhhl.top/gtznondeib.html

Go:   os.Getwd()
来源：http://hz.9152youxi.cn/gtdpyheatj.html

Ruby: Dir.pwd
来源：http://hz.xylfe.cn/gtqkbmpmwx.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.zhoulong.xyz/gtugzshwom.html

[M05] 设置退出码
来源：http://hz.zhoulong.xyz/gtaxiewtff.html

Py:   sys.exit(1)
来源：http://hz.hywenlv.cn/gtmdmvkrsl.html

PHP:  exit(1);
来源：http://hz.chenjidiqi.icu/gtarrwyadc.html

JS:   process.exit(1)
来源：http://hz.meibo888.top/gtfelzkptg.html

TS:   process.exit(1)
来源：http://hz.chenlongwang.top/gthwceivqr.html

Java: System.exit(1)
来源：http://hz.xziqi.cn/gtkvysrzxh.html

Go:   os.Exit(1)
来源：http://hz.sxryk.cn/gtcjikpase.html

Ruby: exit 1
来源：http://hz.jinqigfzy.top/gtsshxgatv.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.gotoacloud.top/gtunfjkdrl.html

[M06] 向标准错误输出
来源：http://hz.c1oappe.top/gtfewyxnml.html

Py:   print("err", file=sys.stderr)
来源：http://hz.jianghu66.top/gtdlbigcep.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.dianchejie.cn/gtrmwnuuud.html

JS:   console.error("err")
来源：http://hz.xziqi.cn/gtozjbnajt.html

TS:   console.error("err")
来源：http://hz.sweek.top/gthspzlree.html

Java: System.err.println("err")
来源：http://hz.yuanzhike.top/gtclwxhsii.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.zycfv.cn/gtxluoalgg.html

Ruby: warn "err"
来源：http://hz.feifeiyinyue.top/gtnpydushq.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.zycfv.cn/gtzvkmooih.html

[M07] 判断是否为主入口
来源：http://hz.yj20258.top/gtsyelthur.html

Py:   if __name__ == "__main__":
来源：http://hz.kuanghao11.cn/gtiojhylai.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.cucudq.cn/gtapqqyuyh.html

JS:   require.main === module
来源：http://hz.nanxuanxn.top/gthqaymadp.html

TS:   require.main === module
来源：http://hz.nanxuanxn.top/gtbykmzcla.html

Java: public static void main(String[] args)
来源：http://hz.daxiang520.top/gtnwsuxvfb.html

Go:   func main()
来源：http://hz.ydjk.org.cn/gtdcdyeqbu.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.daria6918.cn/gtibxnlnqt.html

C#:   static void Main(string[] args)
来源：http://hz.havefunace.top/gtidbkduom.html

[M08] 获取系统与运行时信息
来源：http://hz.ydzc1.top/gtofkfbjiq.html

Py:   platform.system();  platform.python_version()
来源：http://hz.xziqi.cn/gtfcrkzfji.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.zhijiandao.cn/gtjgzjparw.html

JS:   process.platform;  process.version
来源：http://hz.sysykeji.top/gtrlvxouug.html

TS:   process.platform;  process.version
来源：http://hz.quarkkingdee.top/gthfcvlyeg.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.ybcxt.top/gtnrdsskgx.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.jinqigufen.top/gtjlmwbkrt.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.quarkkingdee.top/gtxhkwxkbh.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.iojbl.cn/gtxzzaxili.html

================================================================================
来源：http://hz.zdqjudy.top/gtwsxmfgyp.html

N. 数据结构与算法
来源：http://hz.yongpay.top/gtafsroenr.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtrobuezcu.html

[N01] 二分查找（有序数组）
来源：http://hz.hnxiangtu.top/gtmxluskyo.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.jqgufenzy.top/gtvrwwtyuj.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.ivvv.top/gtjxvwfegh.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.jianghu66.top/gtwddnakgb.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.tanke756.top/gtlkqdbstv.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.hfpthk.cn/gthainzlxg.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.daxiang520.top/gtgotnzvsc.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.birdmap.top/gteunboiil.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.chenjidiqi.icu/gtccvicbsa.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.chenjidiqi.icu/gtuaytzkem.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.shanyushiyangtech.top/gtjmybvzew.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.chenzaomai.com/gtxhtgkbko.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.cucudq.cn/gtmadmhreo.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.zhijiandao.cn/gtugbkenlf.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.feifeiyinyue.top/gteolidrdr.html

Go:   slices.Sort(arr)
来源：http://hz.zdqjudy.top/gtowhotvjv.html

Ruby: arr.sort
来源：http://hz.yongpay.top/gtyendzjea.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.cucudq.cn/gtqwgskkiv.html

[N03] 快速排序（分治示例）
来源：http://hz.zhongyouzk.top/gthcitpqef.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.ydjk.org.cn/gtawcxilsa.html

PHP:  // 递归实现，或用 usort
来源：http://hz.tian-w.cn/gtdbdmcmdx.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.jlsjyb.cn/gtvnizafht.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.nanxuanxn.top/gtflycoept.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.xingfuxueyuan.xyz/gtqntlvyea.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.cashguo.top/gtqnrpobyy.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.zhengqikj.top/gtskieevzz.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.xziqi.cn/gtdcvbwrox.html

[N04] 斐波那契数列
来源：http://hz.zhoulong.xyz/gtvuryrfiu.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.birdmap.top/gtapnoskty.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.shanyushiyangkeji.top/gtqmaoihfc.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.yueranfly.top/gtioqxdqvu.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.jinqigufen.top/gtslbvgodw.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.vqdsnc.cn/gtpdzmlspb.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.jinqigfzy.top/gtygbzqfkp.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.ybcxt.top/gtmqtyfqww.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.yvedp.cn/gtefkumdrd.html

[N05] 最大公约数
来源：http://hz.nwbrower.top/gttwkjeagf.html

Py:   math.gcd(a, b)
来源：http://hz.cucudq.cn/gtgfadxomm.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.ppjwa.cn/gtwrioofjd.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.ydzc1.top/gtiosdrqmu.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.wangdashe.top/gtbtjmhleu.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.kuanghao11.cn/gtjvhjimbr.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.jlsjyb.cn/gtztalsrgq.html

Ruby: a.gcd(b)
来源：http://hz.xingfuxueyuan.xyz/gtwqneemlc.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.gaohongyu789.top/gtzsbwcvkj.html

[N06] 判断回文字符串
来源：http://hz.zhiwuduotai.top/gttrdevhnz.html

Py:   s == s[::-1]
来源：http://hz.jqgufenzy.top/gtgholoebo.html

PHP:  $s === strrev($s);
来源：http://hz.0kj1m.cn/gtvdeehvrn.html

JS:   s === [...s].reverse().join("")
来源：http://hz.c1oappe.top/gtugccyser.html

TS:   s === [...s].reverse().join("")
来源：http://hz.yuanzhike.top/gtxfgwmpjb.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.jqgufenzy.top/gtzzyklzsa.html

Go:   // 双指针从两端比较
来源：http://hz.jqgfzy.top/gtsuhwnfem.html

Ruby: s == s.reverse
来源：http://hz.hongshengwenyu.top/gtwuxuntri.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.xuanzx.com/gtmgufmzdd.html

[N07] 两数之和（返回下标）
来源：http://hz.cucudq.cn/gthwkrzuqu.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.cqqwz.cn/gtvxrqdibd.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.redwolf501.top/gtifjsppkk.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.ydzc1.top/gtzytgczca.html

TS:   // 手写 Map<string, number>
来源：http://hz.dashuyun.cn/gtehtlgofy.html

Java: // 手写 HashMap
来源：http://hz.guowangkeji.top/gtonsuwsrn.html

Go:   // 手写 map[int]int
来源：http://hz.guannengcc.top/gtugankvod.html

Ruby: // 手写 Hash
来源：http://hz.yangfankeji.com/gthdfynxkw.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.jinqigfzy.top/gtqkxkfmry.html

[N08] 生成全排列
来源：http://hz.zhiwuduotai.top/gtxzwlvucb.html

Py:   itertools.permutations(arr)
来源：http://hz.guannengcc.top/gtvnxyzifo.html

PHP:  // 手写递归交换
来源：http://hz.bjfxy.top/gtuasocltb.html

JS:   // 手写回溯递归
来源：http://hz.jinqigfzy.top/gtsbhhwywk.html

TS:   // 手写回溯递归
来源：http://hz.cashguo.top/gthyxccfrh.html

Java: // 手写回溯递归
来源：http://hz.zhaomingkeji.xyz/gtdhuamcjs.html

Go:   // 手写回溯递归
来源：http://hz.jinghuilouyu.cn/gtdrcgwhpp.html

Ruby: arr.permutation.to_a
来源：http://hz.chenzaomai.com/gtiaesiyaq.html

C#:   // 手写回溯递归
来源：http://hz.chenlongwang.top/gtvyilmbkl.html

[N09] 栈与队列
来源：http://hz.nanxinkj.top/gtabphamdq.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.jqgfzy.top/gtwpjasrxq.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.tianlin.xyz/gtruunuufj.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.xinyue.icu/gtdqzaaohr.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.daria6918.cn/gtcchnbrfs.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.havefunace.top/gtabtokiyf.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.ppjwa.cn/gtlamyjpap.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.hywenlv.cn/gtgtfryeqt.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.ehwqpu.com/gtjwtalghc.html

[N10] 链表节点定义
来源：http://hz.jinqigufen.top/gthbmhdibh.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.c1oappe.top/gtmjrwyuqc.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.svipenyu.cn/gtfxzuyxpu.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.cucudq.cn/gtzrtokatz.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.redwolf501.top/gtdhkyefxi.html

Java: class Node { int v; Node next; }
来源：http://hz.chenzaomai.com/gtyekxsjwz.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.hywenlv.cn/gttjenluas.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.cqqwz.cn/gtzlhpzkie.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.0kj1m.cn/gtunehfexp.html

[N11] 二叉树中序遍历
来源：http://hz.yuanzhike.top/gtbnhnifew.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.cheryme.top/gtjexvxhyh.html

PHP:  // 手写递归函数
来源：http://hz.hfpthk.cn/gtbrkatiyr.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.sysykeji.top/gtgrnoqnfb.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.tianlin.xyz/gtgybkoxmh.html

Java: // 手写递归
来源：http://hz.chenlongwang.top/gtqjdxwaco.html

Go:   // 手写递归
来源：http://hz.nanxinkj.top/gtghjfppmx.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.sysykeji.top/gtaezgaeri.html

C#:   // 手写递归
来源：http://hz.sxryk.cn/gtnldlgwko.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.mhx1999.top/gtbarewywt.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.wangdashe.top/gtluhtaqdk.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.gotoacloud.top/gtcrrzwtww.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.gotoacloud.top/gtzwhyyvea.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.jlsjyb.cn/gtfmcmfymk.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.svipenyu.cn/gtmxpiohjh.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.zycfv.cn/gtysahmcpd.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.yj20258.top/gtctxtlzen.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.shanyushiyangkeji.top/gtobfgddnl.html

================================================================================
来源：http://hz.iojbl.cn/gtcyfczfga.html

O. 并发与异步
来源：http://hz.zhongyouzk.top/gtweuclwcf.html

================================================================================
来源：http://hz.yj20258888.top/gtlpdcmouu.html

[O01] 启动一个线程
来源：http://hz.nanxinkj.top/gtigywovpz.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.shuidangran.top/gtkrsvpskz.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.9152youxi.cn/gtwdzuklzp.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.zhongyouzk.top/gtfhgxfbrw.html

TS:   // 同 JS
来源：http://hz.sufxvd.cn/gtqswvmygr.html

Java: new Thread(() -> f()).start()
来源：http://hz.svipenyu.cn/gtdyweiisr.html

Go:   go f()
来源：http://hz.nanxuanxn.top/gtaupgncnb.html

Ruby: Thread.new { f }
来源：http://hz.zhijiandao.cn/gtjjjwmxfg.html

C#:   Task.Run(() => F());
来源：http://hz.guowangkeji.top/gtjejqoqhm.html

[O02] 使用线程池
来源：http://hz.shanyushiyangkeji.top/gtdarjfgvy.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.9152youxi.cn/gtaejtjcky.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.hywenlv.cn/gtkjszejlc.html

JS:   // worker_threads 线程池
来源：http://hz.xziqi.cn/gtwwrdipod.html

TS:   // worker_threads 线程池
来源：http://hz.shuidangran.top/gthlkybtnv.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.zhoulong.xyz/gtogkjfqxo.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.yongpay.top/gthxrjhqzs.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.yonumen.top/gtozfrbyib.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.ydzc1.top/gtzhfoxofx.html

[O03] 加锁保护共享数据
来源：http://hz.yangfankeji.com/gtswvowvdo.html

Py:   with lock: shared += 1
来源：http://hz.yueranfly.top/gtogdxbdrj.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.daria6918.cn/gthliukhtp.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.jianghu66.top/gtvywcrfuy.html

TS:   // 同 JS
来源：http://hz.chenlongwang.top/gtgznfmazl.html

Java: synchronized (this) { shared++; }
来源：http://hz.jlsjyb.cn/gtrodfymlh.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.jianghu66.top/gtbejtibaq.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.jlsjyb.cn/gteknpgdgj.html

C#:   lock (gate) { shared++; }
来源：http://hz.pengpengdd.cyou/gtogegghjk.html

[O04] 定义异步函数并等待
来源：http://hz.jiagoushi.top/gtxlujexgt.html

Py:   async def f():⏎    await g()
来源：http://hz.jianghu66.top/gtxzuojewl.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.jinghuilouyu.cn/gtqzfqdoym.html

JS:   async function f() { await g(); }
来源：http://hz.hnxiangtu.top/gtdibsmlmw.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.hywenlv.cn/gtaogbxugy.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.cheryme.top/gthsvtskyj.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.svipenyu.cn/gtebdokghp.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.ywan-chungtsiang.top/gtslgfppkt.html

C#:   async Task F() { await G(); }
来源：http://hz.haohaochexian.top/gtbzuvzkko.html

[O05] 并发执行并等待全部完成
来源：http://hz.chenzaomai.com/gtsjurwqoh.html

Py:   asyncio.gather(*tasks)
来源：http://hz.jlsjyb.cn/gtgmkcmqdd.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.gogol.net.cn/gttbnqavpf.html

JS:   await Promise.all(tasks)
来源：http://hz.zycfv.cn/gtogzayqkx.html

TS:   await Promise.all(tasks)
来源：http://hz.bjfxy.top/gtmtllerwa.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.havefunace.top/gtlqxmkloj.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.hywenlv.cn/gtiuatvlsd.html

Ruby: threads.map(&:join)
来源：http://hz.feifeiyinyue.top/gtsjfbqipc.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.guannengcc.top/gtmpneagpd.html

[O06] 使用进程池
来源：http://hz.meibo888.top/gtekccufwb.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.birdmap.top/gtbnnheror.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.dianchejie.cn/gtsisjzuad.html

JS:   // child_process / cluster 模块
来源：http://hz.ybcxt.top/gttcgodrfd.html

TS:   // child_process / cluster 模块
来源：http://hz.52xcode.cn/gtokfbnpwl.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.feifeiyinyue.top/gtbopswktp.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.ybcxt.top/gtgmwacajg.html

Ruby: // fork 块
来源：http://hz.chenzaomai.com/gtyflwvika.html

C#:   Parallel.For
来源：http://hz.jinqigfzy.top/gtwjtrmjut.html

================================================================================
来源：http://hz.daxiang520.top/gtzttrxkja.html

P. 常用工具函数
来源：http://hz.xuanzx.com/gtdowklkac.html

================================================================================
来源：http://hz.jiagoushi.top/gtwlbjfmde.html

[P01] 生成 UUID
来源：http://hz.zhiwuduotai.top/gtkikriart.html

Py:   str(uuid.uuid4())
来源：http://hz.kuanghao11.cn/gtsertrwuc.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.chenjidiqi.icu/gtqbxqueya.html

JS:   crypto.randomUUID()
来源：http://hz.feifeiyinyue.top/gtjkmtpuup.html

TS:   crypto.randomUUID()
来源：http://hz.jiagoushi.top/gtdjkzxwkl.html

Java: UUID.randomUUID().toString()
来源：http://hz.shanyushiyangtech.top/gtjgiestmq.html

Go:   // 用 github.com/google/uuid
来源：http://hz.52xcode.cn/gtnvdlwqhp.html

Ruby: SecureRandom.uuid
来源：http://hz.daria6918.cn/gtbzsnjdyi.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.ehwqpu.com/gtaffvoywf.html

[P02] MD5 / SHA256 摘要
来源：http://hz.pengpengdd.cyou/gtecrwtkum.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.yvedp.cn/gtghbvkvqy.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.gaohongyu789.top/gtvgzcwzae.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.gogol.net.cn/gtcdlynfmm.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.sysykeji.top/gtxxpvvxbw.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.meibo888.top/gtuybndzpg.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.zhengqikj.top/gtxwwmpypd.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.316326.xyz/gttasdkxac.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.shanyushiyangtech.top/gtlgvcfnep.html

[P03] 生成短随机字符串
来源：http://hz.jianghu66.top/gtzetbwspx.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.jinghuilouyu.cn/gtzzilbten.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.9152youxi.cn/gtezqogmqe.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.yj202588.top/gttoudfknz.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.cdnleiting.top/gtezchyytk.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.feifeiyinyue.top/gtybiyoujq.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.tanke756.top/gtldajywke.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.ehwqpu.com/gtezcqegxl.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.ywan-chungtsiang.top/gtcypwccui.html

[P04] 求长度
来源：http://hz.jinyuanbaomall.cn/gtlotitcgp.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.fzhhl.top/gtoqhmdafl.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.zhongyouzk.top/gtkegjngda.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.zhaomingkeji.xyz/gtomgopcwu.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.mhx1999.top/gtsoswlaqb.html

Java: list.size();  map.size();  s.length()
来源：http://hz.zhoulong.xyz/gtflmkivcs.html

Go:   len(arr);  len(m)
来源：http://hz.xziqi.cn/gthjhwkbjw.html

Ruby: x.length;  x.size
来源：http://hz.meibo888.top/gtbvmqywyn.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.xuanzx.com/gtlgjgruzu.html

[P05] 判断两个对象内容是否相等
来源：http://hz.yuanzhike.top/gtzivkvdij.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.wangshuangyany.cn/gtzdvmvmio.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.nwbrower.top/gtgiwyvyvm.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.chenjidiqi.icu/gtkdqhmqov.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.0kj1m.cn/gtrmdtwcqy.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.xziqi.cn/gtzjsmreth.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.cucudq.cn/gtttdzmavk.html

Ruby: a == b
来源：http://hz.ybcxt.top/gtcxlkypen.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.jinqigufen.top/gtuptmahfn.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.yanxiufei.cn/gtstpztueo.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.quarkkingdee.top/gtiqsdbgja.html

PHP:  if (empty($x)) {}
来源：http://hz.zhoulong.xyz/gttpaxokxp.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.jinyuanbaomall.cn/gtlqileynr.html

TS:   if (x == null) {}
来源：http://hz.jlsjyb.cn/gtfkemwnng.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.smart0.xyz/gtkuyathak.html

Go:   if x == nil {}
来源：http://hz.zdqjudy.top/gtgsbsoija.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.zhongyouzk.top/gtujqiefax.html

C#:   if (x is null) {}
来源：http://hz.andypj.xyz/gthhejkllx.html

[P07] 防抖与节流
来源：http://hz.nwbrower.top/gtjbroabzb.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.nanxinkj.top/gtzitwjnfr.html

PHP:  // 手写时间戳比较
来源：http://hz.dianchejie.cn/gtbmomqlhb.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.quarkkingdee.top/gtppzrtsip.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.snrcjt.cn/gtjzluaudn.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.ywan-chungtsiang.top/gtvlzcuyqs.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.xuanzx.com/gtyqyykdhb.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.aizwys.cn/gtaedefooh.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.ybcxt.top/gtnwbicwpn.html

[P08] 处理浮点精度问题
来源：http://hz.gzhubu.top/gtqglbycvn.html


<!-- 参考信息 -->