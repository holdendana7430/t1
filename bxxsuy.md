代发 wailian999

TS:   process.cwd()
来源：http://hz.yj20258.top/gtmogshgwy.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.jqgufenzy.top/gtbqopkkjs.html

Go:   os.Getwd()
来源：http://hz.daria6918.cn/gtipvyolff.html

Ruby: Dir.pwd
来源：http://hz.tian-w.cn/gtkfztyzxs.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.sysykeji.top/gtnjqzutll.html

[M05] 设置退出码
来源：http://hz.haohaochexian.top/gtacsztlwy.html

Py:   sys.exit(1)
来源：http://hz.hongshengwenyu.top/gtlhgroptg.html

PHP:  exit(1);
来源：http://hz.xuetiantiany.cn/gtuaxaihfq.html

JS:   process.exit(1)
来源：http://hz.gaohongyu789.top/gtmwburhup.html

TS:   process.exit(1)
来源：http://hz.xuanzx.com/gtmbtzmeuw.html

Java: System.exit(1)
来源：http://hz.daxiang520.top/gtosroewmu.html

Go:   os.Exit(1)
来源：http://hz.haohaochexian.top/gthoqkwchb.html

Ruby: exit 1
来源：http://hz.birdmap.top/gtjwiviebg.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.chenjidiqi.icu/gtdfxnnawx.html

[M06] 向标准错误输出
来源：http://hz.haohaochexian.top/gtsdqckwyk.html

Py:   print("err", file=sys.stderr)
来源：http://hz.xylfe.cn/gtdjhbtzin.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.xziqi.cn/gtakaybnhp.html

JS:   console.error("err")
来源：http://hz.pycfn.com/gtthuvhfzw.html

TS:   console.error("err")
来源：http://hz.wangshuangyany.cn/gtcqslhqkk.html

Java: System.err.println("err")
来源：http://hz.snrcjt.cn/gtwvcjqxxe.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.zhixingplan.top/gtwifiqaxr.html

Ruby: warn "err"
来源：http://hz.shzxlz.cn/gtvuivuuat.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.shzxlz.cn/gtdbangwsp.html

[M07] 判断是否为主入口
来源：http://hz.aizwys.cn/gtosfdfhcp.html

Py:   if __name__ == "__main__":
来源：http://hz.chenlongwang.top/gtzbxjetwk.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.hammf.cn/gtpmvlxadp.html

JS:   require.main === module
来源：http://hz.snrcjt.cn/gtntwejexr.html

TS:   require.main === module
来源：http://hz.ehwqpu.com/gtlcgvscac.html

Java: public static void main(String[] args)
来源：http://hz.jinyuanbaomall.cn/gtzkpjsvlq.html

Go:   func main()
来源：http://hz.jianghu66.top/gtkstcvuae.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.zdqjudy.top/gtxojdgtzf.html

C#:   static void Main(string[] args)
来源：http://hz.tanke756.top/gtvugxkswh.html

[M08] 获取系统与运行时信息
来源：http://hz.kuanghao11.cn/gtwgnzcewy.html

Py:   platform.system();  platform.python_version()
来源：http://hz.nwbrower.top/gtnexwdcbx.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.daxiang520.top/gthgotbcfl.html

JS:   process.platform;  process.version
来源：http://hz.zhijiandao.cn/gtpebuxles.html

TS:   process.platform;  process.version
来源：http://hz.hnqzz.top/gtrwcjscdf.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.pycfn.com/gtrbpmerqn.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.chenlongwang.top/gtbmenhtrq.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.hnxiangtu.top/gtssvemria.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.yangfankeji.com/gtbycgjiui.html

================================================================================
来源：http://hz.fzhhl.top/gtuurucjoo.html

N. 数据结构与算法
来源：http://hz.andypj.xyz/gtjofrbgsd.html

================================================================================
来源：http://hz.shangyingyoupin.top/gthvzptzni.html

[N01] 二分查找（有序数组）
来源：http://hz.jinqigufen.top/gtbsuouzne.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.andypj.xyz/gtchvlwxcz.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.jinyuanbaomall.cn/gtxhjxshcn.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.hammf.cn/gththglwpg.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.nanxinkj.top/gtxcajlsyv.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.jqgufenzy.top/gtwmbdaxcy.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.zhoulong.xyz/gtcprkdans.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.jinqigfzy.top/gtzmjhkzfp.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.bjfxy.top/gtdzjrkvcu.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.gotoacloud.top/gtxietzssn.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.sysykeji.top/gtxnxkxbab.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.shzxlz.cn/gtdckdxpax.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.316326.xyz/gtrhmypnsp.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.shangyingyoupin.top/gtknmmqsje.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.hnxiangtu.top/gtlzbgrtii.html

