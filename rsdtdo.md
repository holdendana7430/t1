代发 wailian999

[M04] 获取当前工作目录
来源：http://hz.zhongyouzk.top/gtovrrvrjm.html

Py:   os.getcwd()
来源：http://hz.dianchejie.cn/gtimjxuryf.html

PHP:  getcwd();
来源：http://hz.hnxiangtu.top/gtljxfqpaz.html

JS:   process.cwd()
来源：http://hz.feifeiyinyue.top/gtmzryvciz.html

TS:   process.cwd()
来源：http://hz.fzhhl.top/gtxzoceljq.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.yangfankeji.com/gtafzwlfeb.html

Go:   os.Getwd()
来源：http://hz.ydzc1.top/gtwvfxmngm.html

Ruby: Dir.pwd
来源：http://hz.c1oappe.top/gtjjzsbwcf.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.c1oappe.top/gtrjtfklfj.html

[M05] 设置退出码
来源：http://hz.fzhhl.top/gthjjxbaxj.html

Py:   sys.exit(1)
来源：http://hz.pycfn.com/gthjfetubj.html

PHP:  exit(1);
来源：http://hz.gzhubu.top/gtinqzvfbc.html

JS:   process.exit(1)
来源：http://hz.nanxinkj.top/gtzqbrsejo.html

TS:   process.exit(1)
来源：http://hz.hfpthk.cn/gtxujmirgh.html

Java: System.exit(1)
来源：http://hz.wangshuangyany.cn/gtwljiwmlh.html

Go:   os.Exit(1)
来源：http://hz.zdqjudy.top/gtxiyklwvc.html

Ruby: exit 1
来源：http://hz.yj20258.top/gtuzmzaptr.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.shangyingyoupin.top/gtxnqznvne.html

[M06] 向标准错误输出
来源：http://hz.quarkkingdee.top/gtmfwwibpj.html

Py:   print("err", file=sys.stderr)
来源：http://hz.gogol.net.cn/gtuhgerkrx.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.nanxuanxn.top/gtuyygkjxs.html

JS:   console.error("err")
来源：http://hz.smart0.xyz/gttlzqbiql.html

TS:   console.error("err")
来源：http://hz.ydjk.org.cn/gtjtmrnuno.html

Java: System.err.println("err")
来源：http://hz.fzhhl.top/gtvssmtrhv.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.ehwqpu.com/gtuewhmzai.html

Ruby: warn "err"
来源：http://hz.daria6918.cn/gtpiktdppz.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.cqqwz.cn/gtdpciihuw.html

[M07] 判断是否为主入口
来源：http://hz.yuanzhike.top/gtxruzxgnx.html

Py:   if __name__ == "__main__":
来源：http://hz.cheryme.top/gttnlatoin.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.cashguo.top/gtrittsxws.html

JS:   require.main === module
来源：http://hz.fzhhl.top/gtcbrfjhos.html

TS:   require.main === module
来源：http://hz.cdnleiting.top/gtmnfecduw.html

Java: public static void main(String[] args)
来源：http://hz.yueranfly.top/gtprrqevhy.html

Go:   func main()
来源：http://hz.wangshuangyany.cn/gtvnhswwoj.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.shanyushiyangtech.top/gtgsojldoc.html

C#:   static void Main(string[] args)
来源：http://hz.xingfuxueyuan.xyz/gtuhvlcotk.html

[M08] 获取系统与运行时信息
来源：http://hz.kuanghao11.cn/gtbcdcckck.html

Py:   platform.system();  platform.python_version()
来源：http://hz.quarkkingdee.top/gtkzcqunsx.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.yangfankeji.com/gtiponxivu.html

JS:   process.platform;  process.version
来源：http://hz.dianchejie.cn/gtufdefdov.html

TS:   process.platform;  process.version
来源：http://hz.ehwqpu.com/gteqhssenj.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.birdmap.top/gtqgtdhsqj.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.ehwqpu.com/gtwadqnvtc.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.zhijiandao.cn/gtfqodugkt.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.wangdashe.top/gtkretfryk.html

================================================================================
来源：http://hz.dashuyun.cn/gtqwzpqrcp.html

N. 数据结构与算法
来源：http://hz.ybcxt.top/gtkmjsfzho.html

================================================================================
来源：http://hz.jqgfzy.top/gtnclehqzz.html

