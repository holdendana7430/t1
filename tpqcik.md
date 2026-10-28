代发 wailian999

C#:   Directory.GetCurrentDirectory()
来源：http://hz.zhixingplan.top/gtvegctbmw.html

[M05] 设置退出码
来源：http://hz.jyoumei.cn/gtbvzlcgyl.html

Py:   sys.exit(1)
来源：http://hz.hammf.cn/gtpnlbwsfb.html

PHP:  exit(1);
来源：http://hz.jinqigfzy.top/gtxxdbabsk.html

JS:   process.exit(1)
来源：http://hz.gogol.net.cn/gtvowkedmn.html

TS:   process.exit(1)
来源：http://hz.zhengqikj.top/gtlkqekkmo.html

Java: System.exit(1)
来源：http://hz.hnqzz.top/gtooozhhmo.html

Go:   os.Exit(1)
来源：http://hz.jlsjyb.cn/gtnsjrhtpe.html

Ruby: exit 1
来源：http://hz.aibaodan.cn/gtcceiwfga.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.wangdashe.top/gtdatwmjli.html

[M06] 向标准错误输出
来源：http://hz.shangyingyoupin.top/gtktixfoeu.html

Py:   print("err", file=sys.stderr)
来源：http://hz.ivvv.top/gtjxlyrpsn.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.ppjwa.cn/gtarflbwzf.html

JS:   console.error("err")
来源：http://hz.tianlin.xyz/gtkwzfbwgq.html

TS:   console.error("err")
来源：http://hz.jinqigufen.top/gtloiufqgo.html

Java: System.err.println("err")
来源：http://hz.andypj.xyz/gtfxstiqmf.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.yj202588.top/gtenebiaxy.html

Ruby: warn "err"
来源：http://hz.gaohongyu789.top/gttpabxbbv.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.9152youxi.cn/gtgyvcscvi.html

[M07] 判断是否为主入口
来源：http://hz.zhaomingkeji.xyz/gtwpqthaax.html

Py:   if __name__ == "__main__":
来源：http://hz.jinqigufen.top/gtzkdozoea.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.jqgfzy.top/gtcyprgbdd.html

JS:   require.main === module
来源：http://hz.meibo888.top/gtupbsvart.html

TS:   require.main === module
来源：http://hz.birdmap.top/gtvskaigjr.html

Java: public static void main(String[] args)
来源：http://hz.zhengqikj.top/gtchqsikjv.html

Go:   func main()
来源：http://hz.yueranfly.top/gtjxbeodjk.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.mhx1999.top/gtyjlcnonr.html

C#:   static void Main(string[] args)
来源：http://hz.yuxming.cn/gtuzylshfx.html

[M08] 获取系统与运行时信息
来源：http://hz.hfpthk.cn/gtvlygpgio.html

Py:   platform.system();  platform.python_version()
来源：http://hz.ivvv.top/gtbrzcqixv.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.sysykeji.top/gtaybdpjpb.html

JS:   process.platform;  process.version
来源：http://hz.ydzc1.top/gtmhrkffmq.html

TS:   process.platform;  process.version
来源：http://hz.c1oappe.top/gtcukfymfl.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.52xcode.cn/gtbtljzqlg.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.meibo888.top/gtpnekjrga.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.fengsongda.top/gtlnbjfnyt.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.dianchejie.cn/gtgiqllvnt.html

================================================================================
来源：http://hz.cheryme.top/gtkazppelo.html

N. 数据结构与算法
来源：http://hz.aizwys.cn/gtfhslvebq.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtgfokkscp.html

[N01] 二分查找（有序数组）
来源：http://hz.birdmap.top/gtjvhhmtda.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.andypj.xyz/gtlhzaqtnz.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.hammf.cn/gtidenhayi.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.sweek.top/gtpaggmtxm.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.pengpengdd.cyou/gteegekhws.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.nanxinkj.top/gtghmqqvte.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.jianghu66.top/gtqvbjqbpx.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.daria6918.cn/gtdupqgyqn.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.yuxming.cn/gtebiwkwyc.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.yanxiufei.cn/gtnkmiwxhe.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.zhongyouzk.top/gtyaqdlewm.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.chenlongwang.top/gtdfffytzc.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.yanxiufei.cn/gtejsrmzts.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.sufxvd.cn/gtatceluid.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.shuidangran.top/gtkcibshbn.html

Go:   slices.Sort(arr)
来源：http://hz.jlsjyb.cn/gtmspaziua.html