Go:   slices.Sort(arr)
来源：http://hz.gzhubu.top/gtkfppwbqr.html

Ruby: arr.sort
来源：http://hz.52xcode.cn/gtqdpqxvjy.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.redwolf501.top/gtpuwrpvxm.html

[N03] 快速排序（分治示例）
来源：http://hz.sysykeji.top/gtclutajsl.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.wangshuangyany.cn/gtnzrlkcnc.html

PHP:  // 递归实现，或用 usort
来源：http://hz.xingfuxueyuan.xyz/gtnppyltdn.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.fzhhl.top/gtbrwefoxo.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.ywan-chungtsiang.top/gtoyvaafqj.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.jinghuilouyu.cn/gtcjzixcay.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.chenjidiqi.icu/gtuotbbijm.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.jqgufenzy.top/gtpwqhnlfn.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.yonumen.top/gtjchqihii.html

[N04] 斐波那契数列
来源：http://hz.fengsongda.top/gtrfeaurzd.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.jinqigufen.top/gtctgzfqmr.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.yuxming.cn/gtwrhlqupj.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.jinghuilouyu.cn/gtqzkstvqt.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.havefunace.top/gtctcugldu.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.feifeiyinyue.top/gtygpjadqs.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.wangdashe.top/gtqzoixcti.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.xinyue.icu/gtlycrtlqy.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.ydjk.org.cn/gtftdqsdbm.html

[N05] 最大公约数
来源：http://hz.shzxlz.cn/gtzhohruuy.html

Py:   math.gcd(a, b)
来源：http://hz.haohaochexian.top/gtlmuabjqc.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.cashguo.top/gtuveqnubj.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.yongpay.top/gtjozzsuye.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.c1oappe.top/gtuyyirvou.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.yuanzhike.top/gtrtavbxzx.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.ivvv.top/gtqsqqgqyv.html

Ruby: a.gcd(b)
来源：http://hz.gzhubu.top/gtsbdfcnsq.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.cqqwz.cn/gtihenqjcf.html

[N06] 判断回文字符串
来源：http://hz.dashuyun.cn/gtxblwqppt.html

Py:   s == s[::-1]
来源：http://hz.haohaochexian.top/gtqnqygctb.html

PHP:  $s === strrev($s);
来源：http://hz.wangshuangyany.cn/gttjgpzqgj.html

JS:   s === [...s].reverse().join("")
来源：http://hz.feifeiyinyue.top/gtyjyfcbgq.html

TS:   s === [...s].reverse().join("")
来源：http://hz.zhixingplan.top/gtqcsermzk.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.vqdsnc.cn/gthkkscyve.html

Go:   // 双指针从两端比较
来源：http://hz.andypj.xyz/gtftwbkinx.html

Ruby: s == s.reverse
来源：http://hz.shanyushiyangtech.top/gtjzvpcfew.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.gzhubu.top/gtybpjvjph.html

[N07] 两数之和（返回下标）
来源：http://hz.tian-w.cn/gtbbkifmqi.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.kuanghao11.cn/gturjuopsq.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.xinyue.icu/gtuijtoidc.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.ywan-chungtsiang.top/gtemexuqdo.html

TS:   // 手写 Map<string, number>
来源：http://hz.zhiwuduotai.top/gtjakbdhdz.html

Java: // 手写 HashMap
来源：http://hz.cqqwz.cn/gtszbcojhe.html

Go:   // 手写 map[int]int
来源：http://hz.xingfuxueyuan.xyz/gtrfpsdnhc.html

Ruby: // 手写 Hash
来源：http://hz.gaohongyu789.top/gtplbeoexz.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.wangshuangyany.cn/gtsfsccolo.html

[N08] 生成全排列
来源：http://hz.sysykeji.top/gtfvunbpqi.html

Py:   itertools.permutations(arr)
来源：http://hz.yongpay.top/gtwsomcwnv.html

PHP:  // 手写递归交换
来源：http://hz.bjfxy.top/gtwvvyfzjc.html

JS:   // 手写回溯递归
来源：http://hz.havefunace.top/gtimokabsl.html

TS:   // 手写回溯递归
来源：http://hz.iojbl.cn/gtjcdylgiq.html

Java: // 手写回溯递归
来源：http://hz.hywenlv.cn/gtxaiyzcxe.html

