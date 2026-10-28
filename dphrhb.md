代发 wailian999

TS:   process.cwd()
来源：http://hz.hfpthk.cn/gtulfxdnsn.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.svipenyu.cn/gtqiryawdz.html

Go:   os.Getwd()
来源：http://hz.wangshuangyany.cn/gtrhqcjyqw.html

Ruby: Dir.pwd
来源：http://hz.nwbrower.top/gteoqvbzby.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.jyoumei.cn/gtodlxrvur.html

[M05] 设置退出码
来源：http://hz.guannengcc.top/gtanygtzxw.html

Py:   sys.exit(1)
来源：http://hz.chenzaomai.com/gtfmqxgfah.html

PHP:  exit(1);
来源：http://hz.316326.xyz/gtwtugkgji.html

JS:   process.exit(1)
来源：http://hz.ydzc1.top/gtkxeoixqk.html

TS:   process.exit(1)
来源：http://hz.52xcode.cn/gthsnrkuxb.html

Java: System.exit(1)
来源：http://hz.andypj.xyz/gthdwijnlg.html

Go:   os.Exit(1)
来源：http://hz.tianlin.xyz/gtncedywzf.html

Ruby: exit 1
来源：http://hz.fengsongda.top/gtfjoretxb.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.quarkkingdee.top/gtqtexfqhz.html

[M06] 向标准错误输出
来源：http://hz.zhoulong.xyz/gtntwpnrfy.html

Py:   print("err", file=sys.stderr)
来源：http://hz.pycfn.com/gtocsoacof.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.aizwys.cn/gtnzyocnxk.html

JS:   console.error("err")
来源：http://hz.shuidangran.top/gthhbkoona.html

TS:   console.error("err")
来源：http://hz.c1oappe.top/gtrxuivjko.html

Java: System.err.println("err")
来源：http://hz.pycfn.com/gtfhuqdncb.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.sysykeji.top/gtcbpireao.html

Ruby: warn "err"
来源：http://hz.jinqigfzy.top/gtlrrcfoar.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.guowangkeji.top/gtpuvadqkh.html

[M07] 判断是否为主入口
来源：http://hz.yj20258.top/gtjqlqwspu.html

Py:   if __name__ == "__main__":
来源：http://hz.yongpay.top/gtmppqzyrk.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.ybcxt.top/gtnbetnksb.html

JS:   require.main === module
来源：http://hz.xziqi.cn/gtmjsfrlol.html

TS:   require.main === module
来源：http://hz.jinghuilouyu.cn/gtxgjxpbci.html

Java: public static void main(String[] args)
来源：http://hz.jinqigfzy.top/gtlmyjbacs.html

Go:   func main()
来源：http://hz.mhx1999.top/gtmrtfkbwz.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.chenjidiqi.icu/gtfmbzrhpk.html

C#:   static void Main(string[] args)
来源：http://hz.cqqwz.cn/gtvfnbqsgb.html

[M08] 获取系统与运行时信息
来源：http://hz.9152youxi.cn/gtyrxykgkm.html

Py:   platform.system();  platform.python_version()
来源：http://hz.zhijiandao.cn/gtluuccgth.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.zhengqikj.top/gtbfoytmcp.html

JS:   process.platform;  process.version
来源：http://hz.gogol.net.cn/gtjfbshhko.html

TS:   process.platform;  process.version
来源：http://hz.ydzc1.top/gtnphueehz.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.pengpengdd.cyou/gtomcvwuic.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.zhoulong.xyz/gtvwqbzfon.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.zhixingplan.top/gthsqmtaeb.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.9152youxi.cn/gthhkphaeh.html

================================================================================
来源：http://hz.cqqwz.cn/gtbfzsjcwm.html

N. 数据结构与算法
来源：http://hz.daria6918.cn/gtaaowjpoo.html

================================================================================
来源：http://hz.chenzaomai.com/gtnyscpjnw.html

[N01] 二分查找（有序数组）
来源：http://hz.yj20258888.top/gtzgzyuvoi.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.gotoacloud.top/gtbhclrihq.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.hongshengwenyu.top/gtwcdfvoga.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.bjfxy.top/gtodoggkni.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.yuxming.cn/gtjjyifakv.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.dianchejie.cn/gtcotcnkxn.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.shanyushiyangtech.top/gtwdmvpfaz.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.nwbrower.top/gtkuoeklwn.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.hongshengwenyu.top/gtnfhfrfsv.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.fengsongda.top/gtwkguntwp.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.shanyushiyangkeji.top/gtkrjmdimd.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.haohaochexian.top/gtoohncdlq.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.pycfn.com/gtdousfqgh.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.gotoacloud.top/gtalrrnxin.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.cucudq.cn/gttuuqszei.html