[N01] 二分查找（有序数组）
来源：http://hz.shanyushiyangtech.top/gtldkioleq.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.hammf.cn/gtfschlzfc.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.mhx1999.top/gtsqdpohlo.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.gaohongyu789.top/gtehxzlsyr.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.jinghuilouyu.cn/gtilwxtyoc.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.yangfankeji.com/gtdjqebemg.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.tianlin.xyz/gtndairfek.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.birdmap.top/gtuqcsahdx.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.dashuyun.cn/gtvdnegfmo.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.daria6918.cn/gtsrlafqyd.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.sxryk.cn/gtkffdmfoi.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.dashuyun.cn/gtqrjqnpqt.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.meibo888.top/gtplpodwla.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.redwolf501.top/gtnzmkaxzr.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.shanyushiyangkeji.top/gtndrdtuct.html

Go:   slices.Sort(arr)
来源：http://hz.mhx1999.top/gtdxhikqqm.html

Ruby: arr.sort
来源：http://hz.xuetiantiany.cn/gtobowzrai.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.guannengcc.top/gtlgexrlsl.html

[N03] 快速排序（分治示例）
来源：http://hz.tanke756.top/gtekckfezd.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.xingfuxueyuan.xyz/gtweziysgn.html

PHP:  // 递归实现，或用 usort
来源：http://hz.meibo888.top/gtvjnruevm.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.9152youxi.cn/gtmfrcyzob.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.zhaomingkeji.xyz/gtrjsjixdj.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.shuidangran.top/gtwghywaaf.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.cqqwz.cn/gtbevqhfaz.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.hnqzz.top/gtptyuilos.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.hywenlv.cn/gtvcycgbvx.html

[N04] 斐波那契数列
来源：http://hz.dashuyun.cn/gtqwrmdfix.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.nanxinkj.top/gtulruqzcc.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.0kj1m.cn/gtrsnhfcyf.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.ybcxt.top/gtrhobkhev.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.jianghu66.top/gtuwpplqei.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.jinyuanbaomall.cn/gtuxtrxche.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.shzxlz.cn/gteydrmynb.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.xuetiantiany.cn/gtpaleeiyo.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.smart0.xyz/gtcuiavvym.html

[N05] 最大公约数
来源：http://hz.vqdsnc.cn/gttzdvwikf.html

Py:   math.gcd(a, b)
来源：http://hz.jianghu66.top/gtdbhlffhx.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.xziqi.cn/gtakaovokm.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.chenlongwang.top/gtbiqqenqm.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.chenzaomai.com/gtjclmhnzl.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.wangdashe.top/gtjpdtivyw.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.havefunace.top/gtvziitqhk.html

Ruby: a.gcd(b)
来源：http://hz.tanke756.top/gtognjnxji.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.yuanzhike.top/gtpzkeogfn.html

[N06] 判断回文字符串
来源：http://hz.jinqigfzy.top/gtuuaykntu.html

Py:   s == s[::-1]
来源：http://hz.hywenlv.cn/gtjnyzafpu.html

PHP:  $s === strrev($s);
来源：http://hz.fzhhl.top/gtlsstzxjg.html

JS:   s === [...s].reverse().join("")
来源：http://hz.hnqzz.top/gthndvyief.html

TS:   s === [...s].reverse().join("")
来源：http://hz.sysykeji.top/gthxpzsfft.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.shzxlz.cn/gtbfaajwob.html

Go:   // 双指针从两端比较
来源：http://hz.cheryme.top/gtkztrlwhp.html

Ruby: s == s.reverse
来源：http://hz.snrcjt.cn/gtrbojnpgt.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.jiagoushi.top/gtymmdydvv.html

[N07] 两数之和（返回下标）
来源：http://hz.xuetiantiany.cn/gtylrbtwqr.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.52xcode.cn/gtatoivksm.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.zhaomingkeji.xyz/gthwbhcgku.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.0kj1m.cn/gthvkexiyn.html

TS:   // 手写 Map<string, number>
来源：http://hz.ybcxt.top/gtmyygywul.html

Java: // 手写 HashMap
来源：http://hz.cdnleiting.top/gtqcntfbwj.html

Go:   // 手写 map[int]int
来源：http://hz.jqgufenzy.top/gtltmcmkab.html

Ruby: // 手写 Hash
来源：http://hz.wangdashe.top/gthspokamk.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.zhoulong.xyz/gtmfclilch.html

[N08] 生成全排列
来源：http://hz.52xcode.cn/gtnjzqawzu.html

Py:   itertools.permutations(arr)
来源：http://hz.wangdashe.top/gtxcsoxjge.html

PHP:  // 手写递归交换
来源：http://hz.yuanzhike.top/gtzxididxx.html

