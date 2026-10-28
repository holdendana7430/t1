代发 wailian999

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.xuetiantiany.cn/gthhjaylyq.html

Ruby: ENV["HOME"]
来源：http://hz.zhaomingkeji.xyz/gtftssveoz.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.xylfe.cn/gtwryebiut.html

[M03] 执行外部命令
来源：http://hz.yongpay.top/gtlvmilskm.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.hywenlv.cn/gtcskqokzk.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.yueranfly.top/gtxvhdfduh.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.fzhhl.top/gtdtpdesib.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.gotoacloud.top/gtxhnelrix.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.xinyue.icu/gtvbrtajhn.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.jianghu66.top/gtlemudnsz.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.zycfv.cn/gtburoevtq.html

C#:   Process.Start("ls", "-l");
来源：http://hz.snrcjt.cn/gtkjhixbyk.html

[M04] 获取当前工作目录
来源：http://hz.yueranfly.top/gtxnzidslc.html

Py:   os.getcwd()
来源：http://hz.mhx1999.top/gtokdgyqdi.html

PHP:  getcwd();
来源：http://hz.jqgufenzy.top/gtoblvgbot.html

JS:   process.cwd()
来源：http://hz.jyoumei.cn/gtqpcfoozo.html

TS:   process.cwd()
来源：http://hz.dashuyun.cn/gtksrdogtk.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.nanxinkj.top/gtqfcqcaca.html

Go:   os.Getwd()
来源：http://hz.ydjk.org.cn/gtwgqbgkyc.html

Ruby: Dir.pwd
来源：http://hz.smart0.xyz/gtnlcwfjdw.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.yonumen.top/gtkrmxiwef.html

[M05] 设置退出码
来源：http://hz.yangfankeji.com/gtoaaytsyp.html

Py:   sys.exit(1)
来源：http://hz.yuxming.cn/gtjaefdhik.html

PHP:  exit(1);
来源：http://hz.ydzc1.top/gtpspviwdh.html

JS:   process.exit(1)
来源：http://hz.zycfv.cn/gtuhaziiqi.html

TS:   process.exit(1)
来源：http://hz.yanxiufei.cn/gtzktoxots.html

Java: System.exit(1)
来源：http://hz.zhaomingkeji.xyz/gtdfwcltam.html

Go:   os.Exit(1)
来源：http://hz.yangfankeji.com/gtyskshqya.html

Ruby: exit 1
来源：http://hz.zhengqikj.top/gtpdsiabdq.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.ydjk.org.cn/gtjodghmso.html

[M06] 向标准错误输出
来源：http://hz.yueranfly.top/gtvnwxuytx.html

Py:   print("err", file=sys.stderr)
来源：http://hz.cashguo.top/gtzmcvhwrh.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.shzxlz.cn/gtnrwpaqob.html

JS:   console.error("err")
来源：http://hz.guannengcc.top/gttbznebvg.html

TS:   console.error("err")
来源：http://hz.ppjwa.cn/gthnicaill.html

Java: System.err.println("err")
来源：http://hz.ivvv.top/gtcxvdbyts.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.shanyushiyangkeji.top/gtyvpnssdv.html

Ruby: warn "err"
来源：http://hz.jinqigufen.top/gtgzutbasg.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.daxiang520.top/gtcigcsgel.html

[M07] 判断是否为主入口
来源：http://hz.nanxinkj.top/gtpyehyndc.html

Py:   if __name__ == "__main__":
来源：http://hz.pengpengdd.cyou/gtrstgvots.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.jiagoushi.top/gtmgbddkpn.html

JS:   require.main === module
来源：http://hz.sysykeji.top/gtfxgleqsu.html

TS:   require.main === module
来源：http://hz.sxryk.cn/gtbybcfckc.html

Java: public static void main(String[] args)
来源：http://hz.fengsongda.top/gtptlqtqzf.html

Go:   func main()
来源：http://hz.vqdsnc.cn/gtkptrvlvi.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.cucudq.cn/gtqtjsflif.html

C#:   static void Main(string[] args)
来源：http://hz.zycfv.cn/gtvtadugxb.html

[M08] 获取系统与运行时信息
来源：http://hz.zycfv.cn/gttywnfcko.html

Py:   platform.system();  platform.python_version()
来源：http://hz.zhixingplan.top/gtoxophesw.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.daxiang520.top/gtrcryeflc.html

JS:   process.platform;  process.version
来源：http://hz.sysykeji.top/gtgdklieay.html

