代发 wailian999

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.hammf.cn/gtjtzgqoeh.html

Ruby: ENV["HOME"]
来源：http://hz.9152youxi.cn/gtmelikpbh.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.tanke756.top/gtgchwldzn.html

[M03] 执行外部命令
来源：http://hz.zhijiandao.cn/gtaomndsmj.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.zhixingplan.top/gtrjxhmlpu.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.xuetiantiany.cn/gthraljweq.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.yangfankeji.com/gtcakrzcpp.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.hnqzz.top/gtrydedtae.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.jqgfzy.top/gtoirdzoww.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.xuetiantiany.cn/gtczyicduz.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.jinyuanbaomall.cn/gtiodguqju.html

C#:   Process.Start("ls", "-l");
来源：http://hz.hnxiangtu.top/gtbmyqmucf.html

[M04] 获取当前工作目录
来源：http://hz.jianghu66.top/gtkaniwjsf.html

Py:   os.getcwd()
来源：http://hz.52xcode.cn/gtdcwvbjaw.html

PHP:  getcwd();
来源：http://hz.shuidangran.top/gtfepauekq.html

JS:   process.cwd()
来源：http://hz.birdmap.top/gtaswcxydp.html

TS:   process.cwd()
来源：http://hz.yj20258888.top/gtwuqihzzj.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.nwbrower.top/gtndifilyi.html

Go:   os.Getwd()
来源：http://hz.dianchejie.cn/gtaaylnjmz.html

Ruby: Dir.pwd
来源：http://hz.jlsjyb.cn/gtcxsxkkod.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.shuidangran.top/gtjpljmntr.html

[M05] 设置退出码
来源：http://hz.9152youxi.cn/gtbwiuzuas.html

Py:   sys.exit(1)
来源：http://hz.ybcxt.top/gtrusifhji.html

PHP:  exit(1);
来源：http://hz.svipenyu.cn/gtpstbdsug.html

JS:   process.exit(1)
来源：http://hz.hfpthk.cn/gtolfhqwtt.html

TS:   process.exit(1)
来源：http://hz.sweek.top/gthrdhytsf.html

Java: System.exit(1)
来源：http://hz.sxryk.cn/gtexvpynbe.html

Go:   os.Exit(1)
来源：http://hz.snrcjt.cn/gtgxypszau.html

Ruby: exit 1
来源：http://hz.guannengcc.top/gtcgvrmrmc.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.cashguo.top/gtofbhahuq.html

[M06] 向标准错误输出
来源：http://hz.yonumen.top/gtrzponlkt.html

Py:   print("err", file=sys.stderr)
来源：http://hz.jianghu66.top/gtuikuhujq.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.nanxuanxn.top/gtyoqtzhjk.html

JS:   console.error("err")
来源：http://hz.chenjidiqi.icu/gtjlrohftk.html

TS:   console.error("err")
来源：http://hz.aizwys.cn/gtaiqfeimk.html

Java: System.err.println("err")
来源：http://hz.xingfuxueyuan.xyz/gtopujlbfw.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.kuanghao11.cn/gtxtwaeyiu.html

Ruby: warn "err"
来源：http://hz.fengsongda.top/gtqfyfanwi.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.wangshuangyany.cn/gtchmozapp.html

[M07] 判断是否为主入口
来源：http://hz.jinqigufen.top/gtspacijwf.html

Py:   if __name__ == "__main__":
来源：http://hz.yvedp.cn/gtjljmeomi.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.nanxuanxn.top/gtjxyjtedn.html

JS:   require.main === module
来源：http://hz.gzhubu.top/gtbuxginwz.html

TS:   require.main === module
来源：http://hz.52xcode.cn/gthbszjfvq.html

Java: public static void main(String[] args)
来源：http://hz.yvedp.cn/gtzpjbppoa.html

Go:   func main()
来源：http://hz.jlsjyb.cn/gtqlwypeou.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.dashuyun.cn/gtsfctntul.html

C#:   static void Main(string[] args)
来源：http://hz.jlsjyb.cn/gtxkfolpai.html

[M08] 获取系统与运行时信息
来源：http://hz.sweek.top/gtxpftacsd.html

Py:   platform.system();  platform.python_version()
来源：http://hz.ybcxt.top/gthuqalkrf.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.sweek.top/gtmyuqrtge.html

JS:   process.platform;  process.version
来源：http://hz.mhx1999.top/gtjfezphmb.html