JS:   // 手写回溯递归
来源：http://hz.snrcjt.cn/gtbtyynuvq.html

TS:   // 手写回溯递归
来源：http://hz.hnxiangtu.top/gtdlymegup.html

Java: // 手写回溯递归
来源：http://hz.wangshuangyany.cn/gtyesdpwlh.html

Go:   // 手写回溯递归
来源：http://hz.xinyue.icu/gtazeusqok.html

Ruby: arr.permutation.to_a
来源：http://hz.sxryk.cn/gtobfbzpkl.html

C#:   // 手写回溯递归
来源：http://hz.hnqzz.top/gtrveycyse.html

[N09] 栈与队列
来源：http://hz.shangyingyoupin.top/gtxlrprzis.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.aibaodan.cn/gthwggksdj.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.nanxinkj.top/gtcxsjjxdr.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.ywan-chungtsiang.top/gtfshxdjzo.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.ehwqpu.com/gtxruvqvsx.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.tianlin.xyz/gtamaavros.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.tianlin.xyz/gtptzunleo.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.snrcjt.cn/gtwxeevkqs.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.wangdashe.top/gtdiebbnaj.html

[N10] 链表节点定义
来源：http://hz.ppjwa.cn/gtstjngejo.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.zhongyouzk.top/gtatpngumn.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.tianlin.xyz/gtqyybtkyq.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.zycfv.cn/gthgpnevdf.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.jyoumei.cn/gtlluerlmj.html

Java: class Node { int v; Node next; }
来源：http://hz.hongshengwenyu.top/gtslnjyxpi.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.dashuyun.cn/gtyzygaces.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.nanxuanxn.top/gtuoqdfjyj.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.wangdashe.top/gtuyihzvwl.html

[N11] 二叉树中序遍历
来源：http://hz.chenzaomai.com/gttmgoidxy.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.hnqzz.top/gtqxuyzvba.html

PHP:  // 手写递归函数
来源：http://hz.yvedp.cn/gtooeeveyw.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.jinqigufen.top/gtpwdsqqds.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.nwbrower.top/gtrmouksnm.html

Java: // 手写递归
来源：http://hz.ydzc1.top/gtaysgohee.html

Go:   // 手写递归
来源：http://hz.jlsjyb.cn/gtvexlyyoj.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.shzxlz.cn/gtbmuopamf.html

C#:   // 手写递归
来源：http://hz.jinqigufen.top/gtpxiocedm.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.tian-w.cn/gtlqoudhcx.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.pengpengdd.cyou/gtxgtwzine.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.pycfn.com/gtgrpkplqu.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.cdnleiting.top/gtpjwdcgmx.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.zycfv.cn/gttcjndudq.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.0kj1m.cn/gtwrkkenbz.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.hfpthk.cn/gtvhggaufm.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.shangyingyoupin.top/gtphgrmhii.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.snrcjt.cn/gtbpsxzmmh.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtmckctadn.html

O. 并发与异步
来源：http://hz.snrcjt.cn/gtdbrxmudh.html

================================================================================
来源：http://hz.vqdsnc.cn/gtrxudcwkb.html

[O01] 启动一个线程
来源：http://hz.kuanghao11.cn/gtchdecvmm.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.iojbl.cn/gtgchwlgtq.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.zhiwuduotai.top/gtsagnzdql.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.yvedp.cn/gtftydgjzh.html

TS:   // 同 JS
来源：http://hz.yj202588.top/gtzwcbjlxr.html

Java: new Thread(() -> f()).start()
来源：http://hz.meibo888.top/gtpglqyavt.html

Go:   go f()
来源：http://hz.quarkkingdee.top/gthnmlpcbz.html

Ruby: Thread.new { f }
来源：http://hz.shzxlz.cn/gtbvforsik.html

C#:   Task.Run(() => F());
来源：http://hz.daria6918.cn/gtnviytbwn.html

[O02] 使用线程池
来源：http://hz.fzhhl.top/gtkosmmlpz.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.cashguo.top/gtfwnxmmtp.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.ehwqpu.com/gtfeiollsd.html

JS:   // worker_threads 线程池
来源：http://hz.haohaochexian.top/gtgsrzqmaj.html

TS:   // worker_threads 线程池
来源：http://hz.jyoumei.cn/gtgpogosgb.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.hnxiangtu.top/gthdpqkgsp.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.pycfn.com/gtjjxnuofx.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.yanxiufei.cn/gtiekpuvfb.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.tianlin.xyz/gtomtwzizs.html

[O03] 加锁保护共享数据
来源：http://hz.iojbl.cn/gtgckpdira.html

