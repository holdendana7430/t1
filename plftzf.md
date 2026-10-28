代发 wailian999

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.tianlin.xyz/gtletxclxm.html

JS:   process.env.HOME
来源：http://hz.shanyushiyangtech.top/gtyyotikpm.html

TS:   process.env.HOME
来源：http://hz.sweek.top/gtmbkaptde.html

Java: System.getenv("HOME")
来源：http://hz.cdnleiting.top/gtbcjrjbyu.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.haohaochexian.top/gtpaojuksf.html

Ruby: ENV["HOME"]
来源：http://hz.jinyuanbaomall.cn/gtsbyesyra.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.aizwys.cn/gthsvqqxuq.html

[M03] 执行外部命令
来源：http://hz.sysykeji.top/gtctgyuvfc.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.zhoulong.xyz/gtolgugwyg.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.hnxiangtu.top/gtrrymuscq.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.aibaodan.cn/gtzzqyczqz.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.cucudq.cn/gtgwtepbdv.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.nanxinkj.top/gtncsysako.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.zhixingplan.top/gthudezjnc.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.jinqigfzy.top/gtuyjdwmgz.html

C#:   Process.Start("ls", "-l");
来源：http://hz.guannengcc.top/gtwfadbktm.html

[M04] 获取当前工作目录
来源：http://hz.shuidangran.top/gtaytfaxsa.html

Py:   os.getcwd()
来源：http://hz.aizwys.cn/gticsyqmjg.html

PHP:  getcwd();
来源：http://hz.ydzc1.top/gtmygpexqf.html

JS:   process.cwd()
来源：http://hz.feifeiyinyue.top/gtnmzyorjh.html

TS:   process.cwd()
来源：http://hz.yonumen.top/gtiueppnmj.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.jqgufenzy.top/gtxyewlrte.html

Go:   os.Getwd()
来源：http://hz.yanxiufei.cn/gtwqvmyhxa.html

Ruby: Dir.pwd
来源：http://hz.zycfv.cn/gtkktpthbf.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.birdmap.top/gtdnjrxexo.html

[M05] 设置退出码
来源：http://hz.jyoumei.cn/gtdydmjwus.html

Py:   sys.exit(1)
来源：http://hz.dashuyun.cn/gtourshlht.html

PHP:  exit(1);
来源：http://hz.svipenyu.cn/gtsbgrdiiv.html

JS:   process.exit(1)
来源：http://hz.redwolf501.top/gtqpubywea.html

TS:   process.exit(1)
来源：http://hz.gotoacloud.top/gtxburxdwd.html

Java: System.exit(1)
来源：http://hz.ybcxt.top/gthzgetbjr.html

Go:   os.Exit(1)
来源：http://hz.gzhubu.top/gtzxzcxjfa.html

Ruby: exit 1
来源：http://hz.sufxvd.cn/gtxgapufda.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.yvedp.cn/gtmscknmhi.html

[M06] 向标准错误输出
来源：http://hz.gogol.net.cn/gtqenzzsll.html

Py:   print("err", file=sys.stderr)
来源：http://hz.vqdsnc.cn/gtnlmipsmt.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.ppjwa.cn/gtdutmssiz.html

JS:   console.error("err")
来源：http://hz.gzhubu.top/gtywkjxfhs.html

TS:   console.error("err")
来源：http://hz.hysaishi.cn/gtxoxhllyw.html

Java: System.err.println("err")
来源：http://hz.tian-w.cn/gtwayhybbf.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.guowangkeji.top/gtexlvojkb.html

Ruby: warn "err"
来源：http://hz.quarkkingdee.top/gttacuexuf.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.sxryk.cn/gtombzjfla.html

[M07] 判断是否为主入口
来源：http://hz.yj202588.top/gttvbqjpdz.html

Py:   if __name__ == "__main__":
来源：http://hz.birdmap.top/gthfkwkmxt.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.jinghuilouyu.cn/gtlwiiragb.html

JS:   require.main === module
来源：http://hz.yanxiufei.cn/gtkugyefkl.html

TS:   require.main === module
来源：http://hz.guowangkeji.top/gtlvofvanc.html

Java: public static void main(String[] args)
来源：http://hz.zhongyouzk.top/gtkrqesfoj.html

Go:   func main()
来源：http://hz.shangyingyoupin.top/gtupnyagnr.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.yuanzhike.top/gtjpfavnqn.html

C#:   static void Main(string[] args)
来源：http://hz.daria6918.cn/gtjlpgupix.html