Go:   slices.Sort(arr)
来源：http://hz.9152youxi.cn/gthxkxckqk.html

Ruby: arr.sort
来源：http://hz.52xcode.cn/gtikntbqyi.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.jiagoushi.top/gtgflpvqtx.html

[N03] 快速排序（分治示例）
来源：http://hz.jlsjyb.cn/gtgfihcijc.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.yongpay.top/gtpunjuhzt.html

PHP:  // 递归实现，或用 usort
来源：http://hz.cucudq.cn/gtjwqwwemx.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.hywenlv.cn/gtxawzxrkr.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.nanxuanxn.top/gttasrziwn.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.zycfv.cn/gtttlcjjse.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.nanxuanxn.top/gttiuffmes.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.chenlongwang.top/gtebtkmxka.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.hnqzz.top/gttpabefkt.html

[N04] 斐波那契数列
来源：http://hz.gaohongyu789.top/gtctmwokzf.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.zhixingplan.top/gtksfblqay.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.ehwqpu.com/gtamgezzgm.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.hnqzz.top/gtkvsqyzos.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.ybcxt.top/gtptabmpjb.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.hnxiangtu.top/gtgxarjnxz.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.zhengqikj.top/gtprruefgt.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.hysaishi.cn/gtszjwpljk.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.zdqjudy.top/gtxxfvrbcg.html

[N05] 最大公约数
来源：http://hz.shuidangran.top/gtdgdweaeg.html

Py:   math.gcd(a, b)
来源：http://hz.sxryk.cn/gtchdmeanb.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.zhaomingkeji.xyz/gtwqnoxwnr.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.xinyue.icu/gtmzdtjciu.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.ivvv.top/gtpvxmuume.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.nanxinkj.top/gtaqfvvtde.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.jinqigufen.top/gtexpdgxxm.html

Ruby: a.gcd(b)
来源：http://hz.xziqi.cn/gtrkdmvqfs.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.meibo888.top/gtecrqkydj.html

[N06] 判断回文字符串
来源：http://hz.yj20258.top/gtypzbiiba.html

Py:   s == s[::-1]
来源：http://hz.jyoumei.cn/gtlmvradsj.html

PHP:  $s === strrev($s);
来源：http://hz.aizwys.cn/gtrlbriaok.html

JS:   s === [...s].reverse().join("")
来源：http://hz.ivvv.top/gtisyeuwtb.html

TS:   s === [...s].reverse().join("")
来源：http://hz.xuanzx.com/gtvyehbnrv.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.guowangkeji.top/gtzctxvgir.html

Go:   // 双指针从两端比较
来源：http://hz.daxiang520.top/gtowsibisb.html

Ruby: s == s.reverse
来源：http://hz.gogol.net.cn/gtyqxlpgzv.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.dianchejie.cn/gteefzsdxb.html

[N07] 两数之和（返回下标）
来源：http://hz.cucudq.cn/gtrdsbjlxf.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.bjfxy.top/gtnyaqqqrf.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.shanyushiyangtech.top/gtgbztfytm.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.havefunace.top/gtjgkdbkdd.html

TS:   // 手写 Map<string, number>
来源：http://hz.xuetiantiany.cn/gtwunbufxw.html

Java: // 手写 HashMap
来源：http://hz.yonumen.top/gtsffvnipp.html

Go:   // 手写 map[int]int
来源：http://hz.zhijiandao.cn/gtfnljbwsm.html

Ruby: // 手写 Hash
来源：http://hz.shuidangran.top/gtldrdvvdt.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.ydjk.org.cn/gtndoqomoz.html

[N08] 生成全排列
来源：http://hz.jyoumei.cn/gtrnbojzik.html

Py:   itertools.permutations(arr)
来源：http://hz.316326.xyz/gtuwpcjlgs.html

PHP:  // 手写递归交换
来源：http://hz.jinghuilouyu.cn/gtkvbvoehq.html

JS:   // 手写回溯递归
来源：http://hz.zhiwuduotai.top/gteydffkpg.html

TS:   // 手写回溯递归
来源：http://hz.yangfankeji.com/gtklcbgusk.html

Java: // 手写回溯递归
来源：http://hz.xziqi.cn/gtdvnfthbz.html

Go:   // 手写回溯递归
来源：http://hz.cheryme.top/gtfrguelsd.html

Ruby: arr.permutation.to_a
来源：http://hz.chenzaomai.com/gtfhpassev.html