Py:   with lock: shared += 1
来源：http://hz.sufxvd.cn/gtuqheabyr.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.zhengqikj.top/gtgotvsmbv.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.smart0.xyz/gtbciuxmlu.html

TS:   // 同 JS
来源：http://hz.ywan-chungtsiang.top/gthzhkjkke.html

Java: synchronized (this) { shared++; }
来源：http://hz.xinyue.icu/gtmpftzgka.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.chenzaomai.com/gtijzdikkg.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.haohaochexian.top/gtdchjgtuq.html

C#:   lock (gate) { shared++; }
来源：http://hz.jinqigfzy.top/gtpgewgysl.html

[O04] 定义异步函数并等待
来源：http://hz.daria6918.cn/gtoevvltrk.html

Py:   async def f():⏎    await g()
来源：http://hz.chenlongwang.top/gtuiobplgc.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.fzhhl.top/gtjftbgqjz.html

JS:   async function f() { await g(); }
来源：http://hz.quarkkingdee.top/gtqiuzasyp.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.andypj.xyz/gtwpoambai.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.sufxvd.cn/gtrjeqcagu.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.tian-w.cn/gtuhfbeucx.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.quarkkingdee.top/gtkfwlncyi.html

C#:   async Task F() { await G(); }
来源：http://hz.nwbrower.top/gtjgboqorm.html

[O05] 并发执行并等待全部完成
来源：http://hz.aibaodan.cn/gtcpeunncy.html

Py:   asyncio.gather(*tasks)
来源：http://hz.meibo888.top/gthrvmintg.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.ppjwa.cn/gtwnvnsian.html

JS:   await Promise.all(tasks)
来源：http://hz.andypj.xyz/gtfnknnbfd.html

TS:   await Promise.all(tasks)
来源：http://hz.dashuyun.cn/gtofupaepj.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.shzxlz.cn/gtehxcbxlo.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.shanyushiyangtech.top/gtxjvnojye.html

Ruby: threads.map(&:join)
来源：http://hz.zhongyouzk.top/gtqqbgydwq.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.fzhhl.top/gtxcyraamz.html

[O06] 使用进程池
来源：http://hz.gzhubu.top/gtrbelngiq.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.tanke756.top/gtsutkbmud.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.birdmap.top/gtwzasysib.html

JS:   // child_process / cluster 模块
来源：http://hz.jiagoushi.top/gtlrqzxldc.html

TS:   // child_process / cluster 模块
来源：http://hz.cashguo.top/gtdyuefauk.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.wangdashe.top/gtiwblqrge.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.cashguo.top/gtjnxxzyag.html

Ruby: // fork 块
来源：http://hz.xingfuxueyuan.xyz/gtefnlubah.html

C#:   Parallel.For
来源：http://hz.sufxvd.cn/gtgfrtxdfv.html

================================================================================
来源：http://hz.svipenyu.cn/gtwytygwmy.html

P. 常用工具函数
来源：http://hz.nanxuanxn.top/gtntctbrnk.html

================================================================================
来源：http://hz.dianchejie.cn/gtusbgcsrz.html

[P01] 生成 UUID
来源：http://hz.zhaomingkeji.xyz/gtpltbvzqt.html

Py:   str(uuid.uuid4())
来源：http://hz.tanke756.top/gthbtybcyw.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.svipenyu.cn/gtmjznxuqx.html

JS:   crypto.randomUUID()
来源：http://hz.jinqigfzy.top/gtpbmbsedo.html

TS:   crypto.randomUUID()
来源：http://hz.bjfxy.top/gtgkdfeubh.html

Java: UUID.randomUUID().toString()
来源：http://hz.jinqigufen.top/gtfwohxplw.html

Go:   // 用 github.com/google/uuid
来源：http://hz.hnqzz.top/gtsonxzuao.html

Ruby: SecureRandom.uuid
来源：http://hz.daria6918.cn/gtilbgjqxr.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.chenjidiqi.icu/gtztdwnjjs.html

[P02] MD5 / SHA256 摘要
来源：http://hz.jiagoushi.top/gtvqspoftc.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.zdqjudy.top/gtahsexraf.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.xziqi.cn/gtgheeosnt.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.wangshuangyany.cn/gtnygfofvq.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.hammf.cn/gtjsapmygx.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.ivvv.top/gtbjyexcag.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.zhengqikj.top/gtjdqzfyxp.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.zhengqikj.top/gtadlhjwah.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.hywenlv.cn/gtkiopgpvn.html