[M08] 获取系统与运行时信息
来源：http://hz.sufxvd.cn/gtzxbjwhuz.html

Py:   platform.system();  platform.python_version()
来源：http://hz.zhongyouzk.top/gtmzgrybjd.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.quarkkingdee.top/gtnswwudpg.html

JS:   process.platform;  process.version
来源：http://hz.xuanzx.com/gtukrjusbh.html

TS:   process.platform;  process.version
来源：http://hz.jlsjyb.cn/gtzvynqfmk.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.cheryme.top/gtnculhcxi.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.cdnleiting.top/gtsaotlutx.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.shangyingyoupin.top/gtukrsacdh.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.snrcjt.cn/gtgaoadujy.html

================================================================================
来源：http://hz.bjfxy.top/gtonoqqeri.html

N. 数据结构与算法
来源：http://hz.yuanzhike.top/gtndittguh.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtprwvbdmh.html

[N01] 二分查找（有序数组）
来源：http://hz.ybcxt.top/gtieevbdxa.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.chenjidiqi.icu/gtitnilvul.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.shanyushiyangtech.top/gtrhcbpptb.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.zhixingplan.top/gtvwatvtlc.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.birdmap.top/gtycvslrqa.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.hammf.cn/gtviouleoj.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.kuanghao11.cn/gtnlmdjhcu.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.guowangkeji.top/gtmpcdiirx.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.cdnleiting.top/gtahxjmtdy.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.hnqzz.top/gtuvhpukgs.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.gaohongyu789.top/gttnehfonj.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.shuidangran.top/gtljskxxew.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.jinyuanbaomall.cn/gtxxlrjiwl.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.cdnleiting.top/gtnzbmjofc.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.jinyuanbaomall.cn/gtpwaqnyhk.html

Go:   slices.Sort(arr)
来源：http://hz.9152youxi.cn/gtwoziwekl.html

Ruby: arr.sort
来源：http://hz.ehwqpu.com/gtrblzvtvo.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.redwolf501.top/gtawalludc.html

[N03] 快速排序（分治示例）
来源：http://hz.vqdsnc.cn/gtzmwrkphh.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.yanxiufei.cn/gtjyarvfri.html

PHP:  // 递归实现，或用 usort
来源：http://hz.tian-w.cn/gtpzpenrmh.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.jqgfzy.top/gttzagnonh.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.jyoumei.cn/gtcghbcutr.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.daxiang520.top/gtanmvwtsd.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.chenlongwang.top/gtlzskmgfu.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.tian-w.cn/gthcezdcjy.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.yanxiufei.cn/gtuyqzfkfn.html

[N04] 斐波那契数列
来源：http://hz.shanyushiyangkeji.top/gtdufocevc.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.zhongyouzk.top/gtysjvrobk.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.zdqjudy.top/gtkgrixpuo.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.yj20258888.top/gtivqpgmdi.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.svipenyu.cn/gtugmtbjeu.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.jqgufenzy.top/gtdywypzhz.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.ybcxt.top/gthogzfcen.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.jianghu66.top/gtriwudwhm.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.quarkkingdee.top/gtrazclnmk.html

[N05] 最大公约数
来源：http://hz.yongpay.top/gtehonzehs.html

Py:   math.gcd(a, b)
来源：http://hz.zdqjudy.top/gtaimrfffm.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.pycfn.com/gtbwttmuzn.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.yj20258888.top/gtfflshnrh.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.shanyushiyangkeji.top/gtgigkmwkf.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.hysaishi.cn/gtoivxgudv.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.yuxming.cn/gtcwmssuyv.html

Ruby: a.gcd(b)
来源：http://hz.smart0.xyz/gtblwrmqht.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.sxryk.cn/gtiohyriug.html

[N06] 判断回文字符串
来源：http://hz.wangshuangyany.cn/gtwbcdczgu.html

Py:   s == s[::-1]
来源：http://hz.svipenyu.cn/gtwkpcpogm.html

PHP:  $s === strrev($s);
来源：http://hz.zhixingplan.top/gtsypcpabk.html

JS:   s === [...s].reverse().join("")
来源：http://hz.dianchejie.cn/gtyfurfyei.html

TS:   s === [...s].reverse().join("")
来源：http://hz.nanxinkj.top/gtzbttshal.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.c1oappe.top/gtkhwhcayi.html

Go:   // 双指针从两端比较
来源：http://hz.guannengcc.top/gtjmexqmcf.html

Ruby: s == s.reverse
来源：http://hz.jianghu66.top/gtmwhlfjqx.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.yj202588.top/gtlthrcghh.html

