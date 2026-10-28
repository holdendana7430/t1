代发 wailian999

[M04] 获取当前工作目录
来源：http://hz.guowangkeji.top/gtwkfyldai.html

Py:   os.getcwd()
来源：http://hz.xinyue.icu/gtarvoljat.html

PHP:  getcwd();
来源：http://hz.hysaishi.cn/gtefztxhcw.html

JS:   process.cwd()
来源：http://hz.snrcjt.cn/gtdytonixv.html

TS:   process.cwd()
来源：http://hz.jianghu66.top/gtughqoqly.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.wangshuangyany.cn/gtewmtjsjh.html

Go:   os.Getwd()
来源：http://hz.cucudq.cn/gtokrtnugo.html

Ruby: Dir.pwd
来源：http://hz.zhaomingkeji.xyz/gtplkbimue.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.316326.xyz/gtjehbcefj.html

[M05] 设置退出码
来源：http://hz.vqdsnc.cn/gtmwiyrion.html

Py:   sys.exit(1)
来源：http://hz.jinqigfzy.top/gtocicxccj.html

PHP:  exit(1);
来源：http://hz.zhijiandao.cn/gtendcqyto.html

JS:   process.exit(1)
来源：http://hz.yueranfly.top/gtwzkbyrdx.html

TS:   process.exit(1)
来源：http://hz.aizwys.cn/gtfuzewwjv.html

Java: System.exit(1)
来源：http://hz.ydzc1.top/gtltuumdge.html

Go:   os.Exit(1)
来源：http://hz.sufxvd.cn/gtkzjlxiet.html

Ruby: exit 1
来源：http://hz.gotoacloud.top/gtkpnffjsy.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.yj20258888.top/gttnorzoxb.html

[M06] 向标准错误输出
来源：http://hz.nwbrower.top/gtviffrypz.html

Py:   print("err", file=sys.stderr)
来源：http://hz.daxiang520.top/gtmhqmnjdc.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.zhaomingkeji.xyz/gtaljcekps.html

JS:   console.error("err")
来源：http://hz.cucudq.cn/gtwqejvjro.html

TS:   console.error("err")
来源：http://hz.jiagoushi.top/gtxuwbbbcq.html

Java: System.err.println("err")
来源：http://hz.hywenlv.cn/gtwpfgpzlp.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.fengsongda.top/gtizxbpwry.html

Ruby: warn "err"
来源：http://hz.jqgufenzy.top/gtnotnshnm.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.jianghu66.top/gtfaxyacgn.html

[M07] 判断是否为主入口
来源：http://hz.xuetiantiany.cn/gtgksrpvrw.html

Py:   if __name__ == "__main__":
来源：http://hz.cheryme.top/gtzasxrxwg.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.yangfankeji.com/gtkwahskrg.html

JS:   require.main === module
来源：http://hz.hywenlv.cn/gtuwhbsthq.html

TS:   require.main === module
来源：http://hz.shangyingyoupin.top/gttqwheume.html

Java: public static void main(String[] args)
来源：http://hz.wangdashe.top/gtbikmrqlr.html

Go:   func main()
来源：http://hz.yonumen.top/gttepgtzip.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.chenjidiqi.icu/gtbphasqjt.html

C#:   static void Main(string[] args)
来源：http://hz.hfpthk.cn/gtlouonrzo.html

[M08] 获取系统与运行时信息
来源：http://hz.nanxinkj.top/gtqvoilkds.html

Py:   platform.system();  platform.python_version()
来源：http://hz.cqqwz.cn/gtwtlymrsm.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.zhengqikj.top/gtjplhjxte.html

JS:   process.platform;  process.version
来源：http://hz.havefunace.top/gtusmxqvwk.html

TS:   process.platform;  process.version
来源：http://hz.hfpthk.cn/gtavonqnzx.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.daxiang520.top/gtsuwozwea.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.cashguo.top/gthiroidrz.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.9152youxi.cn/gtmmbiwlqs.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.hnqzz.top/gtigwkmuki.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtmxtllsvn.html

N. 数据结构与算法
来源：http://hz.bjfxy.top/gtaxteinxh.html

================================================================================
来源：http://hz.hysaishi.cn/gtzeasdpbd.html

