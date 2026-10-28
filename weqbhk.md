代发 wailian999

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.meibo888.top/gtvounbbxf.html

Ruby: ENV["HOME"]
来源：http://hz.jianghu66.top/gtlhqvbjhz.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.jinqigfzy.top/gtndbfxdgm.html

[M03] 执行外部命令
来源：http://hz.zhiwuduotai.top/gtgdnksjay.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.yj20258888.top/gtzccuqqjj.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.iojbl.cn/gtrqsioftu.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.52xcode.cn/gtdigqfhgr.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.jinqigufen.top/gtdsevfomn.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.andypj.xyz/gtodqfagur.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.fengsongda.top/gtppkouyfx.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.hysaishi.cn/gtbphevjum.html

C#:   Process.Start("ls", "-l");
来源：http://hz.gaohongyu789.top/gttitfvsnt.html

[M04] 获取当前工作目录
来源：http://hz.chenlongwang.top/gtsbhgaehk.html

Py:   os.getcwd()
来源：http://hz.quarkkingdee.top/gtclfoycno.html

PHP:  getcwd();
来源：http://hz.0kj1m.cn/gtoycxelzs.html

JS:   process.cwd()
来源：http://hz.shanyushiyangkeji.top/gtwmfrmnds.html

TS:   process.cwd()
来源：http://hz.chenlongwang.top/gteqvtvjdf.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.tian-w.cn/gttkbkttsl.html

Go:   os.Getwd()
来源：http://hz.sxryk.cn/gthtzdzion.html

Ruby: Dir.pwd
来源：http://hz.9152youxi.cn/gtzsrhjnke.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.yj202588.top/gtwokxygew.html

[M05] 设置退出码
来源：http://hz.jqgufenzy.top/gtbwfknbfr.html

Py:   sys.exit(1)
来源：http://hz.zhixingplan.top/gtvxjnlogz.html

PHP:  exit(1);
来源：http://hz.yangfankeji.com/gtiezadxwf.html

JS:   process.exit(1)
来源：http://hz.zhengqikj.top/gtppnplifk.html

TS:   process.exit(1)
来源：http://hz.tianlin.xyz/gthqjstxbr.html

Java: System.exit(1)
来源：http://hz.wangdashe.top/gtsimzclfy.html

Go:   os.Exit(1)
来源：http://hz.gaohongyu789.top/gtjeqnisfa.html

Ruby: exit 1
来源：http://hz.jqgufenzy.top/gtckekptmj.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.chenjidiqi.icu/gtalmqpexw.html

[M06] 向标准错误输出
来源：http://hz.52xcode.cn/gtjxnuvwti.html

Py:   print("err", file=sys.stderr)
来源：http://hz.sufxvd.cn/gturnsehda.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.feifeiyinyue.top/gtmctjxaqo.html

JS:   console.error("err")
来源：http://hz.xingfuxueyuan.xyz/gtjjnoikbn.html

TS:   console.error("err")
来源：http://hz.sysykeji.top/gtneqqjrqc.html

Java: System.err.println("err")
来源：http://hz.zhongyouzk.top/gtserippke.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.chenzaomai.com/gtkwisnafz.html

Ruby: warn "err"
来源：http://hz.jinghuilouyu.cn/gtjwdakoct.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.dashuyun.cn/gtgsdcddcv.html

[M07] 判断是否为主入口
来源：http://hz.yonumen.top/gtqflnorqm.html

Py:   if __name__ == "__main__":
来源：http://hz.hnqzz.top/gtddzvzkkt.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.gogol.net.cn/gtdvrkndmd.html

JS:   require.main === module
来源：http://hz.xinyue.icu/gttpammgnl.html

TS:   require.main === module
来源：http://hz.ppjwa.cn/gtqxvvjhvs.html

Java: public static void main(String[] args)
来源：http://hz.cheryme.top/gttovmpxcd.html

Go:   func main()
来源：http://hz.pycfn.com/gtzbfzlpsk.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.gotoacloud.top/gtjgnyrazx.html

C#:   static void Main(string[] args)
来源：http://hz.haohaochexian.top/gthyehjkil.html

[M08] 获取系统与运行时信息
来源：http://hz.yangfankeji.com/gtogxsfvmk.html

Py:   platform.system();  platform.python_version()
来源：http://hz.quarkkingdee.top/gtdecgjigf.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.cheryme.top/gtvkcqyzky.html

JS:   process.platform;  process.version
来源：http://hz.cdnleiting.top/gtqernpjzo.html