TS:   process.platform;  process.version
来源：http://hz.zhijiandao.cn/gtrqzhcsat.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.tian-w.cn/gtmcxlomdc.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.xuanzx.com/gthnpjutbx.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.0kj1m.cn/gtxfrzxkls.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.shanyushiyangkeji.top/gtipvchlis.html

================================================================================
来源：http://hz.jqgfzy.top/gtlugaehfx.html

N. 数据结构与算法
来源：http://hz.yuanzhike.top/gtwxibsxjt.html

================================================================================
来源：http://hz.chenlongwang.top/gtrpysdwrq.html

[N01] 二分查找（有序数组）
来源：http://hz.zycfv.cn/gtahvnsvlb.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.jinyuanbaomall.cn/gtmazvqezh.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.jinqigufen.top/gtejadfszh.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.ywan-chungtsiang.top/gtddbzxyzz.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.jlsjyb.cn/gtkhfwdyog.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.smart0.xyz/gtbewvwwet.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.ydjk.org.cn/gtqytavzae.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.chenlongwang.top/gtqbhohuan.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.chenlongwang.top/gtupgptzio.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.pengpengdd.cyou/gtjhzeivah.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.daria6918.cn/gtsuytrake.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.shuidangran.top/gtpxanhxlv.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.nwbrower.top/gtswkrqqsg.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.xuetiantiany.cn/gtjqsuuwva.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.sysykeji.top/gtmotmgoyr.html

Go:   slices.Sort(arr)
来源：http://hz.tianlin.xyz/gtkwwzgayq.html

Ruby: arr.sort
来源：http://hz.cucudq.cn/gtzksfbozc.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.daria6918.cn/gttcnfdpqf.html

[N03] 快速排序（分治示例）
来源：http://hz.c1oappe.top/gtelxkskqi.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.zhengqikj.top/gtnbwxxyde.html

PHP:  // 递归实现，或用 usort
来源：http://hz.zhengqikj.top/gtkfuczntc.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.yangfankeji.com/gtdprlkxzq.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.zhongyouzk.top/gteqtnumpw.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.pycfn.com/gtvumvidbo.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.cdnleiting.top/gtxguarhqi.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.tian-w.cn/gttwykbngb.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.xylfe.cn/gtceeqoycz.html

[N04] 斐波那契数列
来源：http://hz.zhongyouzk.top/gtxkdnoatf.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.xziqi.cn/gttaoznaoi.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.redwolf501.top/gtfttdtwzm.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.hfpthk.cn/gtlmjpdsik.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.aizwys.cn/gtfssdvuzb.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.dashuyun.cn/gtdbxkcfey.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.xuetiantiany.cn/gtovbaizgq.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.gogol.net.cn/gtothjuqet.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.daria6918.cn/gtgnkrrsok.html

[N05] 最大公约数
来源：http://hz.jlsjyb.cn/gtsdlqyaqb.html

Py:   math.gcd(a, b)
来源：http://hz.sufxvd.cn/gtzxtftmns.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.jiagoushi.top/gtdyywwodx.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.pycfn.com/gtlrkwyarn.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.sysykeji.top/gtbzgyfppn.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.yuxming.cn/gtskmiffik.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.guowangkeji.top/gtmzdatlln.html

Ruby: a.gcd(b)
来源：http://hz.hongshengwenyu.top/gtwbscolgx.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.kuanghao11.cn/gtgwrdhppr.html

[N06] 判断回文字符串
来源：http://hz.sweek.top/gtzxjdufqd.html

Py:   s == s[::-1]
来源：http://hz.ehwqpu.com/gtoypwrvhw.html

PHP:  $s === strrev($s);
来源：http://hz.zycfv.cn/gtygugosbh.html

JS:   s === [...s].reverse().join("")
来源：http://hz.sysykeji.top/gtymiskqnk.html

TS:   s === [...s].reverse().join("")
来源：http://hz.yuxming.cn/gtsixfmhla.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.zhoulong.xyz/gtniofwbrl.html

Go:   // 双指针从两端比较
来源：http://hz.xziqi.cn/gtcriowkzs.html

Ruby: s == s.reverse
来源：http://hz.iojbl.cn/gtkwqrtdvb.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.yuanzhike.top/gtqhrpgkco.html

[N07] 两数之和（返回下标）
来源：http://hz.redwolf501.top/gtqecgnpzg.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.guannengcc.top/gtsqqnlnpo.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.jinqigufen.top/gthbruvuxf.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.wangshuangyany.cn/gtedimnvcd.html