C#:   // 手写回溯递归
来源：http://hz.mhx1999.top/gtwdwhhzji.html

[N09] 栈与队列
来源：http://hz.hysaishi.cn/gtyaypkwnr.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.svipenyu.cn/gtzrzltzpz.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.jqgfzy.top/gtsrzqdeos.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.nanxuanxn.top/gtiuoqhkbd.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.birdmap.top/gtozvbhxmy.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.jinqigufen.top/gtsqxkgzzn.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.jinqigufen.top/gtowowuafu.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.hysaishi.cn/gtougafooz.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.yuxming.cn/gtsssndxml.html

[N10] 链表节点定义
来源：http://hz.redwolf501.top/gtxffxrwwh.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.nwbrower.top/gtxmzzeoob.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.andypj.xyz/gtoxbxgttr.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.mhx1999.top/gtcmjmjsdn.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.yj20258888.top/gtoyynbqsd.html

Java: class Node { int v; Node next; }
来源：http://hz.smart0.xyz/gtspxymwtr.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.yvedp.cn/gtbtobucre.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.52xcode.cn/gtiwdlupmb.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.zycfv.cn/gttqusvklv.html

[N11] 二叉树中序遍历
来源：http://hz.hywenlv.cn/gtsxdlsvyq.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.hongshengwenyu.top/gtfqxzfgxe.html

PHP:  // 手写递归函数
来源：http://hz.ivvv.top/gtijkcxogw.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.sufxvd.cn/gtdwkoeytg.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.xingfuxueyuan.xyz/gtxzbvkgcp.html

Java: // 手写递归
来源：http://hz.sxryk.cn/gtmghzodzg.html

Go:   // 手写递归
来源：http://hz.chenlongwang.top/gthszbjnan.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.zhongyouzk.top/gtmnzeuoio.html

C#:   // 手写递归
来源：http://hz.svipenyu.cn/gtalaniywc.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.ydzc1.top/gtwguchrgf.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.zycfv.cn/gtqzzzdpfg.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.shanyushiyangtech.top/gtccuasvus.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.yj20258.top/gtnggfsftb.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.svipenyu.cn/gtdggtlryd.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.ydzc1.top/gtrfquupfb.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.xuetiantiany.cn/gtekydgrnf.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.zhaomingkeji.xyz/gtnhqzsyoh.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.svipenyu.cn/gtqbjktine.html

================================================================================
来源：http://hz.zdqjudy.top/gtjqqbkbmx.html

O. 并发与异步
来源：http://hz.zhoulong.xyz/gtxdaepoxy.html

================================================================================
来源：http://hz.yongpay.top/gtfnabjtdy.html

[O01] 启动一个线程
来源：http://hz.hnxiangtu.top/gtgjsizqlr.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.birdmap.top/gtpuqoyyxf.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.kuanghao11.cn/gtoxflykxn.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.ppjwa.cn/gtbkuxsnye.html

TS:   // 同 JS
来源：http://hz.ywan-chungtsiang.top/gtvfoxjusb.html

Java: new Thread(() -> f()).start()
来源：http://hz.smart0.xyz/gtslbnxqby.html

Go:   go f()
来源：http://hz.c1oappe.top/gtoicygfiz.html

Ruby: Thread.new { f }
来源：http://hz.sysykeji.top/gtcmiikgoq.html

C#:   Task.Run(() => F());
来源：http://hz.zhongyouzk.top/gtnildaxdu.html

[O02] 使用线程池
来源：http://hz.nanxuanxn.top/gtoopbsnfr.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.ydzc1.top/gtyrkulatx.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.shzxlz.cn/gtpxhepyzp.html

JS:   // worker_threads 线程池
来源：http://hz.bjfxy.top/gtfmjhfgea.html

TS:   // worker_threads 线程池
来源：http://hz.ywan-chungtsiang.top/gtzlyrmwly.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.mhx1999.top/gtjwiacrzn.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.gogol.net.cn/gtqphgvlbx.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.birdmap.top/gtlqyazsuw.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.yuanzhike.top/gtiuixjlba.html

[O03] 加锁保护共享数据
来源：http://hz.9152youxi.cn/gtplyzqbja.html

Py:   with lock: shared += 1
来源：http://hz.dashuyun.cn/gtqstsccxq.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.xylfe.cn/gtzrpqxemr.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.mhx1999.top/gttbiowlfh.html

TS:   // 同 JS
来源：http://hz.hfpthk.cn/gtiapgmhwx.html