TS:   process.platform;  process.version
来源：http://hz.cheryme.top/gtasfppyrn.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.wangshuangyany.cn/gtojdtmgyp.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.guowangkeji.top/gtbtrwfgfm.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.tanke756.top/gtokjtbutc.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.dianchejie.cn/gtcenqmxat.html

================================================================================
来源：http://hz.hywenlv.cn/gtqmnidshj.html

N. 数据结构与算法
来源：http://hz.ybcxt.top/gtrrfjrjzq.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtyjomalrg.html

[N01] 二分查找（有序数组）
来源：http://hz.zdqjudy.top/gtzgtbrigh.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.xziqi.cn/gtuswueomd.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.jlsjyb.cn/gtasyeycnd.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.zdqjudy.top/gtigqobcyl.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.yj202588.top/gtxaxbvtqf.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.316326.xyz/gtimknqtzx.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.tianlin.xyz/gtehxyxrpp.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.zhoulong.xyz/gtrrbzvxdq.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.9152youxi.cn/gtxrehneue.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.feifeiyinyue.top/gtgxbmqfmy.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.zhixingplan.top/gttasqsret.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.xziqi.cn/gtvqkvwmwg.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.nanxuanxn.top/gtsvnmqfdk.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.shzxlz.cn/gtammtfcfw.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.iojbl.cn/gtbuuxeykz.html

Go:   slices.Sort(arr)
来源：http://hz.vqdsnc.cn/gtgdtohpgh.html

Ruby: arr.sort
来源：http://hz.hfpthk.cn/gtkuoeulds.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.iojbl.cn/gtbnehqkri.html

[N03] 快速排序（分治示例）
来源：http://hz.yj20258.top/gttnuejkhg.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.ydjk.org.cn/gtgluimclj.html

PHP:  // 递归实现，或用 usort
来源：http://hz.52xcode.cn/gtprlaiwfo.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.jyoumei.cn/gtgildtxsp.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.hysaishi.cn/gthbnkkblt.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.jinghuilouyu.cn/gtkyjiatdp.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.yuanzhike.top/gtrvfjxuoq.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.aibaodan.cn/gtlcdlatgy.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.xylfe.cn/gtjtarkpvn.html

[N04] 斐波那契数列
来源：http://hz.wangshuangyany.cn/gtlimohyrx.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.gogol.net.cn/gtyxbmlzqb.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.sufxvd.cn/gtrumsjybb.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.redwolf501.top/gtzeqipcdc.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.daria6918.cn/gtuqeyysqg.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.birdmap.top/gtmmkawylt.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.yueranfly.top/gtqnpldbak.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.hnqzz.top/gttacsmfid.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.0kj1m.cn/gtujoopvtr.html

[N05] 最大公约数
来源：http://hz.ybcxt.top/gtqtnmrlns.html

Py:   math.gcd(a, b)
来源：http://hz.guannengcc.top/gtwuyhmdip.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.pycfn.com/gtglnmyakl.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.meibo888.top/gtxtkluwux.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.zhixingplan.top/gtjdidbejd.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.hfpthk.cn/gtselzlopv.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.9152youxi.cn/gtkkindjbl.html

Ruby: a.gcd(b)
来源：http://hz.wangdashe.top/gtsjquxyxg.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.andypj.xyz/gtlomtsbdg.html

[N06] 判断回文字符串
来源：http://hz.aibaodan.cn/gtvfjugrwn.html

Py:   s == s[::-1]
来源：http://hz.zhoulong.xyz/gtzdjruzhu.html

PHP:  $s === strrev($s);
来源：http://hz.sxryk.cn/gtfowdombb.html

JS:   s === [...s].reverse().join("")
来源：http://hz.sweek.top/gtmpezunsc.html

TS:   s === [...s].reverse().join("")
来源：http://hz.jinqigufen.top/gtzccezyxz.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.yj20258.top/gtdchygubg.html

Go:   // 双指针从两端比较
来源：http://hz.aizwys.cn/gtrefukwxn.html

Ruby: s == s.reverse
来源：http://hz.jinyuanbaomall.cn/gtpmbuprmg.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.fzhhl.top/gtumsnylqg.html

[N07] 两数之和（返回下标）
来源：http://hz.aibaodan.cn/gtcmoriezt.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.birdmap.top/gtrazppbhi.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.nanxuanxn.top/gtogpugykv.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.jiagoushi.top/gtxpzrjawm.html

TS:   // 手写 Map<string, number>
来源：http://hz.xuetiantiany.cn/gtppcbqghw.html