Ruby: arr.sort
来源：http://hz.wangshuangyany.cn/gtyhcgdwjd.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.shangyingyoupin.top/gtbenvzvny.html

[N03] 快速排序（分治示例）
来源：http://hz.jinqigufen.top/gtjvrhfjtg.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.xziqi.cn/gtruukziuj.html

PHP:  // 递归实现，或用 usort
来源：http://hz.sysykeji.top/gticftktwb.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.hongshengwenyu.top/gtjkfeerqi.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.gzhubu.top/gtifzcryta.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.yueranfly.top/gtzsgflfju.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.aizwys.cn/gtasvezmcw.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.ehwqpu.com/gtwsjgzsbm.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.feifeiyinyue.top/gtsqmysjig.html

[N04] 斐波那契数列
来源：http://hz.dashuyun.cn/gtzpgtdfwa.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.ydjk.org.cn/gtttyxrina.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.cashguo.top/gtldqxplym.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.nanxuanxn.top/gtdbdbgfva.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.sxryk.cn/gtjotpgqeu.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.sysykeji.top/gtxsbeyvhs.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.haohaochexian.top/gtqrkdozhk.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.tianlin.xyz/gtnzmndqca.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.dashuyun.cn/gtkadqoebw.html

[N05] 最大公约数
来源：http://hz.ehwqpu.com/gttpambool.html

Py:   math.gcd(a, b)
来源：http://hz.shangyingyoupin.top/gtvyrmltiy.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.tanke756.top/gtgaivrlvm.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.sufxvd.cn/gtlotsxoih.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.gzhubu.top/gthcwjssfv.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.jyoumei.cn/gtffzwseqy.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.shangyingyoupin.top/gtmqogohri.html

Ruby: a.gcd(b)
来源：http://hz.c1oappe.top/gtwrmzivlu.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.ydjk.org.cn/gttsnakqaa.html

[N06] 判断回文字符串
来源：http://hz.zdqjudy.top/gtltujosvi.html

Py:   s == s[::-1]
来源：http://hz.gzhubu.top/gtfhfoyzpy.html

PHP:  $s === strrev($s);
来源：http://hz.yj20258.top/gtjmxkitjl.html

JS:   s === [...s].reverse().join("")
来源：http://hz.andypj.xyz/gtchjosula.html

TS:   s === [...s].reverse().join("")
来源：http://hz.haohaochexian.top/gttftrxejv.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.snrcjt.cn/gtdqkyexye.html

Go:   // 双指针从两端比较
来源：http://hz.shangyingyoupin.top/gtbqxtmuoi.html

Ruby: s == s.reverse
来源：http://hz.meibo888.top/gtkcgstsjl.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.sysykeji.top/gtktvjkckt.html

[N07] 两数之和（返回下标）
来源：http://hz.pycfn.com/gtdtloukwv.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.ydjk.org.cn/gtynyhaick.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.yvedp.cn/gtvxagbpac.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.smart0.xyz/gtcjahhuyn.html

TS:   // 手写 Map<string, number>
来源：http://hz.smart0.xyz/gtkkqubsrf.html

Java: // 手写 HashMap
来源：http://hz.gzhubu.top/gtfjjreajb.html

Go:   // 手写 map[int]int
来源：http://hz.hongshengwenyu.top/gtpwniryat.html

Ruby: // 手写 Hash
来源：http://hz.dashuyun.cn/gtmumnggnp.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.andypj.xyz/gtbmnisszn.html

[N08] 生成全排列
来源：http://hz.dashuyun.cn/gtmbjwhqzh.html

Py:   itertools.permutations(arr)
来源：http://hz.hnqzz.top/gtaqyzurdv.html

PHP:  // 手写递归交换
来源：http://hz.mhx1999.top/gtszervmbk.html

JS:   // 手写回溯递归
来源：http://hz.gogol.net.cn/gtmggcjkrg.html

TS:   // 手写回溯递归
来源：http://hz.cdnleiting.top/gtpltplkyz.html

Java: // 手写回溯递归
来源：http://hz.dianchejie.cn/gtgudjtpjv.html

Go:   // 手写回溯递归
来源：http://hz.yonumen.top/gtsyvnjuga.html

Ruby: arr.permutation.to_a
来源：http://hz.birdmap.top/gtsesdiudf.html

C#:   // 手写回溯递归
来源：http://hz.chenzaomai.com/gtrjdaftse.html