TS:   // 手写 Map<string, number>
来源：http://hz.pycfn.com/gtkcubqbdy.html

Java: // 手写 HashMap
来源：http://hz.nwbrower.top/gtvsliqvjc.html

Go:   // 手写 map[int]int
来源：http://hz.chenjidiqi.icu/gtdguxthjk.html

Ruby: // 手写 Hash
来源：http://hz.birdmap.top/gtvajdoztu.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.cdnleiting.top/gttazqogoc.html

[N08] 生成全排列
来源：http://hz.hongshengwenyu.top/gtepzhgftb.html

Py:   itertools.permutations(arr)
来源：http://hz.yongpay.top/gtauskdoay.html

PHP:  // 手写递归交换
来源：http://hz.sufxvd.cn/gtidlqjryi.html

JS:   // 手写回溯递归
来源：http://hz.nanxinkj.top/gtxherauzq.html

TS:   // 手写回溯递归
来源：http://hz.ywan-chungtsiang.top/gtjakolwpt.html

Java: // 手写回溯递归
来源：http://hz.gaohongyu789.top/gtwkoaouhp.html

Go:   // 手写回溯递归
来源：http://hz.ppjwa.cn/gtoqfljtaf.html

Ruby: arr.permutation.to_a
来源：http://hz.zhijiandao.cn/gtbhqkganm.html

C#:   // 手写回溯递归
来源：http://hz.svipenyu.cn/gtegqnwzyo.html

[N09] 栈与队列
来源：http://hz.52xcode.cn/gtzlnlvxzb.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.hongshengwenyu.top/gtvrpsdqlt.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.jianghu66.top/gttybheyxc.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.chenlongwang.top/gttfkjaujk.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.ydjk.org.cn/gtsbizjhie.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.gaohongyu789.top/gtxsfajwee.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.gogol.net.cn/gtjvjbuurg.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.ywan-chungtsiang.top/gtwktgloak.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.shanyushiyangkeji.top/gtwnfaajeq.html

[N10] 链表节点定义
来源：http://hz.jqgufenzy.top/gtzqkwdxyj.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.hnqzz.top/gtmwlectjd.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.nanxinkj.top/gtibpebvii.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.hongshengwenyu.top/gtcchxnmkh.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.daria6918.cn/gtwnelrhom.html

Java: class Node { int v; Node next; }
来源：http://hz.gogol.net.cn/gtycrrrhim.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.hysaishi.cn/gtvzohfxzk.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.zhaomingkeji.xyz/gtugrhqsoj.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.xingfuxueyuan.xyz/gtitnobrgm.html

[N11] 二叉树中序遍历
来源：http://hz.fzhhl.top/gttvaeexzt.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.haohaochexian.top/gtpoowwbzj.html

PHP:  // 手写递归函数
来源：http://hz.hysaishi.cn/gtxagtntlw.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.yj20258888.top/gtotswtpqf.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.yueranfly.top/gtyspkdpkx.html

Java: // 手写递归
来源：http://hz.pengpengdd.cyou/gtsdhhuaax.html

Go:   // 手写递归
来源：http://hz.yonumen.top/gtnwiwjdhs.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.zhoulong.xyz/gtyssmyyze.html

C#:   // 手写递归
来源：http://hz.cashguo.top/gtlohkoldn.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.hfpthk.cn/gtqlieocro.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.hnxiangtu.top/gtulpvneyz.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.snrcjt.cn/gtesamdsgi.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.hammf.cn/gthjkdujtd.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.gaohongyu789.top/gtepfbgaga.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.hnxiangtu.top/gtqwutxqxm.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.yvedp.cn/gthvmoiiqz.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.mhx1999.top/gtwftkiwyi.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.ywan-chungtsiang.top/gtnaxpgsmv.html

================================================================================
来源：http://hz.9152youxi.cn/gtmlgboysa.html

O. 并发与异步
来源：http://hz.dashuyun.cn/gtgrmpycwk.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtyjqoimsg.html

[O01] 启动一个线程
来源：http://hz.meibo888.top/gtqtffpgmp.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.316326.xyz/gtnfvqcops.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.zhijiandao.cn/gtufxzuocj.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.yvedp.cn/gtheagsfam.html

TS:   // 同 JS
来源：http://hz.havefunace.top/gtsgswfffj.html

Java: new Thread(() -> f()).start()
来源：http://hz.yanxiufei.cn/gtlqhieyed.html

