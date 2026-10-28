代发 wailian999

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.snrcjt.cn/gtrevbttzg.html

Ruby: ENV["HOME"]
来源：http://hz.xingfuxueyuan.xyz/gtdodbovoz.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.andypj.xyz/gtyfuaejfi.html

[M03] 执行外部命令
来源：http://hz.c1oappe.top/gtigyegnpe.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.zhoulong.xyz/gtbwnsuaji.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.9152youxi.cn/gtidshtqum.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.andypj.xyz/gtncbooskn.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.bjfxy.top/gtzckgsthx.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.hnxiangtu.top/gthmaqxjhh.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.hongshengwenyu.top/gtcmhyrbau.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.ydzc1.top/gteqhdfhsd.html

C#:   Process.Start("ls", "-l");
来源：http://hz.aibaodan.cn/gtkzssuwnr.html

[M04] 获取当前工作目录
来源：http://hz.svipenyu.cn/gtkzublcbj.html

Py:   os.getcwd()
来源：http://hz.sysykeji.top/gtvtupslbb.html

PHP:  getcwd();
来源：http://hz.jianghu66.top/gtybjniovh.html

JS:   process.cwd()
来源：http://hz.cashguo.top/gtxbwslizr.html

TS:   process.cwd()
来源：http://hz.hnqzz.top/gtaisvvncv.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.yuanzhike.top/gtqrjqroko.html

Go:   os.Getwd()
来源：http://hz.birdmap.top/gtauuoayuo.html

Ruby: Dir.pwd
来源：http://hz.xinyue.icu/gtncvaiplp.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.tianlin.xyz/gtxevkxlrn.html

[M05] 设置退出码
来源：http://hz.jlsjyb.cn/gtermuvsls.html

Py:   sys.exit(1)
来源：http://hz.sxryk.cn/gtjtmozowo.html

PHP:  exit(1);
来源：http://hz.gotoacloud.top/gtislvmkvm.html

JS:   process.exit(1)
来源：http://hz.ydzc1.top/gtqabvjmaa.html

TS:   process.exit(1)
来源：http://hz.zhoulong.xyz/gtijqtkwcq.html

Java: System.exit(1)
来源：http://hz.wangshuangyany.cn/gtjhwjlwlg.html

Go:   os.Exit(1)
来源：http://hz.ywan-chungtsiang.top/gtpqpibtxq.html

Ruby: exit 1
来源：http://hz.9152youxi.cn/gtenrfclaa.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.ehwqpu.com/gtxbkbjktc.html

[M06] 向标准错误输出
来源：http://hz.mhx1999.top/gtuzzqirkd.html

Py:   print("err", file=sys.stderr)
来源：http://hz.jinqigfzy.top/gtviruastu.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.ivvv.top/gtzdlsifht.html

JS:   console.error("err")
来源：http://hz.meibo888.top/gtzuvagsnc.html

TS:   console.error("err")
来源：http://hz.nanxuanxn.top/gtqthfobbi.html

Java: System.err.println("err")
来源：http://hz.zhongyouzk.top/gtnmcyyecx.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.yuxming.cn/gteovbrrms.html

Ruby: warn "err"
来源：http://hz.guannengcc.top/gtcscdnvbm.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.quarkkingdee.top/gtelrsipum.html

[M07] 判断是否为主入口
来源：http://hz.9152youxi.cn/gtpprhbgoz.html

Py:   if __name__ == "__main__":
来源：http://hz.hammf.cn/gtmxuiojwf.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.tianlin.xyz/gtcuxesoyd.html

JS:   require.main === module
来源：http://hz.haohaochexian.top/gtztltcgxq.html

TS:   require.main === module
来源：http://hz.xziqi.cn/gtuaabnaeo.html

Java: public static void main(String[] args)
来源：http://hz.sysykeji.top/gtbztfmxir.html

Go:   func main()
来源：http://hz.jianghu66.top/gtrptphhwh.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.hongshengwenyu.top/gtbvlrjxgy.html

C#:   static void Main(string[] args)
来源：http://hz.guannengcc.top/gtgsntodcp.html

[M08] 获取系统与运行时信息
来源：http://hz.9152youxi.cn/gtlwpkiegp.html

Py:   platform.system();  platform.python_version()
来源：http://hz.gotoacloud.top/gtamovttpa.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.9152youxi.cn/gttjasvhgv.html

JS:   process.platform;  process.version
来源：http://hz.chenlongwang.top/gtjmlkqxlm.html