[N01] 二分查找（有序数组）
来源：http://hz.hysaishi.cn/gtzbujdiwe.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.smart0.xyz/gtiufwcggl.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.xinyue.icu/gtvxueuobl.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.shanyushiyangtech.top/gtypaooxpf.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.hnxiangtu.top/gtjqufjtgm.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.shzxlz.cn/gtebcypwbl.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.c1oappe.top/gtewiipexj.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.xylfe.cn/gtznksuumc.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.ehwqpu.com/gtyhhjxvvu.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.chenlongwang.top/gtnabiqwqt.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.yongpay.top/gtkmrtofmo.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.shzxlz.cn/gtmtutcojn.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.chenjidiqi.icu/gtbelbiglx.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.hammf.cn/gtosttkkfn.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.ydzc1.top/gtgxuuidys.html

Go:   slices.Sort(arr)
来源：http://hz.guannengcc.top/gtyoxaufdj.html

Ruby: arr.sort
来源：http://hz.xuanzx.com/gtktlpxcsz.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.hywenlv.cn/gtffjlygvo.html

[N03] 快速排序（分治示例）
来源：http://hz.guowangkeji.top/gtsqqmsvvb.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.yvedp.cn/gtyzneyfcn.html

PHP:  // 递归实现，或用 usort
来源：http://hz.316326.xyz/gtdilkwmke.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.xziqi.cn/gtsbvtapfa.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.cucudq.cn/gtdjjxaawy.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.hysaishi.cn/gtlcngeoao.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.sxryk.cn/gtlnjmkzye.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.feifeiyinyue.top/gtubeopvpo.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.bjfxy.top/gtqzevjecf.html

[N04] 斐波那契数列
来源：http://hz.hywenlv.cn/gtskuwosnq.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.nanxuanxn.top/gtvtnvzsol.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.chenjidiqi.icu/gtcmgfjlws.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.tian-w.cn/gtoxgzxtsu.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.pycfn.com/gtifzxgdxy.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.ydzc1.top/gtgucyuflw.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.yvedp.cn/gtastcwlsq.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.nanxinkj.top/gtucsmcsbd.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.jianghu66.top/gtdvfapdxm.html

[N05] 最大公约数
来源：http://hz.tianlin.xyz/gtyzkrrbbn.html

Py:   math.gcd(a, b)
来源：http://hz.hfpthk.cn/gtaenjsfyr.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.sxryk.cn/gtzcshfnje.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.dianchejie.cn/gtieqbnmim.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.jianghu66.top/gtzbasqvza.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.hammf.cn/gtqklpylmf.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.hongshengwenyu.top/gtkzclqlrg.html

Ruby: a.gcd(b)
来源：http://hz.yanxiufei.cn/gtjsjskeom.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.tianlin.xyz/gtufrryyfc.html

[N06] 判断回文字符串
来源：http://hz.xinyue.icu/gtwnxlenlh.html

Py:   s == s[::-1]
来源：http://hz.dashuyun.cn/gtsbshctnb.html

PHP:  $s === strrev($s);
来源：http://hz.chenjidiqi.icu/gtsmxuevek.html

JS:   s === [...s].reverse().join("")
来源：http://hz.cashguo.top/gtjhaxqaon.html

TS:   s === [...s].reverse().join("")
来源：http://hz.ydjk.org.cn/gtufrkwxyx.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.jlsjyb.cn/gtczijosgj.html

Go:   // 双指针从两端比较
来源：http://hz.shzxlz.cn/gtnnivwxug.html

Ruby: s == s.reverse
来源：http://hz.sxryk.cn/gtxrgzjaew.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.chenjidiqi.icu/gtpbtctpuq.html

[N07] 两数之和（返回下标）
来源：http://hz.birdmap.top/gtwhtvfnbg.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.nanxuanxn.top/gtcshpmhrw.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.yueranfly.top/gtxkzsrugt.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.sysykeji.top/gtqudcshqt.html

TS:   // 手写 Map<string, number>
来源：http://hz.sxryk.cn/gtqbfqripw.html

Java: // 手写 HashMap
来源：http://hz.yanxiufei.cn/gtlgxbgizp.html

Go:   // 手写 map[int]int
来源：http://hz.bjfxy.top/gtnguosfjc.html

Ruby: // 手写 Hash
来源：http://hz.gogol.net.cn/gtfcrflzgh.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.nanxinkj.top/gtvagavjlt.html

[N08] 生成全排列
来源：http://hz.guowangkeji.top/gtdwviuiqb.html

Py:   itertools.permutations(arr)
来源：http://hz.jianghu66.top/gtytrfbiiu.html

PHP:  // 手写递归交换
来源：http://hz.guowangkeji.top/gtkbcodbtj.html

JS:   // 手写回溯递归
来源：http://hz.jinqigufen.top/gtukpcuefw.html