Go:   // 手写回溯递归
来源：http://hz.chenlongwang.top/gtkehynnuz.html

Ruby: arr.permutation.to_a
来源：http://hz.wangshuangyany.cn/gtqlpjrwne.html

C#:   // 手写回溯递归
来源：http://hz.shuidangran.top/gtxztlcbet.html

[N09] 栈与队列
来源：http://hz.xingfuxueyuan.xyz/gtcukxkatc.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.wangshuangyany.cn/gthmymsrvp.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.0kj1m.cn/gtkfymejjm.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.shangyingyoupin.top/gtjirwgybd.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.xziqi.cn/gtaiyydjiq.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.zhijiandao.cn/gttdykhzzk.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.hfpthk.cn/gtaimsubdq.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.chenzaomai.com/gtnthcplfj.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.jinghuilouyu.cn/gtqgorqejk.html

[N10] 链表节点定义
来源：http://hz.cashguo.top/gtdybqpbbi.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.jinqigufen.top/gtdhxgsnjg.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.jianghu66.top/gtlxfkkldv.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.gotoacloud.top/gtevbzytgg.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.zhiwuduotai.top/gtyyzjcikj.html

Java: class Node { int v; Node next; }
来源：http://hz.nanxinkj.top/gtyzyxlxlj.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.ppjwa.cn/gtohermsfg.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.cashguo.top/gtlrexoaen.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.cucudq.cn/gtnuvixoce.html

[N11] 二叉树中序遍历
来源：http://hz.svipenyu.cn/gteoiqfnye.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.sysykeji.top/gthbtdyuvt.html

PHP:  // 手写递归函数
来源：http://hz.sxryk.cn/gtrpnthrfw.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.jyoumei.cn/gtuekoxwvz.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.9152youxi.cn/gtzzcyeuuf.html

Java: // 手写递归
来源：http://hz.cqqwz.cn/gtgxljnmqj.html

Go:   // 手写递归
来源：http://hz.xuetiantiany.cn/gtotjgmxxa.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.guowangkeji.top/gtwjyqdrro.html

C#:   // 手写递归
来源：http://hz.redwolf501.top/gtiprkkpgf.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.redwolf501.top/gtyotakdbs.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.hysaishi.cn/gtalfthetd.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.xziqi.cn/gtrxpcncgh.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.xziqi.cn/gtktumaoyd.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.cqqwz.cn/gtsxlbahzx.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.hfpthk.cn/gtkewwujhs.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.smart0.xyz/gthrrtcwgq.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.xinyue.icu/gtzigpfynh.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.yongpay.top/gtwiywcyem.html

================================================================================
来源：http://hz.hammf.cn/gtknwygcwt.html

O. 并发与异步
来源：http://hz.gotoacloud.top/gtkvssvlpu.html

================================================================================
来源：http://hz.yueranfly.top/gtfcbfacxh.html

[O01] 启动一个线程
来源：http://hz.gogol.net.cn/gthhojpyma.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.ppjwa.cn/gtasgzuums.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.yonumen.top/gtnwghsrll.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.nanxinkj.top/gtvihqhkwo.html

TS:   // 同 JS
来源：http://hz.smart0.xyz/gtqxgvuato.html

Java: new Thread(() -> f()).start()
来源：http://hz.redwolf501.top/gtygsrfmyf.html

Go:   go f()
来源：http://hz.zhixingplan.top/gtifiqjssr.html

Ruby: Thread.new { f }
来源：http://hz.xuetiantiany.cn/gtglejuvtt.html

C#:   Task.Run(() => F());
来源：http://hz.nanxinkj.top/gtwmgkqoqt.html

[O02] 使用线程池
来源：http://hz.jqgfzy.top/gtxfhbwyai.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.ppjwa.cn/gtmlnkofct.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.wangshuangyany.cn/gttfojelez.html

JS:   // worker_threads 线程池
来源：http://hz.bjfxy.top/gtqnojciix.html

TS:   // worker_threads 线程池
来源：http://hz.52xcode.cn/gtrpgfgxtn.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.jinyuanbaomall.cn/gtleszxobj.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.haohaochexian.top/gtlqvfduuq.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.shzxlz.cn/gterzucpkr.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.xziqi.cn/gtyzsyayuz.html

[O03] 加锁保护共享数据
来源：http://hz.havefunace.top/gtcjtxkdir.html

Py:   with lock: shared += 1
来源：http://hz.sysykeji.top/gtbnpweoor.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.sufxvd.cn/gtjfxletsl.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.haohaochexian.top/gtpsjthibd.html