TS:   process.platform;  process.version
来源：http://hz.xylfe.cn/gtzzfkivkb.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.zhiwuduotai.top/gtcmghtovy.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.hammf.cn/gtebjgzkqi.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.iojbl.cn/gtxyxbeewz.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.andypj.xyz/gtdypqqgjm.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtfflyfqpe.html

N. 数据结构与算法
来源：http://hz.snrcjt.cn/gtbbkarzij.html

================================================================================
来源：http://hz.jinqigfzy.top/gtqrpgikff.html

[N01] 二分查找（有序数组）
来源：http://hz.gzhubu.top/gtdtmwriyd.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.chenlongwang.top/gtuitblbec.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.quarkkingdee.top/gtxalabbmn.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.sweek.top/gtrpdworwb.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.nanxuanxn.top/gtknojdghl.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.wangdashe.top/gtcujgbeoz.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.cucudq.cn/gtopwoksak.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.wangdashe.top/gtbayzvsaa.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.chenzaomai.com/gtuqdifcvt.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.jqgfzy.top/gtcnxilylh.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.jqgfzy.top/gtkkmrdeov.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.aizwys.cn/gtyqabnqss.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.shanyushiyangkeji.top/gtclcxtzed.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.jinyuanbaomall.cn/gtogppzrzi.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.yueranfly.top/gtpashyrcw.html

Go:   slices.Sort(arr)
来源：http://hz.havefunace.top/gttgseplgq.html

Ruby: arr.sort
来源：http://hz.fengsongda.top/gtywsfyyxp.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.zdqjudy.top/gtdogvfnio.html

[N03] 快速排序（分治示例）
来源：http://hz.yj202588.top/gtoeknyafd.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.hfpthk.cn/gtqadkhslm.html

PHP:  // 递归实现，或用 usort
来源：http://hz.hnqzz.top/gtafwsbtev.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.wangdashe.top/gtktqprqiv.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.svipenyu.cn/gtztnogfwo.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.jinqigfzy.top/gtdjddpbgr.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.jianghu66.top/gtsbydjpwa.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.cucudq.cn/gtvnviearp.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.c1oappe.top/gtfjdsywla.html

[N04] 斐波那契数列
来源：http://hz.cashguo.top/gtfpytiwnd.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.aizwys.cn/gttsepgfcs.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.chenjidiqi.icu/gtxflcjerr.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.kuanghao11.cn/gtngbzfoiv.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.yangfankeji.com/gtqukbdpoa.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.zhijiandao.cn/gtjkxcfbsd.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.dashuyun.cn/gtnyvqhibo.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.zhixingplan.top/gttzawjmrz.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.pycfn.com/gtuzycfqtc.html

[N05] 最大公约数
来源：http://hz.redwolf501.top/gtbtpsjdnb.html

Py:   math.gcd(a, b)
来源：http://hz.52xcode.cn/gtjwrlaxhb.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.snrcjt.cn/gtfmnfrzwd.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.shanyushiyangtech.top/gtawyaioyi.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.daxiang520.top/gtjpvnuclg.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.xinyue.icu/gtdsbsbnar.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.guannengcc.top/gttqvghcql.html

Ruby: a.gcd(b)
来源：http://hz.shanyushiyangtech.top/gtcqwbzhgg.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.nanxinkj.top/gttfhrhurz.html

[N06] 判断回文字符串
来源：http://hz.sysykeji.top/gtepusymzd.html

Py:   s == s[::-1]
来源：http://hz.0kj1m.cn/gtsjfhcsrx.html

PHP:  $s === strrev($s);
来源：http://hz.9152youxi.cn/gtuqvbbnqq.html

JS:   s === [...s].reverse().join("")
来源：http://hz.redwolf501.top/gttvlypzce.html

TS:   s === [...s].reverse().join("")
来源：http://hz.jiagoushi.top/gtwmxujdfw.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.0kj1m.cn/gtvqytwzld.html

Go:   // 双指针从两端比较
来源：http://hz.svipenyu.cn/gtupypqikk.html

Ruby: s == s.reverse
来源：http://hz.gogol.net.cn/gtktlugsjp.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.jinyuanbaomall.cn/gthcfatycu.html

[N07] 两数之和（返回下标）
来源：http://hz.fengsongda.top/gtshcktvdz.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.cdnleiting.top/gtiurqnnmc.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.zhaomingkeji.xyz/gtmmludfrm.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.sweek.top/gtqlprgqnn.html