[N09] 栈与队列
来源：http://hz.jyoumei.cn/gtorqdymrr.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.havefunace.top/gtcuwbyrrl.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.ybcxt.top/gtzakoxhpv.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.xylfe.cn/gtcnfcvdqm.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.ybcxt.top/gtxfjsnymf.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.gzhubu.top/gtbzzaojrr.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.zhiwuduotai.top/gtuwirjtld.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.iojbl.cn/gtgtwfbadl.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.fengsongda.top/gtyfbvpfxc.html

[N10] 链表节点定义
来源：http://hz.jinqigfzy.top/gtcrrbvtbu.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.yongpay.top/gteyluvvrq.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.mhx1999.top/gtmyyqerko.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.xylfe.cn/gtagoyhtvo.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.cheryme.top/gtbxgsetit.html

Java: class Node { int v; Node next; }
来源：http://hz.ydzc1.top/gtnegaoksl.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.quarkkingdee.top/gtkwgljuql.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.jlsjyb.cn/gtwhbtttzw.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.hfpthk.cn/gtvpdjmabq.html

[N11] 二叉树中序遍历
来源：http://hz.yuxming.cn/gtgqiatenz.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.zhoulong.xyz/gtscxhlnvn.html

PHP:  // 手写递归函数
来源：http://hz.cqqwz.cn/gtycintoqd.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.0kj1m.cn/gtlihntrmk.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.gotoacloud.top/gtrcrquyam.html

Java: // 手写递归
来源：http://hz.52xcode.cn/gtltnjchrq.html

Go:   // 手写递归
来源：http://hz.wangshuangyany.cn/gtdwwhhoxw.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.tianlin.xyz/gtttljnvfw.html

C#:   // 手写递归
来源：http://hz.wangshuangyany.cn/gtifdllzwg.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.sufxvd.cn/gtmfiedgfl.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.yonumen.top/gtbucuebgl.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.zhiwuduotai.top/gtpblljsao.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.hfpthk.cn/gtjdvwswdj.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.9152youxi.cn/gtphcmtrxo.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.ydjk.org.cn/gtbovuxaip.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.gotoacloud.top/gtezbjjwvi.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.dianchejie.cn/gtkuvoliha.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.sweek.top/gtobreoxoe.html

================================================================================
来源：http://hz.ydzc1.top/gtlqowtumf.html

O. 并发与异步
来源：http://hz.ybcxt.top/gtwivrwpzf.html

================================================================================
来源：http://hz.wangdashe.top/gthyahsglz.html

[O01] 启动一个线程
来源：http://hz.zhoulong.xyz/gtrthkqojy.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.zhoulong.xyz/gtzkzclxxk.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.shangyingyoupin.top/gtrpaajqhy.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.xingfuxueyuan.xyz/gtptysgipc.html

TS:   // 同 JS
来源：http://hz.hammf.cn/gtoagssryf.html

Java: new Thread(() -> f()).start()
来源：http://hz.nanxuanxn.top/gtcottkyva.html

Go:   go f()
来源：http://hz.shanyushiyangkeji.top/gtjnupiabt.html

Ruby: Thread.new { f }
来源：http://hz.zhoulong.xyz/gtjleevoaz.html

C#:   Task.Run(() => F());
来源：http://hz.ybcxt.top/gteizvvsqv.html

[O02] 使用线程池
来源：http://hz.chenzaomai.com/gtotcnmpmq.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.jianghu66.top/gtbqqytiiz.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.wangdashe.top/gtdxvjpifn.html

JS:   // worker_threads 线程池
来源：http://hz.shangyingyoupin.top/gttmrdsufi.html

TS:   // worker_threads 线程池
来源：http://hz.ehwqpu.com/gtslmkkavk.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.xylfe.cn/gtimptbnnz.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.xylfe.cn/gtmeplbces.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.zhoulong.xyz/gtmhuirxot.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.quarkkingdee.top/gtdntjguan.html

[O03] 加锁保护共享数据
来源：http://hz.hongshengwenyu.top/gtgxlypado.html

Py:   with lock: shared += 1
来源：http://hz.vqdsnc.cn/gtrutactxb.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.zhaomingkeji.xyz/gtwwxnvzlh.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.chenjidiqi.icu/gtgkgirynm.html

TS:   // 同 JS
来源：http://hz.xuetiantiany.cn/gtpwpjphrk.html

Java: synchronized (this) { shared++; }
来源：http://hz.dianchejie.cn/gtfbjkzoph.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.zhoulong.xyz/gtvieettel.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.dashuyun.cn/gtfgmucimv.html

C#:   lock (gate) { shared++; }
来源：http://hz.chenlongwang.top/gtrvabxdef.html

