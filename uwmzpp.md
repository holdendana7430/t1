代发 wailian999

C#:   Directory.GetCurrentDirectory()
来源：http://hz.aizwys.cn/gtsckpekpj.html

[M05] 设置退出码
来源：http://hz.gogol.net.cn/gtmqcqokhy.html

Py:   sys.exit(1)
来源：http://hz.hnqzz.top/gtpbbgjzfk.html

PHP:  exit(1);
来源：http://hz.yuanzhike.top/gtzmmvdzeq.html

JS:   process.exit(1)
来源：http://hz.xuetiantiany.cn/gtntytjxyg.html

TS:   process.exit(1)
来源：http://hz.yj20258.top/gtuvvdrqoc.html

Java: System.exit(1)
来源：http://hz.hammf.cn/gttwxdrfml.html

Go:   os.Exit(1)
来源：http://hz.xziqi.cn/gtgcltbpwa.html

Ruby: exit 1
来源：http://hz.pengpengdd.cyou/gtigunmtkr.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.jlsjyb.cn/gtnbpefowp.html

[M06] 向标准错误输出
来源：http://hz.0kj1m.cn/gtkxlppfqv.html

Py:   print("err", file=sys.stderr)
来源：http://hz.xylfe.cn/gthtdemjfw.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.shuidangran.top/gtjhpefgcy.html

JS:   console.error("err")
来源：http://hz.snrcjt.cn/gtnxtlrbqh.html

TS:   console.error("err")
来源：http://hz.sxryk.cn/gtlgdrhlyi.html

Java: System.err.println("err")
来源：http://hz.guowangkeji.top/gtjgegkhgv.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.birdmap.top/gtootgsboi.html

Ruby: warn "err"
来源：http://hz.yongpay.top/gtogfejoiu.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.c1oappe.top/gtnohkufpn.html

[M07] 判断是否为主入口
来源：http://hz.ydjk.org.cn/gtvhypkzxf.html

Py:   if __name__ == "__main__":
来源：http://hz.vqdsnc.cn/gtqwxasorb.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.kuanghao11.cn/gtkxfvhndk.html

JS:   require.main === module
来源：http://hz.meibo888.top/gtulyonvzo.html

TS:   require.main === module
来源：http://hz.sysykeji.top/gtwqfbedel.html

Java: public static void main(String[] args)
来源：http://hz.jinyuanbaomall.cn/gtupmmibhg.html

Go:   func main()
来源：http://hz.guannengcc.top/gtvmmbmzkb.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.tanke756.top/gtxfclzdhh.html

C#:   static void Main(string[] args)
来源：http://hz.jiagoushi.top/gthxuprdgt.html

[M08] 获取系统与运行时信息
来源：http://hz.shuidangran.top/gtcrwpokmn.html

Py:   platform.system();  platform.python_version()
来源：http://hz.shanyushiyangkeji.top/gtjqmqrdhk.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.dianchejie.cn/gtxndrnjrr.html

JS:   process.platform;  process.version
来源：http://hz.jiagoushi.top/gtiwuiudli.html

TS:   process.platform;  process.version
来源：http://hz.sxryk.cn/gttamdhtdt.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.xuanzx.com/gtdpehohdb.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.ehwqpu.com/gtgstbqxfk.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.zdqjudy.top/gtyzotdpfz.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.yj20258888.top/gthboacyje.html

================================================================================
来源：http://hz.zycfv.cn/gtnfacumtk.html

N. 数据结构与算法
来源：http://hz.c1oappe.top/gtplcvbmuu.html

================================================================================
来源：http://hz.xylfe.cn/gtphvxbpxb.html

[N01] 二分查找（有序数组）
来源：http://hz.ywan-chungtsiang.top/gtqqjqqumw.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.jinghuilouyu.cn/gtivlsznmc.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.pycfn.com/gtnbmndews.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.sweek.top/gtdkiuxhco.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.dashuyun.cn/gtdbmohuao.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.hongshengwenyu.top/gtwjjzbzix.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.smart0.xyz/gtzresnxir.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.zhijiandao.cn/gtlbxhpysa.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.9152youxi.cn/gtvzsgudbe.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.iojbl.cn/gtkurvfbsn.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.iojbl.cn/gtcmfbusjg.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.316326.xyz/gtussqimlo.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.xuetiantiany.cn/gtoveiwsmn.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.shuidangran.top/gtuizdbodz.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.sufxvd.cn/gtgiaptatg.html

Go:   slices.Sort(arr)
来源：http://hz.nanxuanxn.top/gtuyqzbvwo.html