TS:   // 手写 Map<string, number>
来源：http://hz.yj20258888.top/gtslghmegu.html

Java: // 手写 HashMap
来源：http://hz.daxiang520.top/gtxywwxlkx.html

Go:   // 手写 map[int]int
来源：http://hz.yvedp.cn/gtuynrzgpj.html

Ruby: // 手写 Hash
来源：http://hz.shanyushiyangkeji.top/gtwknwsmjm.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.sxryk.cn/gtekqueydx.html

[N08] 生成全排列
来源：http://hz.shuidangran.top/gtirkyqlkx.html

Py:   itertools.permutations(arr)
来源：http://hz.9152youxi.cn/gtuvqdbwvp.html

PHP:  // 手写递归交换
来源：http://hz.pycfn.com/gthvpkrwzu.html

JS:   // 手写回溯递归
来源：http://hz.smart0.xyz/gttjtcckjm.html

TS:   // 手写回溯递归
来源：http://hz.aizwys.cn/gttqxoriar.html

Java: // 手写回溯递归
来源：http://hz.aizwys.cn/gtarbekydq.html

Go:   // 手写回溯递归
来源：http://hz.quarkkingdee.top/gtwinrtlkf.html

Ruby: arr.permutation.to_a
来源：http://hz.jinqigufen.top/gtlfuekusw.html

C#:   // 手写回溯递归
来源：http://hz.hysaishi.cn/gtybwcupmm.html

[N09] 栈与队列
来源：http://hz.haohaochexian.top/gtwzrtngor.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.dashuyun.cn/gtnynennym.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.jinyuanbaomall.cn/gtgiawsvty.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.cheryme.top/gtxwzdshsx.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.fengsongda.top/gtiqwyfwlu.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.yj20258888.top/gtsanklcca.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.quarkkingdee.top/gtozfzmtsq.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.sweek.top/gtopozfkxi.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.zhoulong.xyz/gtqthcqtmn.html

[N10] 链表节点定义
来源：http://hz.tanke756.top/gtiwwclfwz.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.shuidangran.top/gtckwfhzxa.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.hnxiangtu.top/gthtejbdxw.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.yj20258.top/gtqyzkkcaq.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.mhx1999.top/gtrijvfkxe.html

Java: class Node { int v; Node next; }
来源：http://hz.sweek.top/gtlmjpjrli.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.316326.xyz/gtichaovoh.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.ydzc1.top/gtishbshhk.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.ybcxt.top/gtbvubewdm.html

[N11] 二叉树中序遍历
来源：http://hz.redwolf501.top/gtxoykqjta.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.daxiang520.top/gtnffddvrn.html

PHP:  // 手写递归函数
来源：http://hz.zycfv.cn/gtygfkbyzt.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.shangyingyoupin.top/gtoagmbvdi.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.ydzc1.top/gtyayeboau.html

Java: // 手写递归
来源：http://hz.jqgufenzy.top/gtgvwljwxt.html

Go:   // 手写递归
来源：http://hz.guowangkeji.top/gtjzigmrrw.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.9152youxi.cn/gtntiadmbi.html

C#:   // 手写递归
来源：http://hz.gaohongyu789.top/gtuxnorfhw.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.daxiang520.top/gtgznsoxcf.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.daxiang520.top/gtqoffycxt.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.ywan-chungtsiang.top/gtkeqhhvfb.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.shanyushiyangtech.top/gtzkxjtuyn.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.cqqwz.cn/gtodyyiima.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.yuanzhike.top/gttfndwwen.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.xuetiantiany.cn/gtkhysdftp.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.hammf.cn/gtdsllxhkk.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.xinyue.icu/gtyxrevxvy.html

================================================================================
来源：http://hz.shuidangran.top/gtelhuxukv.html

O. 并发与异步
来源：http://hz.vqdsnc.cn/gtjvbqtrws.html

================================================================================
来源：http://hz.zhijiandao.cn/gtffgurono.html

[O01] 启动一个线程
来源：http://hz.mhx1999.top/gtoffwuuns.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.cucudq.cn/gtrlytcvee.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.nanxinkj.top/gtsgzthwvl.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.pycfn.com/gtoitapapo.html

TS:   // 同 JS
来源：http://hz.snrcjt.cn/gtetcdrnib.html

Java: new Thread(() -> f()).start()
来源：http://hz.zhongyouzk.top/gtrfmnpuix.html

Go:   go f()
来源：http://hz.bjfxy.top/gtsuculbgd.html