Java: // 手写 HashMap
来源：http://hz.ywan-chungtsiang.top/gtkxpiulfh.html

Go:   // 手写 map[int]int
来源：http://hz.smart0.xyz/gtncgvgqve.html

Ruby: // 手写 Hash
来源：http://hz.smart0.xyz/gtbhlezkbe.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.yj202588.top/gtttpbfrip.html

[N08] 生成全排列
来源：http://hz.dianchejie.cn/gtccwmrzhd.html

Py:   itertools.permutations(arr)
来源：http://hz.daxiang520.top/gtppqwlidm.html

PHP:  // 手写递归交换
来源：http://hz.chenzaomai.com/gtxpspobto.html

JS:   // 手写回溯递归
来源：http://hz.sysykeji.top/gtlxhxmcax.html

TS:   // 手写回溯递归
来源：http://hz.snrcjt.cn/gtfgbvzdct.html

Java: // 手写回溯递归
来源：http://hz.hfpthk.cn/gtduzhafjt.html

Go:   // 手写回溯递归
来源：http://hz.aibaodan.cn/gtlcwrktpg.html

Ruby: arr.permutation.to_a
来源：http://hz.xuetiantiany.cn/gtnqpbdakq.html

C#:   // 手写回溯递归
来源：http://hz.fzhhl.top/gtwcydbkvv.html

[N09] 栈与队列
来源：http://hz.xinyue.icu/gtyfdeblgq.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.shangyingyoupin.top/gtvnvuituz.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.yj20258.top/gtoepecbhl.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.dianchejie.cn/gthuhjhyiw.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.gogol.net.cn/gtziztaxdd.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.chenzaomai.com/gtmphutwsr.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.jinghuilouyu.cn/gtgpcezeqd.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.shzxlz.cn/gtkkotrwti.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.birdmap.top/gtqjvmkwpf.html

[N10] 链表节点定义
来源：http://hz.yj202588.top/gtxhnuazqn.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.xuetiantiany.cn/gtnkqxopxd.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.wangshuangyany.cn/gtxojxmplv.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.yvedp.cn/gtyrmfavkz.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.cdnleiting.top/gtnevrapxj.html

Java: class Node { int v; Node next; }
来源：http://hz.birdmap.top/gtcqpehfwe.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.xingfuxueyuan.xyz/gtdgjpgygp.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.zycfv.cn/gtxqcvltpr.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.jinghuilouyu.cn/gtxxajmboj.html

[N11] 二叉树中序遍历
来源：http://hz.ybcxt.top/gtusiqtvdo.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.gzhubu.top/gtnclxfcgd.html

PHP:  // 手写递归函数
来源：http://hz.smart0.xyz/gtmoxzktzi.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.yuanzhike.top/gtygknnfue.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.jlsjyb.cn/gthbjutpha.html

Java: // 手写递归
来源：http://hz.yongpay.top/gtvlxwpsny.html

Go:   // 手写递归
来源：http://hz.zhiwuduotai.top/gtfgdlhxpn.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.chenlongwang.top/gtjxbzywjj.html

C#:   // 手写递归
来源：http://hz.cqqwz.cn/gttjbjiwjg.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.shuidangran.top/gthonnkinh.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.yuanzhike.top/gtbwtwtmuz.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.iojbl.cn/gthltkemso.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.316326.xyz/gthnuscaaj.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.zhoulong.xyz/gtainacmcx.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.ydzc1.top/gtwoaqfqsr.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.xuetiantiany.cn/gtsbfhlxjf.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.zhijiandao.cn/gtomunkcnz.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.xinyue.icu/gtuutdalna.html

================================================================================
来源：http://hz.zhixingplan.top/gtmxnjkqey.html

O. 并发与异步
来源：http://hz.jlsjyb.cn/gtqoxzdnjj.html

================================================================================
来源：http://hz.daxiang520.top/gttysoenxy.html

[O01] 启动一个线程
来源：http://hz.yvedp.cn/gtjpmehycu.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.gogol.net.cn/gtpzzgxnjw.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.jinqigufen.top/gtdorsfuza.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.bjfxy.top/gtmtwkwwxs.html

TS:   // 同 JS
来源：http://hz.shzxlz.cn/gtdksokpec.html

Java: new Thread(() -> f()).start()
来源：http://hz.zhengqikj.top/gtufqblnst.html

Go:   go f()
来源：http://hz.zhijiandao.cn/gtibrfofgz.html