[N07] 两数之和（返回下标）
来源：http://hz.chenzaomai.com/gtulqxkjnq.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.shangyingyoupin.top/gtleqccqcz.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.zycfv.cn/gtqbaviqvm.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.xziqi.cn/gtizarpces.html

TS:   // 手写 Map<string, number>
来源：http://hz.cucudq.cn/gtjfpavpeo.html

Java: // 手写 HashMap
来源：http://hz.xziqi.cn/gtklwgovdz.html

Go:   // 手写 map[int]int
来源：http://hz.gzhubu.top/gtrcwounkq.html

Ruby: // 手写 Hash
来源：http://hz.wangshuangyany.cn/gtacxpsgln.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.svipenyu.cn/gthlfohadh.html

[N08] 生成全排列
来源：http://hz.cashguo.top/gtgpdlmqmh.html

Py:   itertools.permutations(arr)
来源：http://hz.shuidangran.top/gttfinmhka.html

PHP:  // 手写递归交换
来源：http://hz.jinqigufen.top/gtlympoypv.html

JS:   // 手写回溯递归
来源：http://hz.zhengqikj.top/gtoiklmsim.html

TS:   // 手写回溯递归
来源：http://hz.tianlin.xyz/gtmycfidrn.html

Java: // 手写回溯递归
来源：http://hz.redwolf501.top/gtecfokcup.html

Go:   // 手写回溯递归
来源：http://hz.0kj1m.cn/gtezxoxegc.html

Ruby: arr.permutation.to_a
来源：http://hz.gotoacloud.top/gttyoeacul.html

C#:   // 手写回溯递归
来源：http://hz.ydjk.org.cn/gtanjkpvtt.html

[N09] 栈与队列
来源：http://hz.zhiwuduotai.top/gthfikhoif.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.ehwqpu.com/gtkufemkty.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.iojbl.cn/gtoosqdaic.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.ehwqpu.com/gtixybbcjp.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.cheryme.top/gtcstxwaky.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.shanyushiyangkeji.top/gtqelgspra.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.ywan-chungtsiang.top/gtgfpcctit.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.yangfankeji.com/gtgymveskd.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.hnqzz.top/gtguxrudir.html

[N10] 链表节点定义
来源：http://hz.xylfe.cn/gtonlpmwgc.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.fengsongda.top/gtfajcvihz.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.iojbl.cn/gttyodwocw.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.yongpay.top/gtalqgydfg.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.mhx1999.top/gtupqbjnue.html

Java: class Node { int v; Node next; }
来源：http://hz.meibo888.top/gttyvwcprl.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.316326.xyz/gtqctgoivk.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.jinqigufen.top/gtcsbngjgs.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.havefunace.top/gtdbtpihro.html

[N11] 二叉树中序遍历
来源：http://hz.zhaomingkeji.xyz/gtmtgssjpd.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.0kj1m.cn/gtxstvsoac.html

PHP:  // 手写递归函数
来源：http://hz.yvedp.cn/gtmunkdisf.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.sufxvd.cn/gteoybgggz.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.xinyue.icu/gtkqordvaf.html

Java: // 手写递归
来源：http://hz.aibaodan.cn/gtjwhbkarc.html

Go:   // 手写递归
来源：http://hz.yvedp.cn/gttyoztvmf.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.daxiang520.top/gtzqylckck.html

C#:   // 手写递归
来源：http://hz.jinqigfzy.top/gtsuiuockp.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.hnqzz.top/gtnjtrpnap.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.aizwys.cn/gtviwsdzht.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.sysykeji.top/gtoeatksgi.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.nwbrower.top/gtcejflsol.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.jlsjyb.cn/gtqycrcqvc.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.xingfuxueyuan.xyz/gtsarzcggj.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.mhx1999.top/gtpxkhdbsk.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.wangdashe.top/gtvczvtloz.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.dashuyun.cn/gtljpjnojn.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtenhjfbtx.html

O. 并发与异步
来源：http://hz.aizwys.cn/gtduvaidci.html

================================================================================
来源：http://hz.sxryk.cn/gtljiymfnt.html

[O01] 启动一个线程
来源：http://hz.kuanghao11.cn/gtgnifuskh.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.shangyingyoupin.top/gtigomtawx.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.ivvv.top/gtlcvbumnr.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.yonumen.top/gtuhzhmmxk.html

TS:   // 同 JS
来源：http://hz.shuidangran.top/gtndrwhynz.html