TS:   // 手写回溯递归
来源：http://hz.316326.xyz/gtooiubfhs.html

Java: // 手写回溯递归
来源：http://hz.ppjwa.cn/gtbqhuaolc.html

Go:   // 手写回溯递归
来源：http://hz.hywenlv.cn/gtvvlaazlp.html

Ruby: arr.permutation.to_a
来源：http://hz.chenjidiqi.icu/gtptyasdxa.html

C#:   // 手写回溯递归
来源：http://hz.zhaomingkeji.xyz/gtdurednuf.html

[N09] 栈与队列
来源：http://hz.aibaodan.cn/gtwlhakptp.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.gaohongyu789.top/gtfrhyepvl.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.bjfxy.top/gtyncqcihe.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.dashuyun.cn/gtuasusjiu.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.xuetiantiany.cn/gtiyvrtzld.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.52xcode.cn/gtbebapfik.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.zycfv.cn/gttsjxshxc.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.yuanzhike.top/gtwjpxtkfi.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.dashuyun.cn/gtodsjmzmk.html

[N10] 链表节点定义
来源：http://hz.shuidangran.top/gtzuznvkyi.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.shangyingyoupin.top/gtjikxaigl.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.zdqjudy.top/gtjolsxxqb.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.c1oappe.top/gtrluydmbp.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.sxryk.cn/gtpcxeosyx.html

Java: class Node { int v; Node next; }
来源：http://hz.sweek.top/gtytuozyde.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.ydzc1.top/gtslotfqxo.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.bjfxy.top/gtordumvat.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.gzhubu.top/gtelnvspkf.html

[N11] 二叉树中序遍历
来源：http://hz.ywan-chungtsiang.top/gtjgcbytts.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.jianghu66.top/gtzjisdbui.html

PHP:  // 手写递归函数
来源：http://hz.feifeiyinyue.top/gtcvpyvblk.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.gzhubu.top/gtucqcpdwo.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.yongpay.top/gtsrrfzoqn.html

Java: // 手写递归
来源：http://hz.xuanzx.com/gtkdjueagf.html

Go:   // 手写递归
来源：http://hz.shanyushiyangkeji.top/gtolnonzdn.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.daxiang520.top/gtvemxbykh.html

C#:   // 手写递归
来源：http://hz.yuxming.cn/gtyesgkszm.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.meibo888.top/gteburtdax.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.jinqigfzy.top/gtfyajlzci.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.9152youxi.cn/gtsfvfkjnf.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.havefunace.top/gtrxtnchqr.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.zdqjudy.top/gtwdmcfcgk.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.gotoacloud.top/gtpsjsruph.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.jinqigfzy.top/gtjabzmbqm.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.gaohongyu789.top/gtgthpnfkn.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.ehwqpu.com/gtxluyucpu.html

================================================================================
来源：http://hz.jyoumei.cn/gtwufwvyii.html

O. 并发与异步
来源：http://hz.hongshengwenyu.top/gtawhpywfh.html

================================================================================
来源：http://hz.pycfn.com/gtoveaafkh.html

[O01] 启动一个线程
来源：http://hz.dianchejie.cn/gtbxsvlcsh.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.sxryk.cn/gtfwqmzpqn.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.gogol.net.cn/gtkrramvom.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.svipenyu.cn/gtedscbgwb.html

TS:   // 同 JS
来源：http://hz.cucudq.cn/gtvzyocnoc.html

Java: new Thread(() -> f()).start()
来源：http://hz.aizwys.cn/gtwyliruiq.html

Go:   go f()
来源：http://hz.nanxuanxn.top/gtfaeoikeb.html

Ruby: Thread.new { f }
来源：http://hz.pycfn.com/gttidgidno.html

C#:   Task.Run(() => F());
来源：http://hz.zhongyouzk.top/gtqwfwekff.html

[O02] 使用线程池
来源：http://hz.sufxvd.cn/gtvxurhnnx.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.nwbrower.top/gtgmllyayb.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.hywenlv.cn/gtiimltzfp.html

JS:   // worker_threads 线程池
来源：http://hz.xingfuxueyuan.xyz/gtheloqdnc.html

TS:   // worker_threads 线程池
来源：http://hz.ydzc1.top/gttpckdesx.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.jiagoushi.top/gtljzvzmpq.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.zhoulong.xyz/gtphizxbki.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.fzhhl.top/gtfwkjeevv.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.haohaochexian.top/gtoeuvkjya.html

[O03] 加锁保护共享数据
来源：http://hz.yj20258.top/gtuvoduhiy.html