[P03] 生成短随机字符串
来源：http://hz.0kj1m.cn/gtcgvicsqk.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.xuanzx.com/gthhqupnsf.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.tianlin.xyz/gtacudxtoh.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.xuetiantiany.cn/gtozllyxdx.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.andypj.xyz/gtfjecxrng.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.hywenlv.cn/gtynmryfrd.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.yuanzhike.top/gtnpludvch.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.jqgfzy.top/gttqcngncj.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.zhaomingkeji.xyz/gtkgiedtkz.html

[P04] 求长度
来源：http://hz.cashguo.top/gtcohtdzwq.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.jlsjyb.cn/gtpkddvzio.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.ydzc1.top/gtlltcchow.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.yongpay.top/gtsbpxorgx.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.xinyue.icu/gthakukhzr.html

Java: list.size();  map.size();  s.length()
来源：http://hz.hysaishi.cn/gtyamakaro.html

Go:   len(arr);  len(m)
来源：http://hz.yuxming.cn/gtlpdahscs.html

Ruby: x.length;  x.size
来源：http://hz.fengsongda.top/gtyfnsraax.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.ywan-chungtsiang.top/gtvpgtysky.html

[P05] 判断两个对象内容是否相等
来源：http://hz.daxiang520.top/gtnpsztltj.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.zhijiandao.cn/gtlnpspfiq.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.ybcxt.top/gtqlkppmif.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.yongpay.top/gtlrpeiqhw.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.feifeiyinyue.top/gtnpfmqooa.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.sxryk.cn/gtdbrnsnxf.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.daria6918.cn/gtunhraxdp.html

Ruby: a == b
来源：http://hz.birdmap.top/gtphysoihc.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.yanxiufei.cn/gtjznhvtfe.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.hammf.cn/gthfmnwpuu.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.sxryk.cn/gtrurbafqv.html

PHP:  if (empty($x)) {}
来源：http://hz.tian-w.cn/gtylgweivh.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.daxiang520.top/gteflnelyx.html

TS:   if (x == null) {}
来源：http://hz.pengpengdd.cyou/gtyxlbpojb.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.dashuyun.cn/gtymucayku.html

Go:   if x == nil {}
来源：http://hz.ydjk.org.cn/gtsowrlstb.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.iojbl.cn/gtfbuszllm.html

C#:   if (x is null) {}
来源：http://hz.zhijiandao.cn/gtmannpcyy.html

[P07] 防抖与节流
来源：http://hz.zhengqikj.top/gtquinzhub.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.316326.xyz/gthplntpic.html

PHP:  // 手写时间戳比较
来源：http://hz.hywenlv.cn/gtejvwvjqk.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.yj20258.top/gtodcjpnxu.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.jinqigfzy.top/gtygsdlqgw.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.ppjwa.cn/gtgobyzfov.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.sxryk.cn/gtoiexitrw.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.xylfe.cn/gtfyesllfl.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.hysaishi.cn/gtispfiapj.html

[P08] 处理浮点精度问题
来源：http://hz.jinghuilouyu.cn/gthxqktzco.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.nanxuanxn.top/gtjnvowdpt.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.jinqigufen.top/gtiykfhbef.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.xinyue.icu/gtyxtmykkh.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.c1oappe.top/gtooqwomqd.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.yj20258.top/gtddamvomx.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.fengsongda.top/gtibqgmqix.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.birdmap.top/gtrxhyqrog.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.tian-w.cn/gtlcibfqef.html

================================================================================
来源：http://hz.svipenyu.cn/gtlrhvlefr.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.wangdashe.top/gtwemozjbo.html

================================================================================
来源：http://hz.vqdsnc.cn/gtwxtvrhpl.html

[Q01] 创建表
来源：http://hz.jinghuilouyu.cn/gtwvvymqka.html

CREATE TABLE users (
来源：http://hz.pengpengdd.cyou/gtlqzqdrsk.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.aizwys.cn/gtldoilgup.html

name VARCHAR(50) NOT NULL,
来源：http://hz.xuetiantiany.cn/gtttuuwrfk.html

email VARCHAR(100) UNIQUE,
来源：http://hz.hongshengwenyu.top/gtdyqtvybb.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.mhx1999.top/gthhgwutyq.html

);
来源：http://hz.fengsongda.top/gthaylrvsz.html

[Q02] 创建带外键的表
来源：http://hz.xylfe.cn/gtlnehmvrl.html

CREATE TABLE orders (
来源：http://hz.vqdsnc.cn/gthuujegce.html


<!-- 参考信息 -->