TS:   // 同 JS
来源：http://hz.zhoulong.xyz/gtwoewolxf.html

Java: synchronized (this) { shared++; }
来源：http://hz.cheryme.top/gtzcuwfbdn.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.zycfv.cn/gtcpcuetuz.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.aizwys.cn/gtlgdjpctd.html

C#:   lock (gate) { shared++; }
来源：http://hz.hywenlv.cn/gtwdjgbuzf.html

[O04] 定义异步函数并等待
来源：http://hz.cqqwz.cn/gtkgkyquop.html

Py:   async def f():⏎    await g()
来源：http://hz.ivvv.top/gtfpnvjfiz.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.bjfxy.top/gtuftypuin.html

JS:   async function f() { await g(); }
来源：http://hz.nanxinkj.top/gtpoajfwwt.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.sweek.top/gtlicpchmv.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.ppjwa.cn/gtzmhpnafx.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.shanyushiyangkeji.top/gtfpobfayo.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.zhixingplan.top/gtxvpxrcjh.html

C#:   async Task F() { await G(); }
来源：http://hz.316326.xyz/gtweoxhjdd.html

[O05] 并发执行并等待全部完成
来源：http://hz.bjfxy.top/gtuknuwjqi.html

Py:   asyncio.gather(*tasks)
来源：http://hz.cucudq.cn/gtzhcsrahs.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.cdnleiting.top/gtzegfwewl.html

JS:   await Promise.all(tasks)
来源：http://hz.zhiwuduotai.top/gtdhamlhbd.html

TS:   await Promise.all(tasks)
来源：http://hz.yj20258.top/gtrnkmxuch.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.dianchejie.cn/gtdotxzzwl.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.mhx1999.top/gtzekjduzo.html

Ruby: threads.map(&:join)
来源：http://hz.yuanzhike.top/gtpotkmsyh.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.cdnleiting.top/gthrgarrto.html

[O06] 使用进程池
来源：http://hz.ybcxt.top/gtgmvyklgw.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.shanyushiyangkeji.top/gtdtkzhcze.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.zycfv.cn/gtqqoyssyc.html

JS:   // child_process / cluster 模块
来源：http://hz.cheryme.top/gtghxgbgid.html

TS:   // child_process / cluster 模块
来源：http://hz.yuxming.cn/gtgqfctmhf.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.nanxuanxn.top/gtsbrxqshe.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.pycfn.com/gtwnjrfeyk.html

Ruby: // fork 块
来源：http://hz.nanxuanxn.top/gtqwcinloa.html

C#:   Parallel.For
来源：http://hz.wangdashe.top/gtdlwdsmna.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtmkuwfetm.html

P. 常用工具函数
来源：http://hz.shanyushiyangtech.top/gtmbrqswer.html

================================================================================
来源：http://hz.ydzc1.top/gtdsyaduzf.html

[P01] 生成 UUID
来源：http://hz.mhx1999.top/gtoahpecby.html

Py:   str(uuid.uuid4())
来源：http://hz.yonumen.top/gtbawmaxjg.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.zhengqikj.top/gtiyfusmdd.html

JS:   crypto.randomUUID()
来源：http://hz.xinyue.icu/gtkmvzroxv.html

TS:   crypto.randomUUID()
来源：http://hz.shzxlz.cn/gtrcigouws.html

Java: UUID.randomUUID().toString()
来源：http://hz.shanyushiyangkeji.top/gtjcbirmzi.html

Go:   // 用 github.com/google/uuid
来源：http://hz.zdqjudy.top/gtmewiintr.html

Ruby: SecureRandom.uuid
来源：http://hz.jqgufenzy.top/gtiaaeknxu.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.shzxlz.cn/gtpogvtfis.html

[P02] MD5 / SHA256 摘要
来源：http://hz.yj20258.top/gterqremam.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.vqdsnc.cn/gthlxmwwjg.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.cdnleiting.top/gtrpujtylx.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.meibo888.top/gttzqmduap.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.yonumen.top/gtelbvjndu.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.svipenyu.cn/gtaxjsszjj.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.yj20258888.top/gtyzaqpnuw.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.0kj1m.cn/gtsmupcfct.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.c1oappe.top/gtfaybjeoq.html

[P03] 生成短随机字符串
来源：http://hz.dashuyun.cn/gtkssjsagk.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.redwolf501.top/gtnzpxmnui.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.aibaodan.cn/gthmapsaos.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.jqgfzy.top/gtkgvjpzhr.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.mhx1999.top/gtxbtntvvp.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.feifeiyinyue.top/gtrfqxuvzg.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.haohaochexian.top/gttnzucdps.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.zhengqikj.top/gtzkhtmblo.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.xinyue.icu/gtpnoiutoc.html