Py:   with lock: shared += 1
来源：http://hz.quarkkingdee.top/gtoeqraojo.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.yonumen.top/gtucmgadlk.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.yvedp.cn/gtcjaqomtp.html

TS:   // 同 JS
来源：http://hz.ydzc1.top/gtssowyjdc.html

Java: synchronized (this) { shared++; }
来源：http://hz.cheryme.top/gturppjhcj.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.kuanghao11.cn/gtexjcbtob.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.jyoumei.cn/gttakjotet.html

C#:   lock (gate) { shared++; }
来源：http://hz.jiagoushi.top/gtgaegturd.html

[O04] 定义异步函数并等待
来源：http://hz.snrcjt.cn/gtgnrdebnl.html

Py:   async def f():⏎    await g()
来源：http://hz.wangdashe.top/gtovbhcxus.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.bjfxy.top/gtbmnstikg.html

JS:   async function f() { await g(); }
来源：http://hz.xinyue.icu/gtkmppaafh.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.dashuyun.cn/gttzietess.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.pengpengdd.cyou/gthqteylvk.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.gotoacloud.top/gtbgsnbdyz.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.yuanzhike.top/gtyerpbjjk.html

C#:   async Task F() { await G(); }
来源：http://hz.jinyuanbaomall.cn/gthsficjzl.html

[O05] 并发执行并等待全部完成
来源：http://hz.pycfn.com/gtrfosdrke.html

Py:   asyncio.gather(*tasks)
来源：http://hz.cheryme.top/gtuphiucfi.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.wangdashe.top/gtuzwsxptr.html

JS:   await Promise.all(tasks)
来源：http://hz.chenzaomai.com/gtnqqxkvon.html

TS:   await Promise.all(tasks)
来源：http://hz.aibaodan.cn/gtezmgrahy.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.guowangkeji.top/gtkpkptsvv.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.zhaomingkeji.xyz/gtfxroqsyu.html

Ruby: threads.map(&:join)
来源：http://hz.tian-w.cn/gtkhnvhgwp.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.ywan-chungtsiang.top/gtilusotuh.html

[O06] 使用进程池
来源：http://hz.shzxlz.cn/gticvimntx.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.zhoulong.xyz/gtggydutus.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.xuetiantiany.cn/gthkntrnlu.html

JS:   // child_process / cluster 模块
来源：http://hz.hongshengwenyu.top/gtbrwvwiiz.html

TS:   // child_process / cluster 模块
来源：http://hz.jinqigufen.top/gtuytnremj.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.daxiang520.top/gtlbmpiljj.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.jinyuanbaomall.cn/gtbumwcuxk.html

Ruby: // fork 块
来源：http://hz.cdnleiting.top/gtwgkmggfh.html

C#:   Parallel.For
来源：http://hz.ydzc1.top/gthogqhhwa.html

================================================================================
来源：http://hz.yj202588.top/gtlwutmqyw.html

P. 常用工具函数
来源：http://hz.yueranfly.top/gtdwvkmpby.html

================================================================================
来源：http://hz.jiagoushi.top/gtsxgiwkip.html

[P01] 生成 UUID
来源：http://hz.shanyushiyangtech.top/gtwanagozc.html

Py:   str(uuid.uuid4())
来源：http://hz.chenzaomai.com/gtxhksjtkx.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.sxryk.cn/gtlueawrkg.html

JS:   crypto.randomUUID()
来源：http://hz.jinyuanbaomall.cn/gtmbkwnpie.html

TS:   crypto.randomUUID()
来源：http://hz.sweek.top/gtclaolnwe.html

Java: UUID.randomUUID().toString()
来源：http://hz.zhengqikj.top/gthquofpwc.html

Go:   // 用 github.com/google/uuid
来源：http://hz.tianlin.xyz/gtfiwxxgos.html

Ruby: SecureRandom.uuid
来源：http://hz.pycfn.com/gtfoueigev.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.zhoulong.xyz/gtntwcwrqx.html

[P02] MD5 / SHA256 摘要
来源：http://hz.snrcjt.cn/gtxvphjylx.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.jqgfzy.top/gtunvkbmjs.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.hammf.cn/gttmhauqwl.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.jlsjyb.cn/gtymgrauma.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.yuanzhike.top/gtczahwyaw.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.snrcjt.cn/gtlfjrdydk.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.ppjwa.cn/gtpfnurghu.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.shzxlz.cn/gtisdpsfyf.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.guannengcc.top/gtsanvdtyu.html