Ruby: arr.sort
来源：http://hz.zhongyouzk.top/gtefdckdtd.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.cucudq.cn/gtcbqmanmo.html

[N03] 快速排序（分治示例）
来源：http://hz.ivvv.top/gtebyqyyfe.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.gaohongyu789.top/gtszkukxcu.html

PHP:  // 递归实现，或用 usort
来源：http://hz.zycfv.cn/gtosippbik.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.shzxlz.cn/gtdrtjczsg.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.xziqi.cn/gtwziiurxf.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.pengpengdd.cyou/gtbhmkiekh.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.birdmap.top/gtxkwmxhxy.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.yuxming.cn/gtrkvizuua.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.birdmap.top/gtxhbleuxd.html

[N04] 斐波那契数列
来源：http://hz.zhongyouzk.top/gttylomarz.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.jyoumei.cn/gtivyrwfwj.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.jiagoushi.top/gtqdpeoxyi.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.fengsongda.top/gtehbtdlbs.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.smart0.xyz/gtwmzjgnfw.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.0kj1m.cn/gtlwkhmdnx.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.zycfv.cn/gtalzzbzzp.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.wangshuangyany.cn/gtckoxkejs.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.yj20258.top/gtukyqqtae.html

[N05] 最大公约数
来源：http://hz.iojbl.cn/gtyfdmmxmi.html

Py:   math.gcd(a, b)
来源：http://hz.zdqjudy.top/gtaoqzruqh.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.jinghuilouyu.cn/gtcaozpqsd.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.hysaishi.cn/gtdqawsxji.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.9152youxi.cn/gtkuczebsf.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.quarkkingdee.top/gtbjrviycx.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.jinghuilouyu.cn/gtnemuphtz.html

Ruby: a.gcd(b)
来源：http://hz.vqdsnc.cn/gtizoxcqax.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.hysaishi.cn/gtequklwit.html

[N06] 判断回文字符串
来源：http://hz.yj20258.top/gtijxwekwj.html

Py:   s == s[::-1]
来源：http://hz.nanxuanxn.top/gthndsjghr.html

PHP:  $s === strrev($s);
来源：http://hz.dashuyun.cn/gtnyrvjfoy.html

JS:   s === [...s].reverse().join("")
来源：http://hz.yvedp.cn/gthwgtzegh.html

TS:   s === [...s].reverse().join("")
来源：http://hz.jqgufenzy.top/gthiptquew.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.dianchejie.cn/gterdzcljz.html

Go:   // 双指针从两端比较
来源：http://hz.pengpengdd.cyou/gtoxsbkwmm.html

Ruby: s == s.reverse
来源：http://hz.yonumen.top/gtrdsuzrxk.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.pengpengdd.cyou/gtaswwvmqk.html

[N07] 两数之和（返回下标）
来源：http://hz.yueranfly.top/gtqzcmsglv.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.xingfuxueyuan.xyz/gtcbyzbvxz.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.bjfxy.top/gtlmbavgss.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.hysaishi.cn/gtgeznodgn.html

TS:   // 手写 Map<string, number>
来源：http://hz.yj202588.top/gtfsfvseow.html

Java: // 手写 HashMap
来源：http://hz.chenlongwang.top/gtkzqdcxby.html

Go:   // 手写 map[int]int
来源：http://hz.feifeiyinyue.top/gtudvwbybl.html

Ruby: // 手写 Hash
来源：http://hz.zhongyouzk.top/gtauzplthw.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.zhijiandao.cn/gtjhtlhfub.html

[N08] 生成全排列
来源：http://hz.zhongyouzk.top/gthlvoqeep.html

Py:   itertools.permutations(arr)
来源：http://hz.jinqigufen.top/gtftvaulyv.html

PHP:  // 手写递归交换
来源：http://hz.0kj1m.cn/gtsxuvvrwf.html

JS:   // 手写回溯递归
来源：http://hz.dianchejie.cn/gtoyanydrk.html

TS:   // 手写回溯递归
来源：http://hz.cdnleiting.top/gtsnchbhkq.html

Java: // 手写回溯递归
来源：http://hz.jinqigufen.top/gtqtjduuzw.html

Go:   // 手写回溯递归
来源：http://hz.shangyingyoupin.top/gthvjeqqhw.html

Ruby: arr.permutation.to_a
来源：http://hz.jinyuanbaomall.cn/gtueapevnu.html

C#:   // 手写回溯递归
来源：http://hz.hammf.cn/gtdyzbrrnv.html