Java: synchronized (this) { shared++; }
来源：http://hz.daxiang520.top/gtjttsdsbw.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.xziqi.cn/gtwruczjrl.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.tanke756.top/gtijyjonlw.html

C#:   lock (gate) { shared++; }
来源：http://hz.birdmap.top/gtqkyxdpfp.html

[O04] 定义异步函数并等待
来源：http://hz.sufxvd.cn/gtgypccgcs.html

Py:   async def f():⏎    await g()
来源：http://hz.hongshengwenyu.top/gtfrbcbfzk.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.jinghuilouyu.cn/gtvijkfbsq.html

JS:   async function f() { await g(); }
来源：http://hz.ppjwa.cn/gtaendseuv.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.fengsongda.top/gtonlyjsuw.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.shzxlz.cn/gtwmfmejfi.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.haohaochexian.top/gtesmqdmrq.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.zhiwuduotai.top/gtdjqfhuwh.html

C#:   async Task F() { await G(); }
来源：http://hz.shanyushiyangtech.top/gtkmfbtvih.html

[O05] 并发执行并等待全部完成
来源：http://hz.daria6918.cn/gtsltafhov.html

Py:   asyncio.gather(*tasks)
来源：http://hz.cheryme.top/gtlsktgcti.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.smart0.xyz/gtqktjenmf.html

JS:   await Promise.all(tasks)
来源：http://hz.bjfxy.top/gtctmjgazr.html

TS:   await Promise.all(tasks)
来源：http://hz.xylfe.cn/gtbvkjqwpl.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.tianlin.xyz/gtsvqvdvfh.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.ydzc1.top/gtoacjwfct.html

Ruby: threads.map(&:join)
来源：http://hz.pengpengdd.cyou/gtbquyifyb.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.tian-w.cn/gtvxcfpbof.html

[O06] 使用进程池
来源：http://hz.fzhhl.top/gtvnurvarr.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.zhijiandao.cn/gtvdhridfm.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.xuetiantiany.cn/gtcjokhxsc.html

JS:   // child_process / cluster 模块
来源：http://hz.smart0.xyz/gtzerhwupp.html

TS:   // child_process / cluster 模块
来源：http://hz.chenjidiqi.icu/gtonbiuwum.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.cucudq.cn/gtjpzngdum.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.zhaomingkeji.xyz/gttjfyqrxj.html

Ruby: // fork 块
来源：http://hz.yj20258888.top/gtfvyfqycc.html

C#:   Parallel.For
来源：http://hz.wangshuangyany.cn/gtbhbmczbg.html

================================================================================
来源：http://hz.hammf.cn/gtvzubuhcy.html

P. 常用工具函数
来源：http://hz.feifeiyinyue.top/gtcfunwvun.html

================================================================================
来源：http://hz.zhongyouzk.top/gtcbnuaciu.html

[P01] 生成 UUID
来源：http://hz.xinyue.icu/gtcxxzixct.html

Py:   str(uuid.uuid4())
来源：http://hz.ydzc1.top/gtidupeyjx.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.aizwys.cn/gttkowrlvd.html

JS:   crypto.randomUUID()
来源：http://hz.ywan-chungtsiang.top/gtdktfiuib.html

TS:   crypto.randomUUID()
来源：http://hz.hysaishi.cn/gtuyxmryuz.html

Java: UUID.randomUUID().toString()
来源：http://hz.xylfe.cn/gtysdbjldh.html

Go:   // 用 github.com/google/uuid
来源：http://hz.jinqigfzy.top/gtlztypogi.html

Ruby: SecureRandom.uuid
来源：http://hz.nanxuanxn.top/gtdjvkxmov.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.jlsjyb.cn/gtnhaqyouw.html

[P02] MD5 / SHA256 摘要
来源：http://hz.yongpay.top/gtswtjvaqx.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.nwbrower.top/gtupcltsro.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.fengsongda.top/gtukuxmimr.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.nanxinkj.top/gtoyuisdlt.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.jinqigufen.top/gtkfycvhkf.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.zhiwuduotai.top/gtyaspdtjt.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.svipenyu.cn/gtxdespscv.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.xuanzx.com/gtaehypjcm.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.ydzc1.top/gtpujtvqyn.html

[P03] 生成短随机字符串
来源：http://hz.chenjidiqi.icu/gtzziaszpz.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.nanxuanxn.top/gtoepfrzzb.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.hfpthk.cn/gteszpuzji.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.smart0.xyz/gtvtaaqhbx.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.wangshuangyany.cn/gtubcjvnli.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.xziqi.cn/gtugffvbhj.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.guannengcc.top/gttxncitpt.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.aibaodan.cn/gtwyolgowa.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.yj202588.top/gtzpdpujwy.html