Ruby: Thread.new { f }
来源：http://hz.sxryk.cn/gtsisbfpon.html

C#:   Task.Run(() => F());
来源：http://hz.gzhubu.top/gtkfiqcdfs.html

[O02] 使用线程池
来源：http://hz.yueranfly.top/gtsqhqulpe.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.nwbrower.top/gtbuhwyxkq.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.zhongyouzk.top/gtciijrers.html

JS:   // worker_threads 线程池
来源：http://hz.jlsjyb.cn/gtvxaiqins.html

TS:   // worker_threads 线程池
来源：http://hz.zdqjudy.top/gtiugtykkv.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.xylfe.cn/gtktrxkcxq.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.jinghuilouyu.cn/gtwngedllg.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.cucudq.cn/gtuekawfuw.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.yj202588.top/gtzdswkndj.html

[O03] 加锁保护共享数据
来源：http://hz.gogol.net.cn/gtttrjuqiw.html

Py:   with lock: shared += 1
来源：http://hz.xingfuxueyuan.xyz/gtxtddhzoo.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.cqqwz.cn/gtwkawumiw.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.yuxming.cn/gtapmfotsn.html

TS:   // 同 JS
来源：http://hz.yj20258.top/gttufwcgsg.html

Java: synchronized (this) { shared++; }
来源：http://hz.jiagoushi.top/gtqeyjvoei.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.meibo888.top/gtvsspuade.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.guowangkeji.top/gtgwezvplr.html

C#:   lock (gate) { shared++; }
来源：http://hz.xuetiantiany.cn/gteykbboec.html

[O04] 定义异步函数并等待
来源：http://hz.fzhhl.top/gthpbvejwq.html

Py:   async def f():⏎    await g()
来源：http://hz.zhongyouzk.top/gtfbqehoek.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.sweek.top/gtvrjhmihc.html

JS:   async function f() { await g(); }
来源：http://hz.daria6918.cn/gtlwkmehrx.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.yueranfly.top/gtkqepvgvf.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.sufxvd.cn/gtfxdinwkn.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.cqqwz.cn/gtrzytjlht.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.nanxinkj.top/gtugmwuutj.html

C#:   async Task F() { await G(); }
来源：http://hz.yuxming.cn/gtvppcbevy.html

[O05] 并发执行并等待全部完成
来源：http://hz.quarkkingdee.top/gtjpfwhxce.html

Py:   asyncio.gather(*tasks)
来源：http://hz.hnqzz.top/gtwvfynlfd.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.0kj1m.cn/gtvjtunamu.html

JS:   await Promise.all(tasks)
来源：http://hz.zhoulong.xyz/gtdagvvrhf.html

TS:   await Promise.all(tasks)
来源：http://hz.hammf.cn/gtiqcwqnpm.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.jinqigfzy.top/gtgfibzdsr.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.jqgfzy.top/gtgetozfkx.html

Ruby: threads.map(&:join)
来源：http://hz.sysykeji.top/gtlknqayrd.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.yanxiufei.cn/gtaztpnosp.html

[O06] 使用进程池
来源：http://hz.xinyue.icu/gtygtczwgt.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.dashuyun.cn/gtrayzzkhi.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.iojbl.cn/gtqxoqazhr.html

JS:   // child_process / cluster 模块
来源：http://hz.vqdsnc.cn/gtxipahzeo.html

TS:   // child_process / cluster 模块
来源：http://hz.52xcode.cn/gtgveoejog.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.chenlongwang.top/gtnlmfljuf.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.jianghu66.top/gtcvgwkscn.html

Ruby: // fork 块
来源：http://hz.haohaochexian.top/gtulnojwpe.html

C#:   Parallel.For
来源：http://hz.sweek.top/gtekziirpk.html

================================================================================
来源：http://hz.yj20258888.top/gtqlfwsnzv.html

P. 常用工具函数
来源：http://hz.aibaodan.cn/gtoxrkzqlh.html

================================================================================
来源：http://hz.fengsongda.top/gtcngvqfjs.html

[P01] 生成 UUID
来源：http://hz.tian-w.cn/gtnowqrcxa.html

Py:   str(uuid.uuid4())
来源：http://hz.yuanzhike.top/gtbmhfwsbk.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.xuanzx.com/gtlgqdycte.html

JS:   crypto.randomUUID()
来源：http://hz.gotoacloud.top/gtzhcfxnzc.html

TS:   crypto.randomUUID()
来源：http://hz.ydjk.org.cn/gtekizqkvv.html