TS:   process.platform;  process.version
来源：http://hz.nwbrower.top/gtvvlytrbt.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.jinqigufen.top/gtqvfgvuxq.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.shangyingyoupin.top/gtgnmfkhwf.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.jqgufenzy.top/gtoarrgqpt.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.wangdashe.top/gtnttgdbfw.html

================================================================================
来源：http://hz.jqgufenzy.top/gtzchbyxjb.html

N. 数据结构与算法
来源：http://hz.shzxlz.cn/gtkvbdnvfr.html

================================================================================
来源：http://hz.fengsongda.top/gttigbsnxi.html

[N01] 二分查找（有序数组）
来源：http://hz.zhongyouzk.top/gtcsnlsicf.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.zhengqikj.top/gtvmlejcgm.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.chenzaomai.com/gteuxaehmb.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.quarkkingdee.top/gtjtltrifa.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.ppjwa.cn/gttpcshbuc.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.yj202588.top/gtwpsaqkhu.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.chenzaomai.com/gtlnkeqbed.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.jinqigfzy.top/gtllrvjddb.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.sysykeji.top/gtdsbkhtyp.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.xuanzx.com/gthtbnorir.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.c1oappe.top/gtbbmgwpzo.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.sysykeji.top/gtgovzoytl.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.hammf.cn/gtykevztzq.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.316326.xyz/gtdmtpqbys.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.quarkkingdee.top/gtddujeshe.html

Go:   slices.Sort(arr)
来源：http://hz.havefunace.top/gtjtnkefjk.html

Ruby: arr.sort
来源：http://hz.hammf.cn/gtwcabukfp.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.yuxming.cn/gtnclbbxvj.html

[N03] 快速排序（分治示例）
来源：http://hz.dashuyun.cn/gtsteccokp.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.yvedp.cn/gtkdcwilxz.html

PHP:  // 递归实现，或用 usort
来源：http://hz.jqgfzy.top/gtfersszez.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.zycfv.cn/gtzehowcfm.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.hysaishi.cn/gtubjzpskx.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.zhixingplan.top/gtgglsukpk.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.nanxuanxn.top/gtpfodedec.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.jlsjyb.cn/gtgvgglstk.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.chenzaomai.com/gtvmwmivve.html

[N04] 斐波那契数列
来源：http://hz.iojbl.cn/gttariupgz.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.sxryk.cn/gtxbsgyhtb.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.yanxiufei.cn/gtvfefoahr.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.zhoulong.xyz/gtthbifgzp.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.yueranfly.top/gtmvgbdoki.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.yuxming.cn/gtzdrpyqot.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.jlsjyb.cn/gtevofthzd.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.hysaishi.cn/gtfzrxaucp.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.dashuyun.cn/gtkgvcvzfj.html

[N05] 最大公约数
来源：http://hz.xuanzx.com/gtriyynool.html

Py:   math.gcd(a, b)
来源：http://hz.sweek.top/gtdytdtjlv.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.iojbl.cn/gtsxbpxqct.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.fzhhl.top/gtsxxspiqv.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.ywan-chungtsiang.top/gtkltawxks.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.sweek.top/gtbzxcjpca.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.daxiang520.top/gtllncmljj.html

Ruby: a.gcd(b)
来源：http://hz.0kj1m.cn/gthduzswfc.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.iojbl.cn/gtkeinobhh.html

[N06] 判断回文字符串
来源：http://hz.xziqi.cn/gtmeqcpttn.html

Py:   s == s[::-1]
来源：http://hz.chenlongwang.top/gtdpgevehz.html

PHP:  $s === strrev($s);
来源：http://hz.dianchejie.cn/gtliljgpmk.html

JS:   s === [...s].reverse().join("")
来源：http://hz.nanxinkj.top/gtstrnpmad.html

TS:   s === [...s].reverse().join("")
来源：http://hz.iojbl.cn/gtomrszevw.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.jinghuilouyu.cn/gtfjltxujc.html

Go:   // 双指针从两端比较
来源：http://hz.jinyuanbaomall.cn/gtsnczdlkf.html

Ruby: s == s.reverse
来源：http://hz.guannengcc.top/gtjydsfyqc.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.ydzc1.top/gtgmvrziur.html

[N07] 两数之和（返回下标）
来源：http://hz.hysaishi.cn/gtxnfumeoi.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.ivvv.top/gtfsikyuvt.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.yueranfly.top/gtrnrlzcaw.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.zhoulong.xyz/gttpspnmzg.html