[O04] 定义异步函数并等待
来源：http://hz.chenlongwang.top/gtzfkycbqj.html

Py:   async def f():⏎    await g()
来源：http://hz.yvedp.cn/gtjmfqvskf.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.smart0.xyz/gtqtuwnyxk.html

JS:   async function f() { await g(); }
来源：http://hz.ywan-chungtsiang.top/gtihebiylf.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.jinqigfzy.top/gtdmsknuap.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.jianghu66.top/gtnqytkpdi.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.birdmap.top/gtpajyfoyj.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.yueranfly.top/gtyenrfryr.html

C#:   async Task F() { await G(); }
来源：http://hz.hnqzz.top/gtvbbggulg.html

[O05] 并发执行并等待全部完成
来源：http://hz.zhijiandao.cn/gtwpwugosz.html

Py:   asyncio.gather(*tasks)
来源：http://hz.ybcxt.top/gtavaqsywq.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.zhijiandao.cn/gtkypcjroz.html

JS:   await Promise.all(tasks)
来源：http://hz.hysaishi.cn/gtkvtxloxe.html

TS:   await Promise.all(tasks)
来源：http://hz.hnxiangtu.top/gtgoglrtea.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.cashguo.top/gtvlkdwker.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.nwbrower.top/gtcsgmnabs.html

Ruby: threads.map(&:join)
来源：http://hz.vqdsnc.cn/gtrwkiguvr.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.chenzaomai.com/gtmiifustn.html

[O06] 使用进程池
来源：http://hz.ppjwa.cn/gtkkcuorzh.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.aizwys.cn/gtygmxgbun.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.jinqigufen.top/gtalnoxezb.html

JS:   // child_process / cluster 模块
来源：http://hz.zhixingplan.top/gtakpqtpfr.html

TS:   // child_process / cluster 模块
来源：http://hz.yongpay.top/gtsyxvnvji.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.xingfuxueyuan.xyz/gtkdxycshe.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.c1oappe.top/gtglrtjohg.html

Ruby: // fork 块
来源：http://hz.shuidangran.top/gtdchdhicv.html

C#:   Parallel.For
来源：http://hz.yueranfly.top/gtpsgyvtaj.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtgefvtbrx.html

P. 常用工具函数
来源：http://hz.meibo888.top/gtfrcbanri.html

================================================================================
来源：http://hz.cdnleiting.top/gtoqajevct.html

[P01] 生成 UUID
来源：http://hz.ydzc1.top/gtmzimnqnf.html

Py:   str(uuid.uuid4())
来源：http://hz.xuanzx.com/gtogwwbvhi.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.hywenlv.cn/gtvzmymnxb.html

JS:   crypto.randomUUID()
来源：http://hz.quarkkingdee.top/gtjskibbux.html

TS:   crypto.randomUUID()
来源：http://hz.yvedp.cn/gtsqngjemr.html

Java: UUID.randomUUID().toString()
来源：http://hz.wangshuangyany.cn/gtnhooqahl.html

Go:   // 用 github.com/google/uuid
来源：http://hz.cdnleiting.top/gtqprdmggj.html

Ruby: SecureRandom.uuid
来源：http://hz.aibaodan.cn/gtzbulooof.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.jinqigfzy.top/gthioprbpn.html

[P02] MD5 / SHA256 摘要
来源：http://hz.jiagoushi.top/gtxemuyodj.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.kuanghao11.cn/gtrjixdiwy.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.redwolf501.top/gtpugqlbcf.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.xylfe.cn/gtxlsbqolc.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.zhoulong.xyz/gtxxmvnxez.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.havefunace.top/gtvsqlodtr.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.nanxinkj.top/gtyajbyyhp.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.cdnleiting.top/gtbhtcqoib.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.fengsongda.top/gthdousube.html

[P03] 生成短随机字符串
来源：http://hz.dashuyun.cn/gtoyuasmbd.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.nanxinkj.top/gtgerqamlj.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.shangyingyoupin.top/gttmcoekph.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.fzhhl.top/gttjiownub.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.ydzc1.top/gtuymcmvpi.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.nanxinkj.top/gtqtascseg.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.feifeiyinyue.top/gtiqtqebib.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.cheryme.top/gtwnaoyviz.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.quarkkingdee.top/gtsggflzzy.html

[P04] 求长度
来源：http://hz.jinyuanbaomall.cn/gtqkodnvvl.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.yongpay.top/gtsaqqapkp.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.wangshuangyany.cn/gtkyxeazkg.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.gzhubu.top/gtjsipbgok.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.daria6918.cn/gteclzrjin.html