[N09] 栈与队列
来源：http://hz.0kj1m.cn/gtpciogvkk.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.yuxming.cn/gtzcyzdydo.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.0kj1m.cn/gtdygsfqha.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.yuxming.cn/gtdhyndpgz.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.cashguo.top/gtoomhgcan.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.jqgfzy.top/gtnfnrkmfi.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.wangdashe.top/gtlfzilpqq.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.svipenyu.cn/gtagfbqenn.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.havefunace.top/gtpzginqhn.html

[N10] 链表节点定义
来源：http://hz.fzhhl.top/gtlkpgutlk.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.ybcxt.top/gtzyxffuni.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.xinyue.icu/gtojehurvr.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.xziqi.cn/gtxirsdvjj.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.tanke756.top/gtaibjkmvl.html

Java: class Node { int v; Node next; }
来源：http://hz.snrcjt.cn/gtlbtvxmve.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.hywenlv.cn/gttaabbwrm.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.hnqzz.top/gtcnhcwxgr.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.yuxming.cn/gtivrultvh.html

[N11] 二叉树中序遍历
来源：http://hz.fengsongda.top/gtvmepofld.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.svipenyu.cn/gtzmrrffaj.html

PHP:  // 手写递归函数
来源：http://hz.fengsongda.top/gtowqtkpxj.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.hnqzz.top/gteubcuvzy.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.cdnleiting.top/gtkjfokqhi.html

Java: // 手写递归
来源：http://hz.zhoulong.xyz/gttnltcmdi.html

Go:   // 手写递归
来源：http://hz.yanxiufei.cn/gtrzouhjwv.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.jqgufenzy.top/gtbiewxdke.html

C#:   // 手写递归
来源：http://hz.sweek.top/gtcsdwrsih.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.tanke756.top/gtvneimnbv.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.chenlongwang.top/gtkzjuereq.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.9152youxi.cn/gtgnisjwua.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.yangfankeji.com/gthyimejnd.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.jiagoushi.top/gtspejflln.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.cashguo.top/gtvlgwfuqw.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.cheryme.top/gtzzxphnut.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.sweek.top/gtvkkuiweu.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.xziqi.cn/gteqgzcdve.html

================================================================================
来源：http://hz.ppjwa.cn/gtxkwvhjaj.html

O. 并发与异步
来源：http://hz.chenlongwang.top/gthrvasqgh.html

================================================================================
来源：http://hz.yonumen.top/gtynzyvxck.html

[O01] 启动一个线程
来源：http://hz.nanxinkj.top/gtpqkekjop.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.cdnleiting.top/gticwgevxm.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.zhengqikj.top/gthlrpuawz.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.shangyingyoupin.top/gtibdzswff.html

TS:   // 同 JS
来源：http://hz.0kj1m.cn/gtqofmoced.html

Java: new Thread(() -> f()).start()
来源：http://hz.cdnleiting.top/gtrqfnyzgl.html

Go:   go f()
来源：http://hz.jqgfzy.top/gtvchirroj.html

Ruby: Thread.new { f }
来源：http://hz.ywan-chungtsiang.top/gtrylutafj.html

C#:   Task.Run(() => F());
来源：http://hz.hnqzz.top/gtignpnilm.html

[O02] 使用线程池
来源：http://hz.yueranfly.top/gtodpmqsgk.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.hywenlv.cn/gtanggfsyl.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.nanxuanxn.top/gtahosxapf.html

JS:   // worker_threads 线程池
来源：http://hz.yuanzhike.top/gtjlkbxlex.html

TS:   // worker_threads 线程池
来源：http://hz.gaohongyu789.top/gtzpcupuoa.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.redwolf501.top/gtrgojutas.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.quarkkingdee.top/gtehittnve.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.ppjwa.cn/gttdlkeocb.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.xuetiantiany.cn/gtitrcokqy.html

[O03] 加锁保护共享数据
来源：http://hz.cheryme.top/gtiktzvjgd.html

Py:   with lock: shared += 1
来源：http://hz.hywenlv.cn/gtnlgvemyn.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.ppjwa.cn/gtvnrmftzy.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.zdqjudy.top/gtyrlhnpjb.html

TS:   // 同 JS
来源：http://hz.svipenyu.cn/gtyvqvvebu.html

Java: synchronized (this) { shared++; }
来源：http://hz.dashuyun.cn/gtvvuwefnd.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.ywan-chungtsiang.top/gtcnaapupu.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.sufxvd.cn/gtndqkzced.html

C#:   lock (gate) { shared++; }
来源：http://hz.jianghu66.top/gtihgwqyek.html