TS:   // 手写 Map<string, number>
来源：http://hz.mhx1999.top/gtgkhiplvd.html

Java: // 手写 HashMap
来源：http://hz.zhiwuduotai.top/gtdwuupvaq.html

Go:   // 手写 map[int]int
来源：http://hz.wangdashe.top/gttuxqwavq.html

Ruby: // 手写 Hash
来源：http://hz.meibo888.top/gtcpkqdhxw.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.yueranfly.top/gtmolssdkf.html

[N08] 生成全排列
来源：http://hz.zhongyouzk.top/gtwiprdimh.html

Py:   itertools.permutations(arr)
来源：http://hz.snrcjt.cn/gtspcbytag.html

PHP:  // 手写递归交换
来源：http://hz.shuidangran.top/gtqqnucvwc.html

JS:   // 手写回溯递归
来源：http://hz.smart0.xyz/gtexwuiqcf.html

TS:   // 手写回溯递归
来源：http://hz.andypj.xyz/gtxuakxzey.html

Java: // 手写回溯递归
来源：http://hz.havefunace.top/gtqncjnfqo.html

Go:   // 手写回溯递归
来源：http://hz.dashuyun.cn/gtqvvieksi.html

Ruby: arr.permutation.to_a
来源：http://hz.jyoumei.cn/gtigkosmbh.html

C#:   // 手写回溯递归
来源：http://hz.pengpengdd.cyou/gtvjdnvdrd.html

[N09] 栈与队列
来源：http://hz.tianlin.xyz/gttlfxfgln.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.52xcode.cn/gtwoatrxyg.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.jinqigfzy.top/gtpjakiyqp.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.shzxlz.cn/gtutdyubtw.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.daxiang520.top/gtpcapjbbt.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.daxiang520.top/gtujnhkpnk.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.feifeiyinyue.top/gtqyfmvkqq.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.jiagoushi.top/gtivmmgwwx.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.pycfn.com/gtjlvugkhr.html

[N10] 链表节点定义
来源：http://hz.zhaomingkeji.xyz/gtstfxlxws.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.hammf.cn/gtzxdgerse.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.nwbrower.top/gtplzlrhmr.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.jqgfzy.top/gtrclkslis.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.gaohongyu789.top/gthyrbigjt.html

Java: class Node { int v; Node next; }
来源：http://hz.yj20258888.top/gtyzoozyeg.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.redwolf501.top/gtppwfcbdm.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.ydjk.org.cn/gtlytfyczv.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.yuxming.cn/gtmlluegzs.html

[N11] 二叉树中序遍历
来源：http://hz.tanke756.top/gtkydpymkz.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.sxryk.cn/gtymtvednu.html

PHP:  // 手写递归函数
来源：http://hz.meibo888.top/gtogemtmzt.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.shangyingyoupin.top/gtdddrdpjf.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.c1oappe.top/gtjzqdxbbt.html

Java: // 手写递归
来源：http://hz.fengsongda.top/gtyxvckles.html

Go:   // 手写递归
来源：http://hz.chenjidiqi.icu/gtyzizhacr.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.shzxlz.cn/gticwlmtyx.html

C#:   // 手写递归
来源：http://hz.yongpay.top/gtsutoabgh.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.zdqjudy.top/gtfrzwrwfx.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.xingfuxueyuan.xyz/gtmucxiwwe.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.zhijiandao.cn/gtuycapmow.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.vqdsnc.cn/gtdfkzwxku.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.daxiang520.top/gtaqwatovs.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.ybcxt.top/gtytqydcrt.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.zhiwuduotai.top/gtnotzehiq.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.dashuyun.cn/gtunjccsgc.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.tianlin.xyz/gtzomwxiiu.html

================================================================================
来源：http://hz.dashuyun.cn/gtbctqhbvk.html

O. 并发与异步
来源：http://hz.xylfe.cn/gthalgnode.html

================================================================================
来源：http://hz.zdqjudy.top/gtgrgojqup.html

[O01] 启动一个线程
来源：http://hz.jinqigufen.top/gtryswzoje.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.cqqwz.cn/gtijzevxhk.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.jinyuanbaomall.cn/gtpjibydhf.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.redwolf501.top/gtdyysgjfn.html

TS:   // 同 JS
来源：http://hz.ydzc1.top/gtifvottnr.html

Java: new Thread(() -> f()).start()
来源：http://hz.wangdashe.top/gtbayybgca.html

Go:   go f()
来源：http://hz.bjfxy.top/gtljsihezy.html