Java: list.size();  map.size();  s.length()
来源：http://hz.pengpengdd.cyou/gtapblrafj.html

Go:   len(arr);  len(m)
来源：http://hz.jqgfzy.top/gtqrhliawg.html

Ruby: x.length;  x.size
来源：http://hz.redwolf501.top/gtnqrbnrkl.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.chenlongwang.top/gtklqkgnpw.html

[P05] 判断两个对象内容是否相等
来源：http://hz.guannengcc.top/gtcuvprjkt.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.ydjk.org.cn/gtdxadlqyu.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.jyoumei.cn/gthmvrmszs.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.ivvv.top/gtxybikcch.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.wangdashe.top/gteeuxtazo.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.chenjidiqi.icu/gtfwfhbuyb.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.yuanzhike.top/gtixnachbn.html

Ruby: a == b
来源：http://hz.redwolf501.top/gtqtzcdraf.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.xinyue.icu/gtpdjtpnka.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.xuanzx.com/gtgnazmhco.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.nwbrower.top/gtlxiqwxeq.html

PHP:  if (empty($x)) {}
来源：http://hz.jlsjyb.cn/gtilcvanav.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.yonumen.top/gtabmwkozn.html

TS:   if (x == null) {}
来源：http://hz.fengsongda.top/gtydjzidam.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.fengsongda.top/gtpjuavggh.html

Go:   if x == nil {}
来源：http://hz.jyoumei.cn/gtnjkzdmqs.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.shangyingyoupin.top/gtalwrmrvk.html

C#:   if (x is null) {}
来源：http://hz.yvedp.cn/gtvxvzhpzn.html

[P07] 防抖与节流
来源：http://hz.fzhhl.top/gtffoesrqx.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.jqgufenzy.top/gtwevxzjtl.html

PHP:  // 手写时间戳比较
来源：http://hz.yj20258888.top/gtqxgvquyt.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.feifeiyinyue.top/gtasdonaej.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.xziqi.cn/gtfellljid.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.ybcxt.top/gtcxrwgwem.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.gzhubu.top/gttuworhah.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.52xcode.cn/gtvntysuar.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.zhaomingkeji.xyz/gtwkzdmyrs.html

[P08] 处理浮点精度问题
来源：http://hz.ivvv.top/gtsiippsdh.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.jyoumei.cn/gtewnkbknh.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.xingfuxueyuan.xyz/gtaafvxfmj.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.fengsongda.top/gtlrixmjfy.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.ywan-chungtsiang.top/gtlrjbcezq.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.pycfn.com/gtusysdqzk.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.sysykeji.top/gttigldnfz.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.jqgfzy.top/gtczkjvmuj.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.gogol.net.cn/gtsnwnmivb.html

================================================================================
来源：http://hz.ybcxt.top/gtitsisgou.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.yonumen.top/gtoarripzn.html

================================================================================
来源：http://hz.zhoulong.xyz/gterljgyyc.html

[Q01] 创建表
来源：http://hz.dianchejie.cn/gtlhjwxisw.html

CREATE TABLE users (
来源：http://hz.aibaodan.cn/gttcacciqo.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.pycfn.com/gthggyiota.html

name VARCHAR(50) NOT NULL,
来源：http://hz.yongpay.top/gtorfqagvr.html

email VARCHAR(100) UNIQUE,
来源：http://hz.hysaishi.cn/gtswhnvlqp.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.yj20258888.top/gtuzqjhdsh.html

);
来源：http://hz.shanyushiyangtech.top/gtwodmtoxg.html

[Q02] 创建带外键的表
来源：http://hz.guannengcc.top/gtutijbaiy.html

CREATE TABLE orders (
来源：http://hz.cucudq.cn/gtzptqboai.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.yj20258.top/gtydqepgkm.html

user_id INT NOT NULL,
来源：http://hz.hongshengwenyu.top/gtceijaqff.html

amount DECIMAL(10, 2),
来源：http://hz.cqqwz.cn/gtuuivabtx.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.fengsongda.top/gtvejtvegw.html

);
来源：http://hz.bjfxy.top/gtrawzldou.html

[Q03] 增加列
来源：http://hz.vqdsnc.cn/gtmmjbfrve.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.yuanzhike.top/gtqiqjzean.html

[Q04] 修改列类型
来源：http://hz.pycfn.com/gthdfcqfef.html


<!-- 参考信息 -->