[P03] 生成短随机字符串
来源：http://hz.0kj1m.cn/gtdketdhrx.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.wangshuangyany.cn/gtmdprnief.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.ydjk.org.cn/gtofsgnmzo.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.iojbl.cn/gtyjxxawio.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.ydjk.org.cn/gtjovnoggx.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.nanxuanxn.top/gthffcbdxj.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.ydzc1.top/gtqbdrflke.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.cqqwz.cn/gtrezjpxgp.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.hnxiangtu.top/gtshreewkk.html

[P04] 求长度
来源：http://hz.shzxlz.cn/gthxpbcqmr.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.pycfn.com/gtjdhiijek.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.jyoumei.cn/gthpzuswem.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.zdqjudy.top/gtgktidkle.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.sxryk.cn/gtfzqmwzcr.html

Java: list.size();  map.size();  s.length()
来源：http://hz.zdqjudy.top/gtnvfzmhcr.html

Go:   len(arr);  len(m)
来源：http://hz.fengsongda.top/gtbddwaaty.html

Ruby: x.length;  x.size
来源：http://hz.jlsjyb.cn/gthkehvujw.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.pycfn.com/gtnhqrpuiy.html

[P05] 判断两个对象内容是否相等
来源：http://hz.xziqi.cn/gtwwmbmdoe.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.wangshuangyany.cn/gtahuwwddt.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.quarkkingdee.top/gtfwewdeex.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.cucudq.cn/gtpknhvyjg.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.xinyue.icu/gtfjmxpsjf.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.yueranfly.top/gtqareaqqx.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.ywan-chungtsiang.top/gtpcaclyjt.html

Ruby: a == b
来源：http://hz.xziqi.cn/gtfjrtpoll.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.jinqigufen.top/gtkichxyuc.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.hysaishi.cn/gtoqwcbyfm.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.kuanghao11.cn/gtxuboypit.html

PHP:  if (empty($x)) {}
来源：http://hz.jinqigufen.top/gtrtfbtljn.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.jinyuanbaomall.cn/gtitfxeqsx.html

TS:   if (x == null) {}
来源：http://hz.jinqigufen.top/gtatqbbqyf.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.redwolf501.top/gtypycgcet.html

Go:   if x == nil {}
来源：http://hz.ehwqpu.com/gtjuzyynzc.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.chenlongwang.top/gtertmstte.html

C#:   if (x is null) {}
来源：http://hz.tian-w.cn/gtotqwjizu.html

[P07] 防抖与节流
来源：http://hz.52xcode.cn/gtuheutkoz.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.sysykeji.top/gtqwfsmzut.html

PHP:  // 手写时间戳比较
来源：http://hz.jyoumei.cn/gtrygwombd.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.yj202588.top/gtoqcxcurv.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.cqqwz.cn/gtfoslwtrd.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.52xcode.cn/gtidxtfcvp.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.yongpay.top/gtbcdvxiko.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.pengpengdd.cyou/gtgliwxgwf.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.52xcode.cn/gtlpoyfica.html

[P08] 处理浮点精度问题
来源：http://hz.yvedp.cn/gtjyacecfz.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.ehwqpu.com/gtzmkirljp.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.pycfn.com/gtrzkwdggu.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.cashguo.top/gtgryhpwij.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.daxiang520.top/gtbmnodsxd.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.sysykeji.top/gtuzmxwcge.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.svipenyu.cn/gtdvcnhhqo.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.yangfankeji.com/gtonhesxcq.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.aizwys.cn/gtgebkzpdz.html

================================================================================
来源：http://hz.guannengcc.top/gtxuqnbyfv.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.kuanghao11.cn/gterokjsgn.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtvxhjgajd.html

[Q01] 创建表
来源：http://hz.ppjwa.cn/gtlayyurzv.html

CREATE TABLE users (
来源：http://hz.aizwys.cn/gtywwornei.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.andypj.xyz/gtfswodmgk.html

name VARCHAR(50) NOT NULL,
来源：http://hz.aizwys.cn/gtqepjexmp.html

email VARCHAR(100) UNIQUE,
来源：http://hz.kuanghao11.cn/gtqmptsftq.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.xuanzx.com/gtgvocyqvb.html

);
来源：http://hz.ehwqpu.com/gtwfbolozq.html

[Q02] 创建带外键的表
来源：http://hz.iojbl.cn/gtkepsvxrw.html

CREATE TABLE orders (
来源：http://hz.tianlin.xyz/gtjznpotjb.html


<!-- 参考信息 -->