Ruby: Thread.new { f }
来源：http://hz.andypj.xyz/gtgxsljkpg.html

C#:   Task.Run(() => F());
来源：http://hz.iojbl.cn/gtcpbppgmf.html

[O02] 使用线程池
来源：http://hz.jqgufenzy.top/gtryhamczg.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.hysaishi.cn/gtirufszmn.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.zhaomingkeji.xyz/gtysterrnm.html

JS:   // worker_threads 线程池
来源：http://hz.jinyuanbaomall.cn/gtlxltkwev.html

TS:   // worker_threads 线程池
来源：http://hz.xylfe.cn/gtejwqhfrg.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.haohaochexian.top/gtusygvunz.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.xingfuxueyuan.xyz/gtuydzsjwx.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.jianghu66.top/gtavbmchen.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.jlsjyb.cn/gtdxzolrqx.html

[O03] 加锁保护共享数据
来源：http://hz.shuidangran.top/gtyonswzxk.html

Py:   with lock: shared += 1
来源：http://hz.sxryk.cn/gtujtjoxlx.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.xinyue.icu/gtywrdkuna.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.ywan-chungtsiang.top/gthinknwmk.html

TS:   // 同 JS
来源：http://hz.xuanzx.com/gtwbcvitra.html

Java: synchronized (this) { shared++; }
来源：http://hz.yanxiufei.cn/gtvyqxlqei.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.jinqigfzy.top/gtzelagxkt.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.c1oappe.top/gtisoqblgf.html

C#:   lock (gate) { shared++; }
来源：http://hz.haohaochexian.top/gtmlvobhpi.html

[O04] 定义异步函数并等待
来源：http://hz.kuanghao11.cn/gtvpypagej.html

Py:   async def f():⏎    await g()
来源：http://hz.ydzc1.top/gtyygvikce.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.jinqigfzy.top/gtideljaqg.html

JS:   async function f() { await g(); }
来源：http://hz.zdqjudy.top/gtlsjgddcj.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.daria6918.cn/gtlmshqqin.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.nwbrower.top/gtrjjkwide.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.zhongyouzk.top/gtcjlhrsia.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.sufxvd.cn/gtxjszjnkb.html

C#:   async Task F() { await G(); }
来源：http://hz.svipenyu.cn/gtmjoenrxm.html

[O05] 并发执行并等待全部完成
来源：http://hz.yuanzhike.top/gtzldqhnwj.html

Py:   asyncio.gather(*tasks)
来源：http://hz.yanxiufei.cn/gtwbaizuxt.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.yueranfly.top/gtnmdgxoyx.html

JS:   await Promise.all(tasks)
来源：http://hz.yj202588.top/gtcvfdqslc.html

TS:   await Promise.all(tasks)
来源：http://hz.bjfxy.top/gtqsqtbfry.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.ppjwa.cn/gtxehcgimo.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.aibaodan.cn/gtjtlodxpg.html

Ruby: threads.map(&:join)
来源：http://hz.zhoulong.xyz/gtizfjtzwn.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.hnxiangtu.top/gtocxwzrch.html

[O06] 使用进程池
来源：http://hz.xuanzx.com/gtxohcvicl.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.nanxuanxn.top/gteuempkqt.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.chenjidiqi.icu/gtvnuruwmb.html

JS:   // child_process / cluster 模块
来源：http://hz.chenlongwang.top/gtrtbililc.html

TS:   // child_process / cluster 模块
来源：http://hz.nanxuanxn.top/gthgrvkngu.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.ydjk.org.cn/gtfqmpqbhj.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.hnqzz.top/gtwelnbpdb.html

Ruby: // fork 块
来源：http://hz.ivvv.top/gtszsuykes.html

C#:   Parallel.For
来源：http://hz.yonumen.top/gtigzvmffh.html

================================================================================
来源：http://hz.gzhubu.top/gtydcotikb.html

P. 常用工具函数
来源：http://hz.tian-w.cn/gtwliidwhk.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtsikugmgr.html

[P01] 生成 UUID
来源：http://hz.nwbrower.top/gtpqojjlhr.html

Py:   str(uuid.uuid4())
来源：http://hz.zdqjudy.top/gtmgcjiyzk.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.jinyuanbaomall.cn/gtfzcoqszi.html

JS:   crypto.randomUUID()
来源：http://hz.yj202588.top/gtqrhwkcnl.html

TS:   crypto.randomUUID()
来源：http://hz.shuidangran.top/gtmrgmhhvn.html