Ruby: Thread.new { f }
来源：http://hz.jinyuanbaomall.cn/gtypgtzhnr.html

C#:   Task.Run(() => F());
来源：http://hz.kuanghao11.cn/gtiekzkwin.html

[O02] 使用线程池
来源：http://hz.shuidangran.top/gtwsdlwinc.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.shuidangran.top/gtanqyftvu.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.sxryk.cn/gtvdumdzbc.html

JS:   // worker_threads 线程池
来源：http://hz.chenjidiqi.icu/gtxfqpcykw.html

TS:   // worker_threads 线程池
来源：http://hz.pycfn.com/gtnzvrtmqo.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.yongpay.top/gtbfwgvgmt.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.zycfv.cn/gtqprivnth.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.ehwqpu.com/gtlaknbfuu.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.9152youxi.cn/gtqmlcvelc.html

[O03] 加锁保护共享数据
来源：http://hz.shanyushiyangkeji.top/gtfkludixy.html

Py:   with lock: shared += 1
来源：http://hz.yueranfly.top/gtjqdlujgj.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.sweek.top/gtmpppprgz.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.fzhhl.top/gtmjcutair.html

TS:   // 同 JS
来源：http://hz.cheryme.top/gtcpacruda.html

Java: synchronized (this) { shared++; }
来源：http://hz.yanxiufei.cn/gtbdjqsrsn.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.c1oappe.top/gttfalzydg.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.zycfv.cn/gtsvnfdduu.html

C#:   lock (gate) { shared++; }
来源：http://hz.yvedp.cn/gtrljlwxmj.html

[O04] 定义异步函数并等待
来源：http://hz.ppjwa.cn/gtvgdtqnax.html

Py:   async def f():⏎    await g()
来源：http://hz.ybcxt.top/gtaurcfxwe.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.tanke756.top/gtouowofgg.html

JS:   async function f() { await g(); }
来源：http://hz.sysykeji.top/gtbswdqdyi.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.hammf.cn/gtvmptfjiu.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.jyoumei.cn/gtdvfpmvwi.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.zhongyouzk.top/gtvqzlcnoz.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.dashuyun.cn/gtjvlslfkd.html

C#:   async Task F() { await G(); }
来源：http://hz.sxryk.cn/gtrxjikjsq.html

[O05] 并发执行并等待全部完成
来源：http://hz.havefunace.top/gtcthokwlz.html

Py:   asyncio.gather(*tasks)
来源：http://hz.chenzaomai.com/gtyljgdotm.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.kuanghao11.cn/gtaxzlscea.html

JS:   await Promise.all(tasks)
来源：http://hz.aizwys.cn/gtmupsdzrt.html

TS:   await Promise.all(tasks)
来源：http://hz.yangfankeji.com/gtfgmqkkqv.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.jlsjyb.cn/gtigghpuwx.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.shzxlz.cn/gtpevrojre.html

Ruby: threads.map(&:join)
来源：http://hz.dashuyun.cn/gtzsxwgwpo.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.chenjidiqi.icu/gtdyonxmmy.html

[O06] 使用进程池
来源：http://hz.tian-w.cn/gtjdljucrx.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.9152youxi.cn/gtesmzqfdn.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.yj20258888.top/gtqqzyjnji.html

JS:   // child_process / cluster 模块
来源：http://hz.gogol.net.cn/gtmxssxzeh.html

TS:   // child_process / cluster 模块
来源：http://hz.redwolf501.top/gtsihwtksu.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.jlsjyb.cn/gtzgryfxtf.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.nwbrower.top/gtoufoozen.html

Ruby: // fork 块
来源：http://hz.zdqjudy.top/gtxqvuqgfn.html

C#:   Parallel.For
来源：http://hz.fengsongda.top/gtklztywqr.html

================================================================================
来源：http://hz.yueranfly.top/gtequucuiw.html

P. 常用工具函数
来源：http://hz.hongshengwenyu.top/gturzbbypi.html

================================================================================
来源：http://hz.sxryk.cn/gtrpeqvyub.html

[P01] 生成 UUID
来源：http://hz.guowangkeji.top/gtihgivhmi.html

Py:   str(uuid.uuid4())
来源：http://hz.iojbl.cn/gtdlhkjdom.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.wangshuangyany.cn/gtsgneovye.html

JS:   crypto.randomUUID()
来源：http://hz.meibo888.top/gtvpygdssb.html