[O04] 定义异步函数并等待
来源：http://hz.cashguo.top/gthlwxqabn.html

Py:   async def f():⏎    await g()
来源：http://hz.shangyingyoupin.top/gtwecdswlr.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.yj20258.top/gtfknyisxd.html

JS:   async function f() { await g(); }
来源：http://hz.yuanzhike.top/gtsvsynixp.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.hnxiangtu.top/gthgjoxpwg.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.hywenlv.cn/gtstjvfqun.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.ivvv.top/gtyxtgwliu.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.ywan-chungtsiang.top/gtkosirbxt.html

C#:   async Task F() { await G(); }
来源：http://hz.nwbrower.top/gtyrtfgknh.html

[O05] 并发执行并等待全部完成
来源：http://hz.jqgfzy.top/gtmhbfycta.html

Py:   asyncio.gather(*tasks)
来源：http://hz.tanke756.top/gtuczpemuy.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.jqgfzy.top/gtkijotqjq.html

JS:   await Promise.all(tasks)
来源：http://hz.snrcjt.cn/gtjvhpiypg.html

TS:   await Promise.all(tasks)
来源：http://hz.gogol.net.cn/gtgvxanmod.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.dashuyun.cn/gttmfbmetw.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.zdqjudy.top/gtngmfkcoc.html

Ruby: threads.map(&:join)
来源：http://hz.yanxiufei.cn/gtqrybqhoy.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.xingfuxueyuan.xyz/gtvacbugsx.html

[O06] 使用进程池
来源：http://hz.feifeiyinyue.top/gtwgmgiqch.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.daxiang520.top/gtdtevpgrx.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.xziqi.cn/gtvjlwswbb.html

JS:   // child_process / cluster 模块
来源：http://hz.nanxinkj.top/gtijgxwrij.html

TS:   // child_process / cluster 模块
来源：http://hz.hnqzz.top/gtgreoutqa.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.cdnleiting.top/gtlsqbnggi.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.ydzc1.top/gtepueebtn.html

Ruby: // fork 块
来源：http://hz.ybcxt.top/gttokkrodg.html

C#:   Parallel.For
来源：http://hz.ehwqpu.com/gtpywmxfys.html

================================================================================
来源：http://hz.xinyue.icu/gtdgnhigvc.html

P. 常用工具函数
来源：http://hz.birdmap.top/gtvkzhfazz.html

================================================================================
来源：http://hz.daxiang520.top/gtrdthkjps.html

[P01] 生成 UUID
来源：http://hz.tanke756.top/gtxznptmfu.html

Py:   str(uuid.uuid4())
来源：http://hz.daxiang520.top/gtxgphtpdz.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.jqgfzy.top/gtdbkxpcvl.html

JS:   crypto.randomUUID()
来源：http://hz.jinqigfzy.top/gtgxboioin.html

TS:   crypto.randomUUID()
来源：http://hz.tian-w.cn/gtyldwigte.html

Java: UUID.randomUUID().toString()
来源：http://hz.yueranfly.top/gtlygztfjg.html

Go:   // 用 github.com/google/uuid
来源：http://hz.jinqigfzy.top/gtyjamlqpw.html

Ruby: SecureRandom.uuid
来源：http://hz.fengsongda.top/gtczdwsbhg.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.ydjk.org.cn/gtvgjvqwjo.html

[P02] MD5 / SHA256 摘要
来源：http://hz.cheryme.top/gtpvfbtfvk.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.sweek.top/gtjpkzaofj.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.sufxvd.cn/gtcwuemqzl.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.xinyue.icu/gtugvookcd.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.cashguo.top/gtpncstgiv.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.daria6918.cn/gtqqslopqe.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.jianghu66.top/gttujkddbj.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.zhixingplan.top/gtfoeqakiy.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.cucudq.cn/gteciuuhcm.html

[P03] 生成短随机字符串
来源：http://hz.yvedp.cn/gtmpvkqkqm.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.zhaomingkeji.xyz/gteltpkwaj.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.nwbrower.top/gtfsntisad.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.sweek.top/gtzdfetbir.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.dianchejie.cn/gtsljaiqiv.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.dianchejie.cn/gtcsquuwhs.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.aizwys.cn/gtvnjuxaxn.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.52xcode.cn/gtytokhfjd.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.chenlongwang.top/gtyojotcbv.html

[P04] 求长度
来源：http://hz.ywan-chungtsiang.top/gtzfzvsqdp.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.ydzc1.top/gtdlpqrfto.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.xuetiantiany.cn/gtexlyenfe.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.svipenyu.cn/gtbvudvpjx.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.ehwqpu.com/gtoccqzrzo.html