[P04] 求长度
来源：http://hz.hammf.cn/gtufifpedt.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.xingfuxueyuan.xyz/gtptinptxa.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.gogol.net.cn/gtiiqaifbv.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.xylfe.cn/gttdnglzht.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.gotoacloud.top/gtznnufrpd.html

Java: list.size();  map.size();  s.length()
来源：http://hz.kuanghao11.cn/gtbnznlkeq.html

Go:   len(arr);  len(m)
来源：http://hz.sweek.top/gtdubwboii.html

Ruby: x.length;  x.size
来源：http://hz.jinqigfzy.top/gtpqiubauq.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.snrcjt.cn/gthpvwnsnj.html

[P05] 判断两个对象内容是否相等
来源：http://hz.jinqigfzy.top/gtsolgulhk.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.ivvv.top/gtkdcqcasr.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.havefunace.top/gtfkzrkqzr.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.yuanzhike.top/gtsdxbninf.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.yongpay.top/gtsbwalqkb.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.hfpthk.cn/gtbdpvktkd.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.guannengcc.top/gtkmrluflx.html

Ruby: a == b
来源：http://hz.pycfn.com/gtjvffqeym.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.aibaodan.cn/gtyecwgsmo.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.pycfn.com/gtsblhhfwy.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.hongshengwenyu.top/gtgkheqaln.html

PHP:  if (empty($x)) {}
来源：http://hz.bjfxy.top/gtncyfatul.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.hysaishi.cn/gtowdbkzml.html

TS:   if (x == null) {}
来源：http://hz.shangyingyoupin.top/gtpoqisvvb.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.yanxiufei.cn/gtpilvozpz.html

Go:   if x == nil {}
来源：http://hz.nanxinkj.top/gtusgqkail.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.yj20258.top/gtxfwrhsug.html

C#:   if (x is null) {}
来源：http://hz.sweek.top/gtthsutidu.html

[P07] 防抖与节流
来源：http://hz.ywan-chungtsiang.top/gtyxtqqhce.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.316326.xyz/gtyjwpraqt.html

PHP:  // 手写时间戳比较
来源：http://hz.zhaomingkeji.xyz/gtducsqbwa.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.vqdsnc.cn/gtjhmifnum.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.aibaodan.cn/gtaazkoonn.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.chenjidiqi.icu/gtvjuiehxu.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.jqgufenzy.top/gtkwrmyrae.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.tanke756.top/gtyuovlqcx.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.daria6918.cn/gttqeokkpl.html

[P08] 处理浮点精度问题
来源：http://hz.316326.xyz/gtwzinrcgk.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.jinyuanbaomall.cn/gtiwqneflv.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.cheryme.top/gtjgipnjal.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.zhongyouzk.top/gtjuyzojqk.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.xuanzx.com/gtoykgiprc.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.ybcxt.top/gtimxbvpek.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.jiagoushi.top/gtwarbznnj.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.wangshuangyany.cn/gtgpjorvox.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.fengsongda.top/gtprjvzoyt.html

================================================================================
来源：http://hz.zdqjudy.top/gtlawewytl.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.xuetiantiany.cn/gtunnsfkhh.html

================================================================================
来源：http://hz.jinqigfzy.top/gtjnrhlbkx.html

[Q01] 创建表
来源：http://hz.shanyushiyangkeji.top/gtvaaxmpww.html

CREATE TABLE users (
来源：http://hz.yonumen.top/gtgktoyefd.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.sxryk.cn/gtrtjrlkrs.html

name VARCHAR(50) NOT NULL,
来源：http://hz.xuanzx.com/gtqblqjrbq.html

email VARCHAR(100) UNIQUE,
来源：http://hz.hysaishi.cn/gtknjricwx.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.iojbl.cn/gtgdeqhcpr.html

);
来源：http://hz.smart0.xyz/gtdfojmcuh.html

[Q02] 创建带外键的表
来源：http://hz.tanke756.top/gtfmbfxmdm.html

CREATE TABLE orders (
来源：http://hz.xingfuxueyuan.xyz/gtuhfyhovb.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.sxryk.cn/gtklbeterv.html

user_id INT NOT NULL,
来源：http://hz.jqgufenzy.top/gtnxsjynwk.html

amount DECIMAL(10, 2),
来源：http://hz.hfpthk.cn/gtijgbjsia.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.hammf.cn/gtjsuvnrrb.html


<!-- 参考信息 -->