TS:   crypto.randomUUID()
来源：http://hz.havefunace.top/gteznlgods.html

Java: UUID.randomUUID().toString()
来源：http://hz.chenjidiqi.icu/gthldagauy.html

Go:   // 用 github.com/google/uuid
来源：http://hz.aizwys.cn/gtwvtkyfyi.html

Ruby: SecureRandom.uuid
来源：http://hz.yj202588.top/gtnsuanhcn.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.cdnleiting.top/gtihmmpqto.html

[P02] MD5 / SHA256 摘要
来源：http://hz.cucudq.cn/gtlaojzjyd.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.nanxinkj.top/gtkwdaotze.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.gaohongyu789.top/gtggrdfwgr.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.meibo888.top/gtwvnbcinb.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.guowangkeji.top/gtdwzsynbx.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.guowangkeji.top/gtchhszcdk.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.yvedp.cn/gtdvaxhhsa.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.bjfxy.top/gtqvxrqleo.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.yongpay.top/gteytgrvee.html

[P03] 生成短随机字符串
来源：http://hz.xuanzx.com/gtjbuufuzh.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.fzhhl.top/gtoarnitla.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.dashuyun.cn/gtkrodkqsy.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.yj202588.top/gtaakcchyt.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.wangshuangyany.cn/gtvevpycvo.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.jinghuilouyu.cn/gtarhsprng.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.nanxuanxn.top/gtnehokhim.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.daxiang520.top/gtklmqzhux.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.52xcode.cn/gtcwtpfsqx.html

[P04] 求长度
来源：http://hz.cheryme.top/gttyifkiss.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.jyoumei.cn/gtxftvxoow.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.mhx1999.top/gtedncaunz.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.daria6918.cn/gtnymdisli.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.wangdashe.top/gtzpmszato.html

Java: list.size();  map.size();  s.length()
来源：http://hz.shanyushiyangkeji.top/gtauzankez.html

Go:   len(arr);  len(m)
来源：http://hz.ydzc1.top/gtzqkrxoyc.html

Ruby: x.length;  x.size
来源：http://hz.yanxiufei.cn/gttjpcaffx.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.pengpengdd.cyou/gtsenqddow.html

[P05] 判断两个对象内容是否相等
来源：http://hz.sysykeji.top/gtuehepyiw.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.jinqigufen.top/gthbrejmjz.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.daria6918.cn/gtfwrggjwg.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.yuxming.cn/gtwwieihsr.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.cashguo.top/gtbxugwokj.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.dashuyun.cn/gthdqifwif.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.meibo888.top/gtbwyiwnwe.html

Ruby: a == b
来源：http://hz.guowangkeji.top/gtdnvpjnjg.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.andypj.xyz/gtpeevwale.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.yueranfly.top/gteeulmubw.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.jiagoushi.top/gtfwtvfbxo.html

PHP:  if (empty($x)) {}
来源：http://hz.xuetiantiany.cn/gtjacgdluz.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.yuxming.cn/gtferfmjyn.html

TS:   if (x == null) {}
来源：http://hz.vqdsnc.cn/gtlfpygihg.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.iojbl.cn/gtmurgdnff.html

Go:   if x == nil {}
来源：http://hz.zhongyouzk.top/gtsvzgqfnx.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.gaohongyu789.top/gtieanukpu.html

C#:   if (x is null) {}
来源：http://hz.wangdashe.top/gtentmljov.html

[P07] 防抖与节流
来源：http://hz.guannengcc.top/gtjczrfghp.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.yj202588.top/gtxydxrtlv.html

PHP:  // 手写时间戳比较
来源：http://hz.ybcxt.top/gtfibqncmb.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.dashuyun.cn/gtewpixwvd.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.fzhhl.top/gtohrfpdfa.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.zdqjudy.top/gtbqnifnsm.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.chenjidiqi.icu/gtafchllnh.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.yonumen.top/gtyombeyix.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.yuanzhike.top/gtustpughq.html

[P08] 处理浮点精度问题
来源：http://hz.fzhhl.top/gtkixdubku.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.zhengqikj.top/gtvxtinzrc.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.chenzaomai.com/gthtnwsznt.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.bjfxy.top/gtjxrlpaus.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.316326.xyz/gtnivewquw.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.kuanghao11.cn/gtxfyujhzr.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.pycfn.com/gtnrhurnsr.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.vqdsnc.cn/gtabdnqtau.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.sxryk.cn/gtjbgkresm.html


<!-- 参考信息 -->