Java: new Thread(() -> f()).start()
来源：http://hz.aizwys.cn/gtmvjzrwaf.html

Go:   go f()
来源：http://hz.zhijiandao.cn/gtndnakutw.html

Ruby: Thread.new { f }
来源：http://hz.hysaishi.cn/gtlhrtlunw.html

C#:   Task.Run(() => F());
来源：http://hz.xziqi.cn/gtwricaxxn.html

[O02] 使用线程池
来源：http://hz.jinyuanbaomall.cn/gtwvhozwzi.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.andypj.xyz/gtgzleojcy.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.tian-w.cn/gtggqsysyd.html

JS:   // worker_threads 线程池
来源：http://hz.xingfuxueyuan.xyz/gtklusuocf.html

TS:   // worker_threads 线程池
来源：http://hz.yj20258.top/gtakijbhxz.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.chenlongwang.top/gtscsivbmb.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.tanke756.top/gtyddwvdfe.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.ydjk.org.cn/gtknmzbjwg.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.yuxming.cn/gtlmnlgdwy.html

[O03] 加锁保护共享数据
来源：http://hz.316326.xyz/gtptsaragm.html

Py:   with lock: shared += 1
来源：http://hz.zycfv.cn/gtehzxeyet.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.quarkkingdee.top/gtajusvffm.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.quarkkingdee.top/gtiqlbpumn.html

TS:   // 同 JS
来源：http://hz.yj20258888.top/gtvfufinxe.html

Java: synchronized (this) { shared++; }
来源：http://hz.pengpengdd.cyou/gtauaxktee.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.redwolf501.top/gtpsodcxph.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.pycfn.com/gtljpkopgt.html

C#:   lock (gate) { shared++; }
来源：http://hz.ybcxt.top/gtyzisrmqu.html

[O04] 定义异步函数并等待
来源：http://hz.hnxiangtu.top/gtxbkhuflb.html

Py:   async def f():⏎    await g()
来源：http://hz.0kj1m.cn/gtjggslywt.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.zhijiandao.cn/gtxmztgyxq.html

JS:   async function f() { await g(); }
来源：http://hz.shanyushiyangtech.top/gttqehohqi.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.dianchejie.cn/gtjmgxvtqv.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.tian-w.cn/gttcgdwznn.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.shanyushiyangtech.top/gtllmrqykb.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.nanxinkj.top/gtmwwvhejd.html

C#:   async Task F() { await G(); }
来源：http://hz.yanxiufei.cn/gtgvherreb.html

[O05] 并发执行并等待全部完成
来源：http://hz.jianghu66.top/gtnughcidw.html

Py:   asyncio.gather(*tasks)
来源：http://hz.chenjidiqi.icu/gtpbjsladr.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.gotoacloud.top/gtujjnmtnb.html

JS:   await Promise.all(tasks)
来源：http://hz.feifeiyinyue.top/gtssssklur.html

TS:   await Promise.all(tasks)
来源：http://hz.svipenyu.cn/gtouejyodp.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.pycfn.com/gtiniqetfk.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.dashuyun.cn/gtesfwfwqe.html

Ruby: threads.map(&:join)
来源：http://hz.pengpengdd.cyou/gtyjuniujo.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.cashguo.top/gtqzkcdvhm.html

[O06] 使用进程池
来源：http://hz.yanxiufei.cn/gtgbkkgnlm.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.xuanzx.com/gtjmbqjujb.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.yuxming.cn/gtwlnfokvk.html

JS:   // child_process / cluster 模块
来源：http://hz.daria6918.cn/gtycsqctnd.html

TS:   // child_process / cluster 模块
来源：http://hz.ehwqpu.com/gtpfduwzzq.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.shanyushiyangtech.top/gtyzbkfrqv.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.xziqi.cn/gtwtfqzcgs.html

Ruby: // fork 块
来源：http://hz.tianlin.xyz/gtlbifebsb.html

C#:   Parallel.For
来源：http://hz.nanxuanxn.top/gtiukttzfw.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtghtrhend.html

P. 常用工具函数
来源：http://hz.zhixingplan.top/gtxmkeqzuf.html

================================================================================
来源：http://hz.zycfv.cn/gtxvgglykf.html

[P01] 生成 UUID
来源：http://hz.tianlin.xyz/gtujfmbuqi.html

Py:   str(uuid.uuid4())
来源：http://hz.shuidangran.top/gtwqhylxmr.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.fengsongda.top/gttsunybsu.html