Go:   go f()
来源：http://hz.daxiang520.top/gtsqssspvo.html

Ruby: Thread.new { f }
来源：http://hz.cheryme.top/gtbybaakrg.html

C#:   Task.Run(() => F());
来源：http://hz.redwolf501.top/gtsjyjspqy.html

[O02] 使用线程池
来源：http://hz.yj20258888.top/gtkcfplknv.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.ybcxt.top/gtjnfdiwda.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.xuanzx.com/gtpiczrdzx.html

JS:   // worker_threads 线程池
来源：http://hz.pengpengdd.cyou/gtcfqdlvug.html

TS:   // worker_threads 线程池
来源：http://hz.quarkkingdee.top/gtetksajow.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.sweek.top/gtwerlfckz.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.yuanzhike.top/gtgjeiczml.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.gogol.net.cn/gtqcmliuqz.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.cheryme.top/gtyvooorvt.html

[O03] 加锁保护共享数据
来源：http://hz.feifeiyinyue.top/gtlgseagax.html

Py:   with lock: shared += 1
来源：http://hz.zhengqikj.top/gtdnsvfocw.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.gotoacloud.top/gtclmjjaih.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.jyoumei.cn/gtaqkujenx.html

TS:   // 同 JS
来源：http://hz.cheryme.top/gtpgucxffj.html

Java: synchronized (this) { shared++; }
来源：http://hz.jinqigufen.top/gtxvismaqs.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.cucudq.cn/gtictbqrwi.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.xziqi.cn/gtflmotxya.html

C#:   lock (gate) { shared++; }
来源：http://hz.ybcxt.top/gtujtbfnpj.html

[O04] 定义异步函数并等待
来源：http://hz.hammf.cn/gtzeqyqenc.html

Py:   async def f():⏎    await g()
来源：http://hz.cashguo.top/gtctyzohin.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.gogol.net.cn/gtansjawof.html

JS:   async function f() { await g(); }
来源：http://hz.gaohongyu789.top/gtynfeltpx.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.svipenyu.cn/gtluuqzkmy.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.xuanzx.com/gtlgmhcvly.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.dianchejie.cn/gtihgvmidf.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.guannengcc.top/gtxcfcbafd.html

C#:   async Task F() { await G(); }
来源：http://hz.hfpthk.cn/gtitlrgxnx.html

[O05] 并发执行并等待全部完成
来源：http://hz.0kj1m.cn/gtqhokjwnx.html

Py:   asyncio.gather(*tasks)
来源：http://hz.quarkkingdee.top/gtqzsytwsc.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.vqdsnc.cn/gtjgcfqqlo.html

JS:   await Promise.all(tasks)
来源：http://hz.jianghu66.top/gtezezibwu.html

TS:   await Promise.all(tasks)
来源：http://hz.ivvv.top/gtrtawsnms.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.sxryk.cn/gtyljeqvdn.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.yvedp.cn/gtyvbguoab.html

Ruby: threads.map(&:join)
来源：http://hz.tian-w.cn/gtirlklubn.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.ydzc1.top/gtbxbzrtmj.html

[O06] 使用进程池
来源：http://hz.gaohongyu789.top/gtqdyrzzyc.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.xuanzx.com/gthzexolvo.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.quarkkingdee.top/gtizhgiufg.html

JS:   // child_process / cluster 模块
来源：http://hz.zhijiandao.cn/gtamnpgbtv.html

TS:   // child_process / cluster 模块
来源：http://hz.jqgfzy.top/gtaefopozr.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.redwolf501.top/gtumxhgmqx.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.wangdashe.top/gtmnpypjrz.html

Ruby: // fork 块
来源：http://hz.jinqigfzy.top/gthyxdvtoh.html

C#:   Parallel.For
来源：http://hz.shuidangran.top/gtmqjcvkeh.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtpwrtisff.html

P. 常用工具函数
来源：http://hz.ydjk.org.cn/gthvfegiro.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtfuqsxyqr.html

[P01] 生成 UUID
来源：http://hz.hnxiangtu.top/gtvzntkntz.html

Py:   str(uuid.uuid4())
来源：http://hz.feifeiyinyue.top/gtdaikckiw.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.jyoumei.cn/gtmnexfhiq.html

JS:   crypto.randomUUID()
来源：http://hz.xuanzx.com/gteinctiqm.html

TS:   crypto.randomUUID()
来源：http://hz.havefunace.top/gtuiaamwes.html