Java: list.size();  map.size();  s.length()
来源：http://hz.xuanzx.com/gtivswsmgl.html

Go:   len(arr);  len(m)
来源：http://hz.dashuyun.cn/gtjdvkxzti.html

Ruby: x.length;  x.size
来源：http://hz.yongpay.top/gtrqxcdxcr.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.hnqzz.top/gtcqzuxwcb.html

[P05] 判断两个对象内容是否相等
来源：http://hz.cdnleiting.top/gtzfafxdkq.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.vqdsnc.cn/gtlktfppoz.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.iojbl.cn/gtijlcjtid.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.hywenlv.cn/gtypaefkir.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.wangshuangyany.cn/gtbpfvxkfw.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.quarkkingdee.top/gtacqkcoog.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.hnqzz.top/gtdsguxpcv.html

Ruby: a == b
来源：http://hz.yvedp.cn/gttrahlxrv.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.iojbl.cn/gtkjxfmosi.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.nwbrower.top/gtqegdzsam.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.andypj.xyz/gtjgmtfqna.html

PHP:  if (empty($x)) {}
来源：http://hz.sweek.top/gtxhteiqrw.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.shanyushiyangkeji.top/gtahmrxfor.html

TS:   if (x == null) {}
来源：http://hz.shanyushiyangkeji.top/gtrmnkiytw.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.gaohongyu789.top/gtdntcecyt.html

Go:   if x == nil {}
来源：http://hz.jinyuanbaomall.cn/gtumyivlra.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.dianchejie.cn/gtywvcwrrz.html

C#:   if (x is null) {}
来源：http://hz.yueranfly.top/gthxprljgc.html

[P07] 防抖与节流
来源：http://hz.mhx1999.top/gtxkfdaptr.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.sysykeji.top/gtmecfgfru.html

PHP:  // 手写时间戳比较
来源：http://hz.ydjk.org.cn/gtpiqnljve.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.quarkkingdee.top/gtyabvshge.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.ydzc1.top/gtchpnwsaw.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.ydzc1.top/gttqhjiuiw.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.shangyingyoupin.top/gtboyjaxcx.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.guowangkeji.top/gtbnzojsas.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.yueranfly.top/gtxqotvniw.html

[P08] 处理浮点精度问题
来源：http://hz.cqqwz.cn/gtptazhotg.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.fengsongda.top/gtpsprdxba.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.ydjk.org.cn/gtlksecidb.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.iojbl.cn/gtuzdvvcjc.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.wangshuangyany.cn/gtanpttrlt.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.hnxiangtu.top/gtlbwqszev.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.tianlin.xyz/gtshxmecbs.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.wangdashe.top/gtwuynphkx.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.yanxiufei.cn/gtgwjarluv.html

================================================================================
来源：http://hz.nanxinkj.top/gtflhtscrp.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.zhixingplan.top/gtavtmxuqf.html

================================================================================
来源：http://hz.guowangkeji.top/gtltfddxkm.html

[Q01] 创建表
来源：http://hz.nanxuanxn.top/gtauqxkhhq.html

CREATE TABLE users (
来源：http://hz.ppjwa.cn/gttgswqdra.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.cdnleiting.top/gtrifnvika.html

name VARCHAR(50) NOT NULL,
来源：http://hz.shzxlz.cn/gtvaltfbqa.html

email VARCHAR(100) UNIQUE,
来源：http://hz.daxiang520.top/gtykwxrlao.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.cucudq.cn/gtmjfhtqsc.html

);
来源：http://hz.wangdashe.top/gtvxgkkfwy.html

[Q02] 创建带外键的表
来源：http://hz.zhiwuduotai.top/gtjdpzfcwy.html

CREATE TABLE orders (
来源：http://hz.daria6918.cn/gtlevcjokb.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.mhx1999.top/gtnbtdicnj.html

user_id INT NOT NULL,
来源：http://hz.ehwqpu.com/gtrrvrsfyj.html

amount DECIMAL(10, 2),
来源：http://hz.meibo888.top/gtnoeokpti.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.andypj.xyz/gtyzdhunlm.html

);
来源：http://hz.smart0.xyz/gtaxolkihf.html

[Q03] 增加列
来源：http://hz.nanxinkj.top/gtyvjnzocy.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.pengpengdd.cyou/gtfpzzavji.html

[Q04] 修改列类型
来源：http://hz.jianghu66.top/gtcmrxjmwj.html


<!-- 参考信息 -->