[P04] 求长度
来源：http://hz.zhongyouzk.top/gtrhsogjvx.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.c1oappe.top/gtfeekkznp.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.zhengqikj.top/gtkyszamya.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.316326.xyz/gttqyoyrei.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.52xcode.cn/gtzbjmhrng.html

Java: list.size();  map.size();  s.length()
来源：http://hz.mhx1999.top/gtlrnbmuey.html

Go:   len(arr);  len(m)
来源：http://hz.ybcxt.top/gtcjyffytr.html

Ruby: x.length;  x.size
来源：http://hz.havefunace.top/gtswhbnlcs.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.havefunace.top/gtxlzrfqbw.html

[P05] 判断两个对象内容是否相等
来源：http://hz.pycfn.com/gtdptzniiz.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.gaohongyu789.top/gtojmnadgx.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.yuanzhike.top/gtprgviaku.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.zhixingplan.top/gtlxtqwpgd.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.jianghu66.top/gtoxahwely.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.nwbrower.top/gtavimohjf.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.pengpengdd.cyou/gtylwrzgtl.html

Ruby: a == b
来源：http://hz.cdnleiting.top/gtikgsdiya.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.jinqigufen.top/gtpjgpaeax.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.tian-w.cn/gttnijypjw.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.havefunace.top/gteudilbdc.html

PHP:  if (empty($x)) {}
来源：http://hz.jyoumei.cn/gtzmxgbsch.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.xingfuxueyuan.xyz/gtarvfehjb.html

TS:   if (x == null) {}
来源：http://hz.zhaomingkeji.xyz/gtyvtumkub.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.ppjwa.cn/gtlmtukgau.html

Go:   if x == nil {}
来源：http://hz.snrcjt.cn/gtnlvjpnqk.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.zhengqikj.top/gtadomjgia.html

C#:   if (x is null) {}
来源：http://hz.fzhhl.top/gtuipbvkxt.html

[P07] 防抖与节流
来源：http://hz.ybcxt.top/gtbnqeaeda.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.gzhubu.top/gtlflkhgwf.html

PHP:  // 手写时间戳比较
来源：http://hz.jinyuanbaomall.cn/gtkmyzohxt.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.zdqjudy.top/gtbxrckbam.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.xylfe.cn/gtmkiutnfp.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.mhx1999.top/gttzomafzk.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.yvedp.cn/gtewknitta.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.havefunace.top/gtmsiadnhl.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.jinghuilouyu.cn/gtkqqhbiza.html

[P08] 处理浮点精度问题
来源：http://hz.chenzaomai.com/gtggogjxhs.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.xingfuxueyuan.xyz/gtcfelacwq.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.ppjwa.cn/gtjyogoqhj.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.nwbrower.top/gtimfbpqso.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.aizwys.cn/gtdgtvkmvs.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.andypj.xyz/gtkamwgblx.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.tianlin.xyz/gtkwuzptrm.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.redwolf501.top/gtnrmatvxg.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.birdmap.top/gthbjlmnzd.html

================================================================================
来源：http://hz.jianghu66.top/gtejnbbsvy.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.hfpthk.cn/gtpsunihxu.html

================================================================================
来源：http://hz.ydjk.org.cn/gtchtydnto.html

[Q01] 创建表
来源：http://hz.tanke756.top/gteomjcctv.html

CREATE TABLE users (
来源：http://hz.daria6918.cn/gtwkaqlywk.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.guannengcc.top/gtcrpmtpkr.html

name VARCHAR(50) NOT NULL,
来源：http://hz.hongshengwenyu.top/gtgiqznoof.html

email VARCHAR(100) UNIQUE,
来源：http://hz.zhoulong.xyz/gtnkkacewv.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.yuanzhike.top/gtnmddnwgd.html

);
来源：http://hz.316326.xyz/gtsibwlckk.html

[Q02] 创建带外键的表
来源：http://hz.yuanzhike.top/gtrxsnfgma.html

CREATE TABLE orders (
来源：http://hz.cdnleiting.top/gtfvodhraj.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.iojbl.cn/gtreaacznj.html

user_id INT NOT NULL,
来源：http://hz.vqdsnc.cn/gtdqpcimpk.html

amount DECIMAL(10, 2),
来源：http://hz.hammf.cn/gtxptpyefw.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.hysaishi.cn/gtkajscsuk.html


<!-- 参考信息 -->