Java: UUID.randomUUID().toString()
来源：http://hz.feifeiyinyue.top/gtrsmyyekp.html

Go:   // 用 github.com/google/uuid
来源：http://hz.nwbrower.top/gtyipmeclo.html

Ruby: SecureRandom.uuid
来源：http://hz.nanxuanxn.top/gtnssqlhoi.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.svipenyu.cn/gtltjdiazb.html

[P02] MD5 / SHA256 摘要
来源：http://hz.yonumen.top/gtigxblzqm.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.jiagoushi.top/gtjvgtuckq.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.pengpengdd.cyou/gtisnzgrlc.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.sufxvd.cn/gtrrhbacfg.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.mhx1999.top/gtukdkrrat.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.cashguo.top/gtphzvyxpr.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.shzxlz.cn/gtttwnrbem.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.zdqjudy.top/gtpdpqusbd.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.ywan-chungtsiang.top/gtwwraqfbv.html

[P03] 生成短随机字符串
来源：http://hz.iojbl.cn/gtsxifwdyx.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.daria6918.cn/gttlzuscbw.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.dashuyun.cn/gtdyqmzuab.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.xinyue.icu/gtltwrvogz.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.hysaishi.cn/gtcpqnpzrh.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.zdqjudy.top/gtnaaikqsf.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.andypj.xyz/gthtscoopj.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.dashuyun.cn/gtmscrjtub.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.zhongyouzk.top/gtebokvbvd.html

[P04] 求长度
来源：http://hz.dashuyun.cn/gtnrhauxgu.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.cashguo.top/gtmboapkrb.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.52xcode.cn/gttmmrgrsg.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.svipenyu.cn/gtsjydjlhh.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.ydjk.org.cn/gtvxmhwbnh.html

Java: list.size();  map.size();  s.length()
来源：http://hz.bjfxy.top/gtrivfqklj.html

Go:   len(arr);  len(m)
来源：http://hz.cheryme.top/gtgcdclowv.html

Ruby: x.length;  x.size
来源：http://hz.yuanzhike.top/gtqchaadds.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.shangyingyoupin.top/gtikdrgzci.html

[P05] 判断两个对象内容是否相等
来源：http://hz.tian-w.cn/gtsdustkqq.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.zhoulong.xyz/gtjfosguin.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.yj202588.top/gtqoyirrbz.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.shzxlz.cn/gtgtypzbbz.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.zhaomingkeji.xyz/gtfleomqwq.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.iojbl.cn/gtwzeapeve.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.fzhhl.top/gtxjdxllht.html

Ruby: a == b
来源：http://hz.smart0.xyz/gtwejwzdfv.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.jianghu66.top/gtzszazxfy.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.yonumen.top/gtfvaixruy.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.daria6918.cn/gtuseimjts.html

PHP:  if (empty($x)) {}
来源：http://hz.zhengqikj.top/gtlaletpnu.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.yj20258888.top/gtlbhmnbei.html

TS:   if (x == null) {}
来源：http://hz.zhoulong.xyz/gtabqsbouj.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.0kj1m.cn/gttqwemqfk.html

Go:   if x == nil {}
来源：http://hz.zhongyouzk.top/gtauwyffzm.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.vqdsnc.cn/gtpehvpnbn.html

C#:   if (x is null) {}
来源：http://hz.jinghuilouyu.cn/gtnhzrxrzk.html

[P07] 防抖与节流
来源：http://hz.tian-w.cn/gtuxjhqqmc.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.shzxlz.cn/gtrdmbkltl.html

PHP:  // 手写时间戳比较
来源：http://hz.xziqi.cn/gtdtqufqob.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.ydzc1.top/gtjzdihdpv.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.yj20258.top/gtmfofqpeg.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.0kj1m.cn/gtlulfpwpg.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.0kj1m.cn/gtlaqaonrz.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.zhengqikj.top/gthtcibpjw.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.xuanzx.com/gtgtaaymql.html

[P08] 处理浮点精度问题
来源：http://hz.daria6918.cn/gtmawbljdy.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.shzxlz.cn/gtisnszzif.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.iojbl.cn/gtmhbsnxcy.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.xuanzx.com/gtgqqnljsp.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.pycfn.com/gtpkxithwc.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.yuxming.cn/gtnfvyjhhd.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.yanxiufei.cn/gttdyujzdf.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.yj202588.top/gtztpnwhmq.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.xuetiantiany.cn/gtihkwwplt.html


<!-- 参考信息 -->