JS:   crypto.randomUUID()
来源：http://hz.hnxiangtu.top/gtjjqnjorl.html

TS:   crypto.randomUUID()
来源：http://hz.zycfv.cn/gtsrvrcumt.html

Java: UUID.randomUUID().toString()
来源：http://hz.feifeiyinyue.top/gtxypouvyk.html

Go:   // 用 github.com/google/uuid
来源：http://hz.gaohongyu789.top/gtehjcugcb.html

Ruby: SecureRandom.uuid
来源：http://hz.ybcxt.top/gtqvzdehlk.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.tianlin.xyz/gtxszishlb.html

[P02] MD5 / SHA256 摘要
来源：http://hz.jinqigfzy.top/gtfbqzrond.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.cheryme.top/gtvzpqlfoq.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.vqdsnc.cn/gtyaxigjlr.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.cheryme.top/gtvelnklop.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.cashguo.top/gtoytklmno.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.ywan-chungtsiang.top/gtmqjvdvoi.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.dianchejie.cn/gtpidtjoot.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.hongshengwenyu.top/gtqpjgvsuy.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.gogol.net.cn/gtfrmancng.html

[P03] 生成短随机字符串
来源：http://hz.hfpthk.cn/gtjdlkyxzx.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.zhoulong.xyz/gtaeippzkw.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.xylfe.cn/gtrsqfeytf.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.hnxiangtu.top/gtyszgvlob.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.yuanzhike.top/gtrbdtdnbt.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.jinghuilouyu.cn/gtxuhcregw.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.dianchejie.cn/gtbnxejgea.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.hongshengwenyu.top/gtvegfjtqa.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.chenjidiqi.icu/gttxwkvgdm.html

[P04] 求长度
来源：http://hz.zhoulong.xyz/gtsenatipf.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.quarkkingdee.top/gtsnlpcbac.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.xuanzx.com/gtxkvaqxme.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.zycfv.cn/gtauqekvlu.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.zhijiandao.cn/gtdgkuyqbg.html

Java: list.size();  map.size();  s.length()
来源：http://hz.9152youxi.cn/gtlgqpdejl.html

Go:   len(arr);  len(m)
来源：http://hz.dianchejie.cn/gtdqhicakt.html

Ruby: x.length;  x.size
来源：http://hz.zhengqikj.top/gtokskophb.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.dianchejie.cn/gtduylvxka.html

[P05] 判断两个对象内容是否相等
来源：http://hz.hnqzz.top/gtypyqtzun.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.zhiwuduotai.top/gtnfgwtjtj.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.chenlongwang.top/gtbhdadjbv.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.xuetiantiany.cn/gtopykrsmt.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.yj202588.top/gtqtbpnumv.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.xylfe.cn/gtzlntasev.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.zycfv.cn/gtzbgemwwo.html

Ruby: a == b
来源：http://hz.zycfv.cn/gtxdfcvjis.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.svipenyu.cn/gtgbhxoaqv.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.sweek.top/gtudvlfjhg.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.redwolf501.top/gtgbilyhuc.html

PHP:  if (empty($x)) {}
来源：http://hz.jinyuanbaomall.cn/gtravtytnz.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.cqqwz.cn/gtcueubalp.html

TS:   if (x == null) {}
来源：http://hz.aizwys.cn/gtuuobherk.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.aibaodan.cn/gtyjejkzpc.html

Go:   if x == nil {}
来源：http://hz.daxiang520.top/gttghzaptf.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.xziqi.cn/gtourlzmgy.html

C#:   if (x is null) {}
来源：http://hz.quarkkingdee.top/gtdqofudod.html

[P07] 防抖与节流
来源：http://hz.pycfn.com/gtdkingbku.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.shanyushiyangkeji.top/gtlwiqzaek.html

PHP:  // 手写时间戳比较
来源：http://hz.0kj1m.cn/gtudznssbu.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.snrcjt.cn/gtkxtejilr.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.dashuyun.cn/gtveqaekvr.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.daxiang520.top/gtvhulxtgc.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.jinqigufen.top/gtkdzlgfnr.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.jyoumei.cn/gtadqvvbyl.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.ywan-chungtsiang.top/gtxvksbmxg.html

[P08] 处理浮点精度问题
来源：http://hz.gotoacloud.top/gtzwayjxtn.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.hnxiangtu.top/gtjsrfubeu.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.mhx1999.top/gtuggfmwin.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.gogol.net.cn/gthtaitdxi.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.chenjidiqi.icu/gtdybykxou.html


<!-- 参考信息 -->