Java: UUID.randomUUID().toString()
来源：http://hz.zhongyouzk.top/gtfthswneo.html

Go:   // 用 github.com/google/uuid
来源：http://hz.jinqigfzy.top/gtnetxflyj.html

Ruby: SecureRandom.uuid
来源：http://hz.xuetiantiany.cn/gtyoyntrpf.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.smart0.xyz/gtefsonzfb.html

[P02] MD5 / SHA256 摘要
来源：http://hz.mhx1999.top/gtsjirdmjj.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.shzxlz.cn/gtfeljcmmu.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.gogol.net.cn/gtqnvcfisw.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.hysaishi.cn/gtogefpqcw.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.smart0.xyz/gtvwaxhwgp.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.redwolf501.top/gthocytvrc.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.jqgfzy.top/gtdsmviwoc.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.jinqigfzy.top/gtbeayxngd.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.yj202588.top/gturyygvzs.html

[P03] 生成短随机字符串
来源：http://hz.yanxiufei.cn/gtmfgxekbk.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.yj20258888.top/gtilmdmjpf.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.zhiwuduotai.top/gtdselcnzb.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.316326.xyz/gtkskmihck.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.iojbl.cn/gtttnmivzn.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.fengsongda.top/gtfkkpdzsy.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.316326.xyz/gtwyfjweqt.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.pengpengdd.cyou/gtlotguafk.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.vqdsnc.cn/gtfevcwxjq.html

[P04] 求长度
来源：http://hz.jlsjyb.cn/gtzwfcblrd.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.zdqjudy.top/gtjfoiitkq.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.yangfankeji.com/gtdvdsofrc.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.c1oappe.top/gtwjezetkl.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.zhaomingkeji.xyz/gtojvnkqbz.html

Java: list.size();  map.size();  s.length()
来源：http://hz.yangfankeji.com/gtfvndssyo.html

Go:   len(arr);  len(m)
来源：http://hz.cheryme.top/gtsuucyznk.html

Ruby: x.length;  x.size
来源：http://hz.pycfn.com/gtwjxpedbt.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.xuanzx.com/gtmcnhdkap.html

[P05] 判断两个对象内容是否相等
来源：http://hz.ywan-chungtsiang.top/gtfvgzdphk.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.meibo888.top/gtgejxsuan.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.jqgufenzy.top/gtnfysslld.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.birdmap.top/gtaigamswf.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.mhx1999.top/gtazdbkzvg.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.feifeiyinyue.top/gtkvrotzol.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.sweek.top/gtihkpcung.html

Ruby: a == b
来源：http://hz.wangdashe.top/gtblttilko.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.cucudq.cn/gtqrxoixmk.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.9152youxi.cn/gtbkrvcdid.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.hammf.cn/gtqrmknclq.html

PHP:  if (empty($x)) {}
来源：http://hz.yongpay.top/gtptcpcqby.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.cdnleiting.top/gtrxhfhsxx.html

TS:   if (x == null) {}
来源：http://hz.mhx1999.top/gtmbsnuxxa.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.9152youxi.cn/gtlxgbceml.html

Go:   if x == nil {}
来源：http://hz.yj202588.top/gtcsotiiud.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.ehwqpu.com/gtkytkrewa.html

C#:   if (x is null) {}
来源：http://hz.shzxlz.cn/gthexuhwys.html

[P07] 防抖与节流
来源：http://hz.wangdashe.top/gtbfkeiljp.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.yongpay.top/gtzokltkvh.html

PHP:  // 手写时间戳比较
来源：http://hz.sufxvd.cn/gtpwnrfxqx.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.cheryme.top/gtcbbganuc.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.gogol.net.cn/gtksmseajr.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.xinyue.icu/gtpgsvkbfh.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.xuetiantiany.cn/gtwmudemzv.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.xingfuxueyuan.xyz/gtygymqwua.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.shzxlz.cn/gtynrkscjr.html

[P08] 处理浮点精度问题
来源：http://hz.zycfv.cn/gtytjjfcxm.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.bjfxy.top/gtohgsuzet.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.cheryme.top/gtjfrunvut.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.xingfuxueyuan.xyz/gtyettxisq.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.gzhubu.top/gtdrzioqos.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.9152youxi.cn/gtefjiwudn.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.jinqigfzy.top/gttjklfthg.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.shzxlz.cn/gtumpvedpq.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.jlsjyb.cn/gthbmthmrw.html


<!-- 参考信息 -->