Java: UUID.randomUUID().toString()
来源：http://hz.gogol.net.cn/gtlraxgwcf.html

Go:   // 用 github.com/google/uuid
来源：http://hz.zhengqikj.top/gtyrglopge.html

Ruby: SecureRandom.uuid
来源：http://hz.quarkkingdee.top/gtjkswmiqu.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.shanyushiyangkeji.top/gtnyfdgnan.html

[P02] MD5 / SHA256 摘要
来源：http://hz.tianlin.xyz/gtcofemvim.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.gogol.net.cn/gtrgtgnuyc.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.ydjk.org.cn/gtbxxeosli.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.feifeiyinyue.top/gtwpetynxv.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.fzhhl.top/gteulhpkme.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.iojbl.cn/gtxitoiwww.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.redwolf501.top/gtuotxvynx.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.dashuyun.cn/gtqjjhfdpz.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.zhongyouzk.top/gtcpzupeqe.html

[P03] 生成短随机字符串
来源：http://hz.yj202588.top/gtnlkhcoty.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.yuanzhike.top/gtylxcagdq.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.hnqzz.top/gtlevkpmbn.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.jlsjyb.cn/gttulvkfdl.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.yanxiufei.cn/gtmupncgzt.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.nwbrower.top/gthzkylijm.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.kuanghao11.cn/gtbzmrkaqv.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.meibo888.top/gtpyeqbmqo.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.jinqigfzy.top/gtnxnrnkhn.html

[P04] 求长度
来源：http://hz.zhongyouzk.top/gtbwjczluv.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.gotoacloud.top/gtpdcjnfpx.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.sufxvd.cn/gtmpzikxls.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.52xcode.cn/gtlscxrabj.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.meibo888.top/gtnmduuahc.html

Java: list.size();  map.size();  s.length()
来源：http://hz.wangshuangyany.cn/gtntcopapo.html

Go:   len(arr);  len(m)
来源：http://hz.iojbl.cn/gtcoupmbcs.html

Ruby: x.length;  x.size
来源：http://hz.wangdashe.top/gtwwvjkvfr.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.pycfn.com/gtequkkgoq.html

[P05] 判断两个对象内容是否相等
来源：http://hz.guowangkeji.top/gtkhmjkris.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.haohaochexian.top/gtlrgppazb.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.hammf.cn/gtwazhldyc.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.feifeiyinyue.top/gtfkcyhvhp.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.shuidangran.top/gtkskejidk.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.kuanghao11.cn/gtjhndmtpq.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.dianchejie.cn/gtfpqyqyuo.html

Ruby: a == b
来源：http://hz.smart0.xyz/gtsnauctnt.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.jqgufenzy.top/gtljqnudcv.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.cdnleiting.top/gtyhutvoxv.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.shuidangran.top/gtloldojru.html

PHP:  if (empty($x)) {}
来源：http://hz.aizwys.cn/gtuotmgtdr.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.zycfv.cn/gtfjerybck.html

TS:   if (x == null) {}
来源：http://hz.hfpthk.cn/gtptnfliou.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.yvedp.cn/gtaukqorkn.html

Go:   if x == nil {}
来源：http://hz.jinqigfzy.top/gtiwntybeh.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.wangshuangyany.cn/gtworgzpmh.html

C#:   if (x is null) {}
来源：http://hz.feifeiyinyue.top/gtosgiqald.html

[P07] 防抖与节流
来源：http://hz.aibaodan.cn/gtzbdjfwpc.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.ehwqpu.com/gtsubgeiwe.html

PHP:  // 手写时间戳比较
来源：http://hz.daxiang520.top/gtcwhcoten.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.xuanzx.com/gtwtictizm.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.shangyingyoupin.top/gtepaedcpf.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.xingfuxueyuan.xyz/gtbgdcudhb.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.chenzaomai.com/gtvbpkzgvb.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.hnxiangtu.top/gtwmheetkj.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.shanyushiyangtech.top/gtuuqcduqg.html

[P08] 处理浮点精度问题
来源：http://hz.pengpengdd.cyou/gterwrgsgz.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.52xcode.cn/gtjpfztqmj.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.smart0.xyz/gtmqtmvffr.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.gotoacloud.top/gtbfrsyehl.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.ivvv.top/gtfrgoxujc.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.andypj.xyz/gtysvrrzac.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.sweek.top/gthxhqapqs.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.ydzc1.top/gtcpgokdku.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.yj20258.top/gtghizwars.html


<!